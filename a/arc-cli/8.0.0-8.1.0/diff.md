# Comparing `tmp/arc_cli-8.0.0.tar.gz` & `tmp/arc_cli-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc_cli-8.0.0.tar", max compression
+gzip compressed data, was "arc_cli-8.1.0.tar", max compression
```

## Comparing `arc_cli-8.0.0.tar` & `arc_cli-8.1.0.tar`

### file list

```diff
@@ -1,67 +1,75 @@
--rw-r--r--   0        0        0      864 2023-02-03 03:54:22.780978 arc_cli-8.0.0/README.md
--rw-r--r--   0        0        0      564 2023-02-03 03:55:02.870566 arc_cli-8.0.0/arc/__init__.py
--rw-r--r--   0        0        0     6475 2022-08-26 04:11:43.412650 arc_cli-8.0.0/arc/autocompletions.py
--rw-r--r--   0        0        0     2093 2022-08-26 04:11:43.412650 arc_cli-8.0.0/arc/autoload.py
--rw-r--r--   0        0        0     8911 2023-02-03 03:54:22.784311 arc_cli-8.0.0/arc/color.py
--rw-r--r--   0        0        0     4117 2023-02-03 03:54:22.784311 arc_cli-8.0.0/arc/config.py
--rw-r--r--   0        0        0      247 2022-08-26 04:11:43.415983 arc_cli-8.0.0/arc/constants.py
--rw-r--r--   0        0        0     1634 2023-02-03 03:54:22.784311 arc_cli-8.0.0/arc/context.py
--rw-r--r--   0        0        0       50 2023-02-03 03:54:22.784311 arc_cli-8.0.0/arc/core/__init__.py
--rw-r--r--   0        0        0     4028 2023-02-03 03:54:22.784311 arc_cli-8.0.0/arc/core/app.py
--rw-r--r--   0        0        0     2818 2023-02-03 03:54:22.784311 arc_cli-8.0.0/arc/core/classful.py
--rw-r--r--   0        0        0    11792 2023-02-03 03:54:22.784311 arc_cli-8.0.0/arc/core/command.py
--rw-r--r--   0        0        0     4403 2022-08-26 04:11:43.415983 arc_cli-8.0.0/arc/core/documentation.py
--rw-r--r--   0        0        0      132 2023-02-03 03:54:22.787644 arc_cli-8.0.0/arc/core/middleware/__init__.py
--rw-r--r--   0        0        0     9147 2023-02-03 03:54:22.787644 arc_cli-8.0.0/arc/core/middleware/exec.py
--rw-r--r--   0        0        0     6598 2023-02-03 03:54:22.787644 arc_cli-8.0.0/arc/core/middleware/init.py
--rw-r--r--   0        0        0      322 2023-02-03 03:54:22.787644 arc_cli-8.0.0/arc/core/middleware/middleware.py
--rw-r--r--   0        0        0      128 2023-02-03 03:54:22.787644 arc_cli-8.0.0/arc/core/param/__init__.py
--rw-r--r--   0        0        0     9604 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/core/param/param.py
--rw-r--r--   0        0        0     6062 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/core/param/param_definition.py
--rw-r--r--   0        0        0     3634 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/core/param/param_mixin.py
--rw-r--r--   0        0        0     1801 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/core/param/param_tree.py
--rw-r--r--   0        0        0     6508 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/decorators.py
--rw-r--r--   0        0        0     2003 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/errors.py
--rw-r--r--   0        0        0     1047 2022-08-26 04:11:43.415983 arc_cli-8.0.0/arc/logging.py
--rw-r--r--   0        0        0     7997 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/params.py
--rw-r--r--   0        0        0    15618 2022-10-19 22:11:04.361279 arc_cli-8.0.0/arc/parser.py
--rw-r--r--   0        0        0      255 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/present/__init__.py
--rw-r--r--   0        0        0      916 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/present/ansi.py
--rw-r--r--   0        0        0     4600 2023-02-03 03:54:22.790978 arc_cli-8.0.0/arc/present/box.py
--rw-r--r--   0        0        0      187 2022-12-27 04:39:04.387148 arc_cli-8.0.0/arc/present/data.py
--rw-r--r--   0        0        0     2127 2022-08-26 04:11:43.419317 arc_cli-8.0.0/arc/present/drawing.py
--rw-r--r--   0        0        0     3204 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/present/formatters.py
--rw-r--r--   0        0        0     8755 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/present/help_formatter.py
--rw-r--r--   0        0        0     2685 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/present/helpers.py
--rw-r--r--   0        0        0     3484 2022-12-27 04:39:04.387148 arc_cli-8.0.0/arc/present/loaders.py
--rw-r--r--   0        0        0     9052 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/present/table.py
--rw-r--r--   0        0        0      460 2022-06-09 21:55:30.449063 arc_cli-8.0.0/arc/prompt/__init__.py
--rw-r--r--   0        0        0     4280 2022-11-30 17:38:55.365972 arc_cli-8.0.0/arc/prompt/_select.py
--rw-r--r--   0        0        0     2232 2022-06-09 21:55:30.449063 arc_cli-8.0.0/arc/prompt/helpers.py
--rw-r--r--   0        0        0     5635 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/prompt/prompt.py
--rw-r--r--   0        0        0      767 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/prompt/prompts.py
--rw-r--r--   0        0        0     4749 2022-06-09 21:55:30.449063 arc_cli-8.0.0/arc/prompt/questions.py
--rw-r--r--   0        0        0     3738 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/pub.py
--rw-r--r--   0        0        0        0 2022-07-26 05:16:38.625272 arc_cli-8.0.0/arc/py.typed
--rw-r--r--   0        0        0      373 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/types/__init__.py
--rw-r--r--   0        0        0    12937 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/types/aliases.py
--rw-r--r--   0        0        0      492 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/types/default.py
--rw-r--r--   0        0        0     4153 2023-02-03 03:54:22.794311 arc_cli-8.0.0/arc/types/file.py
--rw-r--r--   0        0        0      747 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/types/helpers.py
--rw-r--r--   0        0        0     1321 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/types/middleware.py
--rw-r--r--   0        0        0     3464 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/types/network.py
--rw-r--r--   0        0        0      854 2022-08-26 04:11:43.422650 arc_cli-8.0.0/arc/types/numbers.py
--rw-r--r--   0        0        0      813 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/types/path.py
--rw-r--r--   0        0        0     6348 2022-08-26 04:11:43.422650 arc_cli-8.0.0/arc/types/semver.py
--rw-r--r--   0        0        0      820 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/types/state.py
--rw-r--r--   0        0        0      458 2022-08-26 04:11:43.422650 arc_cli-8.0.0/arc/types/strings.py
--rw-r--r--   0        0        0     2361 2022-08-26 04:11:43.422650 arc_cli-8.0.0/arc/types/transforms.py
--rw-r--r--   0        0        0     2077 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/types/type_arg.py
--rw-r--r--   0        0        0     2499 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/types/type_info.py
--rw-r--r--   0        0        0     2930 2022-08-26 04:11:43.425983 arc_cli-8.0.0/arc/types/users.py
--rw-r--r--   0        0        0     3399 2023-02-02 07:02:51.269219 arc_cli-8.0.0/arc/types/validators.py
--rw-r--r--   0        0        0     2104 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/typing.py
--rw-r--r--   0        0        0     3626 2023-02-03 03:54:22.797644 arc_cli-8.0.0/arc/utils.py
--rw-r--r--   0        0        0      974 2023-02-03 03:54:53.493996 arc_cli-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 arc_cli-8.0.0/setup.py
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 arc_cli-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0      948 2023-04-03 06:10:36.617549 arc_cli-8.1.0/README.md
+-rw-r--r--   0        0        0      719 2023-04-24 02:17:23.823406 arc_cli-8.1.0/arc/__init__.py
+-rw-r--r--   0        0        0     1449 2023-04-02 19:49:22.490290 arc_cli-8.1.0/arc/api.py
+-rw-r--r--   0        0        0     6902 2023-04-02 19:50:04.610035 arc_cli-8.1.0/arc/autocompletions.py
+-rw-r--r--   0        0        0     2189 2023-04-24 02:12:55.892295 arc_cli-8.1.0/arc/autoload.py
+-rw-r--r--   0        0        0      114 2023-03-18 01:38:52.866444 arc_cli-8.1.0/arc/color.py
+-rw-r--r--   0        0        0     5732 2023-04-02 19:50:49.346437 arc_cli-8.1.0/arc/config.py
+-rw-r--r--   0        0        0      385 2023-04-02 19:50:56.469728 arc_cli-8.1.0/arc/constants.py
+-rw-r--r--   0        0        0      121 2023-03-18 01:38:52.869777 arc_cli-8.1.0/arc/define/__init__.py
+-rw-r--r--   0        0        0     1379 2023-04-02 17:43:44.931222 arc_cli-8.1.0/arc/define/alias.py
+-rw-r--r--   0        0        0     1768 2023-04-02 18:33:44.151939 arc_cli-8.1.0/arc/define/classful.py
+-rw-r--r--   0        0        0    17181 2023-04-05 15:50:39.351207 arc_cli-8.1.0/arc/define/command.py
+-rw-r--r--   0        0        0     3118 2023-04-02 18:42:11.444896 arc_cli-8.1.0/arc/define/documentation.py
+-rw-r--r--   0        0        0      219 2023-03-18 01:38:52.869777 arc_cli-8.1.0/arc/define/param/__init__.py
+-rw-r--r--   0        0        0     8036 2023-04-02 17:56:17.764120 arc_cli-8.1.0/arc/define/param/constructors.py
+-rw-r--r--   0        0        0     3499 2023-04-02 20:00:29.589991 arc_cli-8.1.0/arc/define/param/groups.py
+-rw-r--r--   0        0        0     8706 2023-04-02 18:33:06.022072 arc_cli-8.1.0/arc/define/param/param.py
+-rw-r--r--   0        0        0     8549 2023-04-02 19:59:52.323512 arc_cli-8.1.0/arc/define/param/param_definition.py
+-rw-r--r--   0        0        0     3388 2023-04-02 18:24:36.069969 arc_cli-8.1.0/arc/define/param/param_mixin.py
+-rw-r--r--   0        0        0     1889 2023-04-02 18:14:05.651853 arc_cli-8.1.0/arc/define/param/param_tree.py
+-rw-r--r--   0        0        0     6314 2023-04-02 19:59:32.173614 arc_cli-8.1.0/arc/errors.py
+-rw-r--r--   0        0        0     1070 2023-04-02 19:53:55.292050 arc_cli-8.1.0/arc/logging.py
+-rw-r--r--   0        0        0    16336 2023-04-03 06:34:53.306993 arc_cli-8.1.0/arc/parser.py
+-rw-r--r--   0        0        0      402 2023-04-02 18:55:17.768463 arc_cli-8.1.0/arc/present/__init__.py
+-rw-r--r--   0        0        0     6168 2023-04-02 18:49:02.832312 arc_cli-8.1.0/arc/present/ansi.py
+-rw-r--r--   0        0        0     4681 2023-04-02 18:50:13.529156 arc_cli-8.1.0/arc/present/box.py
+-rw-r--r--   0        0        0     5101 2023-04-02 01:35:30.112194 arc_cli-8.1.0/arc/present/console.py
+-rw-r--r--   0        0        0      187 2023-03-18 01:38:52.873111 arc_cli-8.1.0/arc/present/data.py
+-rw-r--r--   0        0        0     2126 2023-03-18 01:38:52.873111 arc_cli-8.1.0/arc/present/drawing.py
+-rw-r--r--   0        0        0     2748 2023-04-02 18:50:56.742602 arc_cli-8.1.0/arc/present/formatters.py
+-rw-r--r--   0        0        0     9078 2023-04-05 14:25:08.363048 arc_cli-8.1.0/arc/present/help_formatter.py
+-rw-r--r--   0        0        0     3024 2023-04-02 18:54:21.520831 arc_cli-8.1.0/arc/present/joiner.py
+-rw-r--r--   0        0        0       54 2023-04-02 01:35:30.112194 arc_cli-8.1.0/arc/present/markdown/__init__.py
+-rw-r--r--   0        0        0     6473 2023-04-02 01:35:30.112194 arc_cli-8.1.0/arc/present/markdown/markdown_parser.py
+-rw-r--r--   0        0        0     3754 2023-04-02 18:42:43.214931 arc_cli-8.1.0/arc/present/markdown/nodes.py
+-rw-r--r--   0        0        0     1632 2023-04-02 01:35:30.115527 arc_cli-8.1.0/arc/present/out.py
+-rw-r--r--   0        0        0      987 2023-04-02 18:55:42.314170 arc_cli-8.1.0/arc/present/pager.py
+-rw-r--r--   0        0        0     9825 2023-04-02 18:58:32.921906 arc_cli-8.1.0/arc/present/table.py
+-rw-r--r--   0        0        0     5182 2023-04-02 18:58:53.471341 arc_cli-8.1.0/arc/present/wrap.py
+-rw-r--r--   0        0        0      288 2023-03-18 01:38:52.876444 arc_cli-8.1.0/arc/prompt/__init__.py
+-rw-r--r--   0        0        0     3553 2023-04-02 19:01:30.097653 arc_cli-8.1.0/arc/prompt/helpers.py
+-rw-r--r--   0        0        0     5926 2023-04-02 19:10:04.010602 arc_cli-8.1.0/arc/prompt/prompt.py
+-rw-r--r--   0        0        0      812 2023-04-02 19:06:08.453122 arc_cli-8.1.0/arc/prompt/prompts.py
+-rw-r--r--   0        0        0     7019 2023-04-02 19:05:25.083697 arc_cli-8.1.0/arc/prompt/questions.py
+-rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.1.0/arc/py.typed
+-rw-r--r--   0        0        0      306 2023-03-18 01:38:52.879777 arc_cli-8.1.0/arc/runtime/__init__.py
+-rw-r--r--   0        0        0     2970 2023-04-02 19:11:35.999835 arc_cli-8.1.0/arc/runtime/app.py
+-rw-r--r--   0        0        0     2678 2023-04-02 19:12:32.056081 arc_cli-8.1.0/arc/runtime/context.py
+-rw-r--r--   0        0        0    12517 2023-04-05 16:07:36.763616 arc_cli-8.1.0/arc/runtime/exec.py
+-rw-r--r--   0        0        0     8240 2023-04-03 06:32:50.920598 arc_cli-8.1.0/arc/runtime/init.py
+-rw-r--r--   0        0        0     7402 2023-04-10 14:24:59.927180 arc_cli-8.1.0/arc/runtime/middleware.py
+-rw-r--r--   0        0        0      382 2023-04-02 19:57:53.277453 arc_cli-8.1.0/arc/safe.py
+-rw-r--r--   0        0        0     1866 2023-04-02 19:58:09.647368 arc_cli-8.1.0/arc/suggest.py
+-rw-r--r--   0        0        0      335 2023-03-18 01:38:52.883111 arc_cli-8.1.0/arc/types/__init__.py
+-rw-r--r--   0        0        0    13898 2023-04-02 20:01:19.976406 arc_cli-8.1.0/arc/types/aliases.py
+-rw-r--r--   0        0        0      670 2023-04-02 19:44:25.002266 arc_cli-8.1.0/arc/types/convert.py
+-rw-r--r--   0        0        0      545 2023-04-02 19:36:55.892931 arc_cli-8.1.0/arc/types/default.py
+-rw-r--r--   0        0        0     4422 2023-04-02 19:37:41.742437 arc_cli-8.1.0/arc/types/file.py
+-rw-r--r--   0        0        0       79 2023-03-18 01:38:52.883111 arc_cli-8.1.0/arc/types/middleware/__init__.py
+-rw-r--r--   0        0        0     1403 2023-04-02 19:23:23.836123 arc_cli-8.1.0/arc/types/middleware/observers.py
+-rw-r--r--   0        0        0     2630 2023-04-02 19:24:57.642461 arc_cli-8.1.0/arc/types/middleware/transformers.py
+-rw-r--r--   0        0        0     4042 2023-04-02 19:25:31.049016 arc_cli-8.1.0/arc/types/middleware/validators.py
+-rw-r--r--   0        0        0     3486 2023-04-02 19:38:15.415422 arc_cli-8.1.0/arc/types/network.py
+-rw-r--r--   0        0        0      854 2023-03-18 01:38:52.883111 arc_cli-8.1.0/arc/types/numbers.py
+-rw-r--r--   0        0        0      860 2023-04-02 19:38:33.971903 arc_cli-8.1.0/arc/types/path.py
+-rw-r--r--   0        0        0     6881 2023-04-02 19:41:26.780325 arc_cli-8.1.0/arc/types/semver.py
+-rw-r--r--   0        0        0      877 2023-04-02 19:42:04.026684 arc_cli-8.1.0/arc/types/state.py
+-rw-r--r--   0        0        0     1921 2023-04-02 19:42:33.143116 arc_cli-8.1.0/arc/types/strings.py
+-rw-r--r--   0        0        0     2155 2023-04-02 20:00:43.369922 arc_cli-8.1.0/arc/types/type_arg.py
+-rw-r--r--   0        0        0     2718 2023-04-02 20:01:36.192993 arc_cli-8.1.0/arc/types/type_info.py
+-rw-r--r--   0        0        0     3176 2023-04-02 19:47:49.397539 arc_cli-8.1.0/arc/types/users.py
+-rw-r--r--   0        0        0     2257 2023-04-02 19:36:17.910027 arc_cli-8.1.0/arc/typing.py
+-rw-r--r--   0        0        0     1043 2023-04-24 02:17:24.306735 arc_cli-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 arc_cli-8.1.0/setup.py
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 arc_cli-8.1.0/PKG-INFO
```

### Comparing `arc_cli-8.0.0/README.md` & `arc_cli-8.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # ARC: A Regular CLI
-A tool for building declartive, and highly extendable CLI systems for Python 3.9
+A tool for building declarative, and highly extendable CLI systems for Python 3.9
 
 # ARC Features
 - Command line arguments based on python type hints
 - Arbitrary command nesting
 - Automatic `--help` documentation
-- Dynamic command loading at runtime
+- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...
 
 # [Docs](http://arc.seanrcollings.com)
 
 # Quick Start
 
 ```py
 import arc
 
-@arc.command()
+@arc.command
 def hello(name: str):
     """My first arc program!"""
     arc.arc.print(f"Hello {name}!")
 
 hello()
 ```
 
 ```
 $ python hello.py Sean
 Hello, Sean!
 ```
 
 ```
+$ python hello.py --help
 USAGE
     hello.py [-h] [--] name
 
 DESCRIPTION
     My first arc program!
 
 ARGUMENTS
```

### Comparing `arc_cli-8.0.0/arc/autocompletions.py` & `arc_cli-8.1.0/arc/autocompletions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,84 @@
 from __future__ import annotations
-import typing as t
-import os
-import enum
+from contextlib import redirect_stderr
+
 import dataclasses as dc
+import os
+import typing as t
+
 from arc import errors
-from arc.present.helpers import Joiner
+from arc.present.joiner import Join
 
 if t.TYPE_CHECKING:
-    from arc.context import Context
     from arc.typing import CompletionProtocol
-
-
-def completions(shell: str, ctx: Context):
-
-    info = CompletionInfo.from_env()
-    if shell not in shells:
-        raise errors.ArgumentError(
-            f"Unsupported shell: {shell}. Supported shells: {Joiner.with_comma(shells)}"
-        )
-    comp: ShellCompletion = shells[shell](ctx, info)
-    return comp.complete() if comp.should_complete() else comp.source()
+    from arc.define.command import Command
 
 
 def get_completions(
-    obj: CompletionProtocol, info: CompletionInfo, *args, **kwargs
+    obj: CompletionProtocol,
+    info: CompletionInfo,
+    *args: t.Any,
+    **kwargs: t.Any,
 ) -> list[Completion]:
     """Gets the completions for a particular object that supports the `CompletionProtocol`"""
     comps = obj.__completions__(info, *args, **kwargs)
     if comps is None:
         comps = []
-    elif not isinstance(comps, list):
-        comps = [comps]
+    else:
+        comps = list(comps)
     return comps
 
 
 @dc.dataclass
 class CompletionInfo:
     words: list[str]
     current: str
 
