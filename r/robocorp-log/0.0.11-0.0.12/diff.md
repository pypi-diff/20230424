# Comparing `tmp/robocorp_log-0.0.11.tar.gz` & `tmp/robocorp_log-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log-0.0.11.tar", max compression
+gzip compressed data, was "robocorp_log-0.0.12.tar", max compression
```

## Comparing `robocorp_log-0.0.11.tar` & `robocorp_log-0.0.12.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    10142 2023-04-23 10:52:54.724253 robocorp_log-0.0.11/LICENSE
--rw-r--r--   0        0        0     1021 2023-04-23 10:52:54.724253 robocorp_log-0.0.11/README.md
--rw-r--r--   0        0        0      904 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/pyproject.toml
--rw-r--r--   0        0        0    16923 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/__init__.py
--rw-r--r--   0        0        0     8406 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_ast_utils.py
--rw-r--r--   0        0        0     8469 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_auto_logging_setup.py
--rw-r--r--   0        0        0     5361 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_config.py
--rw-r--r--   0        0        0      572 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_convert_units.py
--rw-r--r--   0        0        0     6699 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_decoder.py
--rw-r--r--   0        0        0    43217 2023-04-23 10:53:35.752983 robocorp_log-0.0.11/src/robocorp/log/_index.py
--rw-r--r--   0        0        0    55054 2023-04-23 10:53:38.061025 robocorp_log-0.0.11/src/robocorp/log/_index_v2.py
--rw-r--r--   0        0        0     2305 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_lifecycle_hooks.py
--rw-r--r--   0        0        0      493 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_logger_instances.py
--rw-r--r--   0        0        0     1208 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_null.py
--rw-r--r--   0        0        0      385 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_obj_info_repr.py
--rw-r--r--   0        0        0    18981 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0     8900 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12339 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_rewrite_importhook.py
--rw-r--r--   0        0        0     9559 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_robo_logger.py
--rw-r--r--   0        0        0    51643 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/_robo_output_impl.py
--rw-r--r--   0        0        0     1057 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/protocols.py
--rw-r--r--   0        0        0        0 2023-04-23 10:52:54.728253 robocorp_log-0.0.11/src/robocorp/log/py.typed
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 robocorp_log-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-24 19:07:45.261923 robocorp_log-0.0.12/LICENSE
+-rw-r--r--   0        0        0     3086 2023-04-24 19:07:45.261923 robocorp_log-0.0.12/README.md
+-rw-r--r--   0        0        0      904 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0    21137 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/__init__.py
+-rw-r--r--   0        0        0     8406 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_ast_utils.py
+-rw-r--r--   0        0        0     8441 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     5361 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_config.py
+-rw-r--r--   0        0        0      572 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_convert_units.py
+-rw-r--r--   0        0        0     6699 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_decoder.py
+-rw-r--r--   0        0        0    43217 2023-04-24 19:08:29.798847 robocorp_log-0.0.12/src/robocorp/log/_index.py
+-rw-r--r--   0        0        0    55054 2023-04-24 19:08:32.106892 robocorp_log-0.0.12/src/robocorp/log/_index_v2.py
+-rw-r--r--   0        0        0     2305 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_logger_instances.py
+-rw-r--r--   0        0        0     1208 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_null.py
+-rw-r--r--   0        0        0      385 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_obj_info_repr.py
+-rw-r--r--   0        0        0    18981 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     8900 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12339 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     8710 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_robo_logger.py
+-rw-r--r--   0        0        0    51335 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_robo_output_impl.py
+-rw-r--r--   0        0        0     1436 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_sensitive_variable_names.py
+-rw-r--r--   0        0        0     1915 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/_suppress_helper.py
+-rw-r--r--   0        0        0     1057 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:07:45.265923 robocorp_log-0.0.12/src/robocorp/log/py.typed
+-rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 robocorp_log-0.0.12/PKG-INFO
```

### Comparing `robocorp_log-0.0.11/LICENSE` & `robocorp_log-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/pyproject.toml` & `robocorp_log-0.0.12/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-log"
-version = "0.0.11"
+version = "0.0.12"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/log", from = "src"}]
 include = ["**/_index.py", "**/_index_v2.py"]
