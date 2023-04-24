# Comparing `tmp/pocketrockit-0.0.1.tar.gz` & `tmp/pocketrockit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketrockit-0.0.1.tar", max compression
+gzip compressed data, was "pocketrockit-0.0.2.tar", max compression
```

## Comparing `pocketrockit-0.0.1.tar` & `pocketrockit-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      806 2023-04-21 04:17:33.415420 pocketrockit-0.0.1/Readme.md
--rw-r--r--   0        0        0        0 2023-04-21 04:17:33.520420 pocketrockit-0.0.1/pocketrockit/__init__.py
--rwxr-xr-x   0        0        0      532 2023-04-23 12:22:42.315502 pocketrockit-0.0.1/pocketrockit/cli.py
--rwxr-xr-x   0        0        0    12204 2023-04-23 12:19:47.624394 pocketrockit-0.0.1/pocketrockit/decorated.py
--rwxr-xr-x   0        0        0     8401 2023-04-22 18:10:33.459355 pocketrockit-0.0.1/pocketrockit/engine.py
--rw-r--r--   0        0        0     1829 2023-04-23 12:24:06.385553 pocketrockit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 pocketrockit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2636 2023-04-24 06:19:57.288246 pocketrockit-0.0.2/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-21 04:17:33.520420 pocketrockit-0.0.2/pocketrockit/__init__.py
+-rwxr-xr-x   0        0        0      532 2023-04-23 12:22:42.315502 pocketrockit-0.0.2/pocketrockit/cli.py
+-rwxr-xr-x   0        0        0    10698 2023-04-24 06:09:42.435969 pocketrockit-0.0.2/pocketrockit/decorated.py
+-rwxr-xr-x   0        0        0     8253 2023-04-24 06:09:42.407969 pocketrockit-0.0.2/pocketrockit/engine.py
+-rw-r--r--   0        0        0     1868 2023-04-24 06:22:20.691311 pocketrockit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 pocketrockit-0.0.2/PKG-INFO
```

### Comparing `pocketrockit-0.0.1/pocketrockit/cli.py` & `pocketrockit-0.0.2/pocketrockit/cli.py`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.1/pocketrockit/engine.py` & `pocketrockit-0.0.2/pocketrockit/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,21 @@
     """
     Todo: make behave like subprocess
     """
     try:
         midi_out = fluidsynth.Synth(gain=2.0, samplerate=44100.0)
         midi_out.setting("audio.period-size", 256)
         midi_out.start(driver="pulseaudio")
-        midi_out.program_select(0, midi_out.sfload("FluidR3_GM.sf2"), 0, 0)
-        midi_out.program_select(1, midi_out.sfload("JV_1080_Drums.sf2"), 128, 0)
+        fluid = midi_out.sfload("FluidR3_GM.sf2")
+        for i in range(128):
+            # 24 harp
+
+            midi_out.program_select(i, fluid, 0, i)
+        # midi_out.program_select(2, fluid, 0, 38)
+        midi_out.program_select(128, midi_out.sfload("JV_1080_Drums.sf2"), 128, 0)
         yield midi_out
     finally:
         midi_out.delete()
 
 
 def pygame_thread_fn(loop, event_queue, terminator):
     """Pygame thread"""
@@ -117,20 +122,14 @@
     try:
         while not terminator.is_set():
             try:
                 event = await event_queue.get()
                 if event.type in {pygame.WINDOWCLOSE, pygame.QUIT}:
                     logger().debug("quit/windowclose")
                     terminate(terminator)
-                #        elif event.type == pygame.KEYDOWN:
-                #            if event.key == pygame.K_SPACE:
-                #                if ball.speed == [0, 0]:
-                #                    ball.speed = [2, 2]
-                #                else:
-                #                    ball.speed = [0, 0]
                 elif event.type == pygame.MOUSEMOTION:
                     pass
                 elif event.type == pygame.TEXTINPUT:
                     pass
                 elif event.type == pygame.KEYDOWN:
                     pass
                 elif event.type == pygame.KEYUP:
@@ -215,15 +214,16 @@
                     print(f"exception in play: {exc}")
                     print("--")
 
             for note in notes:
                 midi_out.noteon(*note)
 
             # make me absolute please
-            await sleep(0.2)
+            waitfor = 60 / singleton.env.bpm / 4
+            await sleep(waitfor)
 
 
 async def watch_changes(filepath):
     load_module(filepath)
     with Inotify() as inotify:
         inotify.add_watch(
             Path(filepath).parent,
```

### Comparing `pocketrockit-0.0.1/pyproject.toml` & `pocketrockit-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "pocketrockit"
-version = "0.0.1"
+version = "0.0.2"
 description = "pocketrockit"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/pocketrockit.git"
 readme = "Readme.md"
 packages = [
   {include = "pocketrockit"}
 ]
 
 [tool.poetry.scripts]
 pri = 'pocketrockit.cli:main'
+pocketrockit = 'pocketrockit.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pygame = "^2.1.2"
 pyfluidsynth = "^1.3.1"
 asyncinotify = "^4.0.1"
 #mido = "^1.2.10"
```

