# Comparing `tmp/perfect_physics-0.1.3-py3-none-any.whl.zip` & `tmp/perfect_physics-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,19 @@
-Zip file size: 14703 bytes, number of entries: 11
+Zip file size: 18646 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      319 b- defN 22-Nov-22 03:19 perfect_physics/__init__.py
 -rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-18 15:33 perfect_physics/_circle.py
 -rw-rw-rw-  2.0 fat     2863 b- defN 23-Apr-20 02:11 perfect_physics/_misc.py
 -rw-rw-rw-  2.0 fat    14665 b- defN 23-Apr-24 02:04 perfect_physics/_physics.py
 -rw-rw-rw-  2.0 fat     3341 b- defN 23-Apr-24 02:13 perfect_physics/_timeline.py
 -rw-rw-rw-  2.0 fat      904 b- defN 22-Nov-18 02:58 perfect_physics/_wall.py
--rw-rw-rw-  2.0 fat    26560 b- defN 23-Apr-24 02:24 perfect_physics/_world.py
--rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      910 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/RECORD
-11 files, 53193 bytes uncompressed, 13163 bytes compressed:  75.3%
+-rw-rw-rw-  2.0 fat    26580 b- defN 23-Apr-24 02:26 perfect_physics/_world.py
+-rw-rw-rw-  2.0 fat     9928 b- defN 22-Nov-09 15:59 perfect_physics-0.1.4.data/data/data/cc_time_solutions.sympy
+-rw-rw-rw-  2.0 fat     9148 b- defN 22-Nov-11 02:53 perfect_physics-0.1.4.data/data/data/cc_velocity_solution.sympy
+-rw-rw-rw-  2.0 fat     1505 b- defN 22-Nov-09 23:07 perfect_physics-0.1.4.data/data/data/cw_time_solutions.sympy
+-rw-rw-rw-  2.0 fat     1925 b- defN 22-Nov-11 18:01 perfect_physics-0.1.4.data/data/data/cw_velocity_limits.sympy
+-rw-rw-rw-  2.0 fat     5315 b- defN 22-Nov-12 15:43 perfect_physics-0.1.4.data/data/data/instant_speed.sympy
+-rw-rw-rw-  2.0 fat     6740 b- defN 22-Nov-12 15:45 perfect_physics-0.1.4.data/data/data/instant_speed_wall.sympy
+-rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 16:36 perfect_physics-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 16:36 perfect_physics-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 16:36 perfect_physics-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1613 b- defN 23-Apr-24 16:36 perfect_physics-0.1.4.dist-info/RECORD
+17 files, 88477 bytes uncompressed, 15928 bytes compressed:  82.0%
```

## zipnote {}

```diff
@@ -15,20 +15,38 @@
 
 Filename: perfect_physics/_wall.py
 Comment: 
 
 Filename: perfect_physics/_world.py
 Comment: 
 
-Filename: perfect_physics-0.1.3.dist-info/METADATA
+Filename: perfect_physics-0.1.4.data/data/data/cc_time_solutions.sympy
 Comment: 
 
-Filename: perfect_physics-0.1.3.dist-info/WHEEL
+Filename: perfect_physics-0.1.4.data/data/data/cc_velocity_solution.sympy
 Comment: 
 
-Filename: perfect_physics-0.1.3.dist-info/top_level.txt
+Filename: perfect_physics-0.1.4.data/data/data/cw_time_solutions.sympy
 Comment: 
 
-Filename: perfect_physics-0.1.3.dist-info/RECORD
+Filename: perfect_physics-0.1.4.data/data/data/cw_velocity_limits.sympy
+Comment: 
+
+Filename: perfect_physics-0.1.4.data/data/data/instant_speed.sympy
+Comment: 
+
+Filename: perfect_physics-0.1.4.data/data/data/instant_speed_wall.sympy
+Comment: 
+
+Filename: perfect_physics-0.1.4.dist-info/METADATA
+Comment: 
+
+Filename: perfect_physics-0.1.4.dist-info/WHEEL
+Comment: 
+
+Filename: perfect_physics-0.1.4.dist-info/top_level.txt
+Comment: 
+
+Filename: perfect_physics-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perfect_physics/_world.py

```diff
@@ -591,14 +591,15 @@
         slice=np.s_[:],
         talkie_codec="png",
         silent_codec="MJPG",
         prefix="",
         **kwargs,
     ):
         from pydub import AudioSegment
+        import cv2
 
         frames_per_half_event = seconds_per_event * fps / 2
         assert frames_per_half_event == int(
             frames_per_half_event
         ), "seconds_per_event * fps must be even"
 
         folder = Path(folder)
```

## Comparing `perfect_physics-0.1.3.dist-info/METADATA` & `perfect_physics-0.1.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-physics
-Version: 0.1.3
+Version: 0.1.4
 Summary: Perfect Physics
 Home-page: https://towardsdatascience.com/perfect-infinite-precision-game-physics-in-python-part-1-698211c08d95
 Author: Carl Kadie
 License: MIT or Apache-2.0
 Description-Content-Type: text/markdown
 Requires-Dist: sympy
 Requires-Dist: numpy
```