```

### Comparing `robocorp_log-0.0.11/src/robocorp/log/__init__.py` & `robocorp_log-0.0.12/src/robocorp/log/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,27 +16,37 @@
     Iterator,
     List,
     Sequence,
     Dict,
     Union,
     Iterable,
     Literal,
+    overload,
+    Callable,
+    Protocol,
 )
 from ._logger_instances import _get_logger_instances
 from .protocols import OptExcInfo, LogHTMLStyle, Status, IReadLines
+from ._suppress_helper import SuppressHelper as _SuppressHelper
 
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "0.0.11"
+__version__ = "0.0.12"
 version_info = [int(x) for x in __version__.split(".")]
 
+from . import _config
+
 # --- Make these a part of the public API.
-from ._config import Filter, FilterKind, BaseConfig, ConfigFilesFiltering
+
+Filter = _config.Filter
+FilterKind = _config.FilterKind
+BaseConfig = _config.BaseConfig
+ConfigFilesFiltering = _config.ConfigFilesFiltering
 
 
 # --- Logging methods for custom messaging.
 
 
 def _log(level, message: str, html: bool = False) -> None:
     back_frame = sys._getframe(2)
@@ -96,148 +106,309 @@
         robo_logger.log_method_except(exc_info, unhandled=True)
 
 
 # --- Methods related to hiding logging information.
 
 
 @contextmanager
-def stop_logging_methods():
-    """
-    Can be used so that method calls are no longer logged.
+def _suppress_contextmanager(variables=True, methods=True):
+    instances = _get_logger_instances()
+    for robo_logger in instances:
+        if variables:
+            robo_logger.stop_logging_variables()
+        if methods:
+            robo_logger.stop_logging_methods()
 
-    i.e.:
-        with stop_logging_methods():
-            ...
-    """
-    for robo_logger in _get_logger_instances():
-        robo_logger.stop_logging_methods()
     try:
         yield
     finally:
-        start_logging_methods()
+        for robo_logger in instances:
+            if variables:
+                robo_logger.start_logging_variables()
+            if methods:
+                robo_logger.start_logging_methods()
 
 
-def start_logging_methods():
+_suppress_helper = _SuppressHelper(_suppress_contextmanager)
+
+
+def suppress_methods():
     """
-    Usually doesn't need to be called as `stop_logging_methods` should be used
-    as a context manager (which would automatically call this method).
+    Can be used as a context manager or decorator so that methods are no
+    longer logged.
+
+    i.e.:
+        @suppress_methods
+        def method():
+            ...
+
+        or
 
-    Can still be used if `stop_logging_methods` with a try..finally if
-    `stop_logging_methods` isn't used as a context manager.
+        with suppress_methods():
+            ...
     """
-    for robo_logger in _get_logger_instances():
-        robo_logger.start_logging_methods()
+    return suppress(variables=False, methods=True)
 
 
-@contextmanager
-def stop_logging_variables():
+def suppress_variables():
     """
-    Can be used (as a context manager) so that variables are no longer logged.
+    Can be used as a context manager or decorator so that variables are no
+    longer logged.
 
     i.e.:
-        with stop_logging_variables():
+        @suppress_variables
+        def method():
+            ...
+
+        or
+
+        with suppress_variables():
             ...
     """
-    for robo_logger in _get_logger_instances():
-        robo_logger.stop_logging_variables()
+    return suppress(variables=True, methods=False)
 
-    try:
-        yield
-    finally:
-        start_logging_variables()
+
+class _AnyCall(Protocol):
+    def __call__(self, *args, **kwargs) -> Any:
+        pass
 
 
-def start_logging_variables():
+@overload
+def suppress(*, variables: bool = True, methods: bool = True) -> _AnyCall:
     """
-    Usually doesn't need to be called as `stop_logging_variables` should be used
-    as a context manager (which would automatically call this method).
+    Arguments when used as a decorator or context manager with parameters.
 
-    Can still be used if `stop_logging_variables` with a try..finally if
-    `stop_logging_variables` isn't used as a context manager.
+    Suppresses everything except the arguments marked as "False"
     """
