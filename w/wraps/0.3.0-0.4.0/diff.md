# Comparing `tmp/wraps-0.3.0.tar.gz` & `tmp/wraps-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraps-0.3.0.tar", max compression
+gzip compressed data, was "wraps-0.4.0.tar", max compression
```

## Comparing `wraps-0.3.0.tar` & `wraps-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1092 2023-01-28 15:19:23.853019 wraps-0.3.0/LICENSE
--rw-r--r--   0        0        0     6663 2023-01-28 15:19:23.853019 wraps-0.3.0/README.md
--rw-r--r--   0        0        0     2991 2023-01-28 15:19:23.853019 wraps-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1449 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/__init__.py
--rw-r--r--   0        0        0     1462 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/early.py
--rw-r--r--   0        0        0    15033 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/either.py
--rw-r--r--   0        0        0     1102 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/errors.py
--rw-r--r--   0        0        0     5905 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/future.py
--rw-r--r--   0        0        0    10272 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/future_option.py
--rw-r--r--   0        0        0    14920 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/future_result.py
--rw-r--r--   0        0        0    43161 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/option.py
--rw-r--r--   0        0        0        0 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/py.typed
--rw-r--r--   0        0        0    56581 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/result.py
--rw-r--r--   0        0        0     1300 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/typing.py
--rw-r--r--   0        0        0      191 2023-01-28 15:19:23.853019 wraps-0.3.0/wraps/utils.py
--rw-r--r--   0        0        0     7555 1970-01-01 00:00:00.000000 wraps-0.3.0/setup.py
--rw-r--r--   0        0        0     7883 1970-01-01 00:00:00.000000 wraps-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-24 21:34:43.395506 wraps-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6490 2023-04-24 21:34:43.395506 wraps-0.4.0/README.md
+-rw-r--r--   0        0        0     3331 2023-04-24 21:34:43.399508 wraps-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2526 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/__init__.py
+-rw-r--r--   0        0        0     2852 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/early.py
+-rw-r--r--   0        0        0    15275 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/either.py
+-rw-r--r--   0        0        0     1187 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/errors.py
+-rw-r--r--   0        0        0     3952 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future.py
+-rw-r--r--   0        0        0     1134 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future_either.py
+-rw-r--r--   0        0        0     9285 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future_option.py
+-rw-r--r--   0        0        0    14054 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/future_result.py
+-rw-r--r--   0        0        0    40999 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/option.py
+-rw-r--r--   0        0        0        0 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/py.typed
+-rw-r--r--   0        0        0     1809 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/reawaitable.py
+-rw-r--r--   0        0        0    53456 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/result.py
+-rw-r--r--   0        0        0      604 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/utils.py
+-rw-r--r--   0        0        0     9436 2023-04-24 21:34:43.399508 wraps-0.4.0/wraps/wraps.py
+-rw-r--r--   0        0        0     7742 1970-01-01 00:00:00.000000 wraps-0.4.0/PKG-INFO
```

### Comparing `wraps-0.3.0/LICENSE` & `wraps-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wraps-0.3.0/README.md` & `wraps-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Installing the library with `pip` is quite simple:
 
 ```console
 $ pip install wraps
 ```
 
-Alternatively, the library can be installed from source:
+Alternatively, the library can be installed from the source:
 
 ```console
 $ git clone https://github.com/nekitdev/wraps.git
 $ cd wraps
 $ python -m pip install .
 ```
 
@@ -40,15 +40,15 @@
 $ poetry add wraps
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-wraps = "^0.3.0"
+wraps = "^0.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.wraps]
 git = "https://github.com/nekitdev/wraps.git"
@@ -57,105 +57,108 @@
 ## Examples
 
 ### Option
 
 [`Option[T]`][wraps.option.Option] type represents an optional value: every option is either
 [`Some[T]`][wraps.option.Some] and contains a value, or [`Null`][wraps.option.Null], and does not.
 
-Here is an example of using [`wrap_option`][wraps.option.wrap_option] to catch any errors:
+Here is an example of using [`wrap_option`][wraps.wraps.wrap_option] to catch any errors:
 
 ```python
 from typing import List, TypeVar
 from wraps import wrap_option
 
 T = TypeVar("T", covariant=True)
 
 
-class SafeList(List[T]):
+class Array(List[T]):
     @wrap_option
     def get(self, index: int) -> T:
         return self[index]
 
 
-array = SafeList([0, 1, 2, 3])
+array = Array([1, 2, 3])
 
-print(array.get(0))  # Some(value=0)
-print(array.get(7))  # Null()
+print(array.get(0).unwrap())  # 1
+print(array.get(5).unwrap_or(0))  # 0
 ```
 
 ### Result
 
 [`Result[T, E]`][wraps.result.Result] is the type used for returning and propagating errors.
 It has two variants, [`Ok[T]`][wraps.result.Ok], representing success and containing a value,
 and [`Error[E]`][wraps.result.Error], representing error and containing an error value.
 
 ```python
-from wraps import Result, wrap_result
+from enum import Enum
 
+from wraps import Error, Ok, Result
 
-@wrap_result[ValueError]
-def parse(string: str) -> int:
-    return int(string)
 
+class DivideError(Enum):
+    DIVISION_BY_ZERO = "division by zero"
 
-def multiply(x: str, y: str) -> Result[int, ValueError]:
-    # try to parse two strings and multiply results
-    return parse(x).and_then(lambda m: parse(y).map(lambda n: m * n))
 
-
-print(multiply("21", "2").unwrap())  # 42
-print(multiply("!", "42").unwrap_error())  # invalid literal for `int` with base 10: `!`
+def divide(numerator: float, denominator: float) -> Result[float, DivideError]:
+    return Ok(numerator / denominator) if denominator else Error(DivideError.DIVISION_BY_ZERO)
 ```
 
-In python versions before 3.9 (where grammar restrictions on decorators were relaxed),
-one can use [`wrap_result`][wraps.result.wrap_result] without a concrete type:
+### Early Return
+
+Early return functionality (`?` operator in Rust) is implemented via `early` methods
+(for both [`Option`][wraps.option.Option] and [`Result`][wraps.result.Result] types)
+combined with the [`@early_option`][wraps.early.early_option] and
+[`@early_result`][wraps.early.early_result] decorators respectively.
 
 ```python
-@wrap_result
-def parse(string: str) -> int:
-    return int(string)
-```
+from wraps import Option, early_option, wrap_option
 
-However this makes the types less specific, since [`Exception`][Exception]
-is caught instead of [`ValueError`][ValueError].
 
-Instead, you can create a new concrete [`WrapResult[E]`][wraps.result.WrapResult] instance:
+@wrap_option[ValueError]
+def parse(string: str) -> float:
+    return float(string)
 
-```python
-from wraps import WrapResult
 
-wrap_value_error = WrapResult(ValueError)
+@wrap_option[ZeroDivisionError]
+def divide(numerator: float, denominator: float) -> float:
+    return numerator / denominator
 
-@wrap_value_error
-def parse(string: str) -> int:
-    return int(string)
+
+@early_option
+def function(x: str, y: str) -> Option[float]:
+    return divide(parse(x).early(), parse(y).early())
 ```
 
-### Early Return
+### Decorators
 
-Early return functionality (`?` operator in Rust) is implemented via `early` function
-(for both [`Option`][wraps.option.Option] and [`Result`][wraps.result.Result] types)
-combined with the [`@early_option`][wraps.early.early_option] or
-[`@early_result`][wraps.early.early_result] decorator respectively.
+In Python 3.9 the restrictions on the decorators' syntax have been lifted, which allows for nifty
+syntax which can be seen above. On older versions of Python, one can use:
 
 ```python
-from wraps import Option, Some, early_option, wrap_option
-
+from wraps import wrap_option
 
 @wrap_option
 def parse(string: str) -> int:
     return int(string)
+```
 
+However, this isn't the best way to handle errors, as *any* normal errors will be caught, without
+a way to distinguish between them.
+To counter this, one can use [`WrapOption`][wraps.wraps.WrapOption] directly,
+passing the concrete error type:
 
-@early_option
-def try_add(x: str, y: str) -> Option[int]:
-    m = parse(x).early()
-    n = parse(y).early()
+```python
+from wraps import WrapOption
 
-    return Some(m + n)
+wrap_value_error = WrapOption(ValueError)
+
+
+@wrap_value_error
+def parse(string: str) -> int:
+    return int(string)
 ```
 
 ## Documentation
 
 You can find the documentation [here][Documentation].
 
 ## Support
@@ -206,21 +209,18 @@
 [Check Badge]: https://github.com/nekitdev/wraps/workflows/check/badge.svg
 [Test Badge]: https://github.com/nekitdev/wraps/workflows/test/badge.svg
 [Coverage Badge]: https://codecov.io/gh/nekitdev/wraps/branch/main/graph/badge.svg
 
 [wraps.option.Option]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Option
 [wraps.option.Some]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Some
 [wraps.option.Null]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Null
-[wraps.option.wrap_option]: https://nekitdev.github.io/wraps/reference/option#wraps.option.wrap_option
 
 [wraps.result.Result]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Result
 [wraps.result.Ok]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Ok
 [wraps.result.Error]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Error
-[wraps.result.wrap_result]: https://nekitdev.github.io/wraps/reference/result#wraps.result.wrap_result
 
-[wraps.result.WrapResult]: https://nekitdev.github.io/wraps/reference/result#wraps.result.WrapResult
+[wraps.wraps.wrap_option]: https://nekitdev.github.io/wraps/reference/wraps#wraps.wraps.wrap_option
+
+[wraps.wraps.WrapOption]: https://nekitdev.github.io/wraps/reference/wraps#wraps.wraps.WrapOption
 
 [wraps.early.early_option]: https://nekitdev.github.io/wraps/reference/early#wraps.early.early_option
 [wraps.early.early_result]: https://nekitdev.github.io/wraps/reference/early#wraps.early.early_result
-
-[Exception]: https://docs.python.org/3/library/exceptions#Exception
-[ValueError]: https://docs.python.org/3/library/exceptions#ValueError
```

### Comparing `wraps-0.3.0/pyproject.toml` & `wraps-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "wraps"
-version = "0.3.0"
+version = "0.4.0"
 description = "Meaningful and safe wrapping types."
-authors = ["nekitdev <nekitdevofficial@gmail.com>"]
+authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/wraps"
 repository = "https://github.com/nekitdev/wraps"
 documentation = "https://nekitdev.github.io/wraps"
@@ -28,56 +28,73 @@
 
 [[tool.poetry.packages]]
 include = "wraps"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
-attrs = ">= 22.2.0"
+attrs = ">= 23.1.0"
 
-typing-extensions = ">= 4.3.0"
+funcs = ">= 0.5.0"
+async-extensions = ">= 1.2.2"
+typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.12.0"
+black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.11.4"
+version = "5.12.0"
+python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.991"
+mypy = "1.2.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
-anyio = "3.6.1"
-trio = "0.21.0"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
+anyio = "3.6.2"
+trio = "0.22.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.2"
+mkdocs-material = "9.1.8"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.21.2"
 extras = ["python"]
 
+[tool.poetry.group.dev.dependencies]
+changelogging = "1.1.0"
+
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+ignore = [
+    "E402",  # module level import not at top of file (circular import fixes)
+]
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov wraps"
 testpaths = ["tests"]
@@ -124,15 +141,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "wraps"
-version = "0.3.0"
+version = "0.4.0"
 url = "https://github.com/nekitdev/wraps"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
