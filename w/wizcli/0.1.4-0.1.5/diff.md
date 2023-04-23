# Comparing `tmp/wizcli-0.1.4.tar.gz` & `tmp/wizcli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizcli-0.1.4.tar", max compression
+gzip compressed data, was "wizcli-0.1.5.tar", max compression
```

## Comparing `wizcli-0.1.4.tar` & `wizcli-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      247 2023-04-22 05:19:10.102030 wizcli-0.1.4/README.md
--rw-r--r--   0        0        0      327 2023-04-23 17:21:18.962177 wizcli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2233 2023-04-23 17:21:08.316888 wizcli-0.1.4/wizcli/cli.py
--rw-r--r--   0        0        0     2444 2023-04-23 17:17:48.394456 wizcli-0.1.4/wizcli/wiz.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 wizcli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      281 2023-04-23 23:26:05.956812 wizcli-0.1.5/README.md
+-rw-r--r--   0        0        0      530 2023-04-23 23:26:05.956812 wizcli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2332 2023-04-23 23:26:05.956812 wizcli-0.1.5/wizcli/cli.py
+-rw-r--r--   0        0        0     2392 2023-04-23 23:26:05.956812 wizcli-0.1.5/wizcli/wiz.py
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 wizcli-0.1.5/PKG-INFO
```

### Comparing `wizcli-0.1.4/wizcli/cli.py` & `wizcli-0.1.5/wizcli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import sys
 import math
-from dataclasses import dataclass
+import json
 import logging
+from dataclasses import dataclass
 
 import typer
 from .wiz import Wiz
 
 run = typer.Typer()
 logger = logging.getLogger(__name__)
 
@@ -54,15 +56,15 @@
 
 
 @run.command()
 def dim(
     ctx: typer.Context,
     value: int = typer.Argument(50, min=0, max=100, help="%"),
 ):
-    value = math.floor(value / 100 * 255)
+    value = max(10, value)
     ctx.obj.wiz.set_brightness(value)
 
 
 @run.command()
 def temp(
     ctx: typer.Context,
     value: int = typer.Argument(50, min=0, max=100, help="%"),
@@ -95,9 +97,13 @@
     r: int = typer.Argument(0, min=0, max=255),
     g: int = typer.Argument(0, min=0, max=255),
     b: int = typer.Argument(0, min=0, max=255),
 ):
     ctx.obj.wiz.set_color((r, g, b))
 
 
-if __name__ == "__main__":
-    run()
+@run.command()
+def get(
+    ctx: typer.Context
+):
+    state = ctx.obj.wiz.get_state()
+    json.dump(state, sys.stdout, indent=2)
```

### Comparing `wizcli-0.1.4/wizcli/wiz.py` & `wizcli-0.1.5/wizcli/wiz.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,23 +30,22 @@
         addr = (self.host, self.port)
 
         logger.debug(f" > {pformat(payload)}")
         self.socket.sendto(body.encode("utf8"), addr)
 
         try:
             content, _ = self.socket.recvfrom(4096)
+            response = json.loads(content)
+            logger.debug(f" < {pformat(response)}")
+
+            return response
         except socket.timeout as e:
             logger.error("wiz bulb timeout")
             raise e
 
-        response = json.loads(content)
-        logger.debug(f" < {pformat(response)}")
-
-        return response
-
     def get_state(self) -> dict:
         return self._send({"method": "getPilot"}).get("result")
 
     def on(self):
         return self._send({"method": "setPilot", "params": {"state": True}})
 
     def off(self):
@@ -70,15 +69,12 @@
 
     def push_state(self):
         """push state to the queue"""
         state = self.get_state()
         self._states.append(state)
 
     def pop_state(self):
-        try:
-            state = self._states.pop()
-        except IndexError:
-            return
+        state = self._states.pop()
         return self._send({
             "method": "setPilot",
             "params": {k: v for k, v in state.items() if k in self.STATE_FIELDS}
         })
```

### Comparing `wizcli-0.1.4/PKG-INFO` & `wizcli-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: wizcli
-Version: 0.1.4
-Summary: wiz cli
+Version: 0.1.5
+Summary: control WiZ bulbs from the CLI
+Home-page: https://github.com/redraw/wizcli
 Author: Agustin B
 Author-email: redraw@sdf.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typer (>=0.7.0,<0.8.0)
+Project-URL: Repository, https://github.com/redraw/wizcli
 Description-Content-Type: text/markdown
 
 # wizcli
 
-Control your WiZ light from the terminal.
+Control your WiZ light from the CLI.
+
+## Install
+
+```bash
+pip install wizcli
+```
+## Use
 
 ```bash
 # turn on
-$ wiz on
+wiz on
 
 # turn off
-$ wiz off
+wiz off
 
 # dim to 20%
-$ wiz dim 20
+wiz dim 20
 
 # set temp to 50%
-$ wiz temp 50
+wiz temp 50
 
 # set cold
-$ wiz cold
+wiz cold
 
-# set hot
-$ wiz hot
+# set warm
+wiz warm
 
 # set RGB color
-$ wiz rgb 255 40 90
+wiz rgb 255 40 90
 ```
```