-    for robo_logger in _get_logger_instances():
-        robo_logger.start_logging_variables()
+
+
+@overload
+def suppress(func: Callable[[], Any]) -> _AnyCall:
+    """
+    Arguments when used as a decorator without any arguments (where it just
+    receives a function).
+    """
+
+
+def suppress(*args, **kwargs):
+    """
+    API to suppress logging to be used as a context manager or decorator.
+
+    By default suppresses everything and its actual API is something as:
+
+    def suppress(variables:bool = True, methods:bool = True):
+        ...
+
+    Args:
+        variables: Whether variables should be suppressed in the scope.
+
+        methods: Whether method calls should be suppressed in the scope.
+
+    Usage as a decorator:
+
+        from robocorp import log
+
+        @log.suppress
+        def func():
+            ....
+
+    Usage as a decorator suppressing only variables:
+
+        from robocorp import log
+
+        @log.suppress(methods=False)
+        def func():
+            ....
+
+    Usage as a context manager:
+
+        from robocorp import log
+
+        with log.suppress(methods=False):
+            ....
+    """
+    return _suppress_helper.handle(*args, **kwargs)
+
+
+from ._sensitive_variable_names import (
+    SensitiveVariableNames as _SensitiveVariableNames,
+)
+
+_sensitive_names = _SensitiveVariableNames(("password", "passwd"))
+
+
+def is_sensitive_variable_name(variable_name: str) -> bool:
+    """
+    Args:
+        variable_name: The variable name to be checked.
+
+    Returns:
+        True if the given variable name is considered to be sensitive (in which
+        case its value should be redacted) and False otherwise.
+    """
+    return _sensitive_names.is_sensitive_variable_name(variable_name)
+
+
+def add_sensitive_variable_name(variable_name: str) -> None:
+    """
+    Marks a given variable name as sensitive (in which case any variable
+    containing the given `variable_name` will be redacted).
+
+    Note that this will add a patterns where any variable containing the given
+    variable name even as a substring will be considered sensitive.
+
+    Args:
+        variable_name: The variable name to be considered sensitive.
+    """
+    _sensitive_names.add_sensitive_variable_name(variable_name)
+
+
+def add_sensitive_variable_name_pattern(variable_name_pattern: str) -> None:
+    """
+    Adds a given pattern to consider a variable name as sensitive. Any variable
+    name matching the given pattern will have its value redacted.
+
+    Args:
+        variable_name_pattern: The variable name pattern to be considered
+        sensitive.
+    """
+    _sensitive_names.add_sensitive_variable_name_pattern(variable_name_pattern)
 
 
 def hide_from_output(string_to_hide: str) -> None:
     """
     Should be called to hide sensitive information from appearing in the output.
 
+    Note that any variable assign or argument which is set to a name containing
+    the string:
+
+    'password' or 'passwd'
+
+    Will be automatically hidden and it's also possible to add new names to
+    be automatically redacted withe the methods: `add_sensitive_variable_name`
+    and `add_sensitive_variable_name_pattern`.
+
     Args:
         string_to_hide: The string that should be hidden from the output.
     """
     for robo_logger in _get_logger_instances():
         robo_logger.hide_from_output(string_to_hide)
 
 
 # --- Logging methods usually called automatically from the framework.
 
 
 def start_run(name: str) -> None:
+    """
+    Starts a run session (adds the related event to the log).
+
+    Args:
+        name: The name of the run.
+
+    Note: robocorp-tasks calls this method automatically.
+    """
     for robo_logger in _get_logger_instances():
         robo_logger.start_run(name)
 
 
 def end_run(name: str, status: str) -> None:
+    """
+    Finishes a run session (adds the related event to the log).
+
+    Args:
+        name: The name of the run.
+        status: The run status.
+
+    Note: robocorp-tasks calls this method automatically.
+    """
     for robo_logger in _get_logger_instances():
         robo_logger.end_run(name, status)
 
 