-    def empty(self):
+    def empty(self) -> bool:
         return not self.words and not self.current
 
     @classmethod
     def from_env(cls) -> CompletionInfo:
         words = os.getenv("COMP_WORDS", "").split()[1:]
         current = os.getenv("COMP_CURRENT", "")
         return cls(words, current)
 
 
-class CompletionType(enum.Enum):
+class CompletionType:
+    """Constants for common completion types"""
+
     FILE = "file"
     DIR = "dir"
     USERS = "users"
     GROUPS = "groups"
     PLAIN = "plain"
 
 
 @dc.dataclass
 class Completion:
     value: t.Any
-    type: CompletionType = CompletionType.PLAIN
     description: t.Optional[str] = None
-    data: dict = dc.field(default_factory=dict)
+    type: str = CompletionType.PLAIN
+    data: dict[str, t.Any] = dc.field(default_factory=dict)
 
 
 class ShellCompletion:
     template: t.ClassVar[str]
-    name: t.ClassVar[str]
+    shells: dict[str, type["ShellCompletion"]] = {}
 
-    def __init__(self, ctx: Context, info: CompletionInfo):
-        self.ctx = ctx
-        self.command = ctx.command
+    def __init__(self, command: Command, info: CompletionInfo):
+        self.command = command
         self.info = info
         self.command_name = self.command.name
 
+    def __init_subclass__(cls, name: str) -> None:
+        ShellCompletion.shells[name] = cls
+
     @property
-    def completion_vars(self) -> dict:
+    def completion_vars(self) -> dict[str, t.Any]:
         return {
             "name_exe": "python cli.py"
             if os.getenv("ARC_DEVELOPMENT")
             else self.command_name,
             "name_com": self.command_name,
             "func_name": f"_{self.command_name}_completions".replace("-", "_"),
             "completion_var": self.completion_var,
@@ -100,23 +98,42 @@
     def complete(self) -> str:
         """Actually provides the completions"""
         return ""
 
     def format_completion(self, comp: Completion) -> str:
         return ""
 
+    @classmethod
+    def run(cls, shell: str, command: Command) -> str:
+        info = CompletionInfo.from_env()
+        if shell not in cls.shells:
+            raise errors.ArgumentError(
+                f"Unsupported shell: {shell}. "
+                f"Supported shells: {Join.with_comma(cls.shells)}"
+            )
+        comp: ShellCompletion = cls.shells[shell](command, info)
+
+        with open("completions.log", "w+") as f, redirect_stderr(f):
+            res = comp.complete() if comp.should_complete() else comp.source()
+            f.write("\n")
+            f.write(" ".join(info.words))
+            f.write("\n")
+            f.write(res)
+            f.write("\n\n")
+
+        return res
+
 
-class BashCompletion(ShellCompletion):
-    name = "bash"
+class BashCompletion(ShellCompletion, name="bash"):
     template = """\
 {func_name}() {{
     local completions;
 
     completions=$(env {completion_var}=true COMP_WORDS="${{COMP_WORDS[*]}}" \
-        COMP_CURRENT="${{COMP_WORDS[COMP_CWORD]}}" {name} --autocomplete bash)
+        COMP_CURRENT="${{COMP_WORDS[COMP_CWORD]}}" {name_exe} --autocomplete bash)
 
     while IFS= read -r comp; do
         IFS="|" read -r type value <<< "$comp"
 
         if [[ $type == "file" ]]; then
             compopt -o default
         elif [[ $type == "dir" ]]; then
@@ -126,36 +143,35 @@
         fi
 
     done <<< "$completions"
 
     return 0
 }}
 
-complete -o nosort -F {func_name} {name}
+complete -o nosort -F {func_name} {name_exe}
 """
 
     def complete(self) -> str:
         comps = get_completions(self.command, self.info)
         return "\n".join([self.format_completion(comp) for comp in comps])
 
     def format_completion(self, comp: Completion) -> str:
-        return f"{comp.type.value}|{comp.value}"
+        return f"{comp.type}|{comp.value}"
 
 
-class ZshCompletion(BashCompletion):
-    name = "zsh"
+class ZshCompletion(BashCompletion, name="zsh"):
     template = """\
-#compdef {name}
+#compdef {name_exe}
 
 {func_name}() {{
     local -a completions;
     local -a array;
 
     completions=("${{(@f)$(env {completion_var}=true COMP_WORDS="${{words[*]}}" \
-        COMP_CURRENT=${{words[$CURRENT]}} {name} --autocomplete zsh)}}")
+        COMP_CURRENT=${{words[$CURRENT]}} {name_exe} --autocomplete zsh)}}")
 
     for comp in $completions; do
         parsed=(${{(@s/|/)comp}})
         type=${{parsed[1]}}
         value=${{parsed[2]}}
 
         if [[ "$type" == "dir" ]]; then
@@ -172,31 +188,30 @@
     done
 
     if [ -n "$array" ]; then
         compadd -U -V unsorted -a array
     fi
 }}
 
-compdef {func_name} {name};
+compdef {func_name} {name_exe};
 """
 
     def complete(self) -> str:
         comps = get_completions(self.command, self.info)
         return "\n".join([self.format_completion(comp) for comp in comps])
 
     def format_completion(self, comp: Completion) -> str:
-        string = f"{comp.type.value}|{comp.value}"
+        string = f"{comp.type}|{comp.value}"
         # if comp.description:
         #     string += f"[{comp.description}]"
 
         return string
 
 
-class FishCompletion(ShellCompletion):
-    name = "fish"
+class FishCompletion(ShellCompletion, name="fish"):
     template = """\
 function {func_name}
     set -l completions (env {completion_var}=true COMP_WORDS=(commandline -cp) \
         COMP_CURRENT=(commandline -t) {name_exe} --autocomplete fish)
 
     for comp in $completions
         set -l parsed (string split '|' $comp)
@@ -226,15 +241,12 @@
 """
 
     def complete(self) -> str:
         comps = get_completions(self.command, self.info)
         return "\n".join([self.format_completion(comp) for comp in comps])
 
     def format_completion(self, comp: Completion) -> str:
-        string = f"{comp.type.value}|{comp.value}"
+        string = f"{comp.type}|{comp.value}"
         if comp.description:
             string += f"\t{comp.description}"
 
         return string
-
-
-shells = {"bash": BashCompletion, "fish": FishCompletion, "zsh": ZshCompletion}
```

### Comparing `arc_cli-8.0.0/arc/autoload.py` & `arc_cli-8.1.0/arc/autoload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
+
+import sys
 import typing as t
 from importlib import import_module
 from pathlib import Path
-import sys
 
 from arc.errors import CommandError
 
 if t.TYPE_CHECKING:
-    from arc.core import Command
+    from arc.define import Command
 
 
 class Autoload:
+    """Autoloads commands from files and adds them to the parent command"""
+
     def __init__(
         self, paths: t.Iterable[str], parent: Command, allow_overrite: bool = False
     ) -> None:
         self.paths = paths
         self.parent = parent
         self.allow_overwrite = allow_overrite
 
@@ -22,18 +25,17 @@
         for path in self.__load_files(self.paths):
             for command in self.__load_commands(path):
                 if command.name in self.parent.subcommands and not self.allow_overwrite:
                     raise CommandError(
                         f"Command {command.name} already exists on {self.parent}\n"
                         "Autoloaded command cannot overwrite prexisting commands"
                     )
-
                 self.parent.add_command(command)
 
-    def __load_files(self, paths: t.Iterable[str]):
+    def __load_files(self, paths: t.Iterable[str]) -> t.Iterator[Path]:
         for filepath in paths:
             path = self.path(filepath)
             if not path:
                 continue
 
             if path.name.startswith("__"):
                 continue
@@ -50,15 +52,15 @@
             getattr(module, name) for name in dir(module) if not name.startswith("__")
         )
         for obj in module_objects:
             if isinstance(obj, type):
                 continue
 
             try:
-                if obj.__autoload__:
+                if obj._autoload:
                     yield obj
             except AttributeError:
                 continue
 
     @staticmethod
     def path(filepath: str) -> t.Optional[Path]:
         path = Path(filepath)
```

### Comparing `arc_cli-8.0.0/arc/context.py` & `arc_cli-8.1.0/arc/runtime/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,100 @@
 from __future__ import annotations
+
+import collections
 import typing as t
 
 import arc.typing as at
 
 if t.TYPE_CHECKING:
-    from arc.core.param.param import ValueOrigin
-    from arc.core.command import Command
-    from arc.core.app import App
     from logging import Logger
+
     from arc.config import Config
+    from arc.define.command import Command
+    from arc.define.param.param import ValueOrigin
+    from arc.prompt.prompt import Prompt
+    from arc.runtime import App
 
 
 T = t.TypeVar("T")
 
 
-class Context:
-    """Context serves as a "view" into the execution enviroment"""
+class Context(collections.UserDict[str, t.Any]):
+    """Context is a dict-like object that serves as
+    the shared execution state for all `arc` component
+    """
 
-    def __init__(self, env: at.ExecEnv) -> None:
-        self.env: at.ExecEnv = env
+    @property
+    def root(self) -> Command:
+        """The root command object. Alias for `ctx["arc.root"]`"""
+        return self["arc.root"]
 
     @property
     def command(self) -> Command:
-        return self.env["arc.command"]
+        """The command object being executed. Alias for `ctx["arc.command"]`"""
+        return self["arc.command"]
 
     @property
-    def state(self) -> dict:
-        return self.env["arc.state"]
+    def state(self) -> dict[str, t.Any]:
+        """The state object passed in. Alias for `ctx["arc.state"]`"""
+        return self["arc.state"]
 
     @property
     def logger(self) -> Logger:
-        return self.env["arc.logger"]
+        """The arc logger. Alias for `ctx["arc.logger"]`"""
+        return self["arc.logger"]
 
     @property
     def app(self) -> App:
-        return self.env["arc.app"]
+        """The arc app. Alias for `ctx["arc.app"]`"""
+        return self["arc.app"]
 
     @property
     def config(self) -> Config:
-        return self.env["arc.config"]
+        """The configuration for this app. Alias for `ctx["arc.config"]`"""
+        return self["arc.config"]
+
+    @property
+    def prompt(self) -> Prompt:
+        """The prompt object congigured. Alias for `ctx["arc.config"].prompt`"""
+        return self.config.prompt
+
+    def execute(self, command: Command, **kwargs: t.Any) -> t.Any:
+        """Execute a command within the context of another command
+        ```py
+        import arc
+
+        @arc.command
+        def command(ctx: arc.Context):
+            ctx.execute(sub, val=2)
+
+        @command.subcommand
+        def sub(val: int):
+            print(sub)
+        ```
 
-    def execute(self, command: Command, **kwargs) -> t.Any:
-        """Execute a command within the context of another command"""
+        """
         return self.app.execute(command, **kwargs)
 
     @t.overload
     def get_origin(self, param_name: str) -> ValueOrigin | None:
         ...
 
     @t.overload
     def get_origin(self, param_name: str, default: T) -> ValueOrigin | T:
         ...
 
-    def get_origin(self, param_name: str, default=None):
+    def get_origin(
+        self, param_name: str, default: T | None = None
+    ) -> ValueOrigin | T | None:
         """Gets the origin of a paramter"""
-        origins: dict[str, ValueOrigin] | None = self.env.get("arc.args.origins")
+        origins: dict[str, ValueOrigin] | None = self.get("arc.args.origins")
 
         if not origins:
             return default
 
         return origins.get(param_name, default)
 
     @classmethod
-    def __depends__(cls, ctx: Context):
+    def __depends__(cls, ctx: Context) -> Context:
+        """Makes the context a dependency"""
         return ctx
```

### Comparing `arc_cli-8.0.0/arc/core/param/param.py` & `arc_cli-8.1.0/arc/define/param/param.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from __future__ import annotations
+
 import argparse
 import enum
-from functools import cached_property
-import os
 import typing as t
+from functools import cached_property
 
-from arc import errors, utils
-from arc import constants
+import arc.typing as at
+from arc import api, constants, errors, safe
 from arc.autocompletions import CompletionInfo, get_completions
-from arc.color import colorize, effects, fg
-from arc.types.helpers import convert_type
+from arc.color import colorize, fg
+from arc.constants import MISSING, Constant
+from arc.types.convert import convert_type
 from arc.types.type_info import TypeInfo
-import arc.typing as at
-from arc.constants import MISSING, MissingType
-
-if t.TYPE_CHECKING:
-    from arc.context import Context
-
 
 T = t.TypeVar("T")
 
 
 class Action(enum.Enum):
     STORE = "store"
     STORE_TRUE = "store_true"
@@ -43,15 +38,15 @@
     """The cannonical name of the function's argument"""
     param_name: str
     """The names used on the command line / for parsing"""
     short_name: str | None
     """Optional single-character name alternabive for keyword params"""
     type: TypeInfo[T]
     """Information on the type of the argument"""
-    default: T | MissingType | None
+    default: T | Constant | None
     """Default value for this Param, will be used if no
     other source provides a value. A value `MISSING` indicates
     that the parameter is required. Otherwise, the parameter is optional"""
     description: str | None
     """Documentation for this parameter. If none is provided explicitly,
     it may also originate from the command's docstring"""
     envvar: str | None
@@ -65,219 +60,199 @@
     expose: bool
     """If a param is 'exposed' it will be passed to the command's callback.
     If it's not 'exposed' then it will not be passed to the command's callback.
     This is useful when the parameter's side effects are desired, but the value
     doesn't matter. This is used to implment the `--version` and `--help` flags"""
     comp_func: at.CompletionFunc | None
     """Function that can provide shell completions for the parameter"""
-    getter_func: at.GetterFunc | None
+    getter_func: at.ParamGetter | None
     """Function that can retrieve a value not provided on the command line"""
+    data: dict[str, t.Any]
+    """Dictionary of any other key values passed to the constructors"""
 
     def __init__(
         self,
         argument_name: str,
-        annotation: at.Annotation,
-        default: T | None | MissingType = MISSING,
+        type: TypeInfo[T],
+        default: T | None | Constant = MISSING,
         param_name: str | None = None,
         short_name: str | None = None,
         description: str | None = None,
-        callback: t.Callable | None = None,
+        callback: at.ParamCallback | None = None,
         envvar: str | None = None,
         prompt: str | None = None,
         action: Action | t.Type[argparse.Action] | None = None,
         expose: bool = True,
         comp_func: at.CompletionFunc | None = None,
-        getter_func: at.GetterFunc | None = None,
+        getter_func: at.ParamGetter | None = None,
+        data: dict[str, t.Any] = None,
     ):
         self.argument_name = argument_name
         self.param_name = param_name or argument_name
+        self.type = type
         self.short_name = short_name
         self.default = default
         self.description = description
         self.callback = callback
         self.envvar = envvar
         self.prompt = prompt
         self.action = action or Action.STORE
-        self.type = TypeInfo.analyze(annotation)
         self.expose = expose
         self.comp_func = comp_func
         self.getter_func = getter_func
-
-        if self.type.is_union_type:
-            for sub in self.type.sub_types:
-                if utils.safe_issubclass(sub.origin, (set, tuple, list)):
-                    raise errors.ParamError(
-                        f"{self.type.original_type} is not a valid type. "
-                        f"lists, sets, and tuples cannot be members of a Union / Optional type"
-                    )
+        self.data = data or {}
 
         if self.type.is_optional_type and self.default is MISSING:
             self.default = None
 
-        if self.short_name and len(self.short_name) > 1:
-            raise errors.ParamError(
-                f"Parameter {self.param_name}'s shortened name is longer than 1 character",
-                self,
-            )
-
-    __repr__ = utils.display("argument_name", "type")
+    __repr__ = api.display("argument_name", "type")
 
-    def __completions__(self, info: CompletionInfo, *args, **kwargs):
+    def __completions__(
+        self, info: CompletionInfo, *args: t.Any, **kwargs: t.Any
+    ) -> at.CompletionReturn:
         if self.comp_func:
             return self.comp_func(info, self)
 
         if hasattr(self.type.resolved_type, "__completions__"):
             return get_completions(self.type.resolved_type, info, self)  # type: ignore
 
+        return None
+
     @property
-    def schema(self):
+    def schema(self) -> dict[str, t.Any]:
         return {
             "argument_name": self.argument_name,
             "type": self.type,
             "param_name": self.param_name,
             "short_name": self.short_name,
             "default": self.default,
         }
 
     @property
-    def is_argument(self):
+    def is_argument(self) -> bool:
         return False
 
     @property
-    def is_keyword(self):
+    def is_keyword(self) -> bool:
         return False
 
     @property
-    def is_option(self):
+    def is_option(self) -> bool:
         return False
 
     @property
-    def is_flag(self):
+    def is_flag(self) -> bool:
         return False
 
     @property
-    def is_injected(self):
+    def is_injected(self) -> bool:
         return False
 
     @property
-    def is_optional(self):
+    def is_optional(self) -> bool:
         return self.type.is_optional_type or self.default is not MISSING
 
     @property
-    def is_required(self):
+    def is_required(self) -> bool:
         return not self.is_optional
 
     @property
-    def prompt_string(self):
+    def prompt_string(self) -> str:
+        assert isinstance(self.prompt, str), "No prompt string provided"
+
         if self.default is not MISSING:
-            return self.prompt + colorize(f" ({self.default})", fg.GREY)
+            return self.prompt + colorize(f" ({self.default}) ", fg.GREY)
         return self.prompt
 
     @property
-    def cli_name(self):
+    def cli_name(self) -> str:
         return self.param_name
 
     @property
-    def parser_default(self):
+    def parser_default(self) -> t.Any:
         return MISSING
 
     @cached_property
     def nargs(self) -> at.NArgs:
         if (
-            utils.safe_issubclass(self.type.origin, tuple)
+            safe.issubclass(self.type.origin, tuple)
             and self.type.sub_types
             and self.type.sub_types[-1].origin is not Ellipsis
         ):
             return len(self.type.sub_types)  # Consume a specific number
-        elif utils.safe_issubclass(self.type.origin, constants.COLLECTION_TYPES):
+        elif self.type.is_collection_type:
             return "*"  # Consume one or more
 
         return "?"  # Optional
 
     def convert(self, value: t.Any) -> T:
-        try:
-            return convert_type(self.type.resolved_type, value, self.type)
-        except errors.ConversionError as e:
-            message = self._fmt_error(e)
-            if e.details:
-                message += colorize(f" ({e.details})", fg.GREY)
-            raise errors.InvalidArgValue(message) from e
+        return convert_type(self.type.resolved_type, value, self.type)
 
-    def run_middleware(self, value: t.Any, ctx: t.Any):
+    def run_middleware(self, value: t.Any, ctx: t.Any) -> t.Any:
         for middleware in self.type.middleware:
-            try:
-                value = utils.dispatch_args(middleware, value, ctx, self)
-            except errors.ValidationError as e:
-                message = self._fmt_error(e)
-                raise errors.InvalidArgValue(message) from e
+            value = api.dispatch_args(middleware, value, ctx, self)
 
         return value
 
     def get_param_names(self) -> list[str]:
         return []
 
-    def _fmt_error(self, error: errors.ArcError):
-        return (
-            f"invalid value for {colorize(self.cli_name, fg.YELLOW)}: "
-            f"{colorize(str(error), effects.BOLD)}"
-        )
-
 
-class ArgumentParam(Param[t.Any]):
+class ArgumentParam(Param[T]):
     @property
-    def is_argument(self):
+    def is_argument(self) -> bool:
         return True
 
     # @property
     # def nargs(self):
-    #     if utils.safe_issubclass(self.type.origin, (tuple, list, set)):
+    #     if safe.issubclass(self.type.origin, (tuple, list, set)):
     #         return "*"  # Consume one or more
 
     #     return "?"  # Optional
 
     def get_param_names(self) -> list[str]:
         return [self.argument_name]
 
 
 class KeywordParam(Param[T]):
     @property
-    def is_keyword(self):
+    def is_keyword(self) -> bool:
         return True
 
     @property
