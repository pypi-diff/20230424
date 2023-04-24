# Comparing `tmp/pocketrockit-0.0.3.tar.gz` & `tmp/pocketrockit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketrockit-0.0.3.tar", max compression
+gzip compressed data, was "pocketrockit-0.0.4.tar", max compression
```

## Comparing `pocketrockit-0.0.3.tar` & `pocketrockit-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2636 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/Readme.md
--rw-r--r--   0        0        0        0 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/pocketrockit/__init__.py
--rwxr-xr-x   0        0        0      532 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/pocketrockit/cli.py
--rwxr-xr-x   0        0        0    10829 2023-04-24 08:05:55.081996 pocketrockit-0.0.3/pocketrockit/decorated.py
--rwxr-xr-x   0        0        0     8253 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/pocketrockit/engine.py
--rw-r--r--   0        0        0     1868 2023-04-24 08:08:10.873576 pocketrockit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 pocketrockit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2636 2023-04-24 06:41:37.681837 pocketrockit-0.0.4/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-24 06:41:37.681837 pocketrockit-0.0.4/pocketrockit/__init__.py
+-rwxr-xr-x   0        0        0     1001 2023-04-24 08:54:19.945411 pocketrockit-0.0.4/pocketrockit/cli.py
+-rwxr-xr-x   0        0        0    10829 2023-04-24 08:05:55.081996 pocketrockit-0.0.4/pocketrockit/decorated.py
+-rwxr-xr-x   0        0        0     8272 2023-04-24 09:13:17.669566 pocketrockit-0.0.4/pocketrockit/engine.py
+-rw-r--r--   0        0        0     1892 2023-04-24 09:11:14.225621 pocketrockit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 pocketrockit-0.0.4/PKG-INFO
```

### Comparing `pocketrockit-0.0.3/Readme.md` & `pocketrockit-0.0.4/Readme.md`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.3/pocketrockit/decorated.py` & `pocketrockit-0.0.4/pocketrockit/decorated.py`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.3/pocketrockit/engine.py` & `pocketrockit-0.0.4/pocketrockit/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,37 +88,37 @@
 def choose(choices: Iterable[str], *wishlist: str) -> str:
     for wish in wishlist:
         with suppress(StopIteration):
             return next(name for name in choices if wish in name)
     raise KeyError(f"{wishlist}")
 
 
-def read_midi(loop, event_queue, terminator):
-    logger().debug(">> read_midi")
+#def read_midi(loop, event_queue, terminator):
+    #logger().debug(">> read_midi")
 
-    try:
-        available_input_ports = set(mido.get_input_names())
-        logger().info("Available MIDI input ports: \n%s", "  \n".join(available_input_ports))
-
-        chosen_input = choose(
-            available_input_ports, "OP-1", "Sylphyo", "USB MIDI Interface", "Midi Through"
-        )
-        logger().info("Chosen: %r", chosen_input)
-
-        with mido.open_input(chosen_input) as inport:
-            while not terminator.is_set():
-                if (event := inport.receive()).type == "clock":
-                    continue
-                asyncio.run_coroutine_threadsafe(event_queue.put(event), loop=loop)
-            logger().debug("read_midi: got termination signal")
+    #try:
+        #available_input_ports = set(mido.get_input_names())
+        #logger().info("Available MIDI input ports: \n%s", "  \n".join(available_input_ports))
+
+        #chosen_input = choose(
+            #available_input_ports, "OP-1", "Sylphyo", "USB MIDI Interface", "Midi Through"
+        #)
+        #logger().info("Chosen: %r", chosen_input)
+
+        #with mido.open_input(chosen_input) as inport:
+            #while not terminator.is_set():
+                #if (event := inport.receive()).type == "clock":
+                    #continue
+                #asyncio.run_coroutine_threadsafe(event_queue.put(event), loop=loop)
+            #logger().debug("read_midi: got termination signal")
 
-    except Exception as exc:
-        logger().error("Unhandled exception in read_midi thread: %s", exc)
+    #except Exception as exc:
+        #logger().error("Unhandled exception in read_midi thread: %s", exc)
 
-    logger().debug("<< read_midi")
+    #logger().debug("<< read_midi")
 
 
 async def handle_events(event_queue, task, terminator):
     logger().debug(">> handle_events")
     try:
         while not terminator.is_set():
             try:
@@ -245,15 +245,15 @@
     asyncio.set_event_loop(loop)
     terminator = threading.Event()
 
     with ExitStack() as context:
         # context.enter_context(setup_midi(event_queue))
         pool = context.enter_context(concurrent.futures.ThreadPoolExecutor())
 
-        midi_reader = loop.run_in_executor(pool, read_midi, loop, event_queue, terminator)
+        #midi_reader = loop.run_in_executor(pool, read_midi, loop, event_queue, terminator)
         pygame_task = (
             None  # loop.run_in_executor(pool, pygame_thread_fn, loop, event_queue, terminator)
         )
         event_task = asyncio.ensure_future(handle_events(event_queue, pygame_task, terminator))
         asyncio.ensure_future(tick(singleton))
         asyncio.ensure_future(watch_changes(singleton.file_to_track))
```

### Comparing `pocketrockit-0.0.3/pyproject.toml` & `pocketrockit-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "pocketrockit"
-version = "0.0.3"
+version = "0.0.4"
 description = "pocketrockit"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/pocketrockit.git"
 readme = "Readme.md"
 packages = [
   {include = "pocketrockit"}
 ]
 
 [tool.poetry.scripts]
 pri = 'pocketrockit.cli:main'
 pocketrockit = 'pocketrockit.cli:main'
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 pygame = "^2.1.2"
 pyfluidsynth = "^1.3.1"
 asyncinotify = "^4.0.1"
 #mido = "^1.2.10"
 #python-rtmidi = "^1.4.9"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
-mypy = "^0.961"
+mypy = "^0.991"
 pylint = "^2.15.3"
 ipython = "^8.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
@@ -52,14 +52,15 @@
   ))
 '''
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
+python_version = "3.11"
 strict="True"
 disallow_untyped_defs = "True"
 disallow_any_unimported = "True"
 no_implicit_optional = "True"
 check_untyped_defs = "True"
 warn_return_any = "True"
 warn_unused_ignores = "True"
```

### Comparing `pocketrockit-0.0.3/PKG-INFO` & `pocketrockit-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pocketrockit
-Version: 0.0.3
+Version: 0.0.4
 Summary: pocketrockit
 Home-page: https://projects.om-office.de/frans/pocketrockit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncinotify (>=4.0.1,<5.0.0)
 Requires-Dist: pyfluidsynth (>=1.3.1,<2.0.0)
 Requires-Dist: pygame (>=2.1.2,<3.0.0)
 Project-URL: Repository, https://projects.om-office.de/frans/pocketrockit.git
 Description-Content-Type: text/markdown
```