-def start_task(
-    name: str, libname: str, source: str, lineno: int, tags: Sequence[str]
-) -> None:
+def start_task(name: str, libname: str, source: str, lineno: int) -> None:
+    """
+    Starts a task (adds the related event to the log).
+
+    Args:
+        name: The name of the task.
+        libname: The library (module name) where the task is defined.
+        source: The source of the task.
+        lineno: The line number of the task in the given source.
+
+    Note: robocorp-tasks calls this method automatically.
+    """
     for robo_logger in _get_logger_instances():
-        robo_logger.start_task(name, libname, source, lineno, tags)
+        robo_logger.start_task(name, libname, source, lineno)
 
 
 def end_task(name: str, libname: str, status: str, message: str) -> None:
+    """
+    Ends a task (adds the related event to the log).
+
+    Args:
+        name: The name of the task.
+        libname: The library (module name) where the task is defined.
+        status: The source of the task.
+        message: The line number of the task in the given source.
+
+    Note: robocorp-tasks calls this method automatically.
+    """
     for robo_logger in _get_logger_instances():
         robo_logger.end_task(name, libname, status, message)
 
 
+# ---- APIs to decode existing log files
+
+
 def iter_decoded_log_format_from_stream(stream: IReadLines) -> Iterator[dict]:
     """
     Args:
         stream: The stream which should be iterated in (anything with a
-            `readlines()` method).
+            `readlines()` method which should provide the messages encoded
+            in the internal format).
 
     Returns:
         An iterator which will decode the messages and provides a dictionary for
         each message found.
 
         Example of messages provided:
 
         {'message_type': 'V', 'version': '1'}
         {'message_type': 'T', 'initial_time': '2022-10-31T07:45:57.116'}
         {'message_type': 'ID', 'part': 1, 'id': 'gen-from-output-xml'}
         {'message_type': 'SR', 'name': 'Robot Check', 'time_delta_in_seconds': 0.3}
-        {'message_type': 'ST', 'name': 'My task', 'libname': 'foo', 'source': 'x:\\vscode-robot\\local_test\\robot_check', 'lineno': 5, 'time_delta_in_seconds': 0.2}
+        ...
+
+        Note: the exact format of the messages provided is not stable across
+        releases.
     """
     from ._decoder import iter_decoded_log_format
 
     return iter_decoded_log_format(stream)
 
 
 def iter_decoded_log_format_from_log_html(log_html: Path) -> Iterator[dict]:
     """
-    This function will read the chunks saved in the log html and provide
-    an iterator which will provide the messages which were encoded into it.
+    This function will read the data saved in the log html and provide an
+    iterator which will provide the decoded messages which were encoded into it.
 
     Returns:
         An iterator which will decode the messages and provides a dictionary for
         each message found.
 
         Example of messages provided:
 
         {'message_type': 'V', 'version': '1'}
         {'message_type': 'T', 'initial_time': '2022-10-31T07:45:57.116'}
         {'message_type': 'ID', 'part': 1, 'id': 'gen-from-output-xml'}
         {'message_type': 'SR', 'name': 'Robot Check', 'time_delta_in_seconds': 0.3}
-        {'message_type': 'ST', 'name': 'My task', 'libname': 'foo', 'source': 'x:\\vscode-robot\\local_test\\robot_check', 'lineno': 5, 'time_delta_in_seconds': 0.2}
+        ...
 
+        Note: the exact format of the messages provided is not stable across
+        releases.
     """
     import zlib
     import base64
     from ast import literal_eval
 
     txt = log_html.read_text(encoding="utf-8")
     i = txt.find("let chunks = [")
@@ -274,16 +445,16 @@
 
 def verify_log_messages_from_messages_iterator(
     messages_iterator: Iterator[dict],
     expected: Sequence[dict],
     not_expected: Sequence[dict] = _DEFAULT_NOT_EXPECTED,
 ) -> List[dict]:
     """
-    A helper for checking that the expected messages are found in the
-    given messages iterator.
+    A helper for checking that the expected messages are found (or not found) in
+    the given messages iterator.
 
     Args:
         messages_iterator: An iterator over the messages found.
         expected: The messages which are expected to be found. If some message
             expected to be found is not found an AssertionError will be raised.
         not_expected: The messages that should not appear.
 
@@ -407,14 +578,17 @@
         matching of messages.
     """
     return verify_log_messages_from_messages_iterator(
         iter_decoded_log_format_from_stream(stream), expected, not_expected
     )
 
 