@@ -141,9 +158,9 @@
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["feature", "change", "fix", "security", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.4.0"]
+requires = ["poetry-core >= 1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wraps-0.3.0/wraps/early.py` & `wraps-0.4.0/wraps/early.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from functools import wraps
+"""Early returns."""
+
 from typing import Callable, TypeVar
 
+from funcs.decorators import wraps
+from funcs.typing import AsyncCallable
 from typing_extensions import ParamSpec
 
 from wraps.errors import EarlyOption, EarlyResult
 from wraps.option import Null, Option
 from wraps.result import Error, Result
 
-__all__ = ("early_option", "early_result")
+__all__ = ("early_option", "early_option_await", "early_result", "early_result_await")
 
 P = ParamSpec("P")
 
 T = TypeVar("T")
 
 E = TypeVar("E")
 
 
 def early_option(function: Callable[P, Option[T]]) -> Callable[P, Option[T]]:
     """Decorates the `function` returning [`Option[T]`][wraps.result.Option]
-    to handle *early returns* via `early` (`?` in Rust) operator.
+    to handle *early returns* via the `early` (`?` in Rust) operator.
 
     Arguments:
         function: The function to wrap.
 
     Returns:
         The wrapping function.
     """
@@ -34,17 +37,39 @@
 
         except EarlyOption:
             return Null()
 
     return wrap
 
 
+def early_option_await(function: AsyncCallable[P, Option[T]]) -> AsyncCallable[P, Option[T]]:
+    """Decorates the asynchronous `function` returning [`Option[T]`][wraps.result.Option]
+    to handle *early returns* via the `early` (`?` in Rust) operator.
+
+    Arguments:
+        function: The asynchronous function to wrap.
+
+    Returns:
+        The asynchronous wrapping function.
+    """
+
+    @wraps(function)
+    async def wrap(*args: P.args, **kwargs: P.kwargs) -> Option[T]:
+        try:
+            return await function(*args, **kwargs)
+
+        except EarlyOption:
+            return Null()
+
+    return wrap
+
+
 def early_result(function: Callable[P, Result[T, E]]) -> Callable[P, Result[T, E]]:
     """Decorates the `function` returning [`Result[T, E]`][wraps.result.Result]
-    to handle *early returns* via `early` (`?` in Rust) operator.
+    to handle *early returns* via the `early` (`?` in Rust) operator.
 
     Arguments:
         function: The function to wrap.
 
     Returns:
         The wrapping function.
     """
@@ -54,7 +79,29 @@
         try:
             return function(*args, **kwargs)
 
         except EarlyResult[E] as early:
             return Error(early.error)
 
     return wrap
+
+
+def early_result_await(function: AsyncCallable[P, Result[T, E]]) -> AsyncCallable[P, Result[T, E]]:
+    """Decorates the asynchronous `function` returning [`Result[T, E]`][wraps.result.Result]
+    to handle *early returns* via the `early` (`?` in Rust) operator.
+
+    Arguments:
+        function: The asynchronous function to wrap.
+
+    Returns:
+        The asynchronous wrapping function.
+    """
+
+    @wraps(function)
+    async def wrap(*args: P.args, **kwargs: P.kwargs) -> Result[T, E]:
+        try:
+            return await function(*args, **kwargs)
+
+        except EarlyResult[E] as early:
+            return Error(early.error)
+
+    return wrap
```

### Comparing `wraps-0.3.0/wraps/either.py` & `wraps-0.4.0/wraps/either.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+"""Either values.
+
+The [`Either[L, R]`][wraps.either.Either] type is symmetric and treats its variants the same way,
+without preference.
+For representing results (values and errors), use the [`Result[T, E]`][wraps.result.Result] instead.
+"""
+
 from __future__ import annotations
 
 from abc import abstractmethod as required
-from typing import TypeVar, Union
+from typing import AsyncIterator, Iterator, TypeVar, Union
 
 from attrs import frozen
-from iters import AsyncIter, Iter, async_iter, iter
-from typing_extensions import Literal, Never, Protocol, TypeGuard, final
-
-from wraps.errors import panic
-from wraps.option import Null, Option, Some
-from wraps.typing import (
+from funcs.typing import (
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from wraps.utils import identity
+from typing_extensions import Literal, Never, Protocol, TypeGuard, final
+
+from wraps.errors import panic
+from wraps.option import Null, Option, Some
+from wraps.utils import async_empty, async_once, empty, identity, once
 
 __all__ = ("Either", "Left", "Right", "is_left", "is_right")
 
 L = TypeVar("L", covariant=True)
 M = TypeVar("M")
 R = TypeVar("R", covariant=True)
 S = TypeVar("S")
@@ -152,19 +158,19 @@
         ...
 
     @required
     async def map_await(self: EitherProtocol[T, T], function: AsyncUnary[T, U]) -> Either[U, U]:
         ...
 
     @required
-    def map_either(self, left: Unary[L, T], right: Unary[R, T]) -> T:
+    def either(self, left: Unary[L, T], right: Unary[R, T]) -> T:
         ...
 
     @required
-    async def map_either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T:
+    async def either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T:
         ...
 
     @required
     def left_and_then(self, function: Unary[L, Either[M, R]]) -> Either[M, R]:
         ...
 
     @required
@@ -176,35 +182,35 @@
         ...
 
     @required
     async def right_and_then_await(self, function: AsyncUnary[R, Either[L, S]]) -> Either[L, S]:
         ...
 
     @required
-    def iter_left(self) -> Iter[L]:
+    def iter_left(self) -> Iterator[L]:
         ...
 
     @required
-    def iter_right(self) -> Iter[R]:
+    def iter_right(self) -> Iterator[R]:
         ...
 
     @required
-    def iter_either(self: EitherProtocol[T, T]) -> Iter[T]:
+    def iter_either(self: EitherProtocol[T, T]) -> Iterator[T]:
         ...
 
     @required
-    def async_iter_left(self) -> AsyncIter[L]:
+    def async_iter_left(self) -> AsyncIterator[L]:
         ...
 
     @required
-    def async_iter_right(self) -> AsyncIter[R]:
+    def async_iter_right(self) -> AsyncIterator[R]:
         ...
 
     @required
-    def async_iter_either(self: EitherProtocol[T, T]) -> AsyncIter[T]:
+    def async_iter_either(self: EitherProtocol[T, T]) -> AsyncIterator[T]:
         ...
 
     def flatten_left(self: EitherProtocol[EitherProtocol[L, R], R]) -> Either[L, R]:
         return self.left_and_then(identity)  # type: ignore
 
     def flatten_right(self: EitherProtocol[L, EitherProtocol[L, R]]) -> Either[L, R]:
         return self.right_and_then(identity)  # type: ignore
@@ -343,49 +349,49 @@
 
     def map(self: Left[T], function: Unary[T, U]) -> Left[U]:
         return self.create(function(self.value))
 
     async def map_await(self: Left[T], function: AsyncUnary[T, U]) -> Left[U]:
         return self.create(await function(self.value))
 
-    def map_either(self, left: Unary[L, T], right: Unary[R, T]) -> T:
+    def either(self, left: Unary[L, T], right: Unary[R, T]) -> T:
         return left(self.value)
 
-    async def map_either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T:
+    async def either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T:
         return await left(self.value)
 
     def left_and_then(self, function: Unary[L, Either[M, R]]) -> Either[M, R]:
         return function(self.value)
 
     async def left_and_then_await(self, function: AsyncUnary[L, Either[M, R]]) -> Either[M, R]:
         return await function(self.value)
 
     def right_and_then(self, function: Unary[R, Either[L, S]]) -> Left[L]:
         return self
 
     async def right_and_then_await(self, function: AsyncUnary[R, Either[L, S]]) -> Left[L]:
         return self
 
-    def iter_left(self) -> Iter[L]:
-        return iter.once(self.value)
+    def iter_left(self) -> Iterator[L]:
+        return once(self.value)
 
-    def iter_right(self) -> Iter[Never]:
-        return iter.empty()
+    def iter_right(self) -> Iterator[Never]:
+        return empty()
 
-    def iter_either(self: Left[T]) -> Iter[T]:
-        return iter.once(self.value)
+    def iter_either(self: Left[T]) -> Iterator[T]:
+        return once(self.value)
 
-    def async_iter_left(self) -> AsyncIter[L]:
-        return async_iter.once(self.value)
+    def async_iter_left(self) -> AsyncIterator[L]:
+        return async_once(self.value)
 
-    def async_iter_right(self) -> AsyncIter[Never]:
-        return async_iter.empty()
+    def async_iter_right(self) -> AsyncIterator[Never]:
+        return async_empty()
 
-    def async_iter_either(self: Left[T]) -> AsyncIter[T]:
-        return async_iter.once(self.value)
+    def async_iter_either(self: Left[T]) -> AsyncIterator[T]:
+        return async_once(self.value)
 
     def contains_left(self, value: M) -> bool:
         return self.value == value
 
     def contains_right(self, value: S) -> Literal[False]:
         return False
 
@@ -497,49 +503,49 @@
 
     def map(self: Right[T], function: Unary[T, U]) -> Right[U]:
         return self.create(function(self.value))
 
     async def map_await(self: Right[T], function: AsyncUnary[T, U]) -> Right[U]:
         return self.create(await function(self.value))
 
-    def map_either(self, left: Unary[L, T], right: Unary[R, T]) -> T:
+    def either(self, left: Unary[L, T], right: Unary[R, T]) -> T:
         return right(self.value)
 
-    async def map_either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T:
+    async def either_await(self, left: AsyncUnary[L, T], right: AsyncUnary[R, T]) -> T:
         return await right(self.value)
 
     def left_and_then(self, function: Unary[L, Either[M, R]]) -> Right[R]:
         return self
 
     async def left_and_then_await(self, function: AsyncUnary[L, Either[M, R]]) -> Right[R]:
         return self
 
     def right_and_then(self, function: Unary[R, Either[L, S]]) -> Either[L, S]:
         return function(self.value)
 
     async def right_and_then_await(self, function: AsyncUnary[R, Either[L, S]]) -> Either[L, S]:
         return await function(self.value)
 
-    def iter_left(self) -> Iter[Never]:
-        return iter.empty()
+    def iter_left(self) -> Iterator[Never]:
+        return empty()
 
-    def iter_right(self) -> Iter[R]:
-        return iter.once(self.value)
+    def iter_right(self) -> Iterator[R]:
+        return once(self.value)
 
-    def iter_either(self: Right[T]) -> Iter[T]:
-        return iter.once(self.value)
+    def iter_either(self: Right[T]) -> Iterator[T]:
+        return once(self.value)
 
-    def async_iter_left(self) -> AsyncIter[Never]:
-        return async_iter.empty()
+    def async_iter_left(self) -> AsyncIterator[Never]:
+        return async_empty()
 
-    def async_iter_right(self) -> AsyncIter[R]:
-        return async_iter.once(self.value)
+    def async_iter_right(self) -> AsyncIterator[R]:
+        return async_once(self.value)
 
-    def async_iter_either(self: Right[T]) -> AsyncIter[T]:
-        return async_iter.once(self.value)
+    def async_iter_either(self: Right[T]) -> AsyncIterator[T]:
+        return async_once(self.value)
 
     def contains_left(self, value: M) -> Literal[False]:
         return False
 
     def contains_right(self, value: S) -> bool:
         return self.value == value
```

### Comparing `wraps-0.3.0/wraps/future_option.py` & `wraps-0.4.0/wraps/future_option.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,209 +1,211 @@
 from __future__ import annotations
 
-from functools import wraps
-from typing import Awaitable, Callable, TypeVar
+from typing import Awaitable, TypeVar, final
 
-from attrs import field, frozen
-from typing_extensions import Never, ParamSpec
-
-from wraps.future import Future, ReAwaitable, identity
-from wraps.option import Null, Option, Some, is_null, is_some
-from wraps.result import Result
-from wraps.typing import (
+from attrs import frozen
+from funcs.typing import (
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
+from typing_extensions import Never
+
+from wraps.future import Future, ReAwaitable, identity
+from wraps.option import Null, Option, Some, is_null, is_some
+from wraps.result import Result
 
-__all__ = ("FutureOption", "wrap_future_option")
+__all__ = ("FutureOption",)
 
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 
 E = TypeVar("E", covariant=True)
 F = TypeVar("F")
 
 
+@final
 @frozen()
 class FutureOption(Future[Option[T]]):
     """[`Future[Option[T]]`][wraps.future.Future], adapted to leverage future functionality."""
 
-    awaitable: ReAwaitable[Option[T]] = field(repr=False, converter=ReAwaitable)
+    @classmethod
+    def from_awaitable(cls, awaitable: Awaitable[Option[U]]) -> FutureOption[U]:  # type: ignore
+        return cls(ReAwaitable(awaitable))  # type: ignore
 
     @classmethod
-    def create(cls, awaitable: Awaitable[Option[U]]) -> FutureOption[U]:  # type: ignore
-        return cls(awaitable)  # type: ignore
+    def from_option(cls, option: Option[U]) -> FutureOption[U]:
+        return cls.from_value(option)  # type: ignore
 
     @classmethod
     def from_some(cls, value: U) -> FutureOption[U]:
-        return cls.from_value(Some(value))  # type: ignore
+        return cls.from_option(Some(value))
 
     @classmethod
     def from_null(cls) -> FutureOption[Never]:
-        return cls.from_value(Null())  # type: ignore
+        return cls.from_option(Null())
 
     def expect(self, message: str) -> Future[T]:
-        return super().create(self.actual_expect(message))
+        return super().from_awaitable(self.actual_expect(message))
 
     async def actual_expect(self, message: str) -> T:
         return (await self.awaitable).expect(message)
 
     def unwrap(self) -> Future[T]:
-        return super().create(self.actual_unwrap())
+        return super().from_awaitable(self.actual_unwrap())
 
     def unwrap_or(self, default: T) -> Future[T]:  # type: ignore
-        return super().create(self.actual_unwrap_or(default))
+        return super().from_awaitable(self.actual_unwrap_or(default))
 
     def unwrap_or_else(self, default: Nullary[T]) -> Future[T]:
-        return super().create(self.actual_unwrap_or_else(default))
+        return super().from_awaitable(self.actual_unwrap_or_else(default))
 
     def unwrap_or_else_await(self, default: AsyncNullary[T]) -> Future[T]:
-        return super().create(self.actual_unwrap_or_else_await(default))
+        return super().from_awaitable(self.actual_unwrap_or_else_await(default))
 
     async def actual_unwrap(self) -> T:
         return (await self.awaitable).unwrap()
 
     async def actual_unwrap_or(self, default: T) -> T:  # type: ignore
         return (await self.awaitable).unwrap_or(default)
 
     async def actual_unwrap_or_else(self, default: Nullary[T]) -> T:
         return (await self.awaitable).unwrap_or_else(default)
 
     async def actual_unwrap_or_else_await(self, default: AsyncNullary[T]) -> T:
         return await (await self.awaitable).unwrap_or_else_await(default)
 
     def inspect(self, function: Inspect[T]) -> FutureOption[T]:
-        return self.create(self.actual_inspect(function))
+        return self.from_awaitable(self.actual_inspect(function))
 
     def inspect_await(self, function: AsyncInspect[T]) -> FutureOption[T]:
-        return self.create(self.actual_inspect_await(function))
+        return self.from_awaitable(self.actual_inspect_await(function))
 
     async def actual_inspect(self, function: Inspect[T]) -> Option[T]:
         return (await self.awaitable).inspect(function)
 
     async def actual_inspect_await(self, function: AsyncInspect[T]) -> Option[T]:
-        return await (await self.awaitable).inspect_await(function)  # type: ignore
+        return await (await self.awaitable).inspect_await(function)
 
     def map(self, function: Unary[T, U]) -> FutureOption[U]:
-        return self.create(self.actual_map(function))
+        return self.from_awaitable(self.actual_map(function))
 
     def map_or(self, default: U, function: Unary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_or(default, function))
+        return super().from_awaitable(self.actual_map_or(default, function))
 
     def map_or_else(self, default: Nullary[U], function: Unary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_or_else(default, function))
+        return super().from_awaitable(self.actual_map_or_else(default, function))
 
     def map_or_else_await(self, default: AsyncNullary[U], function: Unary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_or_else_await(default, function))
+        return super().from_awaitable(self.actual_map_or_else_await(default, function))
 
     def map_await(self, function: AsyncUnary[T, U]) -> FutureOption[U]:
-        return self.create(self.actual_map_await(function))
+        return self.from_awaitable(self.actual_map_await(function))
 
     def map_await_or(self, default: U, function: AsyncUnary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_await_or(default, function))
+        return super().from_awaitable(self.actual_map_await_or(default, function))
 
     def map_await_or_else(self, default: Nullary[U], function: AsyncUnary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_await_or_else(default, function))
+        return super().from_awaitable(self.actual_map_await_or_else(default, function))
 
     def map_await_or_else_await(
         self, default: AsyncNullary[U], function: AsyncUnary[T, U]
     ) -> Future[U]:
-        return super().create(self.actual_map_await_or_else_await(default, function))
+        return super().from_awaitable(self.actual_map_await_or_else_await(default, function))
 
     async def actual_map(self, function: Unary[T, U]) -> Option[U]:
         return (await self.awaitable).map(function)
 
     async def actual_map_or(self, default: U, function: Unary[T, U]) -> U:
         return (await self.awaitable).map_or(default, function)
 
     async def actual_map_or_else(self, default: Nullary[U], function: Unary[T, U]) -> U:
         return (await self.awaitable).map_or_else(default, function)
 
     async def actual_map_or_else_await(self, default: AsyncNullary[U], function: Unary[T, U]) -> U:
         return await (await self.awaitable).map_or_else_await(default, function)
 
     async def actual_map_await(self, function: AsyncUnary[T, U]) -> Option[U]:
-        return await (await self.awaitable).map_await(function)  # type: ignore
+        return await (await self.awaitable).map_await(function)
 
     async def actual_map_await_or(self, default: U, function: AsyncUnary[T, U]) -> U:
         return await (await self.awaitable).map_await_or(default, function)
 
     async def actual_map_await_or_else(self, default: Nullary[U], function: AsyncUnary[T, U]) -> U:
         return await (await self.awaitable).map_await_or_else(default, function)
 
     async def actual_map_await_or_else_await(
         self, default: AsyncNullary[U], function: AsyncUnary[T, U]
     ) -> U:
         return await (await self.awaitable).map_await_or_else_await(default, function)
 
     def ok_or(self, error: F) -> FutureResult[T, F]:
-        return FutureResult.create(self.actual_ok_or(error))
+        return FutureResult.from_awaitable(self.actual_ok_or(error))
 
     def ok_or_else(self, error: Nullary[E]) -> FutureResult[T, E]:
-        return FutureResult.create(self.actual_ok_or_else(error))
+        return FutureResult.from_awaitable(self.actual_ok_or_else(error))
 
     def ok_or_else_await(self, error: AsyncNullary[E]) -> FutureResult[T, E]:
-        return FutureResult.create(self.actual_ok_or_else_await(error))
+        return FutureResult.from_awaitable(self.actual_ok_or_else_await(error))
 
     async def actual_ok_or(self, error: E) -> Result[T, E]:  # type: ignore
         return (await self.awaitable).ok_or(error)
 
     async def actual_ok_or_else(self, error: Nullary[E]) -> Result[T, E]:
         return (await self.awaitable).ok_or_else(error)
 
     async def actual_ok_or_else_await(self, error: AsyncNullary[E]) -> Result[T, E]:
-        return await (await self.awaitable).ok_or_else_await(error)  # type: ignore
+        return await (await self.awaitable).ok_or_else_await(error)
 
     def and_then(self, function: Unary[T, Option[U]]) -> FutureOption[U]:
-        return self.create(self.actual_and_then(function))
+        return self.from_awaitable(self.actual_and_then(function))
 
     def and_then_await(self, function: AsyncUnary[T, Option[U]]) -> FutureOption[U]:
-        return self.create(self.actual_and_then_await(function))
+        return self.from_awaitable(self.actual_and_then_await(function))
 
     def or_else(self, function: Nullary[Option[T]]) -> FutureOption[T]:
-        return self.create(self.actual_or_else(function))
+        return self.from_awaitable(self.actual_or_else(function))
 
     def or_else_await(self, function: AsyncNullary[Option[T]]) -> FutureOption[T]:
-        return self.create(self.actual_or_else_await(function))
+        return self.from_awaitable(self.actual_or_else_await(function))
 
     async def actual_and_then(self, function: Unary[T, Option[U]]) -> Option[U]:
         return (await self.awaitable).and_then(function)
 
     async def actual_and_then_await(self, function: AsyncUnary[T, Option[U]]) -> Option[U]:
         return await (await self.awaitable).and_then_await(function)
 
     async def actual_or_else(self, function: Nullary[Option[T]]) -> Option[T]:
         return (await self.awaitable).or_else(function)
 
     async def actual_or_else_await(self, function: AsyncNullary[Option[T]]) -> Option[T]:
         return await (await self.awaitable).or_else_await(function)
 
     def filter(self, predicate: Predicate[T]) -> FutureOption[T]:
-        return self.create(self.actual_filter(predicate))
+        return self.from_awaitable(self.actual_filter(predicate))
 
     def filter_await(self, predicate: AsyncPredicate[T]) -> FutureOption[T]:
-        return self.create(self.actual_filter_await(predicate))
+        return self.from_awaitable(self.actual_filter_await(predicate))
 
     async def actual_filter(self, predicate: Predicate[T]) -> Option[T]:
         return (await self.awaitable).filter(predicate)
 
     async def actual_filter_await(self, predicate: AsyncPredicate[T]) -> Option[T]:
         return await (await self.awaitable).filter_await(predicate)
 
     def and_then_future(self, function: Unary[T, FutureOption[U]]) -> FutureOption[U]:
-        return self.create(self.actual_and_then_future(function))
+        return self.from_awaitable(self.actual_and_then_future(function))
 
     def or_else_future(self, function: Nullary[FutureOption[T]]) -> FutureOption[T]:
-        return self.create(self.actual_or_else_future(function))
+        return self.from_awaitable(self.actual_or_else_future(function))
 
     async def actual_and_then_future(self, function: Unary[T, FutureOption[U]]) -> Option[U]:
         option = await self.awaitable
 
         if is_some(option):
             return await function(option.unwrap())
 
@@ -217,50 +219,8 @@
 
         return option
 
     def flatten(self: FutureOption[FutureOption[U]]) -> FutureOption[U]:
         return self.and_then_future(identity)
 
 
-P = ParamSpec("P")
-
-
-def wrap_future_option(function: Callable[P, Awaitable[T]]) -> Callable[P, FutureOption[T]]:
-    """Wraps an asynchronous `function` returning `T` into a function
-    returning [`FutureOption[T]`][wraps.future_option.FutureOption].
-
-    This handles all exceptions via returning [`Null`][wraps.option.Null] on errors,
-    wrapping the resulting `value` into [`Some(value)`][wraps.option.Some].
-
-    Example:
-        ```python
-        @wrap_future_option
-        async def identity(value: T) -> T:
-            return value
-
-        value = 42
-
-        assert await identity(value).unwrap() == value
-        ```
-
-    Arguments:
-        function: The asynchronous function to wrap.
-
-    Returns:
-        The wrapping function.
-    """
-
-    async def wrapping(*args: P.args, **kwargs: P.kwargs) -> Option[T]:
-        try:
-            return Some(await function(*args, **kwargs))
-
-        except Exception:
-            return Null()
-
-    @wraps(function)
-    def wrap(*args: P.args, **kwargs: P.kwargs) -> FutureOption[T]:
-        return FutureOption(wrapping(*args, **kwargs))  # type: ignore
-
-    return wrap
-
-
 from wraps.future_result import FutureResult
```

### Comparing `wraps-0.3.0/wraps/future_result.py` & `wraps-0.4.0/wraps/future_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,173 @@
 from __future__ import annotations
 
-from functools import wraps
-from typing import Awaitable, Callable, TypeVar
+from typing import Awaitable, TypeVar, final
 
-from attrs import field, frozen
-from typing_extensions import Never, ParamSpec
+from attrs import frozen
+from funcs.typing import AsyncInspect, AsyncNullary, AsyncUnary, Inspect, Nullary, Unary
+from typing_extensions import Never
 
-from wraps.future import Future, ReAwaitable
+from wraps.future import Future
 from wraps.option import Option
+from wraps.reawaitable import ReAwaitable
 from wraps.result import Error, Ok, Result, is_error, is_ok
-from wraps.typing import AsyncInspect, AsyncNullary, AsyncUnary, Inspect, Nullary, Unary
 from wraps.utils import identity
 
+__all__ = ("FutureResult",)
+
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 
 E = TypeVar("E", covariant=True)
 F = TypeVar("F")
 
 
 V = TypeVar("V")
 
 
+@final
 @frozen()
 class FutureResult(Future[Result[T, E]]):
     """[`Future[Result[T, E]]`][wraps.future.Future], adapted to leverage future functionality."""
 
-    awaitable: ReAwaitable[Result[T, E]] = field(repr=False, converter=ReAwaitable)
+    @classmethod
+    def from_awaitable(cls, awaitable: Awaitable[Result[U, F]]) -> FutureResult[U, F]:  # type: ignore
+        return cls(ReAwaitable(awaitable))  # type: ignore
 
     @classmethod
-    def create(cls, awaitable: Awaitable[Result[U, F]]) -> FutureResult[U, F]:  # type: ignore
-        return cls(awaitable)  # type: ignore
+    def from_result(cls, result: Result[U, F]) -> FutureResult[U, F]:
+        return cls.from_value(result)  # type: ignore
 
     @classmethod
     def from_ok(cls, value: U) -> FutureResult[U, Never]:
-        return cls.from_value(Ok(value))  # type: ignore
+        return cls.from_result(Ok(value))
 
     @classmethod
     def from_error(cls, value: F) -> FutureResult[Never, F]:
-        return cls.from_value(Error(value))  # type: ignore
+        return cls.from_result(Error(value))
 
     def expect(self, message: str) -> Future[T]:
-        return super().create(self.actual_expect(message))
+        return super().from_awaitable(self.actual_expect(message))
 
     def expect_error(self, message: str) -> Future[E]:
-        return super().create(self.actual_expect_error(message))
+        return super().from_awaitable(self.actual_expect_error(message))
 
     async def actual_expect(self, message: str) -> T:
         return (await self.awaitable).expect(message)
 
     async def actual_expect_error(self, message: str) -> E:
         return (await self.awaitable).expect_error(message)
 
     def unwrap(self) -> Future[T]:
-        return super().create(self.actual_unwrap())
+        return super().from_awaitable(self.actual_unwrap())
 
     def unwrap_or(self, default: T) -> Future[T]:  # type: ignore
-        return super().create(self.actual_unwrap_or(default))
+        return super().from_awaitable(self.actual_unwrap_or(default))
 
     def unwrap_or_else(self, default: Nullary[T]) -> Future[T]:
-        return super().create(self.actual_unwrap_or_else(default))
+        return super().from_awaitable(self.actual_unwrap_or_else(default))
 
     def unwrap_or_else_await(self, default: AsyncNullary[T]) -> Future[T]:
-        return super().create(self.actual_unwrap_or_else_await(default))
+        return super().from_awaitable(self.actual_unwrap_or_else_await(default))
 
     async def actual_unwrap(self) -> T:
         return (await self.awaitable).unwrap()
 
     async def actual_unwrap_or(self, default: T) -> T:  # type: ignore
         return (await self.awaitable).unwrap_or(default)
 
     async def actual_unwrap_or_else(self, default: Nullary[T]) -> T:
         return (await self.awaitable).unwrap_or_else(default)
 
     async def actual_unwrap_or_else_await(self, default: AsyncNullary[T]) -> T:
         return await (await self.awaitable).unwrap_or_else_await(default)
 
     def unwrap_error(self) -> Future[E]:
-        return super().create(self.actual_unwrap_error())
+        return super().from_awaitable(self.actual_unwrap_error())
 
     def unwrap_error_or(self, default: E) -> Future[E]:  # type: ignore
-        return super().create(self.actual_unwrap_error_or(default))
+        return super().from_awaitable(self.actual_unwrap_error_or(default))
 
     def unwrap_error_or_else(self, default: Nullary[E]) -> Future[E]:
-        return super().create(self.actual_unwrap_error_or_else(default))
+        return super().from_awaitable(self.actual_unwrap_error_or_else(default))
 
     def unwrap_error_or_else_await(self, default: AsyncNullary[E]) -> Future[E]:
-        return super().create(self.actual_unwrap_error_or_else_await(default))
+        return super().from_awaitable(self.actual_unwrap_error_or_else_await(default))
 
     async def actual_unwrap_error(self) -> E:
         return (await self.awaitable).unwrap_error()
 
     async def actual_unwrap_error_or(self, default: E) -> E:  # type: ignore
         return (await self.awaitable).unwrap_error_or(default)
 
     async def actual_unwrap_error_or_else(self, default: Nullary[E]) -> E:
         return (await self.awaitable).unwrap_error_or_else(default)
 
     async def actual_unwrap_error_or_else_await(self, default: AsyncNullary[E]) -> E:
         return await (await self.awaitable).unwrap_error_or_else_await(default)
 
     def ok(self) -> FutureOption[T]:
-        return FutureOption.create(self.actual_ok())
+        return FutureOption.from_awaitable(self.actual_ok())
 
     def error(self) -> FutureOption[E]:
-        return FutureOption.create(self.actual_error())
+        return FutureOption.from_awaitable(self.actual_error())
 
     async def actual_ok(self) -> Option[T]:
         return (await self.awaitable).ok()
 
     async def actual_error(self) -> Option[E]:
         return (await self.awaitable).error()
 
     def inspect(self, function: Inspect[T]) -> FutureResult[T, E]:
-        return self.create(self.actual_inspect(function))
+        return self.from_awaitable(self.actual_inspect(function))
 
     def inspect_error(self, function: Inspect[E]) -> FutureResult[T, E]:
-        return self.create(self.actual_inspect_error(function))
+        return self.from_awaitable(self.actual_inspect_error(function))
 
     def inspect_await(self, function: AsyncInspect[T]) -> FutureResult[T, E]:
-        return self.create(self.actual_inspect_await(function))
+        return self.from_awaitable(self.actual_inspect_await(function))
 
     def inspect_error_await(self, function: AsyncInspect[E]) -> FutureResult[T, E]:
-        return self.create(self.actual_inspect_error_await(function))
+        return self.from_awaitable(self.actual_inspect_error_await(function))
 
     async def actual_inspect(self, function: Inspect[T]) -> Result[T, E]:
         return (await self.awaitable).inspect(function)
 
     async def actual_inspect_error(self, function: Inspect[E]) -> Result[T, E]:
         return (await self.awaitable).inspect_error(function)
 
     async def actual_inspect_await(self, function: AsyncInspect[T]) -> Result[T, E]:
-        return await (await self.awaitable).inspect_await(function)  # type: ignore
+        return await (await self.awaitable).inspect_await(function)
 
     async def actual_inspect_error_await(self, function: AsyncInspect[E]) -> Result[T, E]:
-        return await (await self.awaitable).inspect_error_await(function)  # type: ignore
+        return await (await self.awaitable).inspect_error_await(function)
 
     def map(self, function: Unary[T, U]) -> FutureResult[U, E]:
-        return self.create(self.actual_map(function))
+        return self.from_awaitable(self.actual_map(function))
 
     def map_or(self, default: U, function: Unary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_or(default, function))
+        return super().from_awaitable(self.actual_map_or(default, function))
 
     def map_or_else(self, default: Nullary[U], function: Unary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_or_else(default, function))
+        return super().from_awaitable(self.actual_map_or_else(default, function))
 
     def map_or_else_await(self, default: AsyncNullary[U], function: Unary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_or_else_await(default, function))
+        return super().from_awaitable(self.actual_map_or_else_await(default, function))
 
     def map_error(self, function: Unary[E, F]) -> FutureResult[T, F]:
-        return self.create(self.actual_map_error(function))
+        return self.from_awaitable(self.actual_map_error(function))
 
     def map_error_or(self, default: F, function: Unary[E, F]) -> Future[F]:
-        return super().create(self.actual_map_error_or(default, function))
+        return super().from_awaitable(self.actual_map_error_or(default, function))
 
     def map_error_or_else(self, default: Nullary[F], function: Unary[E, F]) -> Future[F]:
-        return super().create(self.actual_map_error_or_else(default, function))
+        return super().from_awaitable(self.actual_map_error_or_else(default, function))
 
     def map_error_or_else_await(self, default: AsyncNullary[F], function: Unary[E, F]) -> Future[F]:
-        return super().create(self.actual_map_error_or_else_await(default, function))
+        return super().from_awaitable(self.actual_map_error_or_else_await(default, function))
 
     async def actual_map(self, function: Unary[T, U]) -> Result[U, E]:
         return (await self.awaitable).map(function)
 
     async def actual_map_or(self, default: U, function: Unary[T, U]) -> U:
         return (await self.awaitable).map_or(default, function)
 
@@ -183,57 +188,57 @@
 
     async def actual_map_error_or_else_await(
         self, default: AsyncNullary[F], function: Unary[E, F]
     ) -> F:
         return await (await self.awaitable).map_error_or_else_await(default, function)
 
     def map_await(self, function: AsyncUnary[T, U]) -> FutureResult[U, E]:
-        return self.create(self.actual_map_await(function))
+        return self.from_awaitable(self.actual_map_await(function))
 
     def map_await_or(self, default: U, function: AsyncUnary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_await_or(default, function))
+        return super().from_awaitable(self.actual_map_await_or(default, function))
 
     def map_await_or_else(self, default: Nullary[U], function: AsyncUnary[T, U]) -> Future[U]:
-        return super().create(self.actual_map_await_or_else(default, function))
+        return super().from_awaitable(self.actual_map_await_or_else(default, function))
 
     def map_await_or_else_await(
         self, default: AsyncNullary[U], function: AsyncUnary[T, U]
     ) -> Future[U]:
-        return super().create(self.actual_map_await_or_else_await(default, function))
+        return super().from_awaitable(self.actual_map_await_or_else_await(default, function))
 
     def map_error_await(self, function: AsyncUnary[E, F]) -> FutureResult[T, F]:
-        return self.create(self.actual_map_error_await(function))
+        return self.from_awaitable(self.actual_map_error_await(function))
 
     def map_error_await_or(self, default: F, function: AsyncUnary[E, F]) -> Future[F]:
-        return super().create(self.actual_map_error_await_or(default, function))
+        return super().from_awaitable(self.actual_map_error_await_or(default, function))
 
     def map_error_await_or_else(self, default: Nullary[F], function: AsyncUnary[E, F]) -> Future[F]:
-        return super().create(self.actual_map_error_await_or_else(default, function))
+        return super().from_awaitable(self.actual_map_error_await_or_else(default, function))
 
     def map_error_await_or_else_await(
         self, default: AsyncNullary[F], function: AsyncUnary[E, F]
     ) -> Future[F]:
-        return super().create(self.actual_map_error_await_or_else_await(default, function))
+        return super().from_awaitable(self.actual_map_error_await_or_else_await(default, function))
 
     async def actual_map_await(self, function: AsyncUnary[T, U]) -> Result[U, E]:
-        return await (await self.awaitable).map_await(function)  # type: ignore
+        return await (await self.awaitable).map_await(function)
 
     async def actual_map_await_or(self, default: U, function: AsyncUnary[T, U]) -> U:
         return await (await self.awaitable).map_await_or(default, function)
 
     async def actual_map_await_or_else(self, default: Nullary[U], function: AsyncUnary[T, U]) -> U:
         return await (await self.awaitable).map_await_or_else(default, function)
 
     async def actual_map_await_or_else_await(
         self, default: AsyncNullary[U], function: AsyncUnary[T, U]
     ) -> U:
         return await (await self.awaitable).map_await_or_else_await(default, function)
 
     async def actual_map_error_await(self, function: AsyncUnary[E, F]) -> Result[T, F]:
-        return await (await self.awaitable).map_error_await(function)  # type: ignore
+        return await (await self.awaitable).map_error_await(function)
 
     async def actual_map_error_await_or(self, default: F, function: AsyncUnary[E, F]) -> F:
         return await (await self.awaitable).map_error_await_or(default, function)
 
     async def actual_map_error_await_or_else(
         self, default: Nullary[F], function: AsyncUnary[E, F]
     ) -> F:
@@ -241,42 +246,42 @@
 
     async def actual_map_error_await_or_else_await(
         self, default: AsyncNullary[F], function: AsyncUnary[E, F]
     ) -> F:
         return await (await self.awaitable).map_error_await_or_else_await(default, function)
 
     def and_then(self, function: Unary[T, Result[U, E]]) -> FutureResult[U, E]:
-        return self.create(self.actual_and_then(function))
+        return self.from_awaitable(self.actual_and_then(function))
 
     def and_then_await(self, function: AsyncUnary[T, Result[U, E]]) -> FutureResult[U, E]:
-        return self.create(self.actual_and_then_await(function))
+        return self.from_awaitable(self.actual_and_then_await(function))
 
     def or_else(self, function: Unary[E, Result[T, F]]) -> FutureResult[T, F]:
-        return self.create(self.actual_or_else(function))
+        return self.from_awaitable(self.actual_or_else(function))
 
     def or_else_await(self, function: AsyncUnary[E, Result[T, F]]) -> FutureResult[T, F]:
-        return self.create(self.actual_or_else_await(function))
+        return self.from_awaitable(self.actual_or_else_await(function))
 
     async def actual_and_then(self, function: Unary[T, Result[U, E]]) -> Result[U, E]:
         return (await self.awaitable).and_then(function)
 
     async def actual_and_then_await(self, function: AsyncUnary[T, Result[U, E]]) -> Result[U, E]:
         return await (await self.awaitable).and_then_await(function)
 
     async def actual_or_else(self, function: Unary[E, Result[T, F]]) -> Result[T, F]:
         return (await self.awaitable).or_else(function)
 
     async def actual_or_else_await(self, function: AsyncUnary[E, Result[T, F]]) -> Result[T, F]:
         return await (await self.awaitable).or_else_await(function)
 
     def and_then_future(self, function: Unary[T, FutureResult[U, E]]) -> FutureResult[U, E]:
-        return self.create(self.actual_and_then_future(function))
+        return self.from_awaitable(self.actual_and_then_future(function))
 
     def or_else_future(self, function: Unary[E, FutureResult[T, F]]) -> FutureResult[T, F]:
-        return self.create(self.actual_or_else_future(function))
+        return self.from_awaitable(self.actual_or_else_future(function))
 
     async def actual_and_then_future(self, function: Unary[T, FutureResult[U, E]]) -> Result[U, E]:
         result = await self.awaitable
 
         if is_ok(result):
             return await function(result.unwrap())
 
@@ -293,67 +298,23 @@
     def try_flatten(self: FutureResult[FutureResult[T, E], E]) -> FutureResult[T, E]:
         return self.and_then_future(identity)
 
     def try_flatten_error(self: FutureResult[T, FutureResult[T, E]]) -> FutureResult[T, E]:
         return self.or_else_future(identity)
 
     def flip(self) -> FutureResult[E, T]:
-        return self.create(self.actual_flip())
+        return self.from_awaitable(self.actual_flip())
 
     async def actual_flip(self) -> Result[E, T]:
         return (await self.awaitable).flip()
 
     def into_ok_or_error(self: FutureResult[T, T]) -> Future[T]:
-        return super().create(self.actual_into_ok_or_error())
+        return super().from_awaitable(self.actual_into_ok_or_error())
 
     async def actual_into_ok_or_error(self: FutureResult[T, T]) -> T:
         return (await self.awaitable).into_ok_or_error()
 
     def into_future(self) -> Future[Result[T, E]]:
-        return super().create(self.awaitable)
-
-
-P = ParamSpec("P")
-
-
-def wrap_future_result(
-    function: Callable[P, Awaitable[T]]
-) -> Callable[P, FutureResult[T, Exception]]:
-    """Wraps an asynchronous `function` returning `T` into a function returning
-    [`FutureResult[T, Exception]`][wraps.future_result.FutureResult].
-
-    This handles exceptions via returning [`Error(error)`][wraps.result.Error] on `error`,
-    wrapping the resulting `value` into [`Ok(value)`][wraps.result.Ok].
-
-    Example:
-        ```python
-        @wrap_future_result
-        async def identity(value: T) -> T:
-            return value
-
-        value = 13
-
-        assert await identity(value).unwrap() == value
-        ```
-
-    Arguments:
-        function: The asynchronous function to wrap.
-
-    Returns:
-        The wrapping function.
-    """
-
-    async def wrapping(*args: P.args, **kwargs: P.kwargs) -> Result[T, Exception]:
-        try:
-            return Ok(await function(*args, **kwargs))
-
-        except Exception as error:
-            return Error(error)
-
-    @wraps(function)
-    def wrap(*args: P.args, **kwargs: P.kwargs) -> FutureResult[T, Exception]:
-        return FutureResult(wrapping(*args, **kwargs))  # type: ignore
-
-    return wrap
+        return super().from_awaitable(self.awaitable)
 
 
 from wraps.future_option import FutureOption
```

### Comparing `wraps-0.3.0/wraps/option.py` & `wraps-0.4.0/wraps/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,97 @@
 """Optional values.
 
 [`Option[T]`][wraps.option.Option] represents an optional value:
 every [`Option[T]`][wraps.option.Option] is either [`Some[T]`][wraps.option.Some] and
-contains a value (of type `T`), or [`Null`][wraps.option.Null], and does not.
+contains a value, or [`Null`][wraps.option.Null], and does not.
 
 [`Option[T]`][wraps.option.Option] types can be very common in python code,
 as they have a number of uses:
 
-- Initial values (see [`ReAwaitable[T]`][wraps.future.ReAwaitable]);
+- Initial values (see [`ReAwaitable[T]`][wraps.reawaitable.ReAwaitable]);
 - Return values for functions not defined over their entire input range (partial functions);
 - Return value for otherwise reporting simple errors, where [`Null`][wraps.option.Null]
   is returned on error;
 - Optional function arguments.
 
 [`Option[T]`][wraps.option.Option] is commonly paired with pattern matching to query
 the presence of [`Some[T]`][wraps.option.Some] value (`T`) and take action,
 always accounting for the [`Null`][wraps.option.Null] case:
 
 ```python
-from wraps import wrap_option
+# option.py
 
-@wrap_option
-def divide(numerator: float, denominator: float) -> float:
-    return numerator / denominator
+from wraps import Null, Option, Some
+
+
+def divide(numerator: float, denominator: float) -> Option[float]:
+    return Some(numerator / denominator) if denominator else Null()
 ```
 
 ```python
 from wraps import Null, Some
 
-CAN_NOT_DIVIDE_BY_ZERO = "can not divide by zero"
+from option import divide
+
+DIVISION_BY_ZERO = "division by zero"
 
 option = divide(1.0, 2.0)
 
 match option:
     case Some(result):
         print(result)
 
     case Null():
-        print(CAN_NOT_DIVIDE_BY_ZERO)
+        print(DIVISION_BY_ZERO)
 ```
+
+Her, we know that [`Null`][wraps.option.Null] represents only one case,
+that is, attempts to divide by zero. However, when we need to represent multiple errors
+from one function, we might want to use [`Result[T, E]`][wraps.result.Result] instead,
+as described in the [`result`][wraps.result] section.
 """
 
 from __future__ import annotations
 
 from abc import abstractmethod as required
-from typing import (
-    AsyncIterator,
-    Awaitable,
-    Callable,
-    Iterator,
-    Optional,
-    Tuple,
-    TypeVar,
-    Union,
-    final,
-    overload,
-)
+from typing import AsyncIterator, Iterator, Optional, Tuple, TypeVar, Union, final, overload
 
 from attrs import frozen
-from typing_extensions import Literal, Never, ParamSpec, Protocol, TypeGuard
-
-from wraps.errors import EarlyOption, panic
-from wraps.typing import (
+from funcs.typing import (
     AsyncBinary,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Binary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
-from wraps.utils import identity
+from typing_extensions import Literal, Never, Protocol, TypeGuard
 
-__all__ = (
-    "Option",
-    "Some",
-    "Null",
-    "is_some",
-    "is_null",
-    "wrap_option",
-    "wrap_option_await",
-    "wrap_optional",
-)
+from wraps.errors import EarlyOption, panic
+from wraps.utils import async_empty, async_once, empty, identity, once
 
-P = ParamSpec("P")
+__all__ = ("Option", "Some", "Null", "is_some", "is_null")
 
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 V = TypeVar("V")
 
 E = TypeVar("E")
 
 
 class OptionProtocol(Protocol[T]):  # type: ignore[misc]
     def __iter__(self) -> Iterator[T]:
-        return self.iter().unwrap()
+        return self.iter()
 
     def __aiter__(self) -> AsyncIterator[T]:
-        return self.async_iter().unwrap()
+        return self.async_iter()
 
     @required
     def is_some(self) -> bool:
         """Checks if the option is [`Some[T]`][wraps.option.Some].
 
         Example:
             ```python
@@ -137,15 +124,15 @@
             assert not zero.is_some_and(is_positive)
 
             null = Null()
             assert not null.is_some_and(is_positive)
             ```
 
         Arguments:
-            predicate: The predicate to check the contained value against.
+            predicate: The predicate to check the possibly contained value against.
 
         Returns:
             Whether the option is [`Some[T]`][wraps.option.Some] and the predicate is matched.
         """
         ...
 
     @required
@@ -165,15 +152,15 @@
             assert not await zero.is_some_and_await(is_negative)
 
             null = Null()
             assert not await null.is_some_and_await(is_negative)
             ```
 
         Arguments:
-            predicate: The asynchronous predicate to check the contained value against.
+            predicate: The asynchronous predicate to check the possibly contained value against.
 
         Returns:
             Whether the option is [`Some[T]`][wraps.option.Some] and
             the asynchronous predicate is matched.
         """
         ...
 
@@ -208,15 +195,15 @@
             >>> null.expect("panic!")
             Traceback (most recent call last):
               ...
             wraps.errors.Panic: panic!
             ```
 
         Arguments:
-            message: The message used in panicking.
+            message: The message to use in panicking.
 
         Raises:
             Panic: Panics with the `message` if the option is [`Null`][wraps.option.Null].
 
         Returns:
             The contained value.
         """
@@ -227,18 +214,17 @@
         """Returns the contained [`Some[T]`][wraps.option.Some] value or [`None`][None].
 
         Example:
             ```python
             >>> some = Some(42)
             >>> some.extract()
             42
-
             >>> null = Null()
             >>> null.extract()
-            >>>
+            >>> # None
             ```
 
         Returns:
             The contained value or [`None`][None].
         """
         ...
 
@@ -253,15 +239,14 @@
         or [`unwrap_or_else`][wraps.option.OptionProtocol.unwrap_or_else].
 
         Example:
             ```python
             >>> some = Some(42)
             >>> some.unwrap()
             42
-
             >>> null = Null()
             >>> null.unwrap()
             Traceback (most recent call last):
               ...
             wraps.errors.Panic: called `unwrap` on null
             ```
 
@@ -271,76 +256,74 @@
         Returns:
             The contained value.
         """
         ...
 
     @required
     def unwrap_or(self, default: T) -> T:  # type: ignore
-        """Returns the contained [`Some[T]`][wraps.option.Some] value or a provided default.
+        """Returns the contained [`Some[T]`][wraps.option.Some] value or the provided `default`.
 
         Example:
             ```python
-            default = 0
-
             some = Some(13)
-            assert some.unwrap_or(default)
+            assert some.unwrap_or(0)
 
             null = Null()
-            assert not null.unwrap_or(default)
+            assert not null.unwrap_or(0)
             ```
 
         Arguments:
             default: The default value to use.
 
         Returns:
             The contained value or the `default` one.
         """
         ...
 
     @required
     def unwrap_or_else(self, default: Nullary[T]) -> T:
         """Returns the contained [`Some[T]`][wraps.option.Some] value or
-        computes it from the function.
+        computes it from the `default` function.
 
         Example:
             ```python
             some = Some(13)
             assert some.unwrap_or_else(int)
 
             null = Null()
             assert not null.unwrap_or_else(int)
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
 
         Returns:
             The contained value or the `default()` one.
         """
         ...
 
     @required
     async def unwrap_or_else_await(self, default: AsyncNullary[T]) -> T:
         """Returns the contained [`Some[T]`][wraps.option.Some] value
-        or computes it from the asynchronous function.
+        or computes it from the asynchronous `default` function.
 
         Example:
             ```python
             async def default() -> int:
                 return 0
 
             some = Some(42)
             assert await some.unwrap_or_else_await(default)
 
             null = Null()
             assert not await null.unwrap_or_else_await(default)
             ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
 
         Returns:
             The contained value or the `await default()` one.
         """
         ...
 
     @required
@@ -386,15 +369,15 @@
         Returns:
             The inspected option.
         """
         ...
 
     @required
     def map(self, function: Unary[T, U]) -> Option[U]:
-        """Maps an [`Option[T]`][wraps.option.Option] to [`Option[U]`][wraps.option.Option]
+        """Maps an [`Option[T]`][wraps.option.Option] to an [`Option[U]`][wraps.option.Option]
         by applying the `function` to the contained value.
 
         Example:
             ```python
             some = Some("Hello, world!")
 
             print(some.map(len).unwrap())  # 13
@@ -406,15 +389,15 @@
         Returns:
             The mapped option.
         """
         ...
 
     @required
     def map_or(self, default: U, function: Unary[T, U]) -> U:
-        """Returns the default value (if none), or applies the `function`
+        """Returns the `default` value (if none), or applies the `function`
         to the contained value (if any).
 
         Example:
             ```python
             some = Some("nekit")
 
             print(some.map_or(42, len))  # 5
@@ -425,22 +408,22 @@
             ```
 
         Arguments:
             default: The default value to use.
             function: The function to apply.
 
         Returns:
-            The resulting or the default value.
+            The resulting value or the `default` one.
         """
         ...
 
     @required
     def map_or_else(self, default: Nullary[U], function: Unary[T, U]) -> U:
-        """Computes the default value (if none), or applies the `function`
-        to the contained value (if any).
+        """Computes the default value from the `default` function (if none),
+        or applies the `function` to the contained value (if any).
 
         Example:
             ```python
             def default() -> int:
                 return 42
 
             some = Some("Hello, world!")
@@ -449,26 +432,26 @@
 
             null = Null()
 
             print(null.map_or_else(default, len))  # 42
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
             function: The function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting value or the `default()` one.
         """
         ...
 
     @required
     async def map_or_else_await(self, default: AsyncNullary[U], function: Unary[T, U]) -> U:
-        """Computes the default value (if none), or applies the `function`
-        to the contained value (if any).
+        """Computes the default value from the asynchronous `default` function (if none),
+        or applies the `function` to the contained value (if any).
 
         Example:
             ```python
             async def default() -> int:
                 return 42
 
             some = Some("Hello, world!")
@@ -477,100 +460,103 @@
 
             null = Null()
 
             print(await null.map_or_else_await(default, len))  # 42
             ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
             function: The function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting value or the `await default()` one.
         """
         ...
 
     @required
     async def map_await(self, function: AsyncUnary[T, U]) -> Option[U]:
-        """Maps an [`Option[T]`][wraps.option.Option] to [`Option[U]`][wraps.option.Option]
+        """Maps an [`Option[T]`][wraps.option.Option] to an [`Option[U]`][wraps.option.Option]
         by applying the asynchronous `function` to the contained value.
 
         Example:
             ```python
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
             some = Some("Hello, world!")
 
-            mapped = await some.map_await(async_len)
+            mapped = await some.map_await(function)
 
             print(some.unwrap())  # 13
             ```
 
         Arguments:
             function: The asynchronous function to apply.
 
         Returns:
             The mapped option.
         """
         ...
 
     @required
     async def map_await_or(self, default: U, function: AsyncUnary[T, U]) -> U:
-        """Returns the default value (if none), or applies the asynchronous `function`
+        """Returns the `default` value (if none), or applies the asynchronous `function`
         to the contained value (if any).
 
         Example:
             ```python
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
             some = Some("nekit")
 
-            print(await some.map_await_or(42, async_len))  # 5
+            print(await some.map_await_or(42, function))  # 5
 
             null = Null()
 
-            print(await null.map_await_or(42, async_len))  # 42
+            print(await null.map_await_or(42, function))  # 42
             ```
 
         Arguments:
             default: The default value to use.
             function: The asynchronous function to apply.
 
         Returns:
-            The resulting or the default value.
+            The resulting value or the `default` one.
         """
         ...
 
     @required
     async def map_await_or_else(self, default: Nullary[U], function: AsyncUnary[T, U]) -> U:
-        """Computes the default value (if none), or applies the asynchronous `function`
-        to the contained value (if any).
+        """Computes the default value from the `default` function (if none),
+        or applies the asynchronous `function` to the contained value (if any).
 
         Example:
             ```python
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
+            def default() -> int:
+                return 0
+
             some = Some("Hello, world!")
 
-            print(await some.map_await_or_else(int, async_len))  # 13
+            print(await some.map_await_or_else(default, function))  # 13
 
             null = Null()
 
-            print(await null.map_await_or_else(int, async_len))  # 0
+            print(await null.map_await_or_else(default, function))  # 0
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
             function: The asynchronous function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting value or the `default()` one.
         """
         ...
 
     @required
     async def map_await_or_else_await(
         self, default: AsyncNullary[U], function: AsyncUnary[T, U]
     ) -> U:
@@ -578,32 +564,32 @@
         to the contained value (if any).
 
         Example:
             ```python
             async def default() -> int:
                 return 42
 
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
             some = Some("Hello, world!")
 
-            print(await some.map_await_or_else_await(default, async_len))  # 13
+            print(await some.map_await_or_else_await(default, function))  # 13
 
             null = Null()
 
-            print(await null.map_await_or_else_await(default, async_len))  # 42
+            print(await null.map_await_or_else_await(default, function))  # 42
             ```
 
         Arguments:
             default: The asynchronous default function to use.
             function: The asynchronous function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting value or the `await default()` one.
         """
         ...
 
     @required
     def ok_or(self, error: E) -> Result[T, E]:
         """Transforms an [`Option[T]`][wraps.option.Option]
         into a [`Result[T, E]`][wraps.result.Result], mapping [`Some(value)`][wraps.option.Some]
@@ -645,15 +631,15 @@
             assert some.ok_or_else(error).is_ok()
 
             null = Null()
             assert null.ok_or_else(error).is_error()
             ```
 
         Arguments:
-            error: The error function to use.
+            error: The error-computing function to use.
 
         Returns:
             The transformed result.
         """
         ...
 
     @required
@@ -676,71 +662,65 @@
             null = Null()
             result = await null.ok_or_else_await(error)
 
             assert result.is_error()
             ```
 
         Arguments:
-            error: The error function to use.
+            error: The error-computing function to use.
 
         Returns:
             The transformed result.
         """
         ...
 
     @required
-    def iter(self) -> Iter[T]:
+    def iter(self) -> Iterator[T]:
         """Returns an iterator over the possibly contained value.
 
         Example:
             ```python
             >>> some = Some(42)
-            >>> next(some.iter())
+            >>> next(some.iter(), 0)
             42
-
             >>> null = Null()
-            >>> next(null.iter())
-            Traceback (most recent call last):
-              ...
-            StopIteration
+            >>> next(null.iter(), 0)
+            0
             ```
 
         Returns:
             An iterator over the possible value.
         """
         ...
 
     @required
-    def async_iter(self) -> AsyncIter[T]:
+    def async_iter(self) -> AsyncIterator[T]:
         """Returns an asynchronous iterator over the possibly contained value.
 
         Example:
             ```python
             >>> some = Some(42)
-            >>> await anext(some.async_iter())
+            >>> await async_next(some.async_iter(), 0)
             42
-
             >>> null = Null()
-            >>> await anext(null.async_iter())
-            Traceback (most recent call last):
-              ...
-            StopAsyncIteration
+            >>> await async_next(null.async_iter(), 0)
+            0
             ```
 
         Returns:
             An asynchronous iterator over the possible value.
         """
         ...
 
     @required
     def and_then(self, function: Unary[T, Option[U]]) -> Option[U]:
-        """Returns [`Null`][wraps.option.Null] if the option is [`Null`][wraps.option.Null],
+        """Returns the option if it is [`Null`][wraps.option.Null],
         otherwise calls the `function` with the wrapped value and returns the result.
 
-        This function is also known as *bind*.
+        This function is also known as *bind* in functional programming.
 
         Example:
             ```python
             def inverse(value: float) -> Option[float]:
                 return Some(1.0 / value) if value else Null()
 
             some = Some(2.0)
@@ -759,15 +739,15 @@
         Returns:
             The resulting option.
         """
         ...
 
     @required
     async def and_then_await(self, function: AsyncUnary[T, Option[U]]) -> Option[U]:
-        """Returns [`Null`][wraps.option.Null] if the option is [`Null`][wraps.option.Null],
+        """Returns the option if it is [`Null`][wraps.option.Null],
         otherwise calls the asynchronous `function` with the wrapped value and returns the result.
 
         Example:
             ```python
             async def inverse(value: float) -> Option[float]:
                 return Some(1.0 / value) if value else Null()
 
@@ -793,15 +773,15 @@
         Returns:
             The resulting option.
         """
         ...
 
     @required
     def filter(self, predicate: Predicate[T]) -> Option[T]:
-        """Returns [`Null`][wraps.option.Null] if the option is [`Null`][wraps.option.Null],
+        """Returns the option if it is [`Null`][wraps.option.Null],
         otherwise calls the `predicate` with the wrapped value and returns:
 
         - [`Some(value)`][wraps.option.Some] if the contained `value` matches the predicate, and
         - [`Null`][wraps.option.Null] otherwise.
 
         Example:
             ```python
@@ -815,24 +795,24 @@
             assert even.filter(is_even).is_some()
 
             odd = Some(1)
             assert odd.filter(is_even).is_null()
             ```
 
         Arguments:
-            predicate: The predicate to check the contained value with.
+            predicate: The predicate to check the contained value against.
 
         Returns:
             The resulting option.
         """
         ...
 
     @required
     async def filter_await(self, predicate: AsyncPredicate[T]) -> Option[T]:
-        """Returns [`Null`][wraps.option.Null] if the option is [`Null`][wraps.option.Null],
+        """Returns the option if it is [`Null`][wraps.option.Null],
         otherwise calls the asynchronous `predicate` with the wrapped value and returns:
 
         - [`Some(value)`][wraps.option.Some] if the contained `value` matches the predicate, and
         - [`Null`][wraps.option.Null] otherwise.
 
         Example:
             ```python
@@ -846,61 +826,61 @@
             assert (await even.filter_await(is_even)).is_some()
 
             odd = Some(1)
             assert (await odd.filter_await(is_even)).is_null()
             ```
 
         Arguments:
-            predicate: The asynchronous predicate to check the contained value with.
+            predicate: The asynchronous predicate to check the contained value against.
 
         Returns:
             The resulting option.
         """
         ...
 
     @required
     def or_else(self, default: Nullary[Option[T]]) -> Option[T]:
         """Returns the option if it contains a value, otherwise calls
-        the `default` and returns the result.
+        the `default` function and returns the result.
 
         Example:
             ```python
-            def default() -> Null:
-                return Null()
+            def default() -> Some[int]:
+                return Some(13)
 
             some = Some(42)
             null = Null()
 
             assert some.or_else(default).is_some()
-            assert null.or_else(default).is_null()
+            assert null.or_else(default).is_some()
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
 
         Returns:
             The resulting option.
         """
         ...
 
     @required
     async def or_else_await(self, default: AsyncNullary[Option[T]]) -> Option[T]:
         """Returns the option if it contains a value, otherwise calls
-        the asynchronous `default` and returns the result.
+        the asynchronous `default` function and returns the result.
 
         Example:
             ```python
-            async def default() -> Null:
-                return Null()
+            async def default() -> Some[int]:
+                return Some(13)
 
             some = Some(42)
             null = Null()
 
             assert (await some.or_else_await(default)).is_some()
-            assert (await null.or_else_await(default)).is_null()
+            assert (await null.or_else_await(default)).is_some()
             ```
 
         Arguments:
             default: The asynchronous default function to use.
 
         Returns:
             The resulting option.
@@ -1145,15 +1125,15 @@
         """
         ...
 
     @required
     def early(self) -> T:
         """Functionally similar to `?` operator in Rust.
 
-        See [early](/reference/early) for more information.
+        See [`early`][wraps.early] for more information.
         """
         ...
 
 
 UNWRAP_ON_NULL = "called `unwrap` on null"
 
 
@@ -1236,27 +1216,19 @@
 
     def ok_or_else(self, error: Nullary[E]) -> Error[E]:
         return Error(error())
 
     async def ok_or_else_await(self, error: AsyncNullary[E]) -> Error[E]:
         return Error(await error())
 
-    def iter(self) -> Iter[Never]:
-        return iter(self.actual_iter())
-
-    def async_iter(self) -> AsyncIter[Never]:
-        return async_iter(self.actual_async_iter())
+    def iter(self) -> Iterator[Never]:
+        return empty()
 
-    def actual_iter(self) -> Iterator[Never]:
-        return
-        yield  # type: ignore
-
-    async def actual_async_iter(self) -> AsyncIterator[Never]:
-        return
-        yield  # type: ignore
+    def async_iter(self) -> AsyncIterator[Never]:
+        return async_empty()
 
     def and_then(self, function: Unary[T, Option[U]]) -> Null:
         return self
 
     async def and_then_await(self, function: AsyncUnary[T, Option[U]]) -> Null:
         return self
 
@@ -1379,25 +1351,19 @@
 
     def ok_or_else(self, error: Nullary[E]) -> Ok[T]:
         return Ok(self.value)
 
     async def ok_or_else_await(self, error: AsyncNullary[E]) -> Ok[T]:
         return Ok(self.value)
 
-    def iter(self) -> Iter[T]:
-        return iter(self.actual_iter())
+    def iter(self) -> Iterator[T]:
+        return once(self.value)
 
-    def async_iter(self) -> AsyncIter[T]:
-        return async_iter(self.actual_async_iter())
-
-    def actual_iter(self) -> Iterator[T]:
-        yield self.value
-
-    async def actual_async_iter(self) -> AsyncIterator[T]:
-        yield self.value
+    def async_iter(self) -> AsyncIterator[T]:
+        return async_once(self.value)
 
     def and_then(self, function: Unary[T, Option[U]]) -> Option[U]:
         return function(self.value)
 
     async def and_then_await(self, function: AsyncUnary[T, Option[U]]) -> Option[U]:
         return await function(self.value)
 
@@ -1498,87 +1464,10 @@
 def is_null(option: Option[T]) -> TypeGuard[Null]:
     """This is the same as [`Option.is_null`][wraps.option.OptionProtocol.is_null],
     except it works as a *type guard*.
     """
     return option.is_null()
 
 
-def wrap_option(function: Callable[P, T]) -> Callable[P, Option[T]]:
-    """Wraps a `function` returning `T` into a function returning
-    [`Option[T]`][wraps.option.Option].
-
-    This handles all exceptions via returning [`Null`][wraps.option.Null] on errors,
-    wrapping the resulting `value` into [`Some(value)`][wraps.option.Some].
-
-    Example:
-        ```python
-        @wrap_option
-        def parse(string: str) -> int:
-            return int(string)
-
-        assert parse("128").is_some()
-        assert parse("uwu").is_null()
-        ```
-
-    Arguments:
-        function: The function to wrap.
-
-    Returns:
-        The wrapping function.
-    """
-
-    def wrap(*args: P.args, **kwargs: P.kwargs) -> Option[T]:
-        try:
-            return Some(function(*args, **kwargs))
-
-        except Exception:
-            return Null()
-
-    return wrap
-
-
-def wrap_option_await(function: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[Option[T]]]:
-    """Wraps an asynchronous `function` returning `T` into an asynchronous function returning
-    [`Option[T]`][wraps.option.Option].
-
-    This handles all exceptions via returning [`Null`][wraps.option.Null] on errors,
-    wrapping the resulting `value` into [`Some(value)`][wraps.option.Some].
-
-    Example:
-        ```python
-        @wrap_option_await
-        async def parse(string: str) -> int:
-            return int(string)
-
-        assert (await parse("256")).is_some()
-        assert (await parse("uwu")).is_null()
-        ```
-
-    Arguments:
-        function: The asynchronous function to wrap.
-
-    Returns:
-        The asynchronous wrapping function.
-    """
-
-    async def wrap(*args: P.args, **kwargs: P.kwargs) -> Option[T]:
-        try:
-            return Some(await function(*args, **kwargs))
-
-        except Exception:
-            return Null()
-
-    return wrap
-
-
-def wrap_optional(optional: Optional[T]) -> Option[T]:
-    if optional is None:
-        return Null()
-
-    return Some(optional)
-
-
 # import cycle solution
-from iters.async_iters import AsyncIter, async_iter
-from iters.iters import Iter, iter
 
 from wraps.result import Error, Ok, Result
```

### Comparing `wraps-0.3.0/wraps/result.py` & `wraps-0.4.0/wraps/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,75 @@
+"""Error handling with the [`Result[T, E]`][wraps.result.Result] type.
+
+[`Result[T, E]`][wraps.result.Result] is the type used for returning and propagating errors.
+
+It is an enum with the variants, [`Ok[T]`][wraps.result.Ok],
+representing success and containing a value,
+and [`Error[E]`][wraps.result.Error], representing error and containing an error value.
+
+Functions return [`Result[T, E]`][wraps.result.Result] whenever errors are expected and recoverable.
+
+For instance, our `divide` function from the [`option`][wraps.option] section:
+
+```python
+# result.py
+
+from enum import Enum
+
+from wraps import Error, Ok, Result
+
+
+class DivideError(Enum):
+    DIVISION_BY_ZERO = "division by zero"
+
+
+def divide(numerator: float, denominator: float) -> Result[float, DivideError]:
+    return Ok(numerator / denominator) if denominator else Error(DivideError.DIVISION_BY_ZERO)
+```
+
+```python
+from wraps import Error, Ok
+
+from result import divide
+
+result = divide(1.0, 2.0)
+
+match result:
+    case Ok(value):
+        print(value)
+
+    case Error(error):
+        print(error)
+```
+"""
+
 from __future__ import annotations
 
 from abc import abstractmethod as required
-from functools import wraps
-from typing import (
-    TYPE_CHECKING,
-    AsyncIterator,
-    Awaitable,
-    Callable,
-    Generic,
-    Iterator,
-    Optional,
-    Type,
-    TypeVar,
-    Union,
-    final,
-)
+from typing import AsyncIterator, Iterator, TypeVar, Union, final
 
 from attrs import frozen
-from iters import AsyncIter, Iter, async_iter, iter, wrap_async_iter, wrap_iter
-from typing_extensions import Literal, Never, ParamSpec, Protocol, TypeGuard
-
-from wraps.errors import EarlyResult, panic
-from wraps.option import Null, Option, Some
-from wraps.typing import (
-    AnyException,
+from funcs.typing import (
+    AnyError,
     AsyncInspect,
     AsyncNullary,
     AsyncPredicate,
     AsyncUnary,
     Inspect,
     Nullary,
     Predicate,
     Unary,
 )
+from typing_extensions import Literal, Never, ParamSpec, Protocol, TypeGuard
+
+from wraps.errors import EarlyResult, panic
+from wraps.option import Null, Option, Some
+from wraps.utils import async_empty, async_once, empty, once
 
-__all__ = ("Result", "Ok", "Error", "is_ok", "is_error", "wrap_result")
+__all__ = ("Result", "Ok", "Error", "is_ok", "is_error")
 
 P = ParamSpec("P")
 
 T = TypeVar("T", covariant=True)
 U = TypeVar("U")
 
 E = TypeVar("E", covariant=True)
@@ -209,15 +240,14 @@
         """Returns the contained [`Ok[T]`][wraps.result.Ok] value.
 
         Example:
             ```python
             >>> ok = Ok(42)
             >>> ok.expect("error!")
             42
-
             >>> error = Error(0)
             >>> error.expect("error!")
             Traceback (most recent call last):
               ...
             wraps.errors.Panic: error!
             ```
 
@@ -249,15 +279,15 @@
             0
             ```
 
         Arguments:
             message: The message used in panicking.
 
         Raises:
-            Panic: Panics with `message` if the result is [`Ok[T]`][wraps.result.Ok].
+            Panic: Panics with the `message` if the result is [`Ok[T]`][wraps.result.Ok].
 
         Returns:
             The contained value.
         """
         ...
 
     @required
@@ -289,97 +319,95 @@
         Returns:
             The contained value.
         """
         ...
 
     @required
     def unwrap_or(self, default: T) -> T:  # type: ignore
-        """Returns the contained [`Ok[T]`][wraps.result.Ok] value (of type `T`)
-        or a provided default.
+        """Returns the contained [`Ok[T]`][wraps.result.Ok] value or the provided `default`.
 
         Example:
             ```python
-            default = 0
-
             ok = Ok(69)
-            assert ok.unwrap_or(default)
+            assert ok.unwrap_or(0)
 
-            error = Error(0)
-            assert not error.unwrap_or(default)
+            error = Error(13)
+            assert not error.unwrap_or(0)
             ```
 
         Arguments:
             default: The default value to use.
 
         Returns:
-            The contained value or `default` one.
+            The contained value or the `default` one.
         """
         ...
 
     @required
     def unwrap_or_else(self, default: Nullary[T]) -> T:
-        """Returns the contained [`Ok[T]`][wraps.result.Ok] value (of type `T`) or
-        computes it from the function.
+        """Returns the contained [`Ok[T]`][wraps.result.Ok] value
+        or computes it from the `default` function.
 
         Example:
             ```python
             ok = Ok(5)
             assert ok.unwrap_or_else(int)
 
             error = Error(8)
             assert not error.unwrap_or_else(int)
+            ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
 
         Returns:
-            The contained value or `default()` one.
+            The contained value or the `default()` one.
         """
         ...
 
     @required
     async def unwrap_or_else_await(self, default: AsyncNullary[T]) -> T:
-        """Returns the contained [`Ok[T]`][wraps.result.Ok] value (of type `T`) or
-        computes it from the asynchronous function.
+        """Returns the contained [`Ok[T]`][wraps.result.Ok] value
+        or computes it from the asynchronous `default` function.
 
         Example:
             ```python
             async def default() -> int:
                 return 0
 
             ok = Ok(5)
             assert await ok.unwrap_or_else_await(default)
 
             error = Error(8)
             assert not await error.unwrap_or_else_await(default)
+            ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
 
         Returns:
-            The contained value or `await default()` one.
+            The contained value or the `await default()` one.
         """
         ...
 
     @required
     def unwrap_error(self) -> E:
-        """Returns the contained [`Error[E]`][wraps.result.Error] value (of type `E`).
+        """Returns the contained [`Error[E]`][wraps.result.Error] value.
 
         Because this function may panic, its use is generally discouraged.
 
         Instead, prefer to use pattern matching and handle the [`Ok[T]`][wraps.result.Ok]
         case explicitly, or call [`unwrap_error_or`][wraps.result.ResultProtocol.unwrap_error_or]
         or [`unwrap_error_or_else`][wraps.result.ResultProtocol.unwrap_error_or_else].
 
         Example:
             ```python
             >>> error = Error(13)
             >>> error.unwrap_error()
             13
-
             >>> ok = Ok(42)
             >>> ok.unwrap_error()
             Traceback (most recent call last):
               ...
             wraps.errors.Panic: called `unwrap_error` on ok
             ```
 
@@ -394,109 +422,106 @@
     @required
     def unwrap_error_or(self, default: E) -> E:  # type: ignore
         """Returns the contained [`Error[E]`][wraps.result.Error] value (of type `E`)
         or a provided default.
 
         Example:
             ```python
-            default = 0
-
             error = Error(1)
-            assert error.unwrap_error_or(default)
+            assert error.unwrap_error_or(0)
 
             ok = Ok(2)
-            assert not ok.unwrap_error_or(default)
+            assert not ok.unwrap_error_or(0)
             ```
 
         Arguments:
             default: The default value to use.
 
         Returns:
-            The contained error value or `default` one.
+            The contained error value or the `default` one.
         """
         ...
 
     @required
     def unwrap_error_or_else(self, default: Nullary[E]) -> E:
-        """Returns the contained [`Error[E]`][wraps.result.Error] value (of type `E`) or
-        computes it from the function.
+        """Returns the contained [`Error[E]`][wraps.result.Error] value
+        or computes it from the `default` function.
 
         Example:
             ```python
             error = Error(5)
             assert error.unwrap_error_or_else(int)
 
             ok = Ok(8)
             assert not ok.unwrap_error_or_else(int)
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
 
         Returns:
-            The contained error value or `default()` one.
+            The contained error value or the `default()` one.
         """
         ...
 
     @required
     async def unwrap_error_or_else_await(self, default: AsyncNullary[E]) -> E:
-        """Returns the contained [`Error[E]`][wraps.result.Error] value (of type `E`) or
-        computes it from the asynchronous function.
+        """Returns the contained [`Error[E]`][wraps.result.Error] value
+        or computes it from the asynchronous `default` function.
 
         Example:
             ```python
             async def default() -> int:
                 return 0
 
             error = Error(13)
             assert await error.unwrap_error_or_else_await(default)
 
             ok = Ok(5)
             assert not ok.unwrap_error_or_else_await(default)
             ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
 
         Returns:
-            The contained error value or `await default()` one.
+            The contained error value or the `await default()` one.
         """
         ...
 
     @required
-    def raising(self: ResultProtocol[T, AnyException]) -> T:
+    def raising(self: ResultProtocol[T, AnyError]) -> T:
         """Returns the contained [`Ok[T]`][wraps.result.Ok] value or raises the
-        contained [`Error[AnyException]`][wraps.result.Error] value.
+        contained [`Error[AnyError]`][wraps.result.Error] value.
 
         Example:
             ```python
             >>> ok = Ok(13)
             >>> ok.raising()
             13
-
             >>> error = Error(ValueError("error..."))
             >>> error.raising()
             Traceback (most recent call last):
               ...
             ValueError: error...
             ```
 
         Raises:
-            AnyException: The contained exception, if the result
-                is [`Error[AnyException]`][wraps.result.Error].
+            AnyError: The contained error, if the result is [`Error[AnyError]`][wraps.result.Error].
 
         Returns:
             The contained value.
         """
         ...
 
     @required
     def ok(self) -> Option[T]:
-        """Converts [`Result[T, E]`][wraps.result.Result] to [`Option[T]`][wraps.option.Option].
+        """Converts a [`Result[T, E]`][wraps.result.Result]
+        to an [`Option[T]`][wraps.option.Option].
 
-        Converts `self` into an [`Option[T]`][wraps.option.Option], discarding the error, if any.
+        Converts `self` into an [`Option[T]`][wraps.option.Option], discarding errors, if any.
 
         Example:
             ```python
             ok = Ok(42)
 
             assert ok.ok().is_some()
 
@@ -508,28 +533,29 @@
         Returns:
             The converted option.
         """
         ...
 
     @required
     def error(self) -> Option[E]:
-        """Converts [`Result[T, E]`][wraps.result.Result] to [`Option[E]`][wraps.option.Option].
+        """Converts a [`Result[T, E]`][wraps.result.Result]
+        to an [`Option[E]`][wraps.option.Option].
 
-        Converts `self` into an [`Option[E]`][wraps.option.Option], discarding the success value,
-        if any.
+        Converts `self` into an [`Option[E]`][wraps.option.Option],
+        discarding success values, if any.
 
         Example:
             ```python
             error = Error(13)
 
             assert error.error().is_some()
 
             ok = Ok(2)
 
-            assert error.ok().is_null()
+            assert ok.error().is_null()
             ```
 
         Returns:
             The converted option.
         """
         ...
 
@@ -551,52 +577,52 @@
 
         Returns:
             The inspected result.
         """
         ...
 
     @required
-    def inspect_error(self, function: Inspect[E]) -> Result[T, E]:
-        """Inspects a possibly contained [`Error[E]`][wraps.result.Error] value.
+    async def inspect_await(self, function: AsyncInspect[T]) -> Result[T, E]:
+        """Inspects a possibly contained [`Ok[T]`][wraps.result.Ok] value.
 
         Example:
             ```python
-            error = Error("Bye, world!")
+            async def function(value: str) -> None:
+                print(value)
 
-            same = error.inspect_error(print)  # Bye, world!
+            ok = Ok("Hello, world!")
 
-            assert error == same
+            same = await ok.inspect_await(function)  # Hello, world!
+
+            assert ok == same
             ```
 
         Arguments:
-            function: The inspecting function.
+            function: The asynchronous inspecting function.
 
         Returns:
             The inspected result.
         """
         ...
 
     @required
-    async def inspect_await(self, function: AsyncInspect[T]) -> Result[T, E]:
-        """Inspects a possibly contained [`Ok[T]`][wraps.result.Ok] value.
+    def inspect_error(self, function: Inspect[E]) -> Result[T, E]:
+        """Inspects a possibly contained [`Error[E]`][wraps.result.Error] value.
 
         Example:
             ```python
-            async def function(value: str) -> None:
-                print(value)
-
-            ok = Ok("Hello, world!")
+            error = Error("Bye, world!")
 
-            same = await ok.inspect_await(function)  # Hello, world!
+            same = error.inspect_error(print)  # Bye, world!
 
-            assert ok == same
+            assert error == same
             ```
 
         Arguments:
-            function: The inspecting asynchronous function.
+            function: The error-inspecting function.
 
         Returns:
             The inspected result.
         """
         ...
 
     @required
@@ -612,26 +638,26 @@
 
             same = await error.inspect_error_await(function)  # Bye, world!
 
             assert error == same
             ```
 
         Arguments:
-            function: The inspecting asynchronous function.
+            function: The asynchronous error-inspecting function.
 
         Returns:
             The inspected result.
         """
         ...
 
     @required
     def map(self, function: Unary[T, U]) -> Result[U, E]:
-        """Maps [`Result[T, E]`][wraps.result.Result] to [`Result[U, E]`][wraps.result.Result]
+        """Maps a [`Result[T, E]`][wraps.result.Result] to a [`Result[U, E]`][wraps.result.Result]
         by applying `function` to the contained [`Ok[T]`][wraps.result.Ok] value,
-        leaving any [`Error[E]`][wraps.result.Error] untouched.
+        leaving any [`Error[E]`][wraps.result.Error] values untouched.
 
         This function can be used to compose the results of two functions.
 
         Example:
             ```python
             value = 69
             mapped = "69"
@@ -651,15 +677,15 @@
         Returns:
             The mapped result.
         """
         ...
 
     @required
     def map_or(self, default: U, function: Unary[T, U]) -> U:
-        """Returns the default value (if errored), or applies `function`
+        """Returns the default value (if errored), or applies the `function`
         to the contained value (if succeeded).
 
         Example:
             ```python
             ok = Ok("Hello, world!")
             print(ok.map_or(42, len))  # 13
 
@@ -674,63 +700,66 @@
         Returns:
             The resulting or the default value.
         """
         ...
 
     @required
     def map_or_else(self, default: Nullary[U], function: Unary[T, U]) -> U:
-        """Computes the default value (if errored), or applies `function`
+        """Computes the default value (if errored), or applies the `function`
         to the contained value (if succeeded).
 
         Example:
             ```python
             ok = Ok("Hello, world!")
             print(ok.map_or_else(int, len))  # 13
 
             error = Error("error!")
             print(error.map_or_else(int, len))  # 0
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
             function: The function to apply.
 
         Returns:
             The resulting or the default computed value.
         """
         ...
 
     @required
     async def map_or_else_await(self, default: AsyncNullary[U], function: Unary[T, U]) -> U:
         """Computes the default value (if errored), or applies the `function`
         to the contained value (if succeeded).
 
         Example:
             ```python
+            async def default() -> int:
+                return 0
+
             ok = Ok("Hello, world!")
-            print(await ok.map_or_else_await(int, len))  # 13
+            print(await ok.map_or_else_await(default, len))  # 13
 
             error = Error("error!")
-            print(await error.map_or_else_await(int, len))  # 0
+            print(await error.map_or_else_await(default, len))  # 0
             ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
             function: The function to apply.
 
         Returns:
             The resulting or the default computed value.
         """
         ...
 
     @required
     def map_error(self, function: Unary[E, F]) -> Result[T, F]:
-        """Maps [`Result[T, E]`][wraps.result.Result] to [`Result[T, F]`][wraps.result.Result]
+        """Maps a [`Result[T, E]`][wraps.result.Result] to a [`Result[T, F]`][wraps.result.Result]
         by applying the `function` to the contained [`Error[E]`][wraps.result.Error] value,
-        leaving any [`Ok[T]`][wraps.result.Ok] untouched.
+        leaving any [`Ok[T]`][wraps.result.Ok] values untouched.
 
         Example:
             ```python
             value = 42
             mapped = "42"
 
             error = Error(value)
@@ -784,68 +813,68 @@
             print(error.map_error_or_else(int, len))  # 8
 
             ok = Ok("ok!")
             print(ok.map_error_or_else(int, len))  # 0
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
             function: The function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting or the computed default value.
         """
         ...
 
     @required
     async def map_error_or_else_await(self, default: AsyncNullary[F], function: Unary[E, F]) -> F:
-        """Computes the default value (if succeeded), or applies `function`
+        """Computes the default value (if succeeded), or applies the `function`
         to the contained value (if errored).
 
         Example:
             ```python
             error = Error("error...")
             print(await error.map_error_or_else(int, len))  # 8
 
             ok = Ok("ok!")
             print(await ok.map_error_or_else(int, len))  # 0
             ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
             function: The function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting or the computed default value.
         """
         ...
 
     @required
     async def map_await(self, function: AsyncUnary[T, U]) -> Result[U, E]:
-        """Maps [`Result[T, E]`][wraps.result.Result] to [`Result[U, E]`][wraps.result.Result]
+        """Maps a [`Result[T, E]`][wraps.result.Result] to a [`Result[U, E]`][wraps.result.Result]
         by applying the asynchronous `function` to the contained [`Ok[T]`][wraps.result.Ok] value,
-        leaving any [`Error[E]`][wraps.result.Error] untouched.
+        leaving any [`Error[E]`][wraps.result.Error] values untouched.
 
         This function can be used to compose the results of two functions.
 
         Example:
             ```python
-            async def async_str(value: int) -> str:
+            async def function(value: int) -> str:
                 return str(value)
 
             value = 69
             mapped = "69"
 
             ok = Ok(value)
 
-            assert await ok.map_await(async_str) == Ok(mapped)
+            assert await ok.map_await(function) == Ok(mapped)
 
             error = Error(0)
 
-            assert await error.map_await(async_str) == error
+            assert await error.map_await(function) == error
             ```
 
         Arguments:
             function: The asynchronous function to apply.
 
         Returns:
             The mapped result.
@@ -855,22 +884,22 @@
     @required
     async def map_await_or(self, default: U, function: AsyncUnary[T, U]) -> U:
         """Returns the default value (if errored), or applies the asynchronous `function`
         to the contained value (if succeeded).
 
         Example:
             ```python
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
             ok = Ok("Hello, world!")
-            print(await ok.map_await_or(42, async_len))  # 13
+            print(await ok.map_await_or(42, function))  # 13
 
             error = Error("error...")
-            print(error.map_await_or(42, async_len))  # 42
+            print(error.map_await_or(42, function))  # 42
             ```
 
         Arguments:
             default: The default value to use.
             function: The asynchronous function to apply.
 
         Returns:
@@ -892,19 +921,19 @@
             print(await ok.map_await_or_else(int, async_len))  # 13
 
             error = Error("error!")
             print(await error.map_await_or_else(int, async_len))  # 0
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
             function: The asynchronous function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting or the computed default value.
         """
         ...
 
     @required
     async def map_await_or_else_await(
         self, default: AsyncNullary[U], function: AsyncUnary[T, U]
     ) -> U:
@@ -912,54 +941,54 @@
         to the contained value (if succeeded).
 
         Example:
             ```python
             async def default() -> int:
                 return 0
 
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
             ok = Ok("Hello, world!")
-            print(await ok.map_await_or_else_await(default, async_len))  # 13
+            print(await ok.map_await_or_else_await(default, function))  # 13
 
             error = Error("error!")
-            print(await error.map_await_or_else_await(default, async_len))  # 0
+            print(await error.map_await_or_else_await(default, function))  # 0
             ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
             function: The asynchronous function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting or the computed default value.
         """
         ...
 
     @required
     async def map_error_await(self, function: AsyncUnary[E, F]) -> Result[T, F]:
-        """Maps [`Result[T, E]`][wraps.result.Result] to [`Result[T, F]`][wraps.result.Result]
+        """Maps a [`Result[T, E]`][wraps.result.Result] to a [`Result[T, F]`][wraps.result.Result]
         by applying the asynchronous `function` to the contained [`Error[E]`][wraps.result.Error]
-        value, leaving any [`Ok[T]`][wraps.result.Ok] untouched.
+        value, leaving any [`Ok[T]`][wraps.result.Ok] values untouched.
 
         Example:
             ```python
-            async def async_str(value: int) -> str:
+            async def function(value: int) -> str:
                 return str(value)
 
             value = 42
             mapped = "42"
 
             error = Error(value)
 
-            assert await error.map_error_await(async_str) == Error(mapped)
+            assert await error.map_error_await(function) == Error(mapped)
 
             ok = Ok(13)
 
-            assert await ok.map_error_await(async_str) == ok
+            assert await ok.map_error_await(function) == ok
             ```
 
         Arguments:
             function: The asynchronous function to apply.
 
         Returns:
             The mapped result.
@@ -969,22 +998,22 @@
     @required
     async def map_error_await_or(self, default: F, function: AsyncUnary[E, F]) -> F:
         """Returns the default value (if succeeded), or applies the asynchronous `function`
         to the contained value (if errored).
 
         Example:
             ```python
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
             error = Error("Bye, world!")
-            print(await error.map_error_await_or(42, async_len))  # 11
+            print(await error.map_error_await_or(42, function))  # 11
 
             ok = Ok("Hello, world!")
-            print(await ok.map_error_await_or(42, async_len))  # 42
+            print(await ok.map_error_await_or(42, function))  # 42
             ```
 
         Arguments:
             default: The default value to use.
             function: The asynchronous function to apply.
 
         Returns:
@@ -1006,19 +1035,19 @@
             print(await error.map_error_await_or_else(int, async_len))  # 11
 
             ok = Ok("Hello, world!")
             print(await ok.map_error_await_or_else(int, async_len))  # 0
             ```
 
         Arguments:
-            default: The default function to use.
+            default: The default-computing function to use.
             function: The asynchronous function to apply.
 
         Returns:
-            The resulting or the default computed value.
+            The resulting or the computed default value.
         """
         ...
 
     @required
     async def map_error_await_or_else_await(
         self, default: AsyncNullary[F], function: AsyncUnary[E, F]
     ) -> F:
@@ -1026,249 +1055,241 @@
         to the contained value (if errored).
 
         Example:
             ```python
             async def default() -> int:
                 return 0
 
-            async def async_len(value: str) -> int:
+            async def function(value: str) -> int:
                 return len(value)
 
             error = Error("error")
-            print(await error.map_error_await_or_else_await(default, async_len))  # 5
+            print(await error.map_error_await_or_else_await(default, function))  # 5
 
             ok = Ok("ok")
-            print(await ok.map_error_await_or_else_await(default, async_len))  # 0
+            print(await ok.map_error_await_or_else_await(default, function))  # 0
             ```
 
         Arguments:
-            default: The asynchronous default function to use.
+            default: The asynchronous default-computing function to use.
             function: The asynchronous function to apply.
 
         Returns:
             The resulting or the default computed value.
         """
         ...
 
     @required
-    def iter(self) -> Iter[T]:
+    def iter(self) -> Iterator[T]:
         """Returns an iterator over the possibly contained value.
 
         Example:
             ```python
             >>> ok = Ok(42)
-            >>> ok.iter().next()
+            >>> next(ok.iter(), 0)
             42
-
-            >>> error = Error(0)
-            >>> error.iter().next()
-            Traceback (most recent call last):
-              ...
-            StopIteration
+            >>> error = Error(13)
+            >>> next(error.iter(), 0)
+            0
             ```
 
         Returns:
             An iterator over the possibly contained value.
         """
         ...
 
     @required
-    def iter_error(self) -> Iter[E]:
+    def iter_error(self) -> Iterator[E]:
         """Returns an iterator over the possibly contained error value.
 
         Example:
             ```python
             >>> error = Error(13)
-            >>> error.iter_error().next()
+            >>> next(error.iter_error(), 0)
             13
-
             >>> ok = Ok(1)
-            >>> ok.iter_error().next()
-            Traceback (most recent call last):
-              ...
-            StopIteration
+            >>> next(ok.iter_error(), 0)
+            0
             ```
 
         Returns:
             An iterator over the possibly contained error value.
         """
         ...
 
     @required
-    def async_iter(self) -> AsyncIter[T]:
+    def async_iter(self) -> AsyncIterator[T]:
         """Returns an asynchronous iterator over the possibly contained
         [`Ok[T]`][wraps.result.Ok] value.
 
         Example:
             ```python
             >>> ok = Ok(42)
-            >>> await ok.async_iter().next()
+            >>> await async_next(ok.async_iter(), 0)
             42
-
             >>> error = Error(13)
-            >>> await error.async_iter().next()
-            Traceback (most recent call last):
-              ...
-            StopAsyncIteration
+            >>> await async_next(error.async_iter(), 0)
+            0
             ```
 
         Returns:
-            An asynchronous iterator over the success value.
+            An asynchronous iterator over the possibly contained value.
         """
         ...
 
     @required
-    def async_iter_error(self) -> AsyncIter[E]:
+    def async_iter_error(self) -> AsyncIterator[E]:
         """Returns an asynchronous iterator over the possibly contained
         [`Error[E]`][wraps.result.Error] value.
 
         Example:
             ```python
-            >>> error = Error(0)
-            >>> await error.async_iter_error().next()
-            0
-
+            >>> error = Error(42)
+            >>> await async_next(error.async_iter_error(), 0)
+            42
             >>> ok = Ok(13)
-            >>> await ok.async_iter_error().next()
-            Traceback (most recent call last):
-              ...
-            StopAsyncIteration
+            >>> await async_next(ok.async_iter_error(), 0)
+            0
             ```
 
         Returns:
-            An asynchronous iterator over the error value.
+            An asynchronous iterator over the possibly contained error value.
         """
         ...
 
     @required
     def and_then(self, function: Unary[T, Result[U, E]]) -> Result[U, E]:
-        """Returns [`Error[E]`][wraps.result.Error] if the result
-        is [`Error[E]`][wraps.result.Error], otherwise calls the `function`
-        with the wrapped value and returns the result.
+        """Returns the result if it is an [`Error[E]`][wraps.result.Error],
+        otherwise calls the `function` with the wrapped value and returns the result.
 
         This function is also known as *bind* in functional programming.
 
         Example:
             ```python
-            def inverse(value: float) -> Result[float, str]:
-                return Ok(1.0 / value) if value else Error("can not divide by zero")
+            class InverseError(Enum):
+                DIVISION_BY_ZERO = "division by zero"
+
+            def inverse(value: float) -> Result[float, InverseError]:
+                return Ok(1.0 / value) if value else Error(InverseError.DIVISION_BY_ZERO)
 
-            ok = Ok(2.0)
-            print(ok.and_then(inverse).unwrap())  # 0.5
+            two = Ok(2.0)
+            print(two.and_then(inverse).unwrap())  # 0.5
 
             zero = Ok(0.0)
-            assert zero.and_then(inverse).is_error()
+            print(zero.and_then(inverse).unwrap_error())  # division by zero
 
-            error = Error()
-            assert error.and_then(inverse).is_error()
+            error = Error(1.0)
+            print(error.and_then(inverse).unwrap_error())  # 1.0
             ```
 
         Arguments:
             function: The function to apply.
 
         Returns:
             The bound result.
         """
         ...
 
     @required
     async def and_then_await(self, function: AsyncUnary[T, Result[U, E]]) -> Result[U, E]:
-        """Returns [`Error[E]`][wraps.result.Error] if the result
-        is [`Error[E]`][wraps.result.Error], otherwise calls the asynchronous `function`
-        with the wrapped value and returns the result.
+        """Returns the result if it is an [`Error[E]`][wraps.result.Error],
+        otherwise calls the asynchronous `function` with the wrapped value and returns the result.
 
         Example:
             ```python
-            async def inverse(value: float) -> Result[float, str]:
-                return Ok(1.0 / value) if value else Error("can not divide by zero")
+            class InverseError(Enum):
+                DIVISION_BY_ZERO = "division by zero"
 
-            ok = Ok(2.0)
-            result = await ok.and_then_await(inverse)
-            print(result.unwrap())  # 0.5
+            async def inverse(value: float) -> Result[float, InverseError]:
+                return Ok(1.0 / value) if value else Error(InverseError.DIVISION_BY_ZERO)
+
+            two = Ok(2.0)
+            print((await two.and_then_await(inverse)).unwrap())  # 0.5
 
             zero = Ok(0.0)
-            assert (await zero.and_then_await(inverse)).is_error()
+            print((await zero.and_then_await(inverse)).unwrap_error())  # division by zero
 
-            error = Error()
-            assert (await error.and_then_await(inverse)).is_error()
+            error = Error(1.0)
+            print((await error.and_then_await(inverse)).unwrap_error())  # 1.0
             ```
 
         Arguments:
             function: The asynchronous function to apply.
 
         Returns:
             The bound result.
         """
         ...
 
     @required
     def or_else(self, function: Unary[E, Result[T, F]]) -> Result[T, F]:
-        """Returns [`Ok[T]`][wraps.result.Ok] if the result
-        is [`Ok[T]`][wraps.result.Ok], otherwise calls the `function`
+        """Returns the result if it is [`Ok[T]`][wraps.result.Ok], otherwise calls the `function`
         with the wrapped error value and returns the result.
 
         Example:
             ```python
-            def check_non_zero(value: int) -> Result[int, str]:
-                return Ok(value) if value else Error("the value is zero")
+            class NonZeroError(Enum):
+                ZERO = "the value is zero"
 
-            error = Error(13)
+            def check_non_zero(value: int) -> Result[int, NonZeroError]:
+                return Ok(value) if value else Error(NonZeroError.ZERO)
 
+            five = Error(5)
             print(error.or_else(check_non_zero).unwrap())  # 13
 
             zero = Error(0)
-            assert zero.or_else(check_non_zero).is_error()
+            print(zero.or_else(check_non_zero).unwrap_error())  # the value is zero
 
-            ok = Ok(42)
-            assert ok.or_else(check_non_zero).is_ok()
+            one = Ok(1)
+            print(one.or_else(check_non_zero).unwrap())  # 1
             ```
 
         Arguments:
             function: The function to apply.
 
         Returns:
             The bound result.
         """
         ...
 
     @required
     async def or_else_await(self, function: AsyncUnary[E, Result[T, F]]) -> Result[T, F]:
-        """Returns [`Ok[T]`][wraps.result.Ok] if the result
-        is [`Ok[T]`][wraps.result.Ok], otherwise calls the asynchronous `function`
-        with the wrapped error value and returns the result.
+        """Returns the result if it is [`Ok[T]`][wraps.result.Ok], otherwise calls the asynchronous
+        `function` with the wrapped error value and returns the result.
 
         Example:
             ```python
-            async def check_non_zero(value: int) -> Result[int, str]:
-                return Ok(value) if value else Error("the value is zero")
+            class NonZeroError(Enum):
+                ZERO = "the value is zero"
 
-            error = Error(13)
+            async def check_non_zero(value: int) -> Result[int, NonZeroError]:
+                return Ok(value) if value else Error(NonZeroError.ZERO)
 
-            result = await error.or_else_await(check_non_zero)
+            five = Error(5)
 
-            print(result.unwrap())  # 13
+            print((await error.or_else_await(check_non_zero)).unwrap())  # 13
 
             zero = Error(0)
-            assert (await zero.or_else_await(check_non_zero)).is_error()
+            print((await zero.or_else_await(check_non_zero)).unwrap_error())  # the value is zero
 
-            ok = Ok(42)
-            assert (await ok.or_else_await(check_non_zero)).is_ok()
+            one = Ok(1)
+            print((await ok.or_else_await(check_non_zero)).unwrap())  # 1
             ```
 
         Arguments:
             function: The asynchronous function to apply.
 
         Returns:
             The bound result.
         """
         ...
 
     def try_flatten(self: ResultProtocol[ResultProtocol[T, E], E]) -> Result[T, E]:
         """Flattens a [`Result[Result[T, E], E]`][wraps.result.Result]
-        to [`Result[T, E]`][wraps.result.Result].
+        to a [`Result[T, E]`][wraps.result.Result].
 
         This is equivalent to [`result.and_then(identity)`][wraps.result.ResultProtocol.and_then].
 
         Example:
             ```python
             ok = Ok(42)
             ok_nested = Ok(ok)
@@ -1284,15 +1305,15 @@
         Returns:
             The flattened result.
         """
         return self.and_then(identity)  # type: ignore
 
     def try_flatten_error(self: ResultProtocol[T, ResultProtocol[T, E]]) -> Result[T, E]:
         """Flattens a [`Result[T, Result[T, E]]`][wraps.result.Result]
-        to [`Result[T, E]`][wraps.result.Result].
+        to a [`Result[T, E]`][wraps.result.Result].
 
         This is equivalent to [`result.or_else(identity)`][wraps.result.ResultProtocol.or_else].
 
         Example:
             ```python
             ok = Ok(42)
             ok_nested = Error(ok)
@@ -1333,15 +1354,15 @@
     #     Returns:
     #         The transposed option.
     #     """
     #     ...
 
     @required
     def contains(self, value: U) -> bool:
-        """Checks if the contained value is equal to `value`.
+        """Checks if the contained value is equal to the `value`.
 
         Example:
             ```python
             value = 42
             other = 69
 
             ok = Ok(value)
@@ -1352,21 +1373,21 @@
             assert not error.contains(value)
             ```
 
         Arguments:
             value: The value to check against.
 
         Returns:
-            Whether the contained value is equal to `value`.
+            Whether the contained value is equal to the `value`.
         """
         ...
 
     @required
     def contains_error(self, error: F) -> bool:
-        """Checks if the contained error value is equal to `error`.
+        """Checks if the contained error value is equal to the `error`.
 
         Example:
             ```python
             value = 42
             other = 69
 
             error = Error(value)
@@ -1377,24 +1398,25 @@
             assert not ok.contains_error(value)
             ```
 
         Arguments:
             error: The error value to check against.
 
         Returns:
-            Whether the contained error value is equal to `error`.
+            Whether the contained error value is equal to the `error`.
         """
         ...
 
     @required
     def flip(self) -> Result[E, T]:
-        """Converts [`Result[T, E]`][wraps.result.Result] to [`Result[E, T]`][wraps.result.Result].
+        """Converts a [`Result[T, E]`][wraps.result.Result]
+        to a [`Result[E, T]`][wraps.result.Result].
 
         [`Ok(value)`][wraps.result.Ok] and [`Error(error)`][wraps.result.Error] get swapped to
-        [`Error(value)`][wraps.result.Error] and [`Ok(error)`][wraps.result.Ok], respectively.
+        [`Error(value)`][wraps.result.Error] and [`Ok(error)`][wraps.result.Ok] respectively.
 
         Example:
             ```python
             value = 42
 
             result = Ok(value)
             flipped = Error(value)
@@ -1406,19 +1428,19 @@
             The flipped result.
         """
         ...
 
     @required
     def into_ok_or_error(self: ResultProtocol[V, V]) -> V:
         """Returns the [`Ok[V]`][wraps.result.Ok] value if `self` is [`Ok[V]`][wraps.result.Ok], and
-        the [`Error[V]`][wraps.result.Error] value if `self` is [`Error[V]`][wraps.result.Error].
+        the [`Error[V]`][wraps.result.Error] value if `self` is an [`Error[V]`][wraps.result.Error].
 
-        In other words, this function returns the value (of type `V`) of
-        a [`Result[V, V]`][wraps.result.Result], regardless of whether or not that result
-        is [`Ok[V]`][wraps.result.Ok] or [`Error[V]`][wraps.result.Error].
+        In other words, this function returns the value of a [`Result[V, V]`][wraps.result.Result],
+        regardless of whether or not that result is
+        [`Ok[V]`][wraps.result.Ok] or [`Error[V]`][wraps.result.Error].
 
         Example:
             ```python
             result: Result[int, int] = Ok(69)
 
             print(result.into_ok_or_error())  # 69
             ```
@@ -1426,21 +1448,44 @@
         Returns:
             The contained value, regardless of whether or not it is an error one.
         """
         ...
 
     @required
     def into_either(self) -> Either[T, E]:
+        """Maps a [`Result[T, E]`][wraps.result.Result] to an [`Either[T, E]`][wraps.either.Either].
+
+        [`Ok(value)`][wraps.result.Ok] is mapped to [`Left(value)`][wraps.either.Left]
+        and [`Error(error)`][wraps.result.Error] is mapped to [`Right(error)`][wraps.either.Right].
+
+        Example:
+            ```python
+            value = 42
+
+            ok = Ok(value)
+            left = Left(value)
+
+            assert ok.into_either() == left
+
+            error = Error(value)
+            right = Right(value)
+
+            assert error.into_either() == right
+            ```
+
+        Returns:
+            The mapped either.
+        """
         ...
 
     @required
     def early(self) -> T:
         """Functionally similar to `?` operator in Rust.
 
-        See [early](/reference/early) for more information.
+        See [`early`][wraps.early] for more information.
         """
         ...
 
 
 UNWRAP_ON_ERROR = "called `unwrap` on error"
 UNWRAP_ERROR_ON_OK = "called `unwrap_error` on ok"
 
@@ -1514,22 +1559,22 @@
         return Null()
 
     def inspect(self, function: Inspect[T]) -> Ok[T]:
         function(self.value)
 
         return self
 
-    def inspect_error(self, function: Inspect[E]) -> Ok[T]:
-        return self
-
     async def inspect_await(self, function: AsyncInspect[T]) -> Ok[T]:
         await function(self.value)
 
         return self
 
+    def inspect_error(self, function: Inspect[E]) -> Ok[T]:
+        return self
+
     async def inspect_error_await(self, function: AsyncInspect[E]) -> Ok[T]:
         return self
 
     def map(self, function: Unary[T, U]) -> Ok[U]:
         return self.create(function(self.value))
 
     def map_or(self, default: U, function: Unary[T, U]) -> U:
@@ -1577,29 +1622,25 @@
         return default()
 
     async def map_error_await_or_else_await(
         self, default: AsyncNullary[F], function: AsyncUnary[E, F]
     ) -> F:
         return await default()
 
-    @wrap_iter
     def iter(self) -> Iterator[T]:
-        yield self.value
+        return once(self.value)
 
-    @wrap_iter
     def iter_error(self) -> Iterator[Never]:
-        return iter.empty().unwrap()
+        return empty()
 
-    @wrap_async_iter
-    async def async_iter(self) -> AsyncIterator[T]:
-        yield self.value
+    def async_iter(self) -> AsyncIterator[T]:
+        return async_once(self.value)
 
-    @wrap_async_iter
     def async_iter_error(self) -> AsyncIterator[Never]:
-        return async_iter.empty().unwrap()
+        return async_empty()
 
     def and_then(self, function: Unary[T, Result[U, E]]) -> Result[U, E]:
         return function(self.value)
 
     async def and_then_await(self, function: AsyncUnary[T, Result[U, E]]) -> Result[U, E]:
         return await function(self.value)
 
@@ -1611,19 +1652,16 @@
 
     def contains(self, value: U) -> bool:
         return self.value == value
 
     def contains_error(self, error: F) -> Literal[False]:
         return False
 
-    def flip(self, error_type: Optional[Type[Error[T]]] = None) -> Error[T]:
-        if error_type is None:
-            error_type = Error[T]
-
-        return error_type(self.value)
+    def flip(self) -> Error[T]:
+        return Error(self.value)
 
     def into_ok_or_error(self: Ok[V]) -> V:
         return self.value
 
     def into_either(self) -> Left[T]:
         return Left(self.value)
 
@@ -1695,28 +1733,28 @@
 
     def unwrap_error_or_else(self, default: Nullary[F]) -> E:
         return self.value
 
     async def unwrap_error_or_else_await(self, default: AsyncNullary[F]) -> E:
         return self.value
 
-    def raising(self: Error[AnyException]) -> Never:
+    def raising(self: Error[AnyError]) -> Never:
         raise self.value
 
     def inspect(self, function: Inspect[T]) -> Error[E]:
         return self
 
+    async def inspect_await(self, function: AsyncInspect[T]) -> Error[E]:
+        return self
+
     def inspect_error(self, function: Inspect[E]) -> Error[E]:
         function(self.value)
 
         return self
 
-    async def inspect_await(self, function: AsyncInspect[T]) -> Error[E]:
-        return self
-
     async def inspect_error_await(self, function: AsyncInspect[E]) -> Error[E]:
         await function(self.value)
 
         return self
 
     def map(self, function: Unary[T, U]) -> Error[E]:
         return self
@@ -1766,25 +1804,25 @@
         return await function(self.value)
 
     async def map_error_await_or_else_await(
         self, default: AsyncNullary[F], function: AsyncUnary[E, F]
     ) -> F:
         return await function(self.value)
 
-    def iter(self) -> Iter[Never]:
-        return iter.empty()
+    def iter(self) -> Iterator[Never]:
+        return empty()
 
-    def iter_error(self) -> Iter[E]:
-        return iter.once(self.value)
+    def iter_error(self) -> Iterator[E]:
+        return once(self.value)
 
-    def async_iter(self) -> AsyncIter[Never]:
-        return async_iter.empty()
+    def async_iter(self) -> AsyncIterator[Never]:
+        return async_empty()
 
-    def async_iter_error(self) -> AsyncIter[E]:
-        return async_iter.once(self.value)
+    def async_iter_error(self) -> AsyncIterator[E]:
+        return async_once(self.value)
 
     def and_then(self, function: Unary[T, Result[U, E]]) -> Error[E]:
         return self
 
     async def and_then_await(self, function: AsyncUnary[T, Result[U, E]]) -> Error[E]:
         return self
 
@@ -1829,171 +1867,9 @@
 def is_error(result: Result[T, E]) -> TypeGuard[Error[E]]:
     """This is the same as [`Result.is_error`][wraps.result.ResultProtocol.is_error],
     except it works as a *type guard*.
     """
     return result.is_error()
 
 
-ET = TypeVar("ET", bound=AnyException)
-FT = TypeVar("FT", bound=AnyException)
-
-
-@final
-@frozen()
-class WrapResult(Generic[ET]):
-    """Wraps a `function` returning `T` into a function returning
-    [`Result[T, ET]`][wraps.result.Result].
-
-    This handles exceptions via returning [`Error(error)`][wraps.result.Error] on `error`,
-    wrapping the resulting `value` into [`Ok(value)`][wraps.result.Ok].
-
-    Example:
-        ```python
-        wrap_value_error = WrapResult(ValueError)
-
-        @wrap_value_error
-        def parse(string: str) -> int:
-            return int(string)
-
-        assert parse("256").is_ok()
-        assert parse("uwu").is_error()
-        ```
-    """
-
-    error_type: Type[ET]
-
-    @classmethod
-    def create(cls, error_type: Type[FT]) -> WrapResult[FT]:
-        return cls(error_type)  # type: ignore
-
-    def __call__(self, function: Callable[P, T]) -> Callable[P, Result[T, ET]]:
-        @wraps(function)
-        def wrap(*args: P.args, **kwargs: P.kwargs) -> Result[T, ET]:
-            try:
-                return Ok(function(*args, **kwargs))
-
-            except self.error_type as error:
-                return Error(error)
-
-        return wrap
-
-    def __getitem__(self, error_type: Type[FT]) -> WrapResult[FT]:
-        return self.create(error_type)
-
-
-if TYPE_CHECKING:
-
-    def wrap_result(function: Callable[P, T]) -> Callable[P, Result[T, Exception]]:
-        """Wraps a `function` returning `T` into a function returning
-        [`Result[T, ET]`][wraps.result.Result].
-
-        By default `ET` is [`Exception`][Exception], so this function returns
-        [`Result[T, Exception]`][wraps.result.Result] unless specified otherwise.
-
-        This handles exceptions via returning [`Error(error)`][wraps.result.Error] on `error`,
-        wrapping the resulting `value` into [`Ok(value)`][wraps.result.Ok].
-
-        Example:
-            ```python
-            @wrap_result[ValueError]
-            def parse(string: str) -> int:
-                return int(string)
-
-            assert parse("512").is_ok()
-            assert parse("uwu").is_error()
-            ```
-
-        Arguments:
-            function: The function to wrap.
-
-        Returns:
-            The wrapping function.
-        """
-        ...
-
-else:
-    wrap_result = WrapResult(Exception)
-
-
-@final
-@frozen()
-class WrapResultAwait(Generic[ET]):
-    """Wraps an asynchronous `function` returning `T` into an asynchronous function returning
-    [`Result[T, ET]`][wraps.result.Result].
-
-    This handles exceptions via returning [`Error(error)`][wraps.result.Error] on `error`,
-    wrapping the resulting `value` into [`Ok(value)`][wraps.result.Ok].
-
-    Example:
-        ```python
-        wrap_value_error_await = WrapResultAwait(ValueError)
-
-        @wrap_value_error_await
-        async def parse(string: str) -> int:
-            return int(string)
-
-        assert (await parse("256")).is_ok()
-        assert (await parse("uwu")).is_error()
-        ```
-    """
-
-    error_type: Type[ET]
-
-    @classmethod
-    def create(cls, error_type: Type[FT]) -> WrapResultAwait[FT]:
-        return cls(error_type)  # type: ignore
-
-    def __call__(
-        self, function: Callable[P, Awaitable[T]]
-    ) -> Callable[P, Awaitable[Result[T, ET]]]:
-        @wraps(function)
-        async def wrap(*args: P.args, **kwargs: P.kwargs) -> Result[T, ET]:
-            try:
-                return Ok(await function(*args, **kwargs))
-
-            except self.error_type as error:
-                return Error(error)
-
-        return wrap
-
-    def __getitem__(self, error_type: Type[FT]) -> WrapResultAwait[FT]:
-        return self.create(error_type)
-
-
-if TYPE_CHECKING:
-
-    def wrap_result_await(
-        function: Callable[P, Awaitable[T]]
-    ) -> Callable[P, Awaitable[Result[T, Exception]]]:
-        """Wraps an asynchronous `function` returning `T` into an asynchronous function returning
-        [`Result[T, ET]`][wraps.result.Result].
-
-        By default `ET` is [`Exception`][Exception], so this function returns
-        [`Result[T, Exception]`][wraps.result.Result] unless specified otherwise.
-
-        This handles exceptions via returning [`Error(error)`][wraps.result.Error] on `error`,
-        wrapping the resulting `value` into [`Ok(value)`][wraps.result.Ok].
-
-        Example:
-            ```python
-            @wrap_result_await[ValueError]
-            async def parse(string: str) -> int:
-                return int(string)
-
-            assert (await parse("512")).is_ok()
-            assert (await parse("uwu")).is_error()
-            ```
-
-        Arguments:
-            function: The asynchronous function to wrap.
-
-        Returns:
-            The asynchronous wrapping function.
-        """
-        ...
-
-else:
-    wrap_result_await = WrapResultAwait(Exception)
-
-
 # import cycle solution
 from wraps.either import Either, Left, Right
```

### Comparing `wraps-0.3.0/setup.py` & `wraps-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,259 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: wraps
+Version: 0.4.0
+Summary: Meaningful and safe wrapping types.
+Home-page: https://github.com/nekitdev/wraps
+License: MIT
+Keywords: python,future,either,option,result
+Author: nekitdev
+Requires-Python: >=3.7
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
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: async-extensions (>=1.2.2)
+Requires-Dist: attrs (>=23.1.0)
+Requires-Dist: funcs (>=0.5.0)
+Requires-Dist: typing-extensions (>=4.5.0)
+Project-URL: Documentation, https://nekitdev.github.io/wraps
+Project-URL: Discord, https://nekit.dev/discord
+Project-URL: Funding, https://patreon.com/nekitdev
+Project-URL: Issues, https://github.com/nekitdev/wraps/issues
+Project-URL: Repository, https://github.com/nekitdev/wraps
+Description-Content-Type: text/markdown
 
-packages = \
-['wraps']
+# `wraps`
 
-package_data = \
-{'': ['*']}
+[![License][License Badge]][License]
+[![Version][Version Badge]][Package]
+[![Downloads][Downloads Badge]][Package]
+[![Discord][Discord Badge]][Discord]
 
-install_requires = \
-['attrs>=22.2.0', 'typing-extensions>=4.3.0']
-
-setup_kwargs = {
-    'name': 'wraps',
-    'version': '0.3.0',
-    'description': 'Meaningful and safe wrapping types.',
-    'long_description': '# `wraps`\n\n[![License][License Badge]][License]\n[![Version][Version Badge]][Package]\n[![Downloads][Downloads Badge]][Package]\n[![Discord][Discord Badge]][Discord]\n\n[![Documentation][Documentation Badge]][Documentation]\n[![Check][Check Badge]][Actions]\n[![Test][Test Badge]][Actions]\n[![Coverage][Coverage Badge]][Coverage]\n\n**Meaningful and safe wrapping types.**\n\n## Installing\n\n**Python 3.7 or above is required.**\n\n### pip\n\nInstalling the library with `pip` is quite simple:\n\n```console\n$ pip install wraps\n```\n\nAlternatively, the library can be installed from source:\n\n```console\n$ git clone https://github.com/nekitdev/wraps.git\n$ cd wraps\n$ python -m pip install .\n```\n\n### poetry\n\nYou can add `wraps` as a dependency with the following command:\n\n```console\n$ poetry add wraps\n```\n\nOr by directly specifying it in the configuration like so:\n\n```toml\n[tool.poetry.dependencies]\nwraps = "^0.3.0"\n```\n\nAlternatively, you can add it directly from the source:\n\n```toml\n[tool.poetry.dependencies.wraps]\ngit = "https://github.com/nekitdev/wraps.git"\n```\n\n## Examples\n\n### Option\n\n[`Option[T]`][wraps.option.Option] type represents an optional value: every option is either\n[`Some[T]`][wraps.option.Some] and contains a value, or [`Null`][wraps.option.Null], and does not.\n\nHere is an example of using [`wrap_option`][wraps.option.wrap_option] to catch any errors:\n\n```python\nfrom typing import List, TypeVar\nfrom wraps import wrap_option\n\nT = TypeVar("T", covariant=True)\n\n\nclass SafeList(List[T]):\n    @wrap_option\n    def get(self, index: int) -> T:\n        return self[index]\n\n\narray = SafeList([0, 1, 2, 3])\n\nprint(array.get(0))  # Some(value=0)\nprint(array.get(7))  # Null()\n```\n\n### Result\n\n[`Result[T, E]`][wraps.result.Result] is the type used for returning and propagating errors.\nIt has two variants, [`Ok[T]`][wraps.result.Ok], representing success and containing a value,\nand [`Error[E]`][wraps.result.Error], representing error and containing an error value.\n\n```python\nfrom wraps import Result, wrap_result\n\n\n@wrap_result[ValueError]\ndef parse(string: str) -> int:\n    return int(string)\n\n\ndef multiply(x: str, y: str) -> Result[int, ValueError]:\n    # try to parse two strings and multiply results\n    return parse(x).and_then(lambda m: parse(y).map(lambda n: m * n))\n\n\nprint(multiply("21", "2").unwrap())  # 42\nprint(multiply("!", "42").unwrap_error())  # invalid literal for `int` with base 10: `!`\n```\n\nIn python versions before 3.9 (where grammar restrictions on decorators were relaxed),\none can use [`wrap_result`][wraps.result.wrap_result] without a concrete type:\n\n```python\n@wrap_result\ndef parse(string: str) -> int:\n    return int(string)\n```\n\nHowever this makes the types less specific, since [`Exception`][Exception]\nis caught instead of [`ValueError`][ValueError].\n\nInstead, you can create a new concrete [`WrapResult[E]`][wraps.result.WrapResult] instance:\n\n```python\nfrom wraps import WrapResult\n\nwrap_value_error = WrapResult(ValueError)\n\n@wrap_value_error\ndef parse(string: str) -> int:\n    return int(string)\n```\n\n### Early Return\n\nEarly return functionality (`?` operator in Rust) is implemented via `early` function\n(for both [`Option`][wraps.option.Option] and [`Result`][wraps.result.Result] types)\ncombined with the [`@early_option`][wraps.early.early_option] or\n[`@early_result`][wraps.early.early_result] decorator respectively.\n\n```python\nfrom wraps import Option, Some, early_option, wrap_option\n\n\n@wrap_option\ndef parse(string: str) -> int:\n    return int(string)\n\n\n@early_option\ndef try_add(x: str, y: str) -> Option[int]:\n    m = parse(x).early()\n    n = parse(y).early()\n\n    return Some(m + n)\n```\n\n## Documentation\n\nYou can find the documentation [here][Documentation].\n\n## Support\n\nIf you need support with the library, you can send us an [email][Email]\nor refer to the official [Discord server][Discord].\n\n## Changelog\n\nYou can find the changelog [here][Changelog].\n\n## Security Policy\n\nYou can find the Security Policy of `wraps` [here][Security].\n\n## Contributing\n\nIf you are interested in contributing to `wraps`, make sure to take a look at the\n[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].\n\n## License\n\n`wraps` is licensed under the MIT License terms. See [License][License] for details.\n\n[Email]: mailto:support@nekit.dev\n\n[Discord]: https://nekit.dev/discord\n\n[Actions]: https://github.com/nekitdev/wraps/actions\n\n[Changelog]: https://github.com/nekitdev/wraps/blob/main/CHANGELOG.md\n[Code of Conduct]: https://github.com/nekitdev/wraps/blob/main/CODE_OF_CONDUCT.md\n[Contributing Guide]: https://github.com/nekitdev/wraps/blob/main/CONTRIBUTING.md\n[Security]: https://github.com/nekitdev/wraps/blob/main/SECURITY.md\n\n[License]: https://github.com/nekitdev/wraps/blob/main/LICENSE\n\n[Package]: https://pypi.org/project/wraps\n[Coverage]: https://codecov.io/gh/nekitdev/wraps\n[Documentation]: https://nekitdev.github.io/wraps\n\n[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2\n[License Badge]: https://img.shields.io/pypi/l/wraps\n[Version Badge]: https://img.shields.io/pypi/v/wraps\n[Downloads Badge]: https://img.shields.io/pypi/dm/wraps\n\n[Documentation Badge]: https://github.com/nekitdev/wraps/workflows/docs/badge.svg\n[Check Badge]: https://github.com/nekitdev/wraps/workflows/check/badge.svg\n[Test Badge]: https://github.com/nekitdev/wraps/workflows/test/badge.svg\n[Coverage Badge]: https://codecov.io/gh/nekitdev/wraps/branch/main/graph/badge.svg\n\n[wraps.option.Option]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Option\n[wraps.option.Some]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Some\n[wraps.option.Null]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Null\n[wraps.option.wrap_option]: https://nekitdev.github.io/wraps/reference/option#wraps.option.wrap_option\n\n[wraps.result.Result]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Result\n[wraps.result.Ok]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Ok\n[wraps.result.Error]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Error\n[wraps.result.wrap_result]: https://nekitdev.github.io/wraps/reference/result#wraps.result.wrap_result\n\n[wraps.result.WrapResult]: https://nekitdev.github.io/wraps/reference/result#wraps.result.WrapResult\n\n[wraps.early.early_option]: https://nekitdev.github.io/wraps/reference/early#wraps.early.early_option\n[wraps.early.early_result]: https://nekitdev.github.io/wraps/reference/early#wraps.early.early_result\n\n[Exception]: https://docs.python.org/3/library/exceptions#Exception\n[ValueError]: https://docs.python.org/3/library/exceptions#ValueError\n',
-    'author': 'nekitdev',
-    'author_email': 'nekitdevofficial@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nekitdev/wraps',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7',
-}
+[![Documentation][Documentation Badge]][Documentation]
+[![Check][Check Badge]][Actions]
+[![Test][Test Badge]][Actions]
+[![Coverage][Coverage Badge]][Coverage]
 
+**Meaningful and safe wrapping types.**
+
+## Installing
+
+**Python 3.7 or above is required.**
+
+### pip
+
+Installing the library with `pip` is quite simple:
+
+```console
+$ pip install wraps
+```
+
+Alternatively, the library can be installed from the source:
+
+```console
+$ git clone https://github.com/nekitdev/wraps.git
+$ cd wraps
+$ python -m pip install .
+```
+
+### poetry
+
+You can add `wraps` as a dependency with the following command:
+
+```console
+$ poetry add wraps
+```
+
+Or by directly specifying it in the configuration like so:
+
+```toml
+[tool.poetry.dependencies]
+wraps = "^0.4.0"
+```
+
+Alternatively, you can add it directly from the source:
+
+```toml
+[tool.poetry.dependencies.wraps]
+git = "https://github.com/nekitdev/wraps.git"
+```
+
+## Examples
+
+### Option
+
+[`Option[T]`][wraps.option.Option] type represents an optional value: every option is either
+[`Some[T]`][wraps.option.Some] and contains a value, or [`Null`][wraps.option.Null], and does not.
+
+Here is an example of using [`wrap_option`][wraps.wraps.wrap_option] to catch any errors:
+
+```python
+from typing import List, TypeVar
+from wraps import wrap_option
+
+T = TypeVar("T", covariant=True)
+
+
+class Array(List[T]):
+    @wrap_option
+    def get(self, index: int) -> T:
+        return self[index]
+
+
+array = Array([1, 2, 3])
+
+print(array.get(0).unwrap())  # 1
+print(array.get(5).unwrap_or(0))  # 0
+```
+
+### Result
+
+[`Result[T, E]`][wraps.result.Result] is the type used for returning and propagating errors.
+It has two variants, [`Ok[T]`][wraps.result.Ok], representing success and containing a value,
+and [`Error[E]`][wraps.result.Error], representing error and containing an error value.
+
+```python
+from enum import Enum
+
+from wraps import Error, Ok, Result
+
+
+class DivideError(Enum):
+    DIVISION_BY_ZERO = "division by zero"
+
+
+def divide(numerator: float, denominator: float) -> Result[float, DivideError]:
+    return Ok(numerator / denominator) if denominator else Error(DivideError.DIVISION_BY_ZERO)
+```
+
+### Early Return
+
+Early return functionality (`?` operator in Rust) is implemented via `early` methods
+(for both [`Option`][wraps.option.Option] and [`Result`][wraps.result.Result] types)
+combined with the [`@early_option`][wraps.early.early_option] and
+[`@early_result`][wraps.early.early_result] decorators respectively.
+
+```python
+from wraps import Option, early_option, wrap_option
+
+
+@wrap_option[ValueError]
+def parse(string: str) -> float:
+    return float(string)
+
+
+@wrap_option[ZeroDivisionError]
+def divide(numerator: float, denominator: float) -> float:
+    return numerator / denominator
+
+
+@early_option
+def function(x: str, y: str) -> Option[float]:
+    return divide(parse(x).early(), parse(y).early())
+```
+
+### Decorators
+
+In Python 3.9 the restrictions on the decorators' syntax have been lifted, which allows for nifty
+syntax which can be seen above. On older versions of Python, one can use:
+
+```python
+from wraps import wrap_option
+
+@wrap_option
+def parse(string: str) -> int:
+    return int(string)
+```
+
+However, this isn't the best way to handle errors, as *any* normal errors will be caught, without
+a way to distinguish between them.
+To counter this, one can use [`WrapOption`][wraps.wraps.WrapOption] directly,
+passing the concrete error type:
+
+```python
+from wraps import WrapOption
+
+wrap_value_error = WrapOption(ValueError)
+
+
+@wrap_value_error
+def parse(string: str) -> int:
+    return int(string)
+```
+
+## Documentation
+
+You can find the documentation [here][Documentation].
+
+## Support
+
+If you need support with the library, you can send us an [email][Email]
+or refer to the official [Discord server][Discord].
+
+## Changelog
+
+You can find the changelog [here][Changelog].
+
+## Security Policy
+
+You can find the Security Policy of `wraps` [here][Security].
+
+## Contributing
+
+If you are interested in contributing to `wraps`, make sure to take a look at the
+[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].
+
+## License
+
+`wraps` is licensed under the MIT License terms. See [License][License] for details.
+
+[Email]: mailto:support@nekit.dev
+
+[Discord]: https://nekit.dev/discord
+
+[Actions]: https://github.com/nekitdev/wraps/actions
+
+[Changelog]: https://github.com/nekitdev/wraps/blob/main/CHANGELOG.md
+[Code of Conduct]: https://github.com/nekitdev/wraps/blob/main/CODE_OF_CONDUCT.md
+[Contributing Guide]: https://github.com/nekitdev/wraps/blob/main/CONTRIBUTING.md
+[Security]: https://github.com/nekitdev/wraps/blob/main/SECURITY.md
+
+[License]: https://github.com/nekitdev/wraps/blob/main/LICENSE
+
+[Package]: https://pypi.org/project/wraps
+[Coverage]: https://codecov.io/gh/nekitdev/wraps
+[Documentation]: https://nekitdev.github.io/wraps
+
+[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2
+[License Badge]: https://img.shields.io/pypi/l/wraps
+[Version Badge]: https://img.shields.io/pypi/v/wraps
+[Downloads Badge]: https://img.shields.io/pypi/dm/wraps
+
+[Documentation Badge]: https://github.com/nekitdev/wraps/workflows/docs/badge.svg
+[Check Badge]: https://github.com/nekitdev/wraps/workflows/check/badge.svg
+[Test Badge]: https://github.com/nekitdev/wraps/workflows/test/badge.svg
+[Coverage Badge]: https://codecov.io/gh/nekitdev/wraps/branch/main/graph/badge.svg
+
+[wraps.option.Option]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Option
+[wraps.option.Some]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Some
+[wraps.option.Null]: https://nekitdev.github.io/wraps/reference/option#wraps.option.Null
+
+[wraps.result.Result]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Result
+[wraps.result.Ok]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Ok
+[wraps.result.Error]: https://nekitdev.github.io/wraps/reference/result#wraps.result.Error
+
+[wraps.wraps.wrap_option]: https://nekitdev.github.io/wraps/reference/wraps#wraps.wraps.wrap_option
+
+[wraps.wraps.WrapOption]: https://nekitdev.github.io/wraps/reference/wraps#wraps.wraps.WrapOption
+
+[wraps.early.early_option]: https://nekitdev.github.io/wraps/reference/early#wraps.early.early_option
+[wraps.early.early_result]: https://nekitdev.github.io/wraps/reference/early#wraps.early.early_result
 
-setup(**setup_kwargs)
```