-    def cli_name(self):
+    def cli_name(self) -> str:
         return f"--{self.param_name}"
 
     def get_param_names(self) -> list[str]:
         if self.short_name:
             return [f"-{self.short_name}", f"--{self.param_name}"]
 
         return [f"--{self.param_name}"]
 
 
-class OptionParam(KeywordParam[t.Any]):
-    def __init__(self, *args, **kwargs):
+class OptionParam(KeywordParam[T]):
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         super().__init__(*args, **kwargs)
 
-        if self.type.origin in constants.COLLECTION_TYPES:
+        if self.type.is_collection_type:
             self.action = Action.APPEND
 
     @property
-    def is_option(self):
+    def is_option(self) -> bool:
         return True
 
     @property
-    def parser_default(self):
+    def parser_default(self) -> t.Any:
         if self.action is Action.APPEND:
             return None
         return MISSING
 
 
 class FlagParam(KeywordParam[bool]):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         super().__init__(*args, **kwargs)
 
         # A default of false is always assumed with flags, so they
         # are always optional
         if self.default is MISSING:
             self.default = False
 
@@ -286,32 +261,32 @@
         if self.action == Action.STORE:
             if self.default is True:
                 self.action = Action.STORE_FALSE
             elif self.default is False:
                 self.action = Action.STORE_TRUE
 
     @property
-    def is_flag(self):
+    def is_flag(self) -> bool:
         return True
 
     @property
-    def parser_default(self):
+    def parser_default(self) -> t.Any:
         if self.action is Action.COUNT:
             return 0
         return MISSING
 
 
-class InjectedParam(Param):
+class InjectedParam(Param[T]):
     """Injected Params are params whose values do
     not come from the command line, but from a dependancy injection.
     Used to get access to things like the arc Context and State
     """
 
-    callback: t.Callable
+    callback: at.ParamGetter  # type: ignore[assignment]
 
     def get_injected_value(self, ctx: t.Any) -> t.Any:
-        value = utils.dispatch_args(self.callback, ctx) if self.callback else None
+        value = api.dispatch_args(self.callback, ctx, self)
         return value
 
     @property
-    def is_injected(self):
+    def is_injected(self) -> bool:
         return True
```

### Comparing `arc_cli-8.0.0/arc/core/param/param_definition.py` & `arc_cli-8.1.0/arc/define/param/param_definition.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,236 @@
 from __future__ import annotations
-import typing as t
+
 import collections
 import inspect
+import typing as t
 
-from arc import errors, utils
-from arc.config import config
+from arc import api, errors, safe
+from arc import typing as at
 from arc.constants import MISSING
-from arc.core.param.param_tree import ParamTree, ParamValue
-from arc.types.type_info import TypeInfo
-from arc.params import ParamInfo
-from arc.core.param.param import (
-    InjectedParam,
-    Param,
-    FlagParam,
+from arc.define import classful
+from arc.define.param import groups
+from arc.define.param.constructors import ParamInfo
+from arc.define.param.param import (
     ArgumentParam,
+    FlagParam,
+    InjectedParam,
     OptionParam,
+    Param,
 )
+from arc.define.param.param_tree import ParamTree, ParamValue
+from arc.types.type_info import TypeInfo
 
 
-class ParamDefinition(collections.UserList[Param]):
+class ParamDefinition(collections.deque[Param[t.Any]]):
     """A tree structure that represents how the parameters to a command look.
     This represents the definition of a command's paramaters, and not a particular
     execution of that comamnd with particular values"""
 
     BASE = "__arc_param_group_base"
     """A group with name `BASE` is the base group and
     gets spread into the function arguments"""
 
-    def __init__(self, name: str, cls: type | None = None, *args, **kwargs):
+    def __init__(
+        self,
+        name: str,
+        cls: type | None = None,
+        *args: t.Any,
+        **kwargs: t.Any,
+    ) -> None:
         super().__init__(*args, **kwargs)
         self.name: str = name
         self.cls: type | None = cls
         self.children: list[ParamDefinition] = []
 
-    __repr__ = utils.display("name", "data", "children")
+    __repr__ = api.display("name", "data", "children")
 
     @property
     def is_base(self) -> bool:
         return self.name == self.BASE
 
-    def all_params(self) -> t.Generator[Param, None, None]:
+    def all_params(self) -> t.Generator[Param[t.Any], None, None]:
         """Generator that yields all params in the tree"""
-        yield from self.data
+        yield from self
 
         if self.children:
             for child in self.children:
                 yield from child.all_params()
 
-    def create_instance(self) -> ParamTree:
+    def create_instance(self) -> ParamTree[type[dict[str, t.Any]]]:
         return self.__create_param_instance(self)
 
-    def __create_param_instance(self, definition: ParamDefinition) -> ParamTree:
-        values: dict[str, ParamTree | ParamValue] = {
-            param.argument_name: ParamValue(MISSING, param)
-            for param in definition
-            # if param.expose
+    def __create_param_instance(self, definition: ParamDefinition) -> ParamTree[t.Any]:
+        values: dict[str, ParamTree[t.Any] | ParamValue] = {
+            param.argument_name: ParamValue(MISSING, param) for param in definition
         }
 
         for child in definition.children:
             values[child.name] = self.__create_param_instance(child)
 
         return ParamTree(
             values,
             definition.cls or dict,
         )
 
-    @classmethod
-    def from_function(cls, func: t.Callable) -> ParamDefinition:
-        """Constructs a ParamDefinition from a callable signature"""
-        builder = ParamDefinitionBuilder()
-        root = builder.build(func)
-        return root
-
 
-class ParamDefinitionBuilder:
-    def __init__(self):
+class ParamDefinitionFactory:
+    def __init__(
+        self,
+        get_command_name: t.Callable[..., str],
+        transform_snake_case: bool = True,
+    ):
         self.param_names: set[str] = set()
+        self.get_command_name = get_command_name
+        self.transform_snake_case = transform_snake_case
 
-    def build(self, obj: t.Callable | type) -> ParamDefinition:
-        sig = inspect.signature(obj)
-        annotations = t.get_type_hints(obj, include_extras=True)
+    def from_function(self, func: t.Callable[..., t.Any]) -> ParamDefinition:
+        self.param_names.clear()
+        sig = self._get_sig(func)
+        return self.build(sig)
+
+    def from_class(self, cls: type) -> ParamDefinition:
+        self.param_names.clear()
+        sig = classful.class_signature(cls)
+        return self.build(sig)
+
+    def _from_param_group(self, cls: type, name: str) -> ParamDefinition:
+        definition = groups.get_cached_definition(cls)
+
+        if not definition:
+            options = t.cast(at.ParamGroupOptions, groups.groupoptions(cls))
+            sig = classful.class_signature(cls)
+            definition = self.build(sig, exclude=options["exclude"])
+            definition.name = name
+            definition.cls = cls
+            groups.cache_definition(cls, definition)
 
-        for param in sig.parameters.values():
-            param._annotation = annotations.get(param.name, param.annotation)  # type: ignore
+        return definition
 
+    def build(
+        self, sig: inspect.Signature, exclude: t.Sequence[str] | None = None
+    ) -> ParamDefinition:
+        exclude = exclude or []
         root = ParamDefinition(ParamDefinition.BASE)
 
-        for param in sig.parameters.values():
-            if utils.isgroup(param.annotation):
-                root.children.append(self.build_param_definition(param))
+        iterable = (
+            param for param in sig.parameters.values() if param.name not in exclude
+        )
+        for param in iterable:
+            if groups.isgroup(param.annotation):
+                if param.default is not param.empty:
+                    raise errors.ParamError(
+                        "Parameter groups cannot have a default value",
+                        self.get_command_name(),
+                        param,
+                    )
+                definition = self._from_param_group(param.annotation, param.name)
+                root.children.append(definition)
             else:
-                root.append(self.create_param(param))
+                command_param = self.create_param(param)
 
-        return root
+                if command_param.short_name:
+                    if len(command_param.short_name) > 1:
+                        raise errors.ParamError(
+                            f"Parameter {command_param.param_name}'s shortened name is longer than 1 character",
+                            self.get_command_name(),
+                            command_param,
+                        )
+
+                    if command_param.short_name in self.param_names:
+                        raise errors.ParamError(
+                            f"Parameter {command_param.param_name} shortened name "
+                            f"{command_param.short_name!r} is non-unique.",
+                            self.get_command_name(),
+                        )
+
+                if command_param.type.is_union_type:
+                    for sub in command_param.type.sub_types:
+                        if safe.issubclass(sub.origin, (set, tuple, list)):
+                            raise errors.ParamError(
+                                f"{command_param.type.original_type} is not a valid type. "
+                                f"lists, sets, and tuples cannot be members of a Union / Optional type",
+                                self.get_command_name(),
+                            )
 
-    def build_param_definition(self, param: inspect.Parameter) -> ParamDefinition:
-        if param.default is not param.empty:
-            raise errors.ParamError(
-                "Parameter groups cannot have a default value", param
-            )
+                root.append(command_param)
 
-        cls = param.annotation
-        if hasattr(cls, "__param_group__"):
-            return getattr(cls, "__param_group__")
-
-        definition = self.build(cls)
-        definition.name = param.name
-        definition.cls = param.annotation
-        setattr(cls, "__param_group__", definition)
-        return definition
+        return root
 
-    def create_param(self, param: inspect.Parameter) -> Param:
+    def create_param(self, param: inspect.Parameter) -> Param[t.Any]:
         if param.name in self.param_names:
             raise errors.ParamError(
                 f"Parameter name '{param.name}' is non-unique. "
-                "All parameters for a given command must have a unique name"
+                "All parameters for a given command must have a unique name",
+                self.get_command_name(),
             )
 
         self.param_names.add(param.name)
-        # TODO: pass this type_info into the param, instead of creating it twice
-        type_info = TypeInfo.analyze(param.annotation)
+        annotation = t.Any if param.annotation is param.empty else param.annotation
+        type_info = TypeInfo[t.Any].analyze(annotation)
         info = self.get_param_info(param, type_info)
 
         annotation = param.annotation
         if annotation is param.empty:
             annotation = bool if info.param_cls is FlagParam else str
 
-        if config.transform_snake_case and not info.param_name:
+        if self.transform_snake_case and not info.param_name:
             info.param_name = param.name.replace("_", "-")
 
         return info.param_cls(
             argument_name=param.name,
-            annotation=annotation,
+            type=type_info,
             **info.dict(),
         )
 
     def get_param_info(
-        self, param: inspect.Parameter, type_info: TypeInfo
+        self, param: inspect.Parameter, type_info: TypeInfo[t.Any]
     ) -> ParamInfo:
         if isinstance(param.default, ParamInfo):
             info = param.default
         else:
             info = ParamInfo(
                 param_cls=self.get_param_cls(param, type_info),
                 default=param.default if param.default is not param.empty else MISSING,
             )
 
         if hasattr(type_info.origin, "__depends__"):
             if param.default is not param.empty:
                 raise errors.ParamError(
                     f"type {param.annotation} is a special type used for dependancy injection. "
-                    "As such, it cannot be provided with a default value or parameter value"
+                    "As such, it cannot be provided with a default value or parameter value",
+                    self.get_command_name(),
                 )
             info.callback = type_info.origin.__depends__
 
         return info
 
     def get_param_cls(
-        self, param: inspect.Parameter, type_info: TypeInfo
-    ) -> type[Param]:
+        self, param: inspect.Parameter, type_info: TypeInfo[t.Any]
+    ) -> type[Param[t.Any]]:
         origin = type_info.origin
 
         if param.kind is param.POSITIONAL_ONLY:
             raise errors.ParamError(
                 "Positional only arguments are not allowed. "
                 "please remove the '/' from your function definition",
+                self.get_command_name(),
                 param,
             )
 
         if hasattr(origin, "__depends__"):
             return InjectedParam
         elif origin is bool or isinstance(param.default, bool):
             return FlagParam
         elif param.kind is param.KEYWORD_ONLY:
             return OptionParam
         else:
             return ArgumentParam
+
+    def _get_sig(self, obj: t.Callable[..., t.Any] | type) -> inspect.Signature:
+        sig = inspect.signature(obj)
+        annotations = t.get_type_hints(obj, include_extras=True)
+
+        for param in sig.parameters.values():
+            param._annotation = annotations.get(param.name, param.annotation)  # type: ignore
+
+        return sig
```

### Comparing `arc_cli-8.0.0/arc/core/param/param_mixin.py` & `arc_cli-8.1.0/arc/define/param/param_mixin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,121 +1,111 @@
 from __future__ import annotations
+
 import typing as t
 from functools import cached_property
-from arc import autocompletions
-
-from arc.config import config
-from arc.parser import CustomAutocompleteAction, CustomHelpAction, CustomVersionAction
 
-from .param import FlagParam, OptionParam, Param
-from .param_definition import ParamDefinition, ParamDefinitionBuilder
+import arc.typing as at
+from arc.define.alias import AliasDict
+from arc.parser import CustomHelpAction
+from arc.present.joiner import Join
+from arc.types.type_info import TypeInfo
+
+from .param_definition import ParamDefinition, ParamDefinitionFactory
+from .param import (
+    FlagParam,
+    Param,
+    KeywordParam,
+    OptionParam,
+    ArgumentParam,
+    InjectedParam,
+)
+
+if t.TYPE_CHECKING:
+    from arc.config import Config
+    from arc.define import Command
 
 
 class ParamMixin:
     SPECIAL_PARAMS = {"help", "version", "autocomplete"}
-    callback: t.Callable
+    callback: at.CommandCallback
     parent: t.Any
+    config: Config
 
     @cached_property
     def param_def(self) -> ParamDefinition:
-        root = ParamDefinition.from_function(self.callback)
-
-        if self.is_root and not self.is_namespace:  # type: ignore
-
-            if config.version:
-                self.__add_version_param(root)
-
-            if config.autocomplete:
-                self.__add_autocomplete_param(root)
+        root = ParamDefinitionFactory(
+            lambda: Join.with_space(t.cast("Command", self).doc.fullname),
+            self.config.transform_snake_case,
+        ).from_function(self.callback)
 
         self.__add_help_param(root)
 
         return root
 
+    @cached_property
+    def param_map(self) -> t.Mapping[str, Param[t.Any]]:
+        data: AliasDict[str, Param[t.Any]] = AliasDict()
+        for param in self.params:
+            data[param.argument_name] = param
+            data.add_alias(param.argument_name, param.param_name)
+            if param.short_name:
+                data.add_alias(param.argument_name, param.short_name)
+            data.add_aliases(param.argument_name, *param.get_param_names())
+
+        return data
+
     @property
-    def params(self) -> t.Generator[Param, None, None]:
+    def params(self) -> t.Generator[Param[t.Any], None, None]:
         yield from self.param_def.all_params()
 
     @property
-    def cli_params(self) -> t.Generator[Param, None, None]:
+    def cli_params(self) -> t.Generator[Param[t.Any], None, None]:
         """All params that are available on the command line"""
         for param in self.params:
             if not param.is_injected:
                 yield param
 
     @property
-    def argument_params(self) -> t.Generator[Param, None, None]:
+    def argument_params(self) -> t.Generator[ArgumentParam[t.Any], None, None]:
         for param in self.params:
             if param.is_argument:
-                yield param
+                yield param  # type: ignore
 
     @property
-    def key_params(self) -> t.Generator[Param, None, None]:
+    def key_params(self) -> t.Generator[KeywordParam[t.Any], None, None]:
         for param in self.params:
             if param.is_keyword:
-                yield param
+                yield param  # type: ignore
 
     @property
-    def option_params(self) -> t.Generator[Param, None, None]:
+    def option_params(self) -> t.Generator[OptionParam[t.Any], None, None]:
         for param in self.params:
             if param.is_option:
-                yield param
+                yield param  # type: ignore
 
     @property
-    def flag_params(self) -> t.Generator[Param, None, None]:
+    def flag_params(self) -> t.Generator[FlagParam, None, None]:
         for param in self.params:
             if param.is_flag:
-                yield param
+                yield param  # type: ignore
 
     @property
-    def injected_params(self) -> t.Generator[Param, None, None]:
+    def injected_params(self) -> t.Generator[InjectedParam[t.Any], None, None]:
         for param in self.params:
             if param.is_injected:
-                yield param
-
-    def get_param(self, name: str) -> t.Optional[Param]:
-        for param in self.params:
-            if name in (param.argument_name, param.param_name, param.short_name):
-                return param
+                yield param  # type: ignore
 
-        return None
+    def get_param(self, name: str) -> t.Optional[Param[t.Any]]:
+        return self.param_map.get(name)
 
-    def __add_version_param(self, group: ParamDefinition):
-        group.append(
-            FlagParam(
-                "version",
-                short_name="v",
-                annotation=bool,
-                description="Displays the app's version number",
-                default=False,
-                action=CustomVersionAction,
-                expose=False,
-            ),
-        )
-
-    def __add_help_param(self, group: ParamDefinition):
-        group.insert(
-            0,
+    def __add_help_param(self, group: ParamDefinition) -> None:
+        group.appendleft(
             FlagParam(
                 "help",
                 short_name="h",
-                annotation=bool,
+                type=TypeInfo.analyze(bool),
                 description="Displays this help message",
                 default=False,
                 action=CustomHelpAction,
                 expose=False,
             ),
         )
-
-    def __add_autocomplete_param(self, group: ParamDefinition):
-        annotation = t.Literal[1]
-        annotation.__args__ = tuple(autocompletions.shells.keys())  # type: ignore
-        group.append(
-            OptionParam(
-                "autocomplete",
-                annotation=annotation,  # type: ignore
-                description="Shell completion support",
-                action=CustomAutocompleteAction,
-                default=None,
-                expose=False,
-            ),
-        )
```

### Comparing `arc_cli-8.0.0/arc/core/param/param_tree.py` & `arc_cli-8.1.0/arc/define/param/param_tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from __future__ import annotations
+
 import typing as t
 from dataclasses import dataclass
 
-
 if t.TYPE_CHECKING:
-    from arc.core.param import Param
+    from arc.define.param import Param
+
+T = t.TypeVar("T", bound=type)
 
 
 @dataclass
 class ParamValue:
     value: t.Any
-    param: Param
+    param: Param[t.Any]
 
 
 @dataclass
-class ParamTree:
+class ParamTree(t.Generic[T]):
     """Tree data stucture that represents all
     the param values for a particular command execution"""
 
-    data: dict[str, ParamTree | ParamValue]
-    cls: type
+    data: dict[str, ParamTree[t.Any] | ParamValue]
+    cls: T
 
-    def __getitem__(self, path: t.Sequence[str]):
+    def __getitem__(self, path: t.Sequence[str]) -> t.Any:
         curr = self.__get_from_path(path)
         return curr.value
 
-    def __setitem__(self, path: t.Sequence[str], value: t.Any):
+    def __setitem__(self, path: t.Sequence[str], value: t.Any) -> None:
         curr = self.__get_from_path(path)
         curr.value = value
 
     def __get_from_path(self, path: t.Sequence[str]) -> ParamValue:
         if isinstance(path, str):
             path = (path,)
 
-        curr: ParamTree | ParamValue = self
+        curr: ParamTree[t.Any] | ParamValue = self
 
         for component in path:
             if isinstance(curr, ParamTree):
                 curr = curr.data[component]
             else:
                 raise KeyError(f"{path} not a valid keypath")
 
@@ -49,15 +51,15 @@
     def values(self) -> t.Generator[ParamValue, None, None]:
         for value in self.data.values():
             if isinstance(value, ParamTree):
                 yield from value.values()
             else:
                 yield value
 
-    def compile(self, include_hidden: bool = False):
+    def compile(self, include_hidden: bool = False) -> T:
         compiled: dict[str, t.Any] = {}
         for key, value in self.data.items():
             if isinstance(value, ParamTree):
                 compiled[key] = value.compile(include_hidden)
             else:
                 if value.param.expose or include_hidden:
                     compiled[key] = value.value
```

### Comparing `arc_cli-8.0.0/arc/logging.py` & `arc_cli-8.1.0/arc/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from arc.color import colorize, effects, bg
+
+from arc.color import bg, colorize, fg, fx
 
 DEBUG = logging.DEBUG
 INFO = logging.INFO
 WARNING = logging.WARNING
 ERROR = logging.ERROR
 CRITICAL = logging.CRITICAL
 
@@ -13,27 +14,28 @@
         DEBUG: bg.BLUE,
         INFO: bg.ARC_BLUE,
         WARNING: bg.rgb(204, 195, 63),
         ERROR: bg.RED,
         CRITICAL: bg.BRIGHT_RED,
     }
 
-    def format(self, record: logging.LogRecord):
+    def format(self, record: logging.LogRecord) -> str:
         record.message = record.getMessage()
         record.levelname = colorize(
             f" {record.levelname:^8} ",
             self.level_color[record.levelno],
-            effects.BOLD,
+            fx.BOLD,
+            fg.BLACK,
         )
         record.name = colorize(f"{record.name:^5}", bg.GREY)
         return super().format(record)
 
 
 mode_map = {
-    "development": DEBUG,
+    "development": INFO,
     "production": WARNING,
     "test": ERROR,
 }
 
 
 logger = logging.getLogger("arc")
 logger.setLevel(ERROR)
```

### Comparing `arc_cli-8.0.0/arc/params.py` & `arc_cli-8.1.0/arc/define/param/constructors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 import typing as t
 
-from arc import constants
-from arc.core.classful import modify_group_cls
-from arc.core.param import param
 import arc.typing as at
+from arc import constants
+from arc.define.param import param
 
 
 class ParamInfo:
     def __init__(
         self,
-        param_cls: type[param.Param],
+        param_cls: type[param.Param[t.Any]],
         param_name: str = None,
         short: str = None,
         default: t.Any = constants.MISSING,
         desc: str = None,
-        callback: t.Callable = None,
+        callback: at.ParamCallback = None,
         action: param.Action = None,
         prompt: str = None,
         envvar: str = None,
         complete: at.CompletionFunc = None,
-        getter_func: at.GetterFunc = None,
+        getter_func: at.ParamGetter = None,
+        data: dict[str, t.Any] = None,
     ):
         self.param_cls = param_cls
         self.param_name = param_name
         self.short_name = short
         self.default = default
         self.desc = desc
         self.callback = callback
         self.action = action
         self.prompt = prompt
         self.envvar = envvar
         self.complete = complete
         self.getter_func = getter_func
+        self.data = data or {}
 
-    def dict(self):
+    def dict(self) -> dict[str, t.Any]:
         """Used to pass to `Param()` as **kwargs"""
         return {
             "param_name": self.param_name,
             "short_name": self.short_name,
             "default": self.default,
             "description": self.desc,
             "callback": self.callback,
             "prompt": self.prompt,
             "envvar": self.envvar,
             "action": self.action,
             "comp_func": self.complete,
             "getter_func": self.getter_func,
+            "data": self.data,
         }
 
 
 def Argument(
     *,
     name: str = None,
     default: t.Any = constants.MISSING,
     desc: str = None,
-    callback: t.Callable = None,
+    callback: at.ParamCallback = None,
     prompt: str = None,
     envvar: str = None,
-    get: at.GetterFunc = None,
+    get: at.ParamGetter = None,
     complete: at.CompletionFunc = None,
+    **kwargs: t.Any,
 ) -> t.Any:
     """A CLI argument. Input is passed positionally.
 
 
     Args:
         name (str, optional): The name to use for the parameter on the command line.
         default (t.Any, optional): A default value for the parameter. If one is given,
@@ -95,28 +98,30 @@
         default=default,
         desc=desc,
         callback=callback,
         prompt=prompt,
         envvar=envvar,
         getter_func=get,
         complete=complete,
+        data=kwargs,
     )
 
 
 def Option(
     *,
     name: str = None,
     short: str = None,
     default: t.Any = constants.MISSING,
     desc: str = None,
-    callback: t.Callable = None,
+    callback: at.ParamCallback = None,
     prompt: str = None,
     envvar: str = None,
-    get: at.GetterFunc = None,
+    get: at.ParamGetter = None,
     complete: at.CompletionFunc = None,
+    **kwargs: t.Any,
 ) -> t.Any:
     """A (generally optional) keyword parameter.
 
     Args:
         name (str, optional): The name to use for the parameter on the command line.
         short (str, optional): A single character name to refer to this parameter to on the command line (`--name` vs `-n`)
         default (t.Any, optional): A default value for the parameter. If one is given,
@@ -151,24 +156,26 @@
         default=default,
         desc=desc,
         callback=callback,
         prompt=prompt,
         envvar=envvar,
         getter_func=get,
         complete=complete,
+        data=kwargs,
     )
 
 
 def Flag(
     *,
     name: str = None,
     short: str = None,
     default: bool = False,
     desc: str = None,
-    callback: t.Callable = None,
+    callback: at.ParamCallback = None,
+    **kwargs: t.Any,
 ) -> t.Any:
     """An option that represents a boolean value.
 
     Args:
         name (str, optional): The name to use for the parameter on the command line.
         short (str, optional): A single character name to refer to this parameter to on the command line (`--name` vs `-n`)
         default (boolean, optional): A default value for the parameter. If one is given,
@@ -193,24 +200,26 @@
     return ParamInfo(
         param_cls=param.FlagParam,
         param_name=name,
         short=short,
         default=default,
         desc=desc,
         callback=callback,
+        data=kwargs,
     )
 
 
 def Count(
     *,
     name: str = None,
     short: str = None,
     default: int = 0,
     desc: str = None,
-    callback: t.Callable = None,
+    callback: at.ParamCallback = None,
+    **kwargs: t.Any,
 ) -> t.Any:
     """A Flag that counts it's number of apperances on the command line
 
     Args:
         name (str, optional): The name to use for the parameter on the command line.
         short (str, optional): A single character name to refer to this parameter to on the command line (`--name` vs `-n`)
         default (int, optional): The starting point for the counter. Should be an integer.
