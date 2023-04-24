# Comparing `tmp/perfect-physics-0.1.0.tar.gz` & `tmp/perfect-physics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfect-physics-0.1.0.tar", last modified: Mon Apr 24 01:48:29 2023, max compression
+gzip compressed data, was "perfect-physics-0.1.1.tar", last modified: Mon Apr 24 02:06:11 2023, max compression
```

## Comparing `perfect-physics-0.1.0.tar` & `perfect-physics-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:48:29.647286 perfect-physics-0.1.0/
--rw-rw-rw-   0        0        0     1493 2023-04-24 01:48:29.647286 perfect-physics-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2023-04-03 19:59:56.000000 perfect-physics-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 01:48:29.633274 perfect-physics-0.1.0/perfect_physics/
--rw-rw-rw-   0        0        0      319 2022-11-22 03:19:01.000000 perfect-physics-0.1.0/perfect_physics/__init__.py
--rw-rw-rw-   0        0        0     1959 2023-04-18 15:33:42.000000 perfect-physics-0.1.0/perfect_physics/_circle.py
--rw-rw-rw-   0        0        0     2863 2023-04-20 02:11:51.000000 perfect-physics-0.1.0/perfect_physics/_misc.py
--rw-rw-rw-   0        0        0    14500 2023-04-03 19:53:02.000000 perfect-physics-0.1.0/perfect_physics/_physics.py
--rw-rw-rw-   0        0        0     3339 2022-11-22 03:19:01.000000 perfect-physics-0.1.0/perfect_physics/_timeline.py
--rw-rw-rw-   0        0        0      904 2022-11-18 02:58:40.000000 perfect-physics-0.1.0/perfect_physics/_wall.py
--rw-rw-rw-   0        0        0    26345 2023-04-20 02:09:31.000000 perfect-physics-0.1.0/perfect_physics/_world.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:48:29.646286 perfect-physics-0.1.0/perfect_physics.egg-info/
--rw-rw-rw-   0        0        0     1493 2023-04-24 01:48:29.000000 perfect-physics-0.1.0/perfect_physics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-04-24 01:48:29.000000 perfect-physics-0.1.0/perfect_physics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:48:29.000000 perfect-physics-0.1.0/perfect_physics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-24 01:48:29.000000 perfect-physics-0.1.0/perfect_physics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-24 01:48:29.000000 perfect-physics-0.1.0/perfect_physics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       32 2022-11-21 03:08:34.000000 perfect-physics-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 01:48:29.648285 perfect-physics-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-04-24 01:47:47.000000 perfect-physics-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:06:11.809829 perfect-physics-0.1.1/
+-rw-rw-rw-   0        0        0     1493 2023-04-24 02:06:11.809829 perfect-physics-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2023-04-03 19:59:56.000000 perfect-physics-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 02:06:11.799825 perfect-physics-0.1.1/perfect_physics/
+-rw-rw-rw-   0        0        0      319 2022-11-22 03:19:01.000000 perfect-physics-0.1.1/perfect_physics/__init__.py
+-rw-rw-rw-   0        0        0     1959 2023-04-18 15:33:42.000000 perfect-physics-0.1.1/perfect_physics/_circle.py
+-rw-rw-rw-   0        0        0     2863 2023-04-20 02:11:51.000000 perfect-physics-0.1.1/perfect_physics/_misc.py
+-rw-rw-rw-   0        0        0    14665 2023-04-24 02:04:31.000000 perfect-physics-0.1.1/perfect_physics/_physics.py
+-rw-rw-rw-   0        0        0     3339 2022-11-22 03:19:01.000000 perfect-physics-0.1.1/perfect_physics/_timeline.py
+-rw-rw-rw-   0        0        0      904 2022-11-18 02:58:40.000000 perfect-physics-0.1.1/perfect_physics/_wall.py
+-rw-rw-rw-   0        0        0    26522 2023-04-24 02:04:30.000000 perfect-physics-0.1.1/perfect_physics/_world.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:06:11.808829 perfect-physics-0.1.1/perfect_physics.egg-info/
+-rw-rw-rw-   0        0        0     1493 2023-04-24 02:06:11.000000 perfect-physics-0.1.1/perfect_physics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-04-24 02:06:11.000000 perfect-physics-0.1.1/perfect_physics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 02:06:11.000000 perfect-physics-0.1.1/perfect_physics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-24 02:06:11.000000 perfect-physics-0.1.1/perfect_physics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-24 02:06:11.000000 perfect-physics-0.1.1/perfect_physics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       32 2022-11-21 03:08:34.000000 perfect-physics-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 02:06:11.810830 perfect-physics-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-04-24 02:04:56.000000 perfect-physics-0.1.1/setup.py
```

### Comparing `perfect-physics-0.1.0/PKG-INFO` & `perfect-physics-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-physics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Perfect Physics
 Home-page: https://towardsdatascience.com/perfect-infinite-precision-game-physics-in-python-part-1-698211c08d95
 Author: Carl Kadie
 License: MIT or Apache-2.0
 Description-Content-Type: text/markdown
 
 Perfect Physics
```

### Comparing `perfect-physics-0.1.0/README.md` & `perfect-physics-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `perfect-physics-0.1.0/perfect_physics/_circle.py` & `perfect-physics-0.1.1/perfect_physics/_circle.py`

 * *Files identical despite different names*