+# --- APIs to setup the logging
+
+
 def setup_auto_logging(config: Optional[BaseConfig] = None):
     """
     Sets up automatic logging.
 
     This must be called prior to actually importing the modules which should
     be automatically logged.
 
@@ -519,14 +693,16 @@
     def _exit():
         _get_logger_instances().pop(logger, None)
         logger.close()
 
     return OnExitContextManager(_exit)
 
 
+# --- Private APIs
+
 # Not part of the API, used to determine whether a file is a project file
 # or a library file when running with the FilterKind.log_on_project_call kind.
 from ._rewrite_filtering import FilesFiltering
 
 _files_filtering = FilesFiltering()
 _in_project_roots = _files_filtering.in_project_roots
```

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_ast_utils.py` & `robocorp_log-0.0.12/src/robocorp/log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_auto_logging_setup.py` & `robocorp_log-0.0.12/src/robocorp/log/_auto_logging_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from robocorp.log import critical
+from robocorp.log import critical, is_sensitive_variable_name
 from ._config import BaseConfig
 from ._logger_instances import _get_logger_instances
 from ._obj_info_repr import get_obj_type_and_repr
 from .protocols import OptExcInfo, Status
 import sys
 import threading
 from typing import Tuple, List, Any, Optional
@@ -20,21 +20,19 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.on_exit()
 
 
 def _get_obj_type_and_repr_and_hide_if_needed(key, val):
     obj_type, obj_repr = get_obj_type_and_repr(val)
 
-    for p in ("password", "passwd"):
-        if p in key:
-            for robo_logger in _get_logger_instances():
-                robo_logger.hide_from_output(obj_repr)
-                if isinstance(val, str):
-                    robo_logger.hide_from_output(val)
-            break
+    if is_sensitive_variable_name(key):
+        for robo_logger in _get_logger_instances():
+            robo_logger.hide_from_output(obj_repr)
+            if isinstance(val, str):
+                robo_logger.hide_from_output(val)
     return obj_type, obj_repr
 
 
 class _StackEntry:
     __slots__ = "mod_name name status".split()
 
     def __init__(self, mod_name, name, status):
@@ -134,15 +132,15 @@
                     critical(
                         f"On method return status stack package/name was: {pop_stack_entry.mod_name}.{pop_stack_entry.name}. Received: {mod_name}.{name}."
                     )
                     return
             status = pop_stack_entry.status
 
         for robo_logger in _get_logger_instances():
-            robo_logger.end_method(method_type, name, mod_name, status, [])
+            robo_logger.end_method(method_type, name, mod_name, status)
 
     def call_before_yield(
         self,
         mod_name: str,
         filename: str,
         name: str,
         lineno: int,
```

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_config.py` & `robocorp_log-0.0.12/src/robocorp/log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_convert_units.py` & `robocorp_log-0.0.12/src/robocorp/log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_decoder.py` & `robocorp_log-0.0.12/src/robocorp/log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_index.py` & `robocorp_log-0.0.12/src/robocorp/log/_index.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_index_v2.py` & `robocorp_log-0.0.12/src/robocorp/log/_index_v2.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_lifecycle_hooks.py` & `robocorp_log-0.0.12/src/robocorp/log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_null.py` & `robocorp_log-0.0.12/src/robocorp/log/_null.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_rewrite_ast_add_callbacks.py` & `robocorp_log-0.0.12/src/robocorp/log/_rewrite_ast_add_callbacks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_rewrite_filtering.py` & `robocorp_log-0.0.12/src/robocorp/log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_rewrite_importhook.py` & `robocorp_log-0.0.12/src/robocorp/log/_rewrite_importhook.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_robo_logger.py` & `robocorp_log-0.0.12/src/robocorp/log/_robo_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,34 +137,24 @@
         )
 
     @_log_error
     def end_run(self, name: str, status: str):
         return self._robot_output_impl.end_run(name, status, self._get_time_delta())
 
     @_log_error
-    def start_task(
-        self, name: str, libname: str, source: str, lineno: int, tags: Sequence[str]
-    ):
+    def start_task(self, name: str, libname: str, source: str, lineno: int):
         return self._robot_output_impl.start_task(
             name,
             libname,
             source,
             lineno,
             self._get_time_delta(),
-            tags,
         )
 
     @_log_error
-    def send_tag(self, tag: str):
-        if self._skip_log_methods:
-            return
-
-        return self._robot_output_impl.send_tag(tag)
-
-    @_log_error
     def send_info(self, info: str):
         return self._robot_output_impl.send_info(info)
 
     @_log_error
     def send_start_time_delta(self, time_delta_in_seconds: float):
         if self._skip_log_methods:
             return
@@ -201,29 +191,20 @@
             "c:/my/browser.py",
             lineno=1,
             element_type="METHOD",
             doc="Closes Browser",
             args=[("force", "boolean", "True")],
         )
         """
