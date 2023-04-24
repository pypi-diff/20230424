# Comparing `tmp/retry_extended-0.2.2.tar.gz` & `tmp/retry_extended-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry_extended-0.2.2.tar", max compression
+gzip compressed data, was "retry_extended-0.2.3.tar", max compression
```

## Comparing `retry_extended-0.2.2.tar` & `retry_extended-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-10 19:27:09.510070 retry_extended-0.2.2/LICENSE
--rw-r--r--   0        0        0     1232 2023-04-10 19:27:09.510070 retry_extended-0.2.2/README.md
--rw-r--r--   0        0        0     1172 2023-04-10 19:27:09.510070 retry_extended-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      252 2023-04-10 19:27:09.510070 retry_extended-0.2.2/retry/__init__.py
--rw-r--r--   0        0        0     7280 2023-04-10 19:27:09.510070 retry_extended-0.2.2/retry/api.py
--rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 retry_extended-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 06:54:38.311386 retry_extended-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1232 2023-04-24 06:54:38.311386 retry_extended-0.2.3/README.md
+-rw-r--r--   0        0        0     1172 2023-04-24 06:54:38.311386 retry_extended-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-04-24 06:54:38.311386 retry_extended-0.2.3/retry/__init__.py
+-rw-r--r--   0        0        0     7511 2023-04-24 06:54:38.311386 retry_extended-0.2.3/retry/api.py
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 retry_extended-0.2.3/PKG-INFO
```

### Comparing `retry_extended-0.2.2/LICENSE` & `retry_extended-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `retry_extended-0.2.2/README.md` & `retry_extended-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 Retry API compatible maintained project
 
 This package had been developed on top of the original python [retry](https://github.com/invl/retry) package, and is intended to develop on top of it without implementing any breaking API changes and keeping the simplicity of the package.
 
 
 ### Roadmap
-- [ ] Type Hints and Annotations & Clean up code
-- [ ] Follow [Google Style guide](https://google.github.io/styleguide/pyguide.html)
-- [ ] Async implementation for retry
+- [x] Type Hints and Annotations & Clean up code
+- [x] Follow [Google Style guide](https://google.github.io/styleguide/pyguide.html)
+- [x] Async implementation for retry
```

