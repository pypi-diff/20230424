# Comparing `tmp/evidence_ext-0.5.2.tar.gz` & `tmp/evidence_ext-0.5.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evidence_ext-0.5.2.tar", max compression
+gzip compressed data, was "evidence_ext-0.5.2a1.tar", max compression
```

## Comparing `evidence_ext-0.5.2.tar` & `evidence_ext-0.5.2a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1623 2023-04-24 14:48:16.946415 evidence_ext-0.5.2/README.md
--rw-r--r--   0        0        0       34 2023-04-24 14:48:16.946415 evidence_ext-0.5.2/evidence_ext/__init__.py
--rw-r--r--   0        0        0     5240 2023-04-24 14:48:16.946415 evidence_ext-0.5.2/evidence_ext/config.py
--rw-r--r--   0        0        0     4337 2023-04-24 14:48:16.946415 evidence_ext-0.5.2/evidence_ext/extension.py
--rw-r--r--   0        0        0     4011 2023-04-24 14:48:16.946415 evidence_ext-0.5.2/evidence_ext/main.py
--rw-r--r--   0        0        0     1266 2023-04-24 14:48:34.674589 evidence_ext-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 evidence_ext-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1623 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/README.md
+-rw-r--r--   0        0        0       34 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/__init__.py
+-rw-r--r--   0        0        0     5240 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/config.py
+-rw-r--r--   0        0        0     4337 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/extension.py
+-rw-r--r--   0        0        0     3949 2023-04-17 21:09:01.311210 evidence_ext-0.5.2a1/evidence_ext/main.py
+-rw-r--r--   0        0        0     1446 2023-04-17 21:09:24.167569 evidence_ext-0.5.2a1/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 evidence_ext-0.5.2a1/PKG-INFO
```

### Comparing `evidence_ext-0.5.2/README.md` & `evidence_ext-0.5.2a1/README.md`

 * *Files identical despite different names*

### Comparing `evidence_ext-0.5.2/evidence_ext/config.py` & `evidence_ext-0.5.2a1/evidence_ext/config.py`

 * *Files identical despite different names*

### Comparing `evidence_ext-0.5.2/evidence_ext/extension.py` & `evidence_ext-0.5.2a1/evidence_ext/extension.py`

 * *Files identical despite different names*

### Comparing `evidence_ext-0.5.2/evidence_ext/main.py` & `evidence_ext-0.5.2a1/evidence_ext/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Evidence cli entrypoint."""
 
 from __future__ import annotations
 
 import os
 import sys
-import typing as t
 
 import structlog
 import typer
 from meltano.edk.extension import DescribeFormat
 from meltano.edk.logging import default_logging_config, parse_log_level
 
 from evidence_ext.extension import Evidence
@@ -84,15 +83,15 @@
         )
         sys.exit(1)
 
 
 @app.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
 )
-def invoke(ctx: typer.Context, command_args: t.List[str]) -> None:  # noqa: ARG001
+def invoke(ctx: typer.Context, command_args: list[str]) -> None:  # noqa: ARG001
     """Invoke the plugin.
 
     Note: that if a command argument is a list, such as command_args,
     then unknown options are also included in the list and NOT stored in the
     context as usual.
     """
     command_name, command_args = command_args[0], command_args[1:]
@@ -122,15 +121,15 @@
         )
         sys.exit(1)
 
 
 @app.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
 )
-def npm(ctx: typer.Context, command_args: t.List[str]) -> None:  # noqa: ARG001
+def npm(ctx: typer.Context, command_args: list[str]) -> None:  # noqa: ARG001
     """Run npm commands inside the Evidence project directory."""
     ext.npm(*command_args)
 
 
 @app.command()
 def build(
     ctx: typer.Context,  # noqa: ARG001
@@ -145,11 +144,7 @@
     ext.build(strict=strict)
 
 
 @app.command()
 def dev(ctx: typer.Context) -> None:  # noqa: ARG001
     """Launch the Evidence dev server."""
     ext.dev()
-
-
-if __name__ == "__main__":
-    app()
```

### Comparing `evidence_ext-0.5.2/PKG-INFO` & `evidence_ext-0.5.2a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: evidence-ext
-Version: 0.5.2
+Version: 0.5.2a1
 Summary: `evidence-ext` is a Meltano utility extension.
 License: Apache 2.0
-Author: Meltano
-Author-email: hello@meltano.com
+Author: Ken Payne
 Requires-Python: >=3.7,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