-        hide_from_logs = False
-        if self._skip_log_methods:
-            if name not in (
-                "stop_logging_methods",
-                "start_logging_methods",
-            ):
-                hide_from_logs = True
+        hide_from_logs = bool(self._skip_log_methods)
 
         if args:
             if self._skip_log_variables:
                 args = []
 
-            elif name == "hide_from_output":
-                args = [(name, tp, "<redacted>") for name, tp, _value in args]
-
         return self._robot_output_impl.start_element(
             name,
             libname,
             element_type,
             doc,
             source,
             lineno,
@@ -235,18 +216,15 @@
     def yield_resume(
         self,
         name: str,
         libname: str,
         source: str,
         lineno: int,
     ):
-        hide_from_logs = False
-
-        if self._skip_log_methods:
-            hide_from_logs = True
+        hide_from_logs = bool(self._skip_log_methods)
 
         return self._robot_output_impl.yield_resume(
             name,
             libname,
             source,
             lineno,
             self._get_time_delta(),
@@ -300,26 +278,18 @@
     @_log_error
     def end_method(
         self,
         element_type: LogElementType,
         name: str,
         libname: str,
         status: str,
-        tags: Sequence[str],
     ):
-        try:
-            return self._robot_output_impl.end_method(
-                element_type, name, libname, status, self._get_time_delta()
-            )
-        finally:
-            if tags:
-                if "log:ignore-methods" in tags:
-                    self._skip_log_methods -= 1
-                if "log:ignore-variables" in tags:
-                    self._skip_log_variables -= 1
+        return self._robot_output_impl.end_method(
+            element_type, name, libname, status, self._get_time_delta()
+        )
 
     @_log_error
     def log_message(
         self, level: str, message: str, html: bool, source: str, lineno: int
     ):
         return self._robot_output_impl.log_message(
             level, message, html, source, lineno, self._get_time_delta()
```

### Comparing `robocorp_log-0.0.11/src/robocorp/log/_robo_output_impl.py` & `robocorp_log-0.0.12/src/robocorp/log/_robo_output_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,14 @@
     def start_task(
         self,
         name: str,
         libname: str,
         source: str,
         line: int,
         time_delta: float,
-        tags: Sequence[str],
     ):
         oid = self._obtain_id
         task_id = f"{libname}.{name}"
         with self._stack_handler.push_record("task", task_id, "ST", "RT"):
             self._write_with_separator(
                 "ST ",
                 [
@@ -435,27 +434,14 @@
                     oid(libname),
                     oid(source),
                     self._number(line),
                     self._number(time_delta),
                 ],
             )
 
-            if tags:
-                for tag in tags:
-                    self.send_tag(tag)
-
-    def send_tag(self, tag: str):
-        oid = self._obtain_id
-        self._write_with_separator(
-            "TG ",
-            [
-                oid(tag),
-            ],
-        )
-
     def send_info(self, info: str):
         self._write_json("I ", info)
 
     def send_start_time_delta(self, time_delta_in_seconds: float):
         self._write_with_separator("S ", (self._number(time_delta_in_seconds),))
 
     def end_task(
```

### Comparing `robocorp_log-0.0.11/src/robocorp/log/protocols.py` & `robocorp_log-0.0.12/src/robocorp/log/protocols.py`

 * *Files identical despite different names*