@@ -237,31 +246,13 @@
         param_cls=param.FlagParam,
         param_name=name,
         short=short,
         default=default,
         desc=desc,
         callback=callback,
         action=param.Action.COUNT,
+        data=kwargs,
     )
 
 
-def Depends(callback: t.Callable) -> t.Any:
-    return ParamInfo(param_cls=param.InjectedParam, callback=callback)
-
-
-G = t.TypeVar("G", bound=type)
-
-
-@t.overload
-def group(*, repr: bool = True) -> t.Callable[[G], G]:
-    ...
-
-
-@t.overload
-def group(cls: G, /) -> G:
-    ...
-
-
-def group(cls=None, *, repr: bool = True):
-    if cls:
-        return modify_group_cls(cls)
-    return modify_group_cls
+def Depends(callback: at.ParamCallback, **kwargs: t.Any) -> t.Any:
+    return ParamInfo(param_cls=param.InjectedParam, callback=callback, data=kwargs)
```

### Comparing `arc_cli-8.0.0/arc/parser.py` & `arc_cli-8.1.0/arc/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 from __future__ import annotations
 
 import argparse
-import enum
 import typing as t
 from gettext import gettext as _
 
 import arc
 import arc.typing as at
-from arc import errors
-from arc.core.param import Action, Param
-from arc.autocompletions import completions
+from arc import errors, safe
+from arc.autocompletions import ShellCompletion
 from arc.color import fg
-from arc.config import config
-from arc.context import Context
-from arc.present.helpers import Joiner
-from arc.utils import safe_issubclass
+from arc.define.param import Action, Param
+from arc.present.joiner import Join
+
 
 if t.TYPE_CHECKING:
-    from arc.core.command import Command
+    from arc.define.command import Command
 
 
 class Parser(argparse.ArgumentParser):
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
+        super().__init__(*args, **kwargs)
+        self.param_map: dict[str, Param[t.Any]] = {}
+
     def parse_intermixed_args(  # type: ignore
         self, args: t.Sequence[str] | None = None, namespace=None
     ) -> at.ParseResult:
         res = super().parse_intermixed_args(args, namespace)
         return dict(res._get_kwargs())
 
     def parse_known_intermixed_args(  # type: ignore
         self, args: t.Sequence[str] | None = None, namespace=None
     ) -> tuple[at.ParseResult, list[str]]:
         parsed, rest = super().parse_known_intermixed_args(args, namespace)
         return (dict(parsed._get_kwargs()), rest)
 
-    def add_param(self, param: Param, command: Command):
+    def add_param(self, param: Param[t.Any], command: Command) -> None:
         kwargs: dict[str, t.Any] = {}
 
         kwargs["action"] = (
             param.action.value if isinstance(param.action, Action) else param.action
         )
 
         if (default := param.parser_default) is not None:
             kwargs["default"] = default
 
-        if safe_issubclass(param.action, CustomAction):
+        if safe.issubclass(param.action, CustomAction):
             kwargs["command"] = command
 
         if param.action is Action.STORE:
             kwargs["nargs"] = param.nargs
 
         if not param.is_argument:
             kwargs["dest"] = param.argument_name
 
+        for name in param.get_param_names():
+            self.param_map[name] = param
+
         self.add_argument(*param.get_param_names(), **kwargs)
 
     # NOTE: This method is almost entirely lifted from
     # the actual argparse implementation, because
     # argparse's error handling cusomization is doodoo
     # All modificatiosn to this method will be marked
-    def _parse_known_args(self, arg_strings, namespace):
+    def _parse_known_args(self, arg_strings, namespace):  # type: ignore
         # replace arg strings that are file references
         if self.fromfile_prefix_chars is not None:
             arg_strings = self._read_args_from_files(arg_strings)
 
         # map all mutually exclusive arguments to the other arguments
         # they can't occur with
         action_conflicts = {}
@@ -101,15 +105,15 @@
         # join the pieces together to form the pattern
         arg_strings_pattern = "".join(arg_string_pattern_parts)
 
         # converts arg strings to the appropriate and then takes the action
         seen_actions = set()
         seen_non_default_actions = set()
 
-        def take_action(action, argument_strings, option_string=None):
+        def take_action(action, argument_strings, option_string=None):  # type: ignore
             seen_actions.add(action)
             argument_values = self._get_values(action, argument_strings)
 
             # error if this argument is not allowed with other previously
             # seen arguments, assuming that actions that use the default
             # value don't really count as "present"
             if argument_values is not action.default:
@@ -122,29 +126,33 @@
 
             # take the action if we didn't receive a SUPPRESS value
             # (e.g. from a default)
             if argument_values is not argparse.SUPPRESS:
                 action(self, namespace, argument_values, option_string)
 
         # function to convert arg_strings into an optional action
-        def consume_optional(start_index):
+        def consume_optional(start_index):  # type: ignore
 
             # get the optional identified at this index
             option_tuple = option_string_indices[start_index]
             action, option_string, explicit_arg = option_tuple
 
             # identify additional optionals in the same arg string
             # (e.g. -xyz is the same as -x -y -z if no args are required)
 
             # MODIFIED ------------------------------------------
-            def _wrapped_match_argument(action, args_str_pattern):
+            def _wrapped_match_argument(action, args_str_pattern):  # type: ignore
                 try:
                     return self._match_argument(action, args_str_pattern)
                 except argparse.ArgumentError as e:
-                    raise errors.ParserError(str(e)) from e
+                    # TODO: need to verify that this is the only
+                    # circumstance that this error will be raised given the
+                    # way in which I'm using argparse
+                    param = self.param_map[e.argument_name]
+                    raise errors.MissingOptionValueError(param) from e
 
             match_argument = _wrapped_match_argument
             # ORIGINAL ------------------------------------------
             # match_argument = self._match_argument
             # ---------------------------------------------------
             action_tuples = []
             while True:
@@ -210,15 +218,15 @@
             return stop
 
         # the list of Positionals left to be parsed; this is modified
         # by consume_positionals()
         positionals = self._get_positional_actions()
 
         # function to convert arg_strings into positional actions
-        def consume_positionals(start_index):
+        def consume_positionals(start_index):  # type: ignore
             # match as many Positionals as possible
             match_partial = self._match_arguments_partial
             selected_pattern = arg_strings_pattern[start_index:]
             arg_counts = match_partial(positionals, selected_pattern)
 
             # slice off the appropriate arg strings for each Positional
             # and add the Positional and its args to the list
@@ -297,15 +305,15 @@
                             self._get_value(action, action.default),
                         )
 
         if required_actions:
             # MODIFIED -----------------------------------------------------------
             self.error(
                 _("the following arguments are required: %s")
-                % Joiner.with_comma(required_actions, style=(fg.YELLOW))
+                % Join.with_comma(required_actions, style=(fg.YELLOW))
             )
             # ORIGINAL -----------------------------------------------------------
             # self.error(
             #     _("the following arguments are required: %s")
             #     % ", ".join(required_actions)
             # )
             # --------------------------------------------------------------------
@@ -334,28 +342,35 @@
         raise errors.ParserError(message)
 
     def exit(self, status: int = 0, message: str | None = None) -> t.NoReturn:
         raise errors.Exit(status, message)
 
 
 class CustomAction(argparse.Action):
-    def __init__(self, *args, command: Command, **kwargs) -> None:
+    def __init__(self, *args: t.Any, command: Command, **kwargs: t.Any) -> None:
         super().__init__(*args, **kwargs)
         self.command = command
 
 
 class CustomHelpAction(CustomAction, argparse._HelpAction):
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: t.Any, **kwargs: t.Any) -> None:
         arc.info(self.command.doc.help())
-        raise errors.Exit()
+        arc.exit()
 
 
 class CustomVersionAction(CustomAction, argparse._VersionAction):
-    def __call__(self, *args, **kwargs):
-        arc.info(config.version)
-        raise errors.Exit()
+    def __call__(self, *args: t.Any, **kwargs: t.Any) -> None:
+        arc.info(self.command.config.version)
+        arc.exit()
 
 
 class CustomAutocompleteAction(CustomAction, argparse._StoreAction):
-    def __call__(self, _parser, _ns, value, *args, **kwargs):
-        arc.info(completions(value, Context.current()), end="")
-        raise errors.Exit()
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        ns: argparse.Namespace,
+        value: t.Any,
+        option_string: str | None = None,
+    ) -> None:
+        # arc.exit(1, "Not currently working")
+        print(ShellCompletion.run(value, self.command), end="")
+        arc.exit()
```

### Comparing `arc_cli-8.0.0/arc/present/box.py` & `arc_cli-8.1.0/arc/present/box.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Literal, Union, Optional
 import re
 import shutil
+from typing import Literal, Optional, Union
+
+from arc.present.ansi import bg, fg, fx
+from arc.present.joiner import Join
 
-from arc import color
-from .data import justifications, Justification
-from .drawing import BORDER_HEAVY, BORDER_LIGHT, Border, borders
 from .ansi import Ansi
+from .data import Justification, justifications
+from .drawing import Border, borders
 
 
 class Box:
     """Presenter for creating a Box around provided text
 
     Examples:
     ```
@@ -25,18 +27,18 @@
     ```
     Will accept colorized strings
     """
 
     def __init__(
         self,
         string: str,
-        border: str = "light",
+        border: str = "rounded",
         padding: Union[int, dict[str, int]] = 0,
-        justify: Justification = "left",
-        color: str = color.fg.WHITE,
+        justify: Justification = "center",
+        color: str = fg.WHITE,
     ):
         """
         Args:
             string: String to surround with a box - May be colored
             border: Border style, either 'light' or 'heavy' defaults to 'light'
             padding: Dictionary containing the padding of each side of the string
                     defaults to: `{"top": 0, "left": 0, "bottom": 0, "right": 0}`
@@ -48,85 +50,84 @@
         """
         self.string = string
         self.__border: Border = borders[border]
         self.__justify = justifications[justify]
         self.__padding = self.__get_padding(padding)
         self.__color = color
 
-    def __str__(self):
+    def __str__(self) -> str:
         cleaned = list(
             self.pad_line(Ansi.clean(string)) for string in self.string.split("\n")
         )
         width = len(max(cleaned, key=len)) + 4
         term_width, _ = shutil.get_terminal_size()
         width = min(width, term_width)
 