### Comparing `perfect-physics-0.1.0/perfect_physics/_misc.py` & `perfect-physics-0.1.1/perfect_physics/_misc.py`

 * *Files identical despite different names*

### Comparing `perfect-physics-0.1.0/perfect_physics/_physics.py` & `perfect-physics-0.1.1/perfect_physics/_physics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import logging
 from pathlib import Path
 from typing import Any, List
 
 import numpy as np
-from pysnptools.util.mapreduce1 import map_reduce
+
+try:
+    from pysnptools.util.mapreduce1 import map_reduce
+except ImportError:
+
+    def map_reduce(input_seq, mapper, runner=None):
+        return [mapper(item) for item in input_seq]
+
+
 from sympy import S, im, oo, simplify
 
 from ._circle import Circle
 from ._misc import load
 from ._timeline import Collision, Move, MultipleCollisions
 from ._wall import Wall
 
@@ -73,15 +81,14 @@
                 "y_1": w.y1,
             }
         )
 
         return speed
 
     def _circle_circle_spans(self, a: Circle, b: Circle):
-
         result_list = [
             time_solution.subs(
                 [
                     ("a_x", a.x),
                     ("a_y", a.y),
                     ("a_r", a.r),
                     ("a_vx", a.vx),
@@ -121,15 +128,14 @@
             return self._circle_circle_spans(a, b)
         elif isinstance(b, Wall):
             return self._circle_wall_spans(a, b)
         else:
             raise TypeError("2nd object must be a circle or a wall")
 
     def _circle_circle_velocities(self, a: Circle, b: Circle):
-
         result_list = self._circle_circle_bounce.subs(
             [
                 ("a_x", a.x),
                 ("a_y", a.y),
                 ("a_r", a.r),
                 ("a_vx", a.vx),
                 ("a_vy", a.vy),
@@ -277,15 +283,17 @@
                 ):
                     continue
                 pairs.append((circle, any))
         logging.info(
             f"Looking at {len(pairs)} pairs out of {Physics._combo_count(circle_list, wall_list)} possible pairs"  # noqa E501
         )
 
-        ssca_list = map_reduce(pairs, lambda pair: self._find_span(*pair), runner=runner)
+        ssca_list = map_reduce(
+            pairs, lambda pair: self._find_span(*pair), runner=runner
+        )
         logging.debug("About to _fix_ssca")
         ssca_list = [
             Physics._fix_ssca(ssca, circle_list, wall_list) for ssca in ssca_list
         ] + hint_ssca_list
         logging.debug("About to sort ssa_list on floats")
         ssca_list.sort(key=lambda x: x[1])
         return ssca_list
```

### Comparing `perfect-physics-0.1.0/perfect_physics/_timeline.py` & `perfect-physics-0.1.1/perfect_physics/_timeline.py`

 * *Files identical despite different names*

### Comparing `perfect-physics-0.1.0/perfect_physics/_wall.py` & `perfect-physics-0.1.1/perfect_physics/_wall.py`

 * *Files identical despite different names*

### Comparing `perfect-physics-0.1.0/perfect_physics/_world.py` & `perfect-physics-0.1.1/perfect_physics/_world.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 
 import cloudpickle as pickle
 import cv2
 import numpy as np
 from moviepy.audio.io.AudioFileClip import AudioFileClip
 from moviepy.video.io.VideoFileClip import VideoFileClip
 from pydub import AudioSegment
-from pysnptools.util.mapreduce1 import map_reduce
+
+try:
+    from pysnptools.util.mapreduce1 import map_reduce
+except ImportError:
+
+    def map_reduce(input_seq, mapper, runner=None):
+        return [mapper(item) for item in input_seq]
+
+
 from sympy import Rational, S, simplify, pi, cos, sin
 
 from ._circle import Circle
 from ._misc import plot
 from ._physics import Physics
 from ._timeline import Timeline, TimeNow, TimeReset, Reverse, billiards_audio
 from ._wall import Wall
@@ -300,15 +308,17 @@
 
         if abs(rows) > 1:
             r0 = (
                 r + 0
                 if jitter is None
                 else rng.randint(jitter[0], jitter[1] - 1) * jitter[2]
             )
-            b0 = Circle(x=Rational(length * 3 / 4), y=hw, r=r0, vx=0, vy=0, m=1, id="b1")
+            b0 = Circle(
+                x=Rational(length * 3 / 4), y=hw, r=r0, vx=0, vy=0, m=1, id="b1"
+            )
             world.circle_list.append(b0)
 
         if abs(rows) >= 2:
             place_ball(hw, 1, id="b2")
             place_ball(hw, -1, id="b3")
 
         if abs(rows) >= 3:
```

### Comparing `perfect-physics-0.1.0/perfect_physics.egg-info/PKG-INFO` & `perfect-physics-0.1.1/perfect_physics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-physics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Perfect Physics
 Home-page: https://towardsdatascience.com/perfect-infinite-precision-game-physics-in-python-part-1-698211c08d95
 Author: Carl Kadie
 License: MIT or Apache-2.0
 Description-Content-Type: text/markdown
 
 Perfect Physics
```

### Comparing `perfect-physics-0.1.0/setup.py` & `perfect-physics-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 # Version number
-version = "0.1.0"
+version = "0.1.1"
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
```

