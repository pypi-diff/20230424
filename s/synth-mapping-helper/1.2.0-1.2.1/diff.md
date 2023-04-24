# Comparing `tmp/synth_mapping_helper-1.2.0.tar.gz` & `tmp/synth_mapping_helper-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.2.0.tar", last modified: Tue Apr 11 19:53:00 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.2.1.tar", last modified: Mon Apr 24 21:32:41 2023, max compression
```

## Comparing `synth_mapping_helper-1.2.0.tar` & `synth_mapping_helper-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.750025 synth_mapping_helper-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.754025 synth_mapping_helper-1.2.0/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25631 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27963 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 19:53:00.000000 synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:53:00.758025 synth_mapping_helper-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 19:52:48.000000 synth_mapping_helper-1.2.0/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.056683 synth_mapping_helper-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27963 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 21:32:41.000000 synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:32:41.060683 synth_mapping_helper-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 21:32:30.000000 synth_mapping_helper-1.2.1/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.2.0/LICENSE` & `synth_mapping_helper-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/PKG-INFO` & `synth_mapping_helper-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.0/README.md` & `synth_mapping_helper-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/setup.py` & `synth_mapping_helper-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     movement_group.add_argument("--offset-random", type=utils.parse_xy_range, metavar="[MIN_X:]MAX_X,[MIN_Y:]MAX_Y", help="Offset by a random amount in the X and Y axis. When no MIN is given, uses negative MAX.")
 
     movement_group.add_argument("-c", "--stack-count", type=int, help="Instead of moving, create copies. Must have time offset set.")
     movement_group.add_argument("--stack-duration", type=utils.parse_time, help="Like --stack-count, but you can give it during in beats ('4') or seconds ('2s').")
     movement_group.add_argument("--autostack", nargs="?", choices=("OFFSET", "SPIRAL", "OUTSET", "SCALE"), action="append", metavar="OFFSET/SPIRAL/OUTSET/SCALE", help="Find the first pair of matching objects and continue the pattern. For continuing the positions, the following modes are supported: OFFSET (default, absolute xy), SPIRAL (rotate around implied pivot), OUTSET (distance from pivot) and SCALE (xy ratio).")
 
     postproc_group = parser.add_argument_group("post-processing")
+    postproc_group.add_argument("--parallels", type=utils.parse_number, metavar="DISTANCE", help="Create parallel left/right handed patterns with given spacing from input. Negative numbers result in crossovers.")
     postproc_group.add_argument("--split-rails", action="store_true", help="Split rails at single notes")
     postproc_group.add_argument("--rails-to-singles", type=int, nargs="?", action="append", metavar="KEEP_RAIL", help="Replace rails with single notes at all nodes. KEEP_RAIL is optional and can be '1' if you want to keep the rail instead of replacing it")
     postproc_group.add_argument("--keep-alignment", action="store_true", help="Do NOT shift the start of selection to first element")
 
     return parser
 
 def abort(reason: str):
@@ -161,26 +162,28 @@
             abort(f"Could not find any {options.note_pivot} notes")
         options.pivot = notes[sorted(notes)[0]][:3]
 
     # stacking
     if options.autostack is not None:
         if not options.stack_count and not options.stack_duration:
             abort("Cannot --autostack without count/duration")
+        obj_type = None
         first = None
         second = None
-        for t in synth_format.ALL_TYPES:
+        for t in synth_format.ALL_TYPES[::-1]:  # start with walls (for SPIRAL mode)
             obj_dict = data.get_object_dict(t)
             if len(obj_dict) >= 2:
                 it = iter(sorted(obj_dict.items()))
                 _, t_first = next(it)
                 if first is None or t_first[0,2] < first[0,2]:
                     first = t_first[0]  # rail head only
                     _, t_second = next(it)
                     second = t_second[0]
-        if first is None or second is None:
+                    obj_type = t
+        if first is None:
             abort("Could not find object pair for autostack")
 
         if options.autostack[0] == "SPIRAL":
             if first.shape[0] != 5:
                 abort("Can only spiral-autostack based on walls")
             # rotation from point 'a' to point 'b', around pivot 'p' by angle 'ang':
             #   x_b = (x_a - x_p) * cos(ang) - (y_a - y_p) * sin(ang) + x_p
@@ -208,14 +211,20 @@
             elif options.autostack[0] == "SCALE":
                 options.scale = (second[0] / first[0], second[1] / first[1], 1)
                 options.offset = (0, 0, second[2] - first[2])
 
             if first.shape[0] == 5:
                 options.wall_rotate = ((second[4] - first[4]) - (options.rotate or 0)) or None  # see if we need to correct wall rotation
 
+        # remove second object so it doesn't get stacked
+        if obj_type in synth_format.NOTE_TYPES:
+            del getattr(data, obj_type)[second[2]]
+        else:
+            del data.walls[second[2]]
+
     if options.stack_duration:
         if options.stack_count:
             abort("Cannot use --stack-count and --stack-duration at the same time")
         options.stack_count = int(options.stack_duration / options.offset[2])
 
     if options.stack_count and (options.offset is None or not options.offset[2]):
         abort("Cannot stack with time offset of 0")
@@ -360,14 +369,32 @@
             abort("Cannot use offset-along or rotate-with without stacking")
         do_movement(options, data, filter_types=filter_types)
         if options.offset_random is not None:
             random_offset = pattern_generation.random_xy(1, options.offset_random[0], options.offset_random[1])[0]
             data.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0], mirror_left=options.mirror_left)
 
     # postprocessing
+    if options.parallels:
+        left_orig, right_orig = data.left, data.right  # create a backup of the input
+        data.left = (
+            left_orig
+            | {t: nodes - [options.parallels,0,0] for t, nodes in sorted(right_orig.items())}  # shift over right hand by <distance>
+            | {t: nodes - [options.parallels/2,0,0] for t, nodes in sorted(data.single.items())}  # shift over single & both by <distance>/2
+            | {t: nodes - [options.parallels/2,0,0] for t, nodes in sorted(data.both.items())}
+        )
+        # vice versa for right hand
+        data.right = (
+            right_orig 
+            | {t: nodes + [options.parallels,0,0] for t, nodes in sorted(left_orig.items())}
+            | {t: nodes + [options.parallels/2,0,0] for t, nodes in sorted(data.single.items())}
+            | {t: nodes + [options.parallels/2,0,0] for t, nodes in sorted(data.both.items())}
+        )
+        # wipe single & both
+        data.single = {}
+        data.both = {}
     if options.split_rails:
         data.apply_for_note_types(rails.split_rails, types=filter_types)
     if options.rails_to_singles:
         data.apply_for_note_types(rails.rails_to_singles, keep_rail=bool(options.rails_to_singles[0]), types=filter_types)
     synth_format.export_clipboard(data, not options.keep_alignment)
 
 if __name__ == "__main__":
```

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/companion.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/rails.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/synth_format.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.0/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.2.1/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