-        pad_top = "".join(
+        pad_top = Join.together(
             self.format_line("", width) for _ in range(0, self.__padding["top"])
         )
-        content = "".join(
+        content = Join.together(
             self.format_line(line, width, clean_line)
             for line, clean_line in zip(self.string.split("\n"), cleaned)
         )
-        pad_btm = "".join(
+        pad_btm = Join.together(
             self.format_line("", width) for _ in range(0, self.__padding["bottom"])
         )
 
         content = f"{pad_top}{content}{pad_btm}"
 
         top = self.horizontal_border(width, "top")
         bottom = self.horizontal_border(width, "bot")
         return f"{top}\n{content}{bottom}"
 
     @property
-    def border(self):
+    def border(self) -> Border:
         """Dictionary containting the border stylings"""
         return self.__border
 
     @border.setter
-    def border(self, value):
+    def border(self, value: str) -> None:
         self.__border = borders[value]
 
     # Utils
 
-    def horizontal_border(self, width, side: str):
-        return "".join(
+    def horizontal_border(self, width: int, side: str) -> str:
+        return Join.together(
             (
-                self.__color,
-                self.border["corner"][f"{side}_left"],
+                self.border["corner"][f"{side}_left"],  # type: ignore
                 self.border["horizontal"] * (width - 2),
-                self.border["corner"][f"{side}_right"],
-                color.effects.CLEAR,
-            )
+                self.border["corner"][f"{side}_right"],  # type: ignore
+            ),
+            style=self.__color,
         )
 
     def format_line(
         self,
         line: str,
         width: int,
         cleaned: Optional[str] = None,
-    ):
+    ) -> str:
         cleaned = cleaned or line
         formatted = (
-            f"{self.__color}{self.border['vertical']}{color.effects.CLEAR}"
+            f"{self.__color}{self.border['vertical']}{fx.CLEAR}"
             f"{cleaned:{self.__justify}{width - 2}}"
-            f"{self.__color}{self.border['vertical']}{color.effects.CLEAR}\n"
+            f"{self.__color}{self.border['vertical']}{fx.CLEAR}\n"
         )
 
         if line == "":
             return formatted
 
         # Uses the clean string for calculating the necessary
         # amount of padding on the right, but we want the color, so
         # just re.sub it back in after
         regex = re.compile(cleaned)
         formatted = regex.sub(self.pad_line(line), formatted)
         return formatted
 
-    def pad_line(self, line: str):
+    def pad_line(self, line: str) -> str:
         return " " * self.__padding["left"] + line + " " * self.__padding["right"]
 
     @staticmethod
     def __get_padding(padding: Union[int, dict[str, int]]) -> dict[str, int]:
         default_padding = {"top": 0, "left": 0, "bottom": 0, "right": 0}
         if isinstance(padding, int):
             return dict.fromkeys(default_padding, padding)
```

### Comparing `arc_cli-8.0.0/arc/present/drawing.py` & `arc_cli-8.1.0/arc/present/drawing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import typing as t
 
-
 justify = {
     "left": "<",
     "center": "^",
     "right": ">",
 }
 
 Justification = t.Literal["left", "center", "right"]
```

### Comparing `arc_cli-8.0.0/arc/present/formatters.py` & `arc_cli-8.1.0/arc/present/formatters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # https://github.com/pallets/click/blob/main/src/click/formatting.py
 import shutil
-from contextlib import contextmanager
-import textwrap
 import typing as t
-from .ansi import Ansi
+from contextlib import contextmanager
+
+from arc.present import wrap
+
 
 DEFAULT_MAX_WIDTH = 80
 
 
 class TextFormatter:
     def __init__(
         self,
@@ -22,97 +23,82 @@
             width = min(shutil.get_terminal_size().columns, width) - 2
 
         self.width = width
         self.current_indent = 0
         self._buffer: list[str] = []
 
     @property
-    def value(self):
+    def value(self) -> str:
         """Current value of the formatter"""
         return "".join(self._buffer)
 
-    def indent(self):
+    def indent(self) -> None:
         """Indents text by `indent_increment`"""
         self.current_indent += self.indent_increment
 
-    def dedent(self):
+    def dedent(self) -> None:
         """Dedents text by `indent_increment`"""
         self.current_indent -= self.indent_increment
 
-    def write(self, string: str):
+    def write(self, string: str) -> None:
         self._buffer.append(string)
 
-    def write_heading(self, heading: str):
+    def write_heading(self, heading: str) -> None:
         self.write(f"{'':>{self.current_indent}}{heading}\n")
 
-    def write_text(self, text: t.Union[str, list[str]]):
+    def write_text(self, text: t.Union[str, list[str]]) -> None:
         self.write(
             self.wrap_text(
                 text,
                 width=self.width,
                 initial_indent=" " * self.current_indent,
                 subsequent_indent=" " * self.current_indent,
             )
         )
 
-    def write_paragraph(self):
+    def write_paragraph(self) -> None:
         if self._buffer:
             self.write("\n")
 
     # TODO: This is not handling colored text properly :(
     def wrap_text(
         self,
         text: t.Union[str, list[str]],
         width: int,
         initial_indent: str = "",
         subsequent_indent: str = "",
-        paragraph_seperator: str = "\n\n",
-    ):
+    ) -> str:
         if isinstance(text, str):
             text = [text]
 
         wrapped = ""
 
-        wrapper = textwrap.TextWrapper(
+        wrapper = wrap.TextWrapper(
             width=width,
             initial_indent=initial_indent,
             subsequent_indent=subsequent_indent,
             replace_whitespace=True,
             drop_whitespace=True,
         )
 
         for para in text:
-            if para.startswith("\b"):
-                wrapped += (
-                    self.wrap_text(
-                        para.lstrip("\b\n").split("\n"),
-                        width,
-                        initial_indent,
-                        subsequent_indent,
-                        "\n",
-                    )
-                    + paragraph_seperator
-                )
-            else:
-                width = width + (len(para) - Ansi.len(para))
-                wrapper.width = width
-                wrapped += wrapper.fill(para) + paragraph_seperator
+            wrapped += wrapper.fill(para)
 
         return wrapped.rstrip("\n")
 
     @contextmanager
-    def indentation(self):
+    def indentation(self) -> t.Generator[None, None, None]:
         self.indent()
         try:
             yield
         finally:
             self.dedent()
 
     @contextmanager
-    def section(self, name: str):
+    def section(self, name: str) -> t.Generator[None, None, None]:
         self.write_paragraph()
         self.write_heading(name)
         self.indent()
 
         try:
             yield
         finally:
```

### Comparing `arc_cli-8.0.0/arc/present/help_formatter.py` & `arc_cli-8.1.0/arc/present/help_formatter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,175 +1,186 @@
 from __future__ import annotations
-from itertools import repeat
 
-import typing as t
 import textwrap
-from arc import constants
+import typing as t
+from itertools import repeat
 
-from arc.color import colorize, fg, effects
-from arc.config import config
-from arc.present.helpers import Joiner
-from arc.present.formatters import TextFormatter
+from arc import constants
+from arc.color import colorize, fx
+from arc.config import PresentConfig
 from arc.present.ansi import Ansi
+from arc.present.formatters import TextFormatter
+from arc.present.joiner import Join
+from arc.present.markdown import MarkdownParser
 
 if t.TYPE_CHECKING:
-    from arc.core.documentation import Documentation, ParamDoc
-    from arc.core.command import Command
-
-
-def paragraphize(string: str) -> list[str]:
-    return [textwrap.dedent(para).strip("\n") for para in string.split("\n\n")]
+    from arc.define.command import Command
+    from arc.define.documentation import Documentation, ParamDoc
 
 
 class HelpFormatter(TextFormatter):
     _longest_intro: int = 0
 
-    def __init__(self, doc: Documentation, *args, **kwargs):
+    def __init__(
+        self,
+        doc: Documentation,
+        config: PresentConfig,
+        *args: t.Any,
+        **kwargs: t.Any,
+    ):
         super().__init__(*args, **kwargs)
         self.doc = doc
         self.command = self.doc.command
+        self.config = config
+        self.color = config.color
+        self.parser = MarkdownParser()
 
     @property
-    def argument_params(self):
+    def argument_params(self) -> list[ParamDoc]:
         return [param for param in self.doc.params if param["kind"] == "argument"]
 
     @property
-    def key_params(self):
+    def key_params(self) -> list[ParamDoc]:
         return [param for param in self.doc.params if param["kind"] != "argument"]
 
-    def write_help(self):
+    def format_help(self) -> str:
+        self.write_help()
+        res = self.parser.parse(self.value)
+        return res.fmt(self.config)
+
+    def format_usage(self) -> str:
+        self.write_usage()
+        res = self.parser.parse(self.value)
+        return res.fmt(self.config)
+
+    def write_help(self) -> None:
         doc = self.doc
         self.write_usage()
 
         if doc.description:
-            with self.section(config.default_section_name.upper()):
-                self.write_text(paragraphize(doc.description))
+            with self.section(f"# DESCRIPTION"):
+                self.write(doc.description)
 
         args = self.get_params(self.argument_params)
         options = self.get_params(self.key_params)
         subcommands = self.get_subcommands(
             self.command, self.command.subcommands.values()
         )
 
         longest = max(map(Ansi.len, (v[0] for v in args + options + subcommands))) + 2
 
         if args:
-            self.write_section("ARGUMENTS", args, longest)
+            self.write_section("# ARGUMENTS", args, longest)
         if options:
-            self.write_section("OPTIONS", options, longest)
+            self.write_section("# OPTIONS", options, longest)
         if subcommands:
-            self.write_section("SUBCOMMANDS", subcommands, longest)
-
-        for section, body in doc.docstring.items():
-            if section in {"arguments", config.default_section_name}:
-                continue
+            self.write_section("# SUBCOMMANDS", subcommands, longest)
 
-            with self.section(section):
-                self.write_text(paragraphize(body))
+        self.write(doc.sections)
 
-    def write_heading(self, heading: str):
-        super().write_heading(colorize(heading.upper(), effects.BOLD))
-
-    def write_usage(self):
+    def write_usage(self) -> None:
         command = self.command
 
-        with self.section("USAGE"):
+        with self.section("# USAGE"):
+            self.write("```\n")
             if command.is_root and command.subcommands:
-                params_str = self.usage_params(
-                    [p for p in self.key_params if p["name"] in command.SPECIAL_PARAMS],
-                    self.argument_params,
-                )
-                global_param_str = self.usage_params(self.doc.global_params, [])
+                params_str = self.usage_params(self.key_params, self.argument_params)
                 self.write_text(
-                    Joiner.with_space(
-                        [colorize(command.root.name, config.brand_color), params_str]
+                    Join.with_space(
+                        [
+                            colorize(command.root.name, self.color.accent),
+                            params_str,
+                        ]
                     )
                 )
 
                 if self.doc.command.subcommands:
                     self.write_paragraph()
                     self.write_text(
-                        Joiner.with_space(
+                        Join.with_space(
                             [
-                                colorize(command.root.name, config.brand_color),
-                                global_param_str,
-                                colorize("<subcommand>", effects.UNDERLINE),
+                                colorize(command.root.name, self.color.accent),
+                                colorize("<subcommand>", fx.UNDERLINE),
                                 "[ARGUMENTS ...]",
                             ],
                             remove_falsey=True,
                         )
                     )
             else:
                 params_str = self.usage_params(self.key_params, self.argument_params)
                 fullname = self.doc.fullname
                 path = " ".join(fullname[0:-1]) if fullname else ""
-                name = colorize(fullname[-1], effects.UNDERLINE) if fullname else ""
+                name = colorize(fullname[-1], fx.UNDERLINE) if fullname else ""
 
                 if not command.is_namespace:
                     self.write_text(
-                        Joiner.with_space(
+                        Join.with_space(
                             [
-                                colorize(command.root.name, config.brand_color),
+                                colorize(command.root.name, self.color.accent),
                                 path,
                                 name,
                                 params_str,
                             ],
                             remove_falsey=True,
                         )
                     )
                     if self.doc.command.subcommands:
                         self.write_paragraph()
 
                 if self.doc.command.subcommands:
                     self.write_text(
-                        Joiner.with_space(
+                        Join.with_space(
                             [
-                                colorize(command.root.name, config.brand_color),
+                                colorize(command.root.name, self.color.accent),
                                 path,
                                 name,
-                                colorize("<subcommand>", effects.UNDERLINE),
+                                colorize("<subcommand>", fx.UNDERLINE),
                                 "[ARGUMENTS ...]",
                             ],
                             remove_falsey=True,
                         )
                     )
+            self.write("\n```")
 
-    def usage_params(self, key_params: list[ParamDoc], arg_params: list[ParamDoc]):
+    def usage_params(
+        self, key_params: list[ParamDoc], arg_params: list[ParamDoc]
+    ) -> str:
         formatted = []
         for param in sorted(
             key_params,
             key=lambda p: not p["optional"],
         ):
             if param["kind"] != "argument":
                 formatted.append(self.format_single_param(param))
 
-        if len(formatted) > 0 and len(arg_params) > 0:
-            formatted.append("[--]")
+        # TODO: get this working in the parser
+        # if len(formatted) > 0 and len(arg_params) > 0:
+        #     formatted.append("[--]")
 
         for param in arg_params:
             if param["kind"] == "argument":
                 formatted.append(self.format_single_param(param))
 
-        return Joiner.with_space(formatted, remove_falsey=True)
+        return Join.with_space(formatted, remove_falsey=True)
 
-    def format_single_param(self, param: ParamDoc):
+    def format_single_param(self, param: ParamDoc) -> str:
         fmt = ""
         kind = param["kind"]
         name = param["name"]
         optional = param["optional"]
 
         if kind == "argument":
             fmt = name
 
             nargs = param["nargs"]
             if isinstance(nargs, int) and nargs:
                 if optional:
-                    fmt = Joiner.with_space(repeat(f"[{fmt}]", nargs))
+                    fmt = Join.with_space(repeat(f"[{fmt}]", nargs))
                 else:
-                    fmt = Joiner.with_space(repeat(fmt, nargs))
+                    fmt = Join.with_space(repeat(fmt, nargs))
             elif nargs == "*":
                 fmt += f" [{fmt}...]"
                 if optional:
                     fmt = f"[{fmt}]"
             else:
                 if optional:
                     fmt = f"[{fmt}]"
@@ -184,66 +195,75 @@
                 fmt += f" {param['name'].upper()}"
 
             if optional:
                 fmt = f"[{fmt}]"
 
         return fmt
 
-    def get_params(self, params: t.Collection[ParamDoc]):
+    def get_params(self, params: t.Collection[ParamDoc]) -> list[tuple[str, str]]:
         data = []
         for param in params:
             name: str = ""
             if param["kind"] == "argument":
-                name = colorize(param["name"], config.brand_color)
+                name = colorize(param["name"], self.color.accent)
             else:
-                name = colorize(f"--{param['name']}", config.brand_color)
+                name = colorize(f"--{param['name']}", self.color.accent)
                 if param["short_name"]:
-                    name += colorize(f" (-{param['short_name']})", fg.GREY)
+                    name += colorize(f" (-{param['short_name']})", self.color.subtle)
 
             desc = textwrap.dedent(param["description"] or "")
             if (
                 param["default"] not in (None, constants.MISSING)
                 and param["kind"] != "flag"
             ):
                 if isinstance(param["default"], constants.COLLECTION_TYPES):
-                    default = Joiner.with_comma(param["default"])
+                    default = Join.with_comma(param["default"])
                 else:
                     default = param["default"]
 
-                desc += colorize(f" (default: {default})", fg.GREY)
+                if desc:
+                    desc += " "
 
-            desc = desc.strip("\n")
+                desc += f"[[color.subtle]](default: {default})[[/color.subtle]]"
 
             data.append((name, desc))
 
         return data
 
-    def get_subcommands(self, parent: Command, commands: t.Collection[Command]):
+    def get_subcommands(
+        self, parent: Command, commands: t.Collection[Command]
+    ) -> list[tuple[str, str]]:
         data = []
         for command in commands:
-            name = colorize(command.name, config.brand_color)
+            name = colorize(command.name, self.color.accent)
             desc = command.doc.short_description or ""
             aliases = parent.subcommands.aliases_for(command.name)
             if aliases:
-                name += colorize(f" ({Joiner.with_comma(aliases)})", fg.GREY)
+                name += colorize(f" ({Join.with_comma(aliases)})", self.color.subtle)
 
             data.append((name, desc))
 
         return data
 
-    def write_section(self, section: str, data: list[tuple[str, str]], longest: int):
+    def write_section(
+        self, section: str, data: list[tuple[str, str]], longest: int
+    ) -> None:
         with self.section(section):
+            self.write("```\n")
             for name, desc in data:
                 diff = longest - Ansi.len(name)
 
+                desc = self.parser.parse_inline(desc.strip("\n")).fmt(self.config)
+
                 self.write(
                     self.wrap_text(
                         f"{name}{' ' * diff}{desc}",
                         width=self.width,
                         initial_indent=" " * self.current_indent,
                         subsequent_indent=(" " * self.current_indent) + (" " * longest),
                     )
                 )
                 self.write_paragraph()
+            self.write("```\n")
 
         # Quick fix for added empty line from self.section()
         self._buffer.pop()
```

### Comparing `arc_cli-8.0.0/arc/present/helpers.py` & `arc_cli-8.1.0/arc/present/joiner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,105 @@
 import typing as t
 
 from arc import color
 
 
-class Joiner:
+class Join:
     @staticmethod
-    def join(
-        values: t.Iterable,
-        string: str,
+    def together(
+        values: t.Iterable[t.Any],
+        string: str = "",
         remove_falsey: bool = False,
         style: str = None,
     ) -> str:
         if remove_falsey:
             values = [v for v in values if v]
 
         if style:
             return string.join(color.colorize(v, style) for v in values)
 
         return string.join(str(v) for v in values)
 
     @staticmethod
-    def with_space(values: t.Iterable, *args, **kwargs) -> str:
-        return Joiner.join(values, " ", *args, **kwargs)
+    def with_space(values: t.Iterable[t.Any], *args: t.Any, **kwargs: t.Any) -> str:
+        return Join.together(values, " ", *args, **kwargs)
+
+    @staticmethod
+    def with_comma(values: t.Iterable[t.Any], *args: t.Any, **kwargs: t.Any) -> str:
+        return Join.together(values, ", ", *args, **kwargs)
 
     @staticmethod
-    def with_comma(values: t.Iterable, *args, **kwargs) -> str:
-        return Joiner.join(values, ", ", *args, **kwargs)
+    def with_newline(values: t.Iterable[t.Any], *args: t.Any, **kwargs: t.Any) -> str:
+        return Join.together(values, "\n", *args, **kwargs)
 
     @staticmethod
     def in_groups(
-        first: t.Iterable,
-        second: t.Iterable,
+        first: t.Iterable[t.Any],
+        second: t.Iterable[t.Any],
         string: str,
         between: str,
-        *args,
-        **kwargs
+        *args: t.Any,
+        **kwargs: t.Any,
     ) -> str:
         """Joins two groups objects with `string`, then joins the two groups together with `between`"""
-        return Joiner.join(
+        return Join.together(
             (
-                Joiner.join(first, string, *args, **kwargs),
-                Joiner.join(second, string, *args, **kwargs),
+                Join.together(first, string, *args, **kwargs),
+                Join.together(second, string, *args, **kwargs),
             ),
             between,
         )
 
     @staticmethod
     def with_last(
-        values: t.Sequence, string: str, last_string: str, *args, **kwargs
+        values: t.Sequence[t.Any],
+        string: str,
+        last_string: str,
+        *args: t.Any,
+        **kwargs: t.Any,
     ) -> str:
         """Joins values together with an additional `last_string` to format how
         the final value is joined to the rest of the list
 
         Args:
             values (Sequence): Values to join
             string (str): What to join values 0 - penultimate value with.
             last_string (str): What to use to join the last value to the rest.
         """
         if len(values) == 0:
             return ""
 
         if len(values) == 1:
-            return Joiner.join(values, "", *args, **kwargs)
+            return Join.together(values, "", *args, **kwargs)
 
-        return Joiner.in_groups(
+        return Join.in_groups(
             values[:-1], [values[-1]], string, last_string, *args, **kwargs
         )
 
     @staticmethod
-    def with_and(values: t.Sequence) -> str:
+    def with_and(values: t.Sequence[t.Any]) -> str:
         """Joins a Sequence of items with commas
         and an "and" at the end
 
         Args:
             values (Sequence): Values to join
 
         Returns:
             string: joined values
         """
-        return Joiner.with_last(values, ", ", " and ")
+        return Join.with_last(values, ", ", " and ")
 
     @staticmethod
-    def with_or(values: t.Sequence, *args, **kwargs) -> str:
+    def with_or(values: t.Sequence[t.Any], *args: t.Any, **kwargs: t.Any) -> str:
         """Joins a Sequence of items with commas
         and an "or" at the end
 
         [1, 2, 3, 4] -> "1, 2, 3 or 4"
 
         Args:
             values (Sequence): Values to join
 
         Returns:
             string: joined values
         """
 
-        return Joiner.with_last(values, ", ", " or ", *args, **kwargs)
+        return Join.with_last(values, ", ", " or ", *args, **kwargs)
```

### Comparing `arc_cli-8.0.0/arc/present/table.py` & `arc_cli-8.1.0/arc/present/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
+
 import functools
 import itertools
 import typing as t
 
-from arc.errors import ArcError
-from arc.color import colorize, effects, fg
-from arc.present.ansi import Ansi
+from arc import errors
 from arc.present import drawing
+from arc.present.ansi import Ansi, colorize, fg, fx
 
 
 class ColumnBase(t.TypedDict):  # pylint: disable=inherit-non-class
     """ColumnBase Type"""
 
     name: str
 
@@ -56,48 +56,47 @@
 
 def has_next(seq: t.Sequence[T]) -> t.Generator[tuple[T, bool], None, None]:
     length = len(seq)
     for idx, val in enumerate(seq):
         yield val, idx < length - 1
 
 
-def _format_cell(value: t.Any):
+def _format_cell(value: t.Any) -> str:
     return str(value)
 
 
-def _format_header_cell(value: t.Any):
-    return colorize(str(value), effects.BOLD)
+def _format_header_cell(value: t.Any) -> str:
+    return colorize(str(value), fx.BOLD)
 
 
-def _format_bool(val: bool):
+def _format_bool(val: bool) -> str:
     return colorize(str(val), fg.GREEN if val else fg.RED)
 
 
-def _format_int(val: int):
+def _format_int(val: int) -> str:
     return colorize(str(val), fg.BLUE)
 
 
 _DEFAULT_TYPE_FORMATTERS: dict[type, TableFormatter] = {
     bool: _format_bool,
     int: _format_int,
 }
 
 
 class Table:
     """Display information in a table
 
     ```py
-    from arc.color import colorize, fg
     from arc.present.table import Table
 
     t = Table(["Name", "Age", "Stand"])
     t.add_row(["Jonathen Joestar", 20, "-"])
     t.add_row(["Joseph Joestar", 18, "Hermit Purple (in Part 3)"])
     t.add_row(["Jotaro Kujo", 18, "Star Platinum"])
-    t.add_row(["Josuke Higashikata", 16, "Crazy Diamon"])
+    t.add_row(["Josuke Higashikata", 16, "Crazy Diamond"])
     t.add_row(["Giorno Giovanna", 15, "Gold Experience"])
     t.add_row(["Joylene Kujo", 19, "Stone Free"])
 
 
     print(t)
     ```
 
@@ -105,35 +104,42 @@
     ```console
     ┏━━━━━━━━━━━━━━━━━━━━┳━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
     ┃ Name               ┃ Age ┃ Stand                     ┃
     ┡━━━━━━━━━━━━━━━━━━━━╇━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
     │ Jonathen Joestar   │ 20  │ -                         │
     │ Joseph Joestar     │ 18  │ Hermit Purple (in Part 3) │
     │ Jotaro Kujo        │ 18  │ Star Platinum             │
-    │ Josuke Higashikata │ 16  │ Crazy Diamon              │
+    │ Josuke Higashikata │ 16  │ Crazy Diamond             │
     │ Giorno Giovanna    │ 15  │ Gold Experience           │
     │ Joylene Kujo       │ 19  │ Stone Free                │
     └────────────────────┴─────┴───────────────────────────┘
     ```
     """
 
-    def __init__(self, columns: ColumnInput, default_formatting: bool = True) -> None:
+    def __init__(
+        self,
+        columns: ColumnInput,
+        rows: t.Sequence[t.Sequence[t.Any]] | None = None,
+        default_formatting: bool = True,
+    ) -> None:
         self.__columns: t.Sequence[Column] = self.__resolve_columns(columns)
         self.__rows: list[Row] = []
         self._border = drawing.borders["light"]
         self._head_border = BORDER_HEAVY_TRANS
         self._header_cell_formatter: TableFormatter = (
             _format_header_cell if default_formatting else _format_cell
         )
         self._cell_formatter: TableFormatter = _format_cell
         self._type_formatters: dict[type, TableFormatter] = (
             _DEFAULT_TYPE_FORMATTERS if default_formatting else {}
         )
+        if rows:
+            self.add_rows(rows)
 
-    def __str__(self):
+    def __str__(self) -> str:
         for col in self.__columns:
             cells = [row[col["name"]] for row in self.__rows]
             cells.append(col["name"])
 
             col["width"] = max(
                 Ansi.len(self._fmt_cell_contents(cell)) + 2 for cell in cells
             )
@@ -145,48 +151,69 @@
         for row, has_next_row in has_next(self.__rows):
             table += self._fmt_row(row, has_next_row)
             if has_next_row:
                 table += "\n"
 
         return table
 
-    def add_row(self, row: t.Sequence[t.Any]):
+    def add_row(self, row: t.Sequence[t.Any]) -> None:
         if len(row) > len(self.__columns):
-            raise ArcError("Too many values")
+            raise errors.ArcError("Too many values")
 
         resolved = {}
         for col, value in itertools.zip_longest(self.__columns, row, fillvalue=""):
-            resolved[col["name"]] = value
+            resolved[col["name"]] = value  # type: ignore
 
         self.__rows.append(resolved)
 
-    def fmt_header_cell(self, func: TableFormatter | None = None):
-        def inner(func: TableFormatter):
+    def add_rows(self, rows: t.Sequence[t.Sequence[t.Any]]) -> None:
+        for row in rows:
+            self.add_row(row)
+
+    def fmt_header_cell(
+        self, func: TableFormatter | None = None
+    ) -> TableFormatter | t.Callable[[TableFormatter], TableFormatter]:
+        def inner(func: TableFormatter) -> TableFormatter:
             self._cell_formatter = func
             return func
 
         if func:
             return inner(func)
 
         return inner
 
-    def fmt_cell(self, func: TableFormatter | None = None):
-        """Formats any cell that does not already have a formatter applied"""
+    def fmt_cell(
+        self, func: TableFormatter | None = None
+    ) -> TableFormatter | t.Callable[[TableFormatter], TableFormatter]:
+        """Formats any cell that does not already have a formatter applied
+
+        ```py
+        from arc.color import fg, fx
+        from arc.present import Table
+
+        table = Table()
+
+        @table.fmt_cell
+        def fmt(cell):
+            return f"{fg.RED}{cell}{fx.CLEAR}"
+
+        ```
+        """
 
-        def inner(func: TableFormatter):
+        def inner(func: TableFormatter) -> TableFormatter:
             self._cell_formatter = func
             return func
 
         if func:
             return inner(func)
 
         return inner
 
-    def fmt_type(self, cls: type):
-        def inner(func: t.Callable[[t.Any], str]):
+    def fmt_type(self, cls: type) -> t.Callable[[TableFormatter], TableFormatter]:
+        def inner(func: t.Callable[[t.Any], str]) -> TableFormatter:
             self._type_formatters[cls] = func
             return func
 
         return inner
 
     def _fmt_header(self) -> str:
         border = self._head_border
@@ -218,15 +245,15 @@
             if has_next_column:
                 header += border["intersect"]["cross"]
             else:
                 header += border["intersect"]["vert_right"]
 
         return header
 
-    def _fmt_row(self, row: Row, next_row: bool):
+    def _fmt_row(self, row: Row, next_row: bool) -> str:
         border = self._border
         fmt = ""
 
         fmt += border["vertical"]
 
         for col in self.__columns:
             cell = row.get(col["name"], "")
@@ -247,15 +274,15 @@
 
     def _fmt_cell(
         self,
         cell: t.Any,
         width: int,
         justify: drawing.Justification,
         header: bool = False,
-    ):
+    ) -> str:
         formatted_cell = self._fmt_cell_contents(cell, header)
         width = width - 2
         padding = " " * (width - Ansi.len(formatted_cell))
 
         if justify == "left":
             return " " + formatted_cell + padding + " "
         elif justify == "right":
@@ -264,15 +291,15 @@
             padding_width, remainder = divmod(width - Ansi.len(formatted_cell), 2)
             padding = " " * padding_width
             return (
                 " " + padding + formatted_cell + padding + ("  " if remainder else " ")
             )
 
     @functools.cache
-    def _fmt_cell_contents(self, cell: t.Any, header: bool = False):
+    def _fmt_cell_contents(self, cell: t.Any, header: bool = False) -> str:
         if header:
             return self._header_cell_formatter(cell)
         if type(cell) in self._type_formatters:
             return self._type_formatters[type(cell)](cell)
         else:
             return self._cell_formatter(cell)
 
@@ -286,12 +313,12 @@
             if isinstance(column, str):
                 copy.update({"name": column})
 
             elif isinstance(column, dict):
                 column = t.cast(Column, column)
                 copy.update(column)  # type: ignore
             else:
-                raise ArcError("Columns must either be a string or a dictionary")
+                raise errors.ArcError("Columns must either be a string or a dictionary")
 
             resolved.append(copy)
 
         return resolved
```

### Comparing `arc_cli-8.0.0/arc/types/aliases.py` & `arc_cli-8.1.0/arc/types/aliases.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,65 @@
 """Module for all Alias types. Alias types are types that handle to conversion for other types.
 All builtin types (int, str, float, etc...) have a corresponding Alias type.
 """
 from __future__ import annotations
 
+import collections
 import enum
+import ipaddress
 import pathlib
+import re
 import types
 import typing as t
-import ipaddress
-import dataclasses
-import re
 
 import _io  # type: ignore
 
-from arc import errors, utils
-from arc import autocompletions
+from arc import api, autocompletions, errors, safe
 from arc.autocompletions import Completion, CompletionInfo, CompletionType
 from arc.color import colorize, fg
-from arc.present.helpers import Joiner
-from arc.types.helpers import (
-    safe_issubclass,
-    convert_type,
-)
+from arc.present.joiner import Join
 from arc.prompt.prompts import select_prompt
-
-
+from arc.types.convert import convert_type
+from arc.types.type_arg import TypeArg
 from arc.typing import Annotation, TypeProtocol
 
-from arc.types import type_info
-
 if t.TYPE_CHECKING:
+    from arc.define.param import Param
+    from arc.runtime import Context
     from arc.types.type_info import TypeInfo
-    from arc.context import Context
-    from arc.core.param import Param
 
 
 AliasFor = t.Union[Annotation, t.Tuple[Annotation, ...]]
 
+T = t.TypeVar("T")
+
 
 class Alias:
     """Parent class for all aliases. Stores references to all
     known alias types and handles resolving them. Additionally,
     it provides a convenience wrapper for alias types by implementing
     a custom `cls.__convert__()` that calls `cls.convert()` for non-parameterized
     types and `cls.g_convert()` for generic types.
     """
 
     aliases: dict[Annotation, type[TypeProtocol]] = {}
     alias_for: t.ClassVar[AliasFor | tuple[AliasFor]] = None  # type: ignore
     name: t.ClassVar[t.Optional[str]] = None
-    convert: t.Callable
-    g_convert: t.Callable
+    convert: t.Callable[..., t.Any]
+    g_convert: t.Callable[..., t.Any]
 
     @classmethod
-    def __convert__(cls, value, typ: TypeInfo):
+    def __convert__(cls, value: str, typ: TypeInfo[T]) -> T:
         if cls.name:
             typ.name = cls.name
 
         if not typ.sub_types:
-            obj = utils.dispatch_args(cls.convert, value, typ)
+            obj = api.dispatch_args(cls.convert, value, typ)
         else:
-            obj = utils.dispatch_args(cls.g_convert, value, typ)
+            obj = api.dispatch_args(cls.g_convert, value, typ)
 
         return obj
 
     def __init_subclass__(cls, of: t.Optional[AliasFor | tuple[AliasFor]] = None):
         if of:
             cls.alias_for = of
 
@@ -76,41 +71,41 @@
             for alias in aliases:
                 Alias.aliases[alias] = cls  # type: ignore
 
     @classmethod
     def resolve(cls, annotation: type) -> type[TypeProtocol]:
         """Handles resolving alias types"""
 
-        if safe_issubclass(annotation, TypeProtocol):
+        if safe.issubclass(annotation, TypeProtocol):
             return annotation
         elif annotation in cls.aliases:
             # Type is a key
             # We perform this check once before hand
             # because some typing types don't have
             # the mro() method
             return cls.aliases[annotation]
         else:
             # Type is a subclass of a key
             for parent in annotation.mro():
                 if parent in cls.aliases:
                     return cls.aliases[parent]
 
         name = colorize(annotation.__name__, fg.YELLOW)
-        raise errors.ParamError(
+        raise TypeError(
             f"{name} is not a valid type. "
             f"Please ensure that {name} conforms to the custom type protocol "
             f"or that there is a alias type registered for it: "
-            "https://arc.seanrcollings.com/usage/parameter-types/#custom-types"
+            "https://arc.seancollings.dev/usage/parameters/types/custom-types"
         )
 
 
 # Builtin Types ---------------------------------------------------------------------------------
 
 
-class StringAlias(Alias, str, of=str):
+class StringAlias(Alias, str, of=(str, t.Any, collections.UserString)):  # type: ignore
     @classmethod
     def convert(cls, value: str, info: TypeInfo[str]) -> str:
         try:
             return str(value)
         except ValueError as e:
             raise errors.ConversionError(value, str(e))
 
@@ -133,32 +128,32 @@
                 return int(value)
         except ValueError as e:
             raise errors.ConversionError(value, "must be an integer", e)
 
 
 class FloatAlias(Alias, of=float):
     @classmethod
-    def convert(cls, value, info: TypeInfo[float]) -> float:
+    def convert(cls, value: str, info: TypeInfo[float]) -> float:
         try:
             return info.origin(value)
         except ValueError as e:
             raise errors.ConversionError(value, "must be a float", e)
 
 
 class _CollectionAlias(Alias):
     alias_for: t.ClassVar[type]
 
     @classmethod
-    def convert(cls, value: t.Any):
+    def convert(cls, value: t.Any) -> t.Any:
         if isinstance(value, str):
             return cls.alias_for(value.split(","))
         return cls.alias_for(value)
 
     @classmethod
-    def g_convert(cls, value: str, typ: TypeInfo):
+    def g_convert(cls, value: str, typ: TypeInfo[t.Any]) -> t.Any:
         lst = cls.convert(value)
         sub = typ.sub_types[0]
         sub_type = sub.resolved_type
 
         try:
             return cls.alias_for([sub_type.__convert__(v, sub) for v in lst])
         except errors.ConversionError as e:
@@ -167,25 +162,25 @@
                     value,
                     f"{colorize(' '.join(value), fg.YELLOW)} is not a valid {typ.name} of {name}s",
                     e,
                 ) from e
             raise e
 
 
-class ListAlias(list, _CollectionAlias, of=list):
+class ListAlias(list[t.Any], _CollectionAlias, of=list):
     ...
 
 
-class SetAlias(set, _CollectionAlias, of=set):
+class SetAlias(set[t.Any], _CollectionAlias, of=set):
     ...
 
 
-class TupleAlias(tuple, _CollectionAlias, of=tuple):
+class TupleAlias(tuple[t.Any], _CollectionAlias, of=tuple):
     @classmethod
-    def g_convert(cls, value: str, info: TypeInfo):
+    def g_convert(cls, value: str, info: TypeInfo[T]) -> tuple[t.Any, ...]:
         tup = cls.convert(value)
 
         # Arbitraryily sized tuples
         if cls.any_size(info):
             return super().g_convert(value, info)
 
         # Statically sized tuples
@@ -198,33 +193,32 @@
 
         return tuple(
             convert_type(item_type.resolved_type, item, item_type)
             for item_type, item in zip(info.sub_types, tup)
         )
 
     @classmethod
-    def any_size(cls, info: TypeInfo):
+    def any_size(cls, info: TypeInfo[T]) -> bool:
         return info.sub_types[-1].origin is Ellipsis
 
 
-class DictAlias(dict, Alias, of=dict):
+class DictAlias(dict[str, t.Any], Alias, of=dict):
     alias_for: t.ClassVar[type]
-    name = "dictionary"
 
     @classmethod
-    def convert(cls, value: str, info: TypeInfo) -> dict[str, str]:
+    def convert(cls, value: str, info: TypeInfo[t.Any]) -> dict[str, str]:
         dct = cls.alias_for(i.split("=") for i in value.split(","))
         if isinstance(info.origin, t._TypedDictMeta):  # type: ignore
             return cls.__typed_dict_convert(dct, info)
 
         return dct
 
     @classmethod
-    def g_convert(cls, value, info: TypeInfo):
-        dct: dict = cls.convert(value, info)
+    def g_convert(cls, value: str, info: TypeInfo[t.Any]) -> dict[str, t.Any]:
+        dct: dict[str, t.Any] = cls.convert(value, info)
         key_sub = info.sub_types[0]
         key_type = key_sub.resolved_type
         value_sub = info.sub_types[1]
         value_type = value_sub.resolved_type
 
         try:
             return cls.alias_for(
@@ -241,88 +235,92 @@
                 value,
                 f"{value} is not a valid {info.name} of "
                 f"{key_sub.name} keys and {value_sub.name} values",
                 e,
             ) from e
 
     @classmethod
-    def __typed_dict_convert(cls, elements: dict[str, str], info: TypeInfo):
+    def __typed_dict_convert(
+        cls, elements: dict[str, str], info: TypeInfo[t.Any]
+    ) -> dict[str, t.Any]:
         hints = t.get_type_hints(info.origin, include_extras=True)
         for key, value in elements.items():
             if key not in hints:
                 raise errors.ConversionError(
                     elements,
                     f"{key} is not a valid key name. "
-                    f"Valid keys are: {Joiner.with_and(list(hints.keys()))}",
+                    f"Valid keys are: {Join.with_and(list(hints.keys()))}",
                 )
 
-            sub_info = type_info.TypeInfo.analyze(hints[key])
+            sub_info = type(info).analyze(hints[key])
             try:
                 elements[key] = convert_type(sub_info.resolved_type, value, sub_info)
             except errors.ConversionError as e:
                 raise errors.ConversionError(
                     value, f"{value} is not a valid value for key {key}", e
                 ) from e
 
         return elements
 
 
 class NoneAlias(Alias, of=types.NoneType):
     @classmethod
-    def convert(self, value: t.Any):
+    def convert(self, value: t.Any) -> t.NoReturn:
         raise errors.ConversionError(value, "")
 
 
 # Typing types ---------------------------------------------------------------------------------
 
 
-class UnionAlias(Alias, of=(t.Union, types.UnionType)):  # type: ignore
+class UnionAlias(Alias, of=(t.Union, types.UnionType)):
     @classmethod
-    def g_convert(cls, value: t.Any, info: TypeInfo):
+    def g_convert(cls, value: t.Any, info: TypeInfo[t.Any]) -> t.Any:
 
         for sub in info.sub_types:
             try:
                 return convert_type(sub.resolved_type, value, sub)
             except Exception:
                 ...
 
-        options = Joiner.with_or(
+        options = Join.with_or(
             list(sub.name for sub in info.sub_types if sub.origin is not types.NoneType)
         )
         raise errors.ConversionError(
             value,
             f"must be a {options}",
         )
 
 
 class LiteralAlias(Alias, of=t.Literal):
     @classmethod
-    def g_convert(cls, value: t.Any, info: TypeInfo):
+    def g_convert(cls, value: t.Any, info: TypeInfo[t.Any]) -> t.Any:
         for sub in info.sub_types:
             if str(sub.original_type) == value:
                 return sub.original_type
 
         raise errors.ConversionError(
             value,
-            f"must be {Joiner.with_or(list(sub.original_type for sub in info.sub_types))}",
+            f"must be {Join.with_or(list(sub.original_type for sub in info.sub_types))}",
         )
 
     @classmethod
-    def __prompt__(cls, param: Param, ctx: Context):
+    def __prompt__(cls, param: Param[t.Any], ctx: Context) -> str:
         return select_prompt(
+            ctx.prompt,
+            t.cast(str, param.prompt),
             list(str(tp.origin) for tp in param.type.sub_types),
-            param,
-            highlight_color=ctx.config.brand_color,
+            highlight_color=ctx.config.present.color.accent,
         )
 
     @classmethod
-    def __completions__(cls, info, param):
-        return [
-            autocompletions.Completion(str(tp.origin)) for tp in param.type.sub_types
-        ]
+    def __completions__(
+        cls, info: CompletionInfo, param: Param[t.Any]
+    ) -> t.Iterator[autocompletions.Completion]:
+        for tp in param.type.sub_types:
+            yield autocompletions.Completion(str(tp.origin))
 
 
 # Stdlib types ---------------------------------------------------------------------------------
 
 
 class EnumAlias(Alias, of=enum.Enum):
     @classmethod
@@ -331,64 +329,76 @@
             if issubclass(info.origin, enum.IntEnum):
                 return info.origin(int(value))
 
             return info.origin(value)
         except ValueError as e:
             raise errors.ConversionError(
                 value,
-                f"must be {Joiner.with_or([m.value for m in info.origin.__members__.values()])}",
+                f"must be {Join.with_or([m.value for m in info.origin.__members__.values()])}",
             ) from e
 
     @classmethod
     def __prompt__(cls, param: Param[enum.Enum], ctx: Context) -> t.Any:
         enum_cls: type[enum.Enum] = param.type.origin
         return select_prompt(
+            ctx.prompt,
+            t.cast(str, param.prompt),
             list(str(m.value) for m in enum_cls.__members__.values()),
-            param,
-            highlight_color=ctx.config.brand_color,
+            highlight_color=ctx.config.present.color.accent,
         )
 
     @classmethod
-    def __completions__(cls, info, param):
-        return [
-            autocompletions.Completion(str(m.value))
-            for m in param.type_info.origin.__members__.values()
-        ]
+    def __completions__(
+        cls, info: CompletionInfo, param: Param[enum.Enum]
+    ) -> t.Iterator[autocompletions.Completion]:
+        for m in param.type.origin.__members__.values():
+            yield autocompletions.Completion(str(m.value))
 
 
 class PathAlias(Alias, of=pathlib.Path):
     @classmethod
-    def convert(cls, value: t.Any):
+    def convert(cls, value: t.Any) -> pathlib.Path:
         return pathlib.Path(value)
 
+    @classmethod
+    def __completions__(
+        cls, info: CompletionInfo, _param: Param[pathlib.Path]
+    ) -> t.Iterator[Completion]:
+        yield Completion(info.current, type=CompletionType.FILE)
+
 
 class IOAlias(Alias, of=(_io._IOBase, t.IO)):
     name = "file"
 
     @classmethod
-    def convert(cls, value: str, info: TypeInfo) -> t.IO:
+    def convert(cls, value: str, info: TypeInfo[t.Any]) -> t.IO[str]:
         error_msg = f"Cannot access {value}:"
+        arg = TypeArg.ensure(info.type_arg, str(info.origin))
         try:
-            file: t.IO = open(value, **info.type_arg.dict())
+            file: t.IO[str] = open(value, **arg.dict())
             return file
         except FileNotFoundError as e:
             raise errors.ConversionError(value, f"{error_msg} file not found") from e
         except PermissionError as e:
             raise errors.ConversionError(value, f"{error_msg} permission denied") from e
 
     @classmethod
-    def __completions__(cls, info: CompletionInfo, _param):
-        return Completion(info.current, CompletionType.FILE)
+    def __completions__(
+        cls, info: CompletionInfo, _param: Param[t.IO[str]]
+    ) -> t.Iterator[Completion]:
+        yield Completion(info.current, type=CompletionType.FILE)
 
 
 class _Address(Alias):
     alias_for: t.ClassVar[type]
 
     @classmethod
-    def convert(cls, value: str, info):
+    def convert(
+        cls, value: str, info: TypeInfo[t.Any]
+    ) -> ipaddress.IPv4Address | ipaddress.IPv6Address:
         try:
             if value.isnumeric():
                 return cls.alias_for(int(value))
 
             return cls.alias_for(value)
         except ipaddress.AddressValueError as e:
             raise errors.ConversionError(
@@ -402,20 +412,20 @@
 
 class IPv6Alias(ipaddress.IPv6Address, _Address, of=ipaddress.IPv6Address):
     name = "IPv6"
 
 
 class PatternAlias(Alias, of=re.Pattern):
     @classmethod
-    def convert(cls, value: str, info: TypeInfo):
+    def convert(cls, value: str, info: TypeInfo[t.Any]) -> re.Pattern[str]:
         try:
             return re.compile(value, cls.flags(info))
         except re.error as e:
             raise errors.ConversionError(
                 value, "Not a valid regular expression", e
             ) from e
 
     @classmethod
-    def flags(cls, info: TypeInfo):
+    def flags(cls, info: TypeInfo[t.Any]) -> int:
         if len(info.annotations) == 0:
             return 0
         return info.annotations[0]
```

### Comparing `arc_cli-8.0.0/arc/types/file.py` & `arc_cli-8.1.0/arc/types/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import abc
+import sys
+import types
 import typing as t
 from dataclasses import dataclass
-import types
-import sys
-from arc.types.default import Default, unwrap
-from arc.types.helpers import convert_type
 
+from arc.types.convert import convert_type
+from arc.types.default import Default, unwrap
 from arc.types.type_arg import TypeArg
 from arc.types.type_info import TypeInfo
 
-
 __all__ = ["File", "Stdin"]
 
 
 OpenNewline = t.Literal[None, "", "\n", "\r", "\r\n"]
 OpenErrors = t.Literal[
     None,
     "strict",
@@ -22,36 +21,36 @@
     "surrogateescape",
     "xmlcharrefreplace",
     "backslashreplace",
     "namereplace",
 ]
 
 
-class File(t.IO, abc.ABC):
+class File(t.IO[str], abc.ABC):
     """Obtains a handler to a file. Handles
     the access to the file, and gurantees that
     it is closed before exiting.
 
 
     ## Example
     ```py
-    @arc.command()
+    @arc.command
     def command(file: File.Read):
         arc.print(file.read())
     ```
 
     There are constants defined on `File` (like `File.Read` above) for
     all common actions (`Read`, `Write`, `Append`, `ReadWrite`, etc...).
     View all of them below.
 
     If none of the pre-defiend constants match your needs, you can customize
     it with an `Annotated` type.
 
     ```py
-    @arc.command()
+    @arc.command
     def command(file: Annotated[File, File.Args(...)]):
         arc.print(file.read())
     ```
 
     `File.Args`'s call signature matches that of `open` (minus the filename), so
     all of the same properties apply
 
@@ -73,15 +72,15 @@
             self,
             mode: str = Default("r"),
             buffering: int = Default(-1),
             encoding: t.Optional[str] = Default(None),
             errors: OpenErrors = Default(None),
             newline: OpenNewline = Default(None),
             closefd: bool = Default(True),
-            opener: t.Optional[t.Callable] = Default(None),
+            opener: t.Optional[t.Callable[..., t.Any]] = Default(None),
         ):
             self.mode = mode
             self.buffering = buffering
             self.encoding = encoding
             self.errors = errors
             self.newline = newline
             self.closefd = closefd
@@ -112,31 +111,39 @@
     """Equivalent to `open(filename, "ab")`"""
     BinaryAppendRead = t.Annotated[t.BinaryIO, Args("ab+")]
     """Equivalent to `open(filename, "ab+")`"""
 
 
 T = t.TypeVar("T")
 
+StreamOrigin = t.Literal["cli", "stream"]
 
-class Stream(t.Generic[T]):
-    class Args(TypeArg):
-        __slots__ = ("stream", "char")
-
-        def __init__(self, stream: t.IO = sys.stdin, char: str = Default("-")):
-            self.stream = stream
-            self.char = char
 
-    def __init__(self, value: T) -> None:
+class Stream(t.Generic[T]):
+    def __init__(self, value: T, origin: StreamOrigin) -> None:
         self.value: T = value
+        self.origin = origin
 
     @classmethod
-    def __convert__(cls, value, info: TypeInfo):
-        arg: Stream.Args = TypeArg.ensure(info.type_arg, cls.__name__)
+    def __convert__(cls, value: str, info: TypeInfo[t.Any]) -> "Stream[T]":
+        arg: Stream.Args = TypeArg.ensure(
+            t.cast(t.Optional[Stream.Args], info.type_arg), cls.__name__
+        )
+
+        origin: StreamOrigin = "cli"
 
         if value == unwrap(arg.char):
             value = arg.stream.read()
+            origin = "stream"
 
         sub = info.sub_types[0]
-        return cls(convert_type(sub.resolved_type, value, sub))
+        return cls(convert_type(sub.resolved_type, value, sub), origin)
+
+    class Args(TypeArg):
+        __slots__ = ("stream", "char")
+
+        def __init__(self, stream: t.IO[str] = sys.stdin, char: str = Default("-")):
+            self.stream = stream
+            self.char = char
 
 
 Stdin = t.Annotated[Stream[T], Stream.Args(sys.stdin)]
```

### Comparing `arc_cli-8.0.0/arc/types/middleware.py` & `arc_cli-8.1.0/arc/types/middleware/observers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 from __future__ import annotations
+
 import typing as t
 
-from arc.core.param import ValueOrigin
+from arc import logging
+from arc.define.param import ValueOrigin
 
 if t.TYPE_CHECKING:
-    from arc.core.param import Param
     from arc import Context
+    from arc.define.param import Param
 
 
 class Log:
     """Type middleware to log the value provided
 
     ## Example
     ```py
     import typing as t
     import arc
     from arc.types.middleware import Log
 
     arc.configure(environment="development")
 
 
-    @arc.command()
+    @arc.command
     def command(
         val: t.Annotated[int, Log()],
         flag_name: t.Annotated[bool, Log()],
-        ctx: t.Annotated[arc.Context, Log()],
     ):
-        print("hello there!")
+        arc.print("hello there!")
 
 
     command()
     ```
     """
 
-    def __init__(self, name_kind: t.Literal["arg", "param", "cli"] = "arg") -> None:
+    def __init__(
+        self,
+        level: int = logging.INFO,
+        name_kind: t.Literal["arg", "param", "cli"] = "arg",
+    ) -> None:
+        self.level = level
         self.name_kind = name_kind
 
     def __call__(
         self,
         value: t.Any,
         ctx: Context | None = None,
-        param: Param | None = None,
+        param: Param[t.Any] | None = None,
     ) -> t.Any:
         if param and ctx:
             names = {
                 "arg": param.argument_name,
                 "param": param.param_name,
                 "cli": param.cli_name,
             }
 
             origin = ctx.get_origin(param.argument_name, ValueOrigin.DEFAULT)
-            ctx.logger.debug(
-                f"{names.get(self.name_kind, param.argument_name)} = {value} ({origin.value})"
-            )
+            name = names.get(self.name_kind, param.argument_name)
+
+            ctx.logger.log(self.level, f"{name} = {value} ({origin.value})")
 
         return value
```

### Comparing `arc_cli-8.0.0/arc/types/network.py` & `arc_cli-8.1.0/arc/types/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
+
 import ipaddress
-from urllib.parse import urlparse
 import typing as t
+from urllib.parse import urlparse
 
 from arc import errors
-from arc.present.helpers import Joiner
+from arc.present.joiner import Join
 
 __all__ = [
     "IPAddress",
     "Url",
     "HttpUrl",
     "PostgresUrl",
     "WebSocketUrl",
@@ -22,15 +23,15 @@
 class AllowedUrlProtocols:
     def __init__(self, *allowed: str) -> None:
         self.allowed_protocols = set(allowed)
 
     def __call__(self, value: Url) -> Url:
         if value.protocol not in self.allowed_protocols:
             raise errors.ValidationError(
-                f"protocol must be {Joiner.with_or(tuple(self.allowed_protocols))}"
+                f"protocol must be {Join.with_or(tuple(self.allowed_protocols))}"
             )
 
         return value
 
 
 class RequiredUrlComponents:
     def __init__(self, *components: str) -> None:
@@ -55,15 +56,15 @@
         "port",
         "path",
         "params",
         "query",
         "fragment",
     )
 
-    def __new__(cls, url: str, **_kwargs):
+    def __new__(cls, url: str, **_kwargs: t.Any) -> Url:
         return super().__new__(cls, url)
 
     def __init__(
         self,
         url: str,
         *,
         protocol: str | None = None,
@@ -87,15 +88,15 @@
         self.port = port
         self.path = path
         self.params = params
         self.query = query
         self.fragment = fragment
 
     @classmethod
-    def parse(cls, url: str):
+    def parse(cls, url: str) -> Url:
 
         url = url.strip()
 
         result = urlparse(url.strip())
 
         parsed: Url = cls(
             url=url,
@@ -110,15 +111,15 @@
             query=result.query,
             fragment=result.fragment,
         )
 
         return parsed
 
     @classmethod
-    def __convert__(cls, value) -> Url:
+    def __convert__(cls, value: str) -> Url:
         try:
             return cls.parse(value)
         except ValueError as e:
             raise errors.ConversionError(value, str(e)) from e
 
 
 HttpUrl = t.Annotated[Url, AllowedUrlProtocols("http", "https")]
```

### Comparing `arc_cli-8.0.0/arc/types/numbers.py` & `arc_cli-8.1.0/arc/types/numbers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
+
 import typing as t
 
 from arc.types.default import Default
 from arc.types.type_arg import TypeArg
-from arc.types.validators import GreaterThan, LessThan
-
+from arc.types.middleware import GreaterThan, LessThan
 
 __all__ = [
     "Hex",
     "Oct",
     "Binary",
     "PositiveInt",
     "NegativeInt",
```

### Comparing `arc_cli-8.0.0/arc/types/path.py` & `arc_cli-8.1.0/arc/types/path.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import pathlib
 import typing as t
 
 from arc import errors
 from arc.autocompletions import Completion, CompletionInfo, CompletionType
 
-
 __all__ = ["ValidPath", "FilePath", "DirectoryPath"]
 
 
-def valid_path(value: pathlib.Path):
+def valid_path(value: pathlib.Path) -> pathlib.Path:
     if not value.exists():
         raise errors.ValidationError(f"{value} is not a file or directory")
 
     return value
 
 
-def valid_directory(value: pathlib.Path):
+def valid_directory(value: pathlib.Path) -> pathlib.Path:
     if not value.is_dir():
         raise errors.ValidationError(f"{value} is not a directory")
 
     return value
 
 
-def valid_file(value: pathlib.Path):
+def valid_file(value: pathlib.Path) -> pathlib.Path:
     if not value.is_file():
         raise errors.ValidationError(f"{value} is not a file")
 
     return value
 
 
 ValidPath = t.Annotated[pathlib.Path, valid_path]
```

### Comparing `arc_cli-8.0.0/arc/types/semver.py` & `arc_cli-8.1.0/arc/types/semver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 from __future__ import annotations
+
 import re
 import typing as t
-from arc import errors, typing as at
-from arc.utils import cmp
+
+from arc import errors
+
+CompareReturn = t.Literal[-1, 0, 1]
+
+
+def cmp(a: t.Any, b: t.Any) -> CompareReturn:
+    """Compare two values
+
+    Args:
+        a (Any): First value
+        b (Any): Second value
+
+    Returns:
+        - `a < b  => -1`
+        - `a == b =>  0`
+        - `a > b  =>  1`
+    """
+    return (a > b) - (a < b)
 
 
 # https://semver.org/#is-there-a-suggested-regular-expression-regex-to-check-a-semver-string
 SEMVAR_REGEX = re.compile(
     r"^(?P<major>0|[1-9]\d*)\.(?P<minor>0|[1-9]\d*)\.(?P<patch>0|[1-9]\d*)"
     r"(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)"
     r"(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?"
@@ -36,54 +54,54 @@
         self._prerelease: tuple[str, ...] = (
             tuple(prerelease.split(self._metadata_sep)) if prerelease else tuple()
         )
         self._build: tuple[str, ...] = (
             tuple(build.split(self._metadata_sep)) if build else tuple()
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         string = f"{self.major}.{self.minor}.{self.patch}"
         if self.prerelease:
             string += (
                 f"{self._prerelease_prefix}{self._metadata_sep.join(self.prerelease)}"
             )
         if self.build:
             string += f"{self._build_prefix}{self._metadata_sep.join(self.build)}"
 
         return string
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"SemVer({str(self)!r})"
 
-    def __iter__(self):
+    def __iter__(self) -> t.Iterator[t.Any]:
         yield from (a for a in self.tuple() if a)
 
     @property
-    def major(self):
+    def major(self) -> int:
         return self._major
 
     @property
-    def minor(self):
+    def minor(self) -> int:
         return self._minor
 
     @property
-    def patch(self):
+    def patch(self) -> int:
         return self._patch
 
     @property
-    def prerelease(self):
+    def prerelease(self) -> tuple[str, ...]:
         return self._prerelease
 
     @property
-    def build(self):
+    def build(self) -> tuple[str, ...]:
         return self._build
 
     # Comparison Operators --------------------------------------------------------------------
 
-    def compare(self, other: object) -> at.CompareReturn:
+    def compare(self, other: object) -> CompareReturn:
         """Compares `self` with `other`
 
         Args:
             other (SemVer): the second version for comparison
 
         Returns:
             at.CompareReturn: is negative if self < other,
@@ -121,15 +139,15 @@
             if comp:
                 return comp
 
         return cmp(len(pr1), len(pr2))
 
     def _cmp_prerelease_tag(
         self, a: t.Union[str, int], b: t.Union[str, int]
-    ) -> at.CompareReturn:
+    ) -> CompareReturn:
         """Compares two prerelease tags given the following conditions:
         - Identifiers consisting of only digits are compared numerically.
         - Identifiers with letters or hyphens are compared lexically in ASCII sort order.
         - Numeric identifiers always have lower precedence than non-numeric identifiers.
         """
         # Compared numerically
         if isinstance(a, int) and isinstance(b, int):
@@ -139,62 +157,62 @@
             return -1
         elif isinstance(b, int):
             return 1
 
         # Compared lexically
         return cmp(a, b)
 
-    def __eq__(self, other) -> bool:
+    def __eq__(self, other: object) -> bool:
         return self.compare(other) == 0
 
-    def __ne__(self, other) -> bool:
+    def __ne__(self, other: object) -> bool:
         return self.compare(other) != 0
 
-    def __lt__(self, other) -> bool:
+    def __lt__(self, other: object) -> bool:
         return self.compare(other) == -1
 
-    def __le__(self, other) -> bool:
+    def __le__(self, other: object) -> bool:
         return self.compare(other) <= 0
 
-    def __gt__(self, other) -> bool:
+    def __gt__(self, other: object) -> bool:
         return self.compare(other) == 1
 
-    def __ge__(self, other) -> bool:
+    def __ge__(self, other: object) -> bool:
         return self.compare(other) >= 0
 
     # Utility Functions -----------------------------------------------------------------------
 
-    def tuple(self):
+    def tuple(self) -> tuple[int, int, int, tuple[str, ...], tuple[str, ...]]:
         return (self.major, self.minor, self.patch, self.prerelease, self.build)
 
-    def dict(self):
+    def dict(self) -> dict[str, t.Any]:
         return {
             "major": self.major,
             "minor": self.minor,
             "patch": self.patch,
             "prerelease": self.prerelease,
             "build": self.build,
         }
 
-    def bump_major(self):
+    def bump_major(self) -> SemVer:
         cls = type(self)
         return cls(self.major + 1)
 
-    def bump_minor(self):
+    def bump_minor(self) -> SemVer:
         cls = type(self)
         return cls(self.major, self.minor + 1)
 
-    def bump_patch(self):
+    def bump_patch(self) -> SemVer:
         cls = type(self)
         return cls(self.major, self.minor, self.patch + 1)
 
     # Conversion Utilities --------------------------------------------------------------------
 
     @classmethod
-    def parse(cls, string: str):
+    def parse(cls, string: str) -> SemVer:
         match = SEMVAR_REGEX.match(string)
         if not match:
             raise ValueError("Invalid semantic version string")
 
         groups = match.groupdict()
 
         return cls(
@@ -202,12 +220,12 @@
             minor=int(groups["minor"]),
             patch=int(groups["patch"]),
             prerelease=groups["prerelease"],
             build=groups["build"],
         )
 
     @classmethod
-    def __convert__(cls, value: str):
+    def __convert__(cls, value: str) -> SemVer:
         try:
             return cls.parse(value)
         except ValueError as e:
             raise errors.ConversionError(value, str(e)) from e
```

### Comparing `arc_cli-8.0.0/arc/types/transforms.py` & `arc_cli-8.1.0/arc/types/middleware/transformers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
+
 import typing as t
 
 
 class Round:
     """Type Tranformation to round given input to `ndigits`
 
     ## Type Contraints
     - Supports `round()`
 
     ## Example
     ```py
     import arc
-    from arc.transforms import Round
+    from arc.types.middleware import Round
 
-    @arc.command()
+    @arc.command
     def command(val: Annotated[float, Round(2)])
         arc.print(val)
 
     command()
     ```
 
     ```console
@@ -27,15 +28,15 @@
     """
 
     __slots__ = ("ndigits",)
 
     def __init__(self, ndigits: int) -> None:
         self.ndigits = ndigits
 
-    def __call__(self, value: t.SupportsRound) -> t.SupportsRound:
+    def __call__(self, value: t.SupportsRound[t.Any]) -> t.SupportsRound[t.Any]:
         return round(value, self.ndigits)
 
 
 class SupportsSlice(t.Protocol):
     def __getitem__(self, slice: slice) -> SupportsSlice:
         ...
 
@@ -45,17 +46,17 @@
 
     ## Type Constraints
     - Support list-like slice access
 
     ## Example
     ```py
     import arc
-    from arc.transforms import Truncate
+    from arc.types.middleware import Truncate
 
-    @arc.command()
+    @arc.command
     def command(val: Annotated[str, Truncate(6)])
         arc.print(val)
 
     command()
     ```
 
     ```console
@@ -68,15 +69,15 @@
         self.length = length
 
     def __call__(self, value: SupportsSlice) -> SupportsSlice:
         return value[0 : self.length]
 
 
 class PadProtocol(t.Protocol):
-    def __add__(self, other) -> PadProtocol:
+    def __add__(self, other: t.Any) -> PadProtocol:
         ...
 
     def __len__(self) -> int:
         ...
 
 
 class Pad:
@@ -87,31 +88,38 @@
     ## Type Constraints
     - Support `len()`
     - Support `+` for concatenation (like `str` or `list`)
 
     ## Example
     ```py
     import arc
-    from arc.transforms import Pad
+    from arc.types.middleware import Pad
 
-    @arc.command()
+    @arc.command
     def command(val: Annotated[str, Pad(6, 'b')])
         arc.print(val)
 
     command()
     ```
 
     ```console
     $ python example.py a
     abbbbbb
     ```
     """
 
-    def __init__(self, length: int, padding: t.Any = None):
+    def __init__(
+        self, length: int, padding: t.Any, side: t.Literal["left", "right"] = "right"
+    ):
         self.length = length
         self.padding = padding
+        self.side = side
 
-    def __call__(self, value: PadProtocol):
-        while len(value) < self.length:
-            value += self.padding
+    def __call__(self, value: PadProtocol) -> PadProtocol:
+        if self.side == "right":
+            while len(value) < self.length:
+                value += self.padding
+        else:
+            while len(value) < self.length:
+                value = self.padding + value
 
         return value
```

### Comparing `arc_cli-8.0.0/arc/types/type_arg.py` & `arc_cli-8.1.0/arc/types/type_arg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
+
 import typing as t
+
 from arc import errors
 from arc.types.default import isdefault, unwrap
 
-T = t.TypeVar("T", bound="TypeArg")
+T = t.TypeVar("T")
 
 
 class TypeArg:
     __slots__: tuple[str, ...]
 
     def __repr__(self) -> str:
         values = ", ".join(
@@ -21,37 +23,37 @@
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, TypeArg):
             return NotImplemented
         return all(
             getattr(self, attr) == getattr(other, attr) for attr in self.__slots__
         )
 
-    def __iter__(self):
+    def __iter__(self) -> t.Iterator[t.Tuple[str, t.Any]]:
         for slot in self.__slots__:
             yield slot, getattr(self, slot)
 
-    def __or__(self, other: TypeArg):
-        merged: dict = {}
+    def __or__(self, other: TypeArg) -> TypeArg:
+        merged: dict[str, t.Any] = {}
 
         for (attr, value), (_, other_value) in zip(self, other):
             if isdefault(other_value):
                 merged[attr] = value
             else:
                 merged[attr] = other_value
 
-        return type(self)(**merged)  # type: ignore
+        return type(self)(**merged)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return id(self)
 
     def __init_subclass__(cls) -> None:
-        init: t.Callable = getattr(cls, "__init__")
-        setattr: t.Callable = cls.__setattr__
+        init: t.Callable[..., None] = getattr(cls, "__init__")
+        setattr: t.Callable[..., None] = cls.__setattr__
 
-        def __init__(self, *args, **kwargs) -> None:
+        def __init__(self: object, *args: t.Any, **kwargs: t.Any) -> None:
             cls.__setattr__ = object.__setattr__  # type: ignore
             init(self, *args, **kwargs)
             cls.__setattr__ = setattr  # type: ignore
 
         cls.__init__ = __init__  # type: ignore
 
     def dict(self, unwrap_defaults: bool = True) -> dict[str, t.Any]:
```

### Comparing `arc_cli-8.0.0/arc/types/type_info.py` & `arc_cli-8.1.0/arc/types/type_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 from __future__ import annotations
-from functools import cached_property
+
 import types
 import typing as t
-from arc.types.aliases import Alias
-from arc.types.type_arg import TypeArg
+from functools import cached_property
+from arc.constants import COLLECTION_TYPES
 
 import arc.typing as at
-from arc.utils import safe_issubclass
-
+from arc.types.aliases import Alias
+from arc.types.type_arg import TypeArg
 
 T = t.TypeVar("T")
 
 
 class TypeInfo(t.Generic[T]):
     def __init__(
         self,
         original_type: at.Annotation,
         origin: type[T],
-        sub_types: tuple[TypeInfo, ...],
+        sub_types: tuple[TypeInfo[t.Any], ...],
         annotations: tuple[t.Any, ...],
         name: str | None = None,
     ):
         self.original_type = original_type
-        self.origin = origin
+        self.origin: t.Any = origin
         self.sub_types = sub_types
         self.annotations = annotations
         self.name = (
             name
             or getattr(self.origin, "name", None)
             or getattr(self.origin, "__name__", None)
             or str(self.origin)
         )
 
     @cached_property
-    def type_arg(self):
+    def type_arg(self) -> TypeArg | None:
         args = (a for a in self.annotations if isinstance(a, TypeArg))
         try:
             curr = next(args)
         except StopIteration:
             return None
 
         for arg in args:
             curr |= arg
         return curr
 
     @cached_property
-    def middleware(self) -> list[at.MiddlewareCallable]:
+    def middleware(self) -> list[at.TypeMiddleware]:
         return [a for a in self.annotations if callable(a)]
 
     @cached_property
     def resolved_type(self) -> type[at.TypeProtocol]:
         return Alias.resolve(self.origin)
 
     @property
     def is_union_type(self) -> bool:
         """The type is `Union[T...]`"""
-        return self.origin in (t.Union, types.UnionType)  # type: ignore
+        return self.origin in (t.Union, types.UnionType)
 
     @property
     def is_optional_type(self) -> bool:
         """The type is `Optional[T]`"""
         return (
-            self.origin in (t.Union, types.UnionType)  # type: ignore
+            self.origin in (t.Union, types.UnionType)
             and len(self.sub_types) == 2
             and self.sub_types[-1].original_type is type(None)
         )
 
+    @property
+    def is_collection_type(self) -> bool:
+        return self.origin in COLLECTION_TYPES
+
     @classmethod
-    def analyze(cls, annotation) -> TypeInfo:
+    def analyze(cls, annotation: at.Annotation) -> TypeInfo[T]:
+        """Create a `TypeInfo` object based on a type annotation"""
         original_type = annotation
         origin = t.get_origin(annotation) or annotation
-        annotated_args: tuple = tuple()
+        annotated_args: tuple[t.Any, ...] = tuple()
 
         if origin is t.Annotated:
             args = t.get_args(annotation)
             annotation = args[0]
             origin = t.get_origin(annotation) or annotation
             annotated_args = args[1:]
 
         sub_types = tuple(cls.analyze(arg) for arg in t.get_args(annotation))
 
         return cls(
             original_type=original_type,
-            origin=origin,
+            origin=origin,  # type: ignore
             sub_types=sub_types,
             annotations=annotated_args,
         )
```

### Comparing `arc_cli-8.0.0/arc/types/users.py` & `arc_cli-8.1.0/arc/types/users.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
-import pwd
-import grp
+import typing as t
 import functools
+import grp
 import pathlib
+import pwd
 
-from arc import errors, utils, autocompletions as ac
+from arc import autocompletions as ac
+from arc import errors, typing as at, api
 
 
 class User:
     def __init__(
         self,
         name: str,
         password: str,
@@ -22,72 +24,76 @@
         self.password = password
         self.id = uid
         self.group_id = gid
         self.gecos = gecos
         self.directory = pathlib.Path(directory)
         self.shell = pathlib.Path(shell)
 
-    __repr__ = utils.display("name", "id", "group_id", "gecos", "directory", "shell")
+    __repr__ = api.display("name", "id", "group_id", "gecos", "directory", "shell")
 
     @classmethod
-    def __convert__(cls, value):
+    def __convert__(cls, value: str) -> User:
         users = {p[0]: p for p in pwd.getpwall()}
 
         if value in users:
             return cls(*users[value])
 
         raise errors.ConversionError(value, f"{value} is not a valid user")
 
     @classmethod
-    def __completions__(cls, info: ac.CompletionInfo, *_args, **_kwargs):
-        return ac.Completion(info.current, ac.CompletionType.USERS)
+    def __completions__(
+        cls, info: ac.CompletionInfo, *_args: t.Any, **_kwargs: t.Any
+    ) -> at.CompletionReturn:
+        yield ac.Completion(info.current, type=ac.CompletionType.USERS)
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, User):
             return self.id == other.id
 
         return NotImplemented
 
     @classmethod
-    def all(cls):
+    def all(cls) -> list[User]:
         return [cls(*g) for g in pwd.getpwall()]
 
     @functools.cached_property
-    def group(self):
+    def group(self) -> Group:
         group = grp.getgrgid(self.group_id)
         return Group(*group)
 
     @functools.cached_property
-    def groups(self):
+    def groups(self) -> list[Group]:
         return [Group(*g) for g in grp.getgrall() if self.name in g.gr_mem]
 
 
 class Group:
     def __init__(
         self, name: str, password: str | None, gid: int, mem: list[str] = None
     ) -> None:
         self.name = name
         self.password = password
         self.id = gid
         self._mem = mem or []
 
-    __repr__ = utils.display("name", "id", "members")
+    __repr__ = api.display("name", "id", "members")
 
     @classmethod
-    def __convert__(cls, value):
+    def __convert__(cls, value: str) -> Group:
         groups = {p[0]: p for p in grp.getgrall()}
 
         if value in groups:
             return cls(*groups[value])
 
         raise errors.ConversionError(value, f"{value} is not a valid group")
 
     @classmethod
-    def __completions__(cls, info: ac.CompletionInfo, *_args, **_kwargs):
-        return ac.Completion(info.current, ac.CompletionType.GROUPS)
+    def __completions__(
+        cls, info: ac.CompletionInfo, *_args: t.Any, **_kwargs: t.Any
+    ) -> at.CompletionReturn:
+        yield ac.Completion(info.current, type=ac.CompletionType.GROUPS)
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, Group):
             return self.id == other.id
 
         return NotImplemented
 
@@ -97,13 +103,13 @@
         elif isinstance(item, str):
             return item in self._mem
         elif isinstance(item, int):
             user = pwd.getpwuid(item)
             return user.pw_name in self._mem
 
     @classmethod
-    def all(cls):
+    def all(cls) -> list[Group]:
         return [cls(*g) for g in grp.getgrall()]
 
     @functools.cached_property
-    def members(self):
+    def members(self) -> list[User]:
         return [User(*pwd.getpwnam(m)) for m in self._mem]
```

### Comparing `arc_cli-8.0.0/arc/types/validators.py` & `arc_cli-8.1.0/arc/types/middleware/validators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
-import typing as t
+
 import re
+import typing as t
 
 from arc import errors
 
+if t.TYPE_CHECKING:
+    from arc.define.param.param import Param
+    from arc.runtime.context import Context
+
 
 class Matches:
     """Validator to match a regular expression.
 
     ## Type Constraints
     - Matches against `str(value)`, so the type must have a sensible string representation
     """
 
     def __init__(self, pattern: str | re.Pattern[str], flags: int = 0):
         self.pattern = pattern
         self.flags = flags
 
-    def __call__(self, value: t.Any):
+    def __call__(self, value: t.Any) -> t.Any:
         if not re.match(self.pattern, str(value), self.flags):
             raise errors.ValidationError(
                 f"does not match expected format: {self.pattern}"
             )
 
         return value
 
@@ -34,35 +39,46 @@
     """Validator for the length of a value.
 
     - `Len(4)` - Value must be length 4
     - `Len(1, 4)` - Value must be from length 1 to 4
 
     ## Type Constraints
     - Supports `len()`
+
+    **Note**: If you find yourself doing something similar to `Annotated[list[int], Len(2)]`,
+    it's generally going to be a bettter idea to do: `tuple[int, int]`
     """
 
     def __init__(self, min: int, max: int | None = None):
         self.min = min
         self.max = max
 
-    def __call__(self, value: SupportsLen):
+    def __call__(
+        self,
+        value: SupportsLen,
+        ctx: Context | None = None,
+        param: Param[t.Any] | None = None,
+    ) -> SupportsLen:
         length = len(value)
 
         if self.max:
-            if length < self.min:
-                raise errors.ValidationError(
-                    f"must have a length between {self.min} and {self.max}"
-                )
-            if length > self.max:
+            if length < self.min or length > self.max:
+                if param and param.type.is_collection_type:
+                    raise errors.ValidationError(
+                        f"expects between {self.min} and {self.max} arguments"
+                    )
+
                 raise errors.ValidationError(
                     f"must have a length between {self.min} and {self.max}"
                 )
-        else:
-            if length != self.min:
-                raise errors.ValidationError(f"must have a length equal to {self.min}")
+        elif length != self.min:
+            if param and param.type.is_collection_type:
+                raise errors.ValidationError(f"expects {self.min} arguments")
+
+            raise errors.ValidationError(f"must have a length equal to {self.min}")
 
         return value
 
 
 class SupportsComparison(t.Protocol):
     def __gt__(self, other: SupportsComparison) -> bool:
         ...
@@ -86,15 +102,15 @@
     ## Type Constraints
     - Supports Comparison (<, >, ==)
     """
 
     def __init__(self, smallest: SupportsComparison):
         self.smallest = smallest
 
-    def __call__(self, value: SupportsComparison):
+    def __call__(self, value: SupportsComparison) -> SupportsComparison:
         if value <= self.smallest:
             raise errors.ValidationError(f"must be greater than {self.smallest}")
 
         return value
 
 
 class LessThan:
@@ -103,15 +119,15 @@
     ## Type Constraints
     - Supports Comparison (<, >, ==)
     """
 
     def __init__(self, largest: SupportsComparison):
         self.largest = largest
 
-    def __call__(self, value: SupportsComparison):
+    def __call__(self, value: SupportsComparison) -> SupportsComparison:
         if value >= self.largest:
             raise errors.ValidationError(f"must be less than {self.largest}")
 
         return value
 
 
 class Between:
@@ -121,14 +137,14 @@
     - Supports Comparison (<, >, ==)
     """
 
     def __init__(self, lower: SupportsComparison, upper: SupportsComparison):
         self.lower = lower
         self.upper = upper
 
-    def __call__(self, value: SupportsComparison):
+    def __call__(self, value: SupportsComparison) -> SupportsComparison:
         if value <= self.lower or value >= self.upper:
             raise errors.ValidationError(
                 f"must be between {self.lower} and {self.upper}"
             )
 
         return value
```

### Comparing `arc_cli-8.0.0/arc/typing.py` & `arc_cli-8.1.0/arc/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,106 @@
 """Module contains custom type defintions that arc uses"""
 from __future__ import annotations
+
 import typing as t
 
-from arc.autocompletions import CompletionInfo, Completion
+from arc.autocompletions import Completion, CompletionInfo
+from arc.constants import Constant
 
 if t.TYPE_CHECKING:
-    from arc.context import Context
-    from arc.core.param import Param
+    from arc.define.param import Param
+    from arc.runtime import Context
 
 T = t.TypeVar("T")
 
 ExecEnv = dict[str, t.Any]
 
-ExecMode = t.Literal["global", "single", "subcommand"]
-
 Annotation = t.Union[t._SpecialForm, type]
 
 NArgs = t.Union[int, t.Literal["+", "*", "?"], None]
 
-ParseResult = dict[str, t.Union[str, list[str], None]]
-
-Env = t.Literal["production", "development"]
+ParseResult = dict[str, t.Union[str, list[str], None, Constant]]
 
-CommandName = t.Union[str, t.Sequence[str], None]
+Env = t.Literal["production", "development", "test"]
 
 InputArgs = t.Union[str, t.Sequence[str], None]
 
-CompareReturn = t.Literal[-1, 0, 1]
-
 CompletionFunc = t.Callable[
-    [CompletionInfo, "Param"], t.Union[list[Completion], Completion, None]
+    [CompletionInfo, "Param"], t.Union[t.Iterable[Completion], None]
 ]
 
-GetterFunc = t.Union[
+CompletionReturn = t.Iterable[Completion] | None
+
+TypeMiddleware = t.Callable[[t.Any, "Context", "Param"], t.Any]
+
+ParamGetter = t.Union[
     t.Callable[["Param", "Context"], t.Any],
     t.Callable[["Param"], t.Any],
     t.Callable[[], t.Any],
 ]
 
-MiddlewareCallable = t.Callable[[T], T]
+ParamCallback = t.Union[
+    t.Callable[[t.Any, "Param", "Context"], t.Any],
+    t.Callable[[t.Any, "Param"], t.Any],
+    t.Callable[[t.Any], t.Any],
+    t.Callable[[], t.Any],
+]
 
-DecoratorFunc = t.Callable[["Context"], t.Optional[t.Generator[None, t.Any, None]]]
 
-ErrorHandlerFunc = t.Callable[[Exception, "Context"], None]
+class ParamGroupOptions(t.TypedDict):
+    exclude: t.Sequence[str] | None
 
 
 @t.runtime_checkable
 class ClassCallback(t.Protocol):
-    def handle(self):
+    def handle(self) -> t.Any:
         ...
 
 
-CommandCallback = t.Union[t.Callable, type[ClassCallback]]
+FunctionCallback = t.Callable[..., t.Any]
+
+CommandCallback = t.Union[FunctionCallback, type[ClassCallback]]
 """The type of a command's callback.
 
 May be a function
 ```py
-@arc.command()
+@arc.command
 def command(name: str):
     print(f"Hello {name}!")
 ```
 
 Or a class
 ```py
-@arc.command()
+@arc.command
 class command:
     name: str
 
     def handle(self):
         print(f"Hello {self.name}!")
 
 ```
 """
 
 
 class CompletionProtocol(t.Protocol):
     """Protocal that objects need to implement if they are expected to provide completions"""
 
     def __completions__(
-        self, info: CompletionInfo, *args, **kwargs
-    ) -> list[Completion] | Completion | None:
+        self,
+        info: CompletionInfo,
+    ) -> t.Iterable[Completion] | None:
         ...
 
 
 @t.runtime_checkable
 class TypeProtocol(t.Protocol):
     """Protocol that custom types need to conform to"""
 
     @classmethod
-    def __convert__(cls, value, *args):
+    def __convert__(cls, value: t.Any, *args: t.Any) -> t.Any:
         ...
 
 
 class Suggestions(t.TypedDict):
     distance: int
     suggest_params: bool
     suggest_commands: bool
```

### Comparing `arc_cli-8.0.0/pyproject.toml` & `arc_cli-8.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arc-cli"
-version = "8.0.0"
+version = "8.1.0"
 description = "A Regular CLI"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/arc"
 documentation = "https://arc.seanrcollings.com"
 keywords = ["CLI", "extendable", "easy", "arc"]
@@ -14,25 +14,28 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
 packages=[{ include = "arc" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+hypothesis = "^6.68.2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "^20.8b1"
-mypy = "^0.910"
+mypy = "^1.0"
 pylint = "^2.7.0"
 pytest = "^6.2.4"
 pdoc = "^7.1.1"
 mkdocs-material = "^8.1.3"
 PyYAML = "^6.0"
 types-PyYAML = "^6.0.1"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 Jinja2 = "3.0.3"
 mkdocs-awesome-pages-plugin = "^2.8.0"
 
+[tool.poetry.scripts]
+cli = "cli:command"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `arc_cli-8.0.0/setup.py` & `arc_cli-8.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['arc',
- 'arc.core',
- 'arc.core.middleware',
- 'arc.core.param',
+ 'arc.define',
+ 'arc.define.param',
  'arc.present',
+ 'arc.present.markdown',
  'arc.prompt',
- 'arc.types']
+ 'arc.runtime',
+ 'arc.types',
+ 'arc.types.middleware']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['hypothesis>=6.68.2,<7.0.0']
+
+entry_points = \
+{'console_scripts': ['cli = cli:command']}
+
 setup_kwargs = {
     'name': 'arc-cli',
-    'version': '8.0.0',
+    'version': '8.1.0',
     'description': 'A Regular CLI',
-    'long_description': '# ARC: A Regular CLI\nA tool for building declartive, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Dynamic command loading at runtime\n\n# [Docs](http://arc.seanrcollings.com)\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command()\ndef hello(name: str):\n    """My first arc program!"""\n    arc.arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
+    'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# [Docs](http://arc.seanrcollings.com)\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/arc',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `arc_cli-8.0.0/PKG-INFO` & `arc_cli-8.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 Metadata-Version: 2.1
 Name: arc-cli
-Version: 8.0.0
+Version: 8.1.0
 Summary: A Regular CLI
 Home-page: https://github.com/seanrcollings/arc
 License: MIT
 Keywords: CLI,extendable,easy,arc
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: hypothesis (>=6.68.2,<7.0.0)
 Project-URL: Documentation, https://arc.seanrcollings.com
 Description-Content-Type: text/markdown
 
 # ARC: A Regular CLI
-A tool for building declartive, and highly extendable CLI systems for Python 3.9
+A tool for building declarative, and highly extendable CLI systems for Python 3.9
 
 # ARC Features
 - Command line arguments based on python type hints
 - Arbitrary command nesting
 - Automatic `--help` documentation
-- Dynamic command loading at runtime
+- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...
 
 # [Docs](http://arc.seanrcollings.com)
 
 # Quick Start
 
 ```py
 import arc
 
-@arc.command()
+@arc.command
 def hello(name: str):
     """My first arc program!"""
     arc.arc.print(f"Hello {name}!")
 
 hello()
 ```
 
 ```
 $ python hello.py Sean
 Hello, Sean!
 ```
 
 ```
+$ python hello.py --help
 USAGE
     hello.py [-h] [--] name
 
 DESCRIPTION
     My first arc program!
 
 ARGUMENTS
```