### Comparing `retry_extended-0.2.2/pyproject.toml` & `retry_extended-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retry-extended"
-version = "0.2.2"
+version = "0.2.3"
 description = "Retry API compatible extended library"
 authors = ["Strollby Developers <backend.developers@strollby.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/strollby/retry-extended"
 repository = "https://github.com/strollby/retry-extended"
 documentation = "https://github.com/strollby/retry-extended"
```

### Comparing `retry_extended-0.2.2/retry/api.py` & `retry_extended-0.2.3/retry/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import asyncio
 import logging
 import random
 import time
-
+import functools
 from typing import Callable, Optional, Any
 
-
 DEFAULT_LOGGER = logging.getLogger(__name__)
 DEFAULT_ASYNC_LOGGER = logging.getLogger("asyncio")
 
 
 def __retry_internal(
-    f: Callable,
-    args: tuple,
-    kwargs: dict,
-    exceptions: tuple = (Exception,),
-    tries: int = -1,
-    delay: int = 0,
-    max_delay: Optional[int] = None,
-    backoff: int = 1,
-    jitter: int = 0,
-    logger: logging.Logger = DEFAULT_LOGGER,
+        f: Callable,
+        args: tuple,
+        kwargs: dict,
+        exceptions: tuple = (Exception,),
+        tries: int = -1,
+        delay: int = 0,
+        max_delay: Optional[int] = None,
+        backoff: int = 1,
+        jitter: int = 0,
+        logger: logging.Logger = DEFAULT_LOGGER,
 ):
     """
     Executes a function and retries it if it failed.
 
     Args:
         f:
             the function to execute.
@@ -68,24 +67,24 @@
                 _delay += jitter
 
             if max_delay is not None:
                 _delay = min(_delay, max_delay)
 
 
 async def __retry_internal_async(
-    f: Callable,
-    args: tuple,
-    kwargs: dict,
-    exceptions: tuple = (Exception,),
-    tries: int = -1,
-    delay: int = 0,
-    max_delay: Optional[int] = None,
-    backoff: int = 1,
-    jitter: int = 0,
-    logger: logging.Logger = DEFAULT_ASYNC_LOGGER,
+        f: Callable,
+        args: tuple,
+        kwargs: dict,
+        exceptions: tuple = (Exception,),
+        tries: int = -1,
+        delay: int = 0,
+        max_delay: Optional[int] = None,
+        backoff: int = 1,
+        jitter: int = 0,
+        logger: logging.Logger = DEFAULT_ASYNC_LOGGER,
 ):
     """
     Executes a function and retries it if it failed.
 
     Args:
         f:
             the coroutine function to execute.
@@ -129,22 +128,22 @@
                 _delay += jitter
 
             if max_delay is not None:
                 _delay = min(_delay, max_delay)
 
 
 def retry(
-    # func,
-    exceptions: tuple = (Exception,),
-    tries: int = -1,
-    delay: int = 0,
-    max_delay: Optional[int] = None,
-    backoff: int = 1,
-    jitter: int = 0,
-    logger: logging.Logger = DEFAULT_LOGGER,
+        # func,
+        exceptions: tuple = (Exception,),
+        tries: int = -1,
+        delay: int = 0,
+        max_delay: Optional[int] = None,
+        backoff: int = 1,
+        jitter: int = 0,
+        logger: logging.Logger = DEFAULT_LOGGER,
 ):
     """
     Returns a retry decorator.
 
     Args:
         exceptions:
             an exception or a tuple of exceptions to catch. default: Exception.
@@ -164,40 +163,42 @@
             default: retry.DEFAULT_LOGGER. if None, logging is disabled.
 
     Returns:
         a retry decorator.
     """
 
     def retry_decorator(func):
-        def wrapper(*args: dict, **kwargs: dict) -> Any:
+        @functools.wraps(func)
+        def wrapper(*args: tuple, **kwargs: dict) -> Any:
             return __retry_internal(func, args, kwargs, exceptions, tries, delay, max_delay, backoff, jitter, logger)
 
-        async def wrapper_async(*args: dict, **kwargs: dict) -> Any:
+        @functools.wraps(func)
+        async def wrapper_async(*args: tuple, **kwargs: dict) -> Any:
             return await __retry_internal_async(
                 func, args, kwargs, exceptions, tries, delay, max_delay, backoff, jitter, logger
             )
 
         if asyncio.iscoroutinefunction(func):
             return wrapper_async
         return wrapper
 
     return retry_decorator
 
 
 def retry_call(
-    f,
-    fargs: tuple = None,
-    fkwargs: dict = None,
-    exceptions: tuple = (Exception,),
-    tries: int = -1,
-    delay: int = 0,
-    max_delay: Optional[int] = None,
-    backoff: int = 1,
-    jitter: int = 0,
-    logger: logging.Logger = DEFAULT_LOGGER,
+        f,
+        fargs: tuple = None,
+        fkwargs: dict = None,
+        exceptions: tuple = (Exception,),
+        tries: int = -1,
+        delay: int = 0,
+        max_delay: Optional[int] = None,
+        backoff: int = 1,
+        jitter: int = 0,
+        logger: logging.Logger = DEFAULT_LOGGER,
 ):
     """
     Calls a function and re-executes it if it failed.
 
     Args:
         f:
             the function to execute.
```

### Comparing `retry_extended-0.2.2/PKG-INFO` & `retry_extended-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-extended
-Version: 0.2.2
+Version: 0.2.3
 Summary: Retry API compatible extended library
 Home-page: https://github.com/strollby/retry-extended
 License: Apache-2.0
 Keywords: retry,retry-extended,python-retry
 Author: Strollby Developers
 Author-email: backend.developers@strollby.com
 Requires-Python: >=3.7,<4.0
@@ -32,11 +32,11 @@
 
 Retry API compatible maintained project
 
 This package had been developed on top of the original python [retry](https://github.com/invl/retry) package, and is intended to develop on top of it without implementing any breaking API changes and keeping the simplicity of the package.
 
 
 ### Roadmap
-- [ ] Type Hints and Annotations & Clean up code
-- [ ] Follow [Google Style guide](https://google.github.io/styleguide/pyguide.html)
-- [ ] Async implementation for retry
+- [x] Type Hints and Annotations & Clean up code
+- [x] Follow [Google Style guide](https://google.github.io/styleguide/pyguide.html)
+- [x] Async implementation for retry
```

