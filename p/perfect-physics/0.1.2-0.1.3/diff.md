# Comparing `tmp/perfect_physics-0.1.2-py3-none-any.whl.zip` & `tmp/perfect_physics-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14700 bytes, number of entries: 11
+Zip file size: 14703 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      319 b- defN 22-Nov-22 03:19 perfect_physics/__init__.py
 -rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-18 15:33 perfect_physics/_circle.py
 -rw-rw-rw-  2.0 fat     2863 b- defN 23-Apr-20 02:11 perfect_physics/_misc.py
 -rw-rw-rw-  2.0 fat    14665 b- defN 23-Apr-24 02:04 perfect_physics/_physics.py
 -rw-rw-rw-  2.0 fat     3341 b- defN 23-Apr-24 02:13 perfect_physics/_timeline.py
 -rw-rw-rw-  2.0 fat      904 b- defN 22-Nov-18 02:58 perfect_physics/_wall.py
--rw-rw-rw-  2.0 fat    26550 b- defN 23-Apr-24 02:16 perfect_physics/_world.py
--rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 02:18 perfect_physics-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 02:18 perfect_physics-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 02:18 perfect_physics-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      910 b- defN 23-Apr-24 02:18 perfect_physics-0.1.2.dist-info/RECORD
-11 files, 53183 bytes uncompressed, 13160 bytes compressed:  75.3%
+-rw-rw-rw-  2.0 fat    26560 b- defN 23-Apr-24 02:24 perfect_physics/_world.py
+-rw-rw-rw-  2.0 fat     1564 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      910 b- defN 23-Apr-24 02:25 perfect_physics-0.1.3.dist-info/RECORD
+11 files, 53193 bytes uncompressed, 13163 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: perfect_physics/_wall.py
 Comment: 
 
 Filename: perfect_physics/_world.py
 Comment: 
 
-Filename: perfect_physics-0.1.2.dist-info/METADATA
+Filename: perfect_physics-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: perfect_physics-0.1.2.dist-info/WHEEL
+Filename: perfect_physics-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: perfect_physics-0.1.2.dist-info/top_level.txt
+Filename: perfect_physics-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: perfect_physics-0.1.2.dist-info/RECORD
+Filename: perfect_physics-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perfect_physics/_world.py

```diff
@@ -3,15 +3,14 @@
 import glob
 import logging
 import random
 from pathlib import Path
 from typing import List
 
 import cloudpickle as pickle
-import cv2
 import numpy as np
 
 try:
     from pysnptools.util.mapreduce1 import map_reduce
 except ImportError:
 
     def map_reduce(input_seq, mapper, runner=None):
@@ -481,14 +480,16 @@
         round_time=True,
         talkie_codec="png",
         silent_codec="MJPG",
         prefix="",
         runner=None,
         **kwargs,
     ):
+        import cv2
+
         folder = Path(folder)
         clock_list, world_list, timeline = World._cp_to_lists(
             folder, slice=slice, filter_same_time=True
         )
 
         frame_count = int((clock_list[-1] - clock_list[0]) * fps / speed_up) + 1
         logging.info(f"frame_count {frame_count}")
```

## Comparing `perfect_physics-0.1.2.dist-info/METADATA` & `perfect_physics-0.1.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-physics
-Version: 0.1.2
+Version: 0.1.3
 Summary: Perfect Physics
 Home-page: https://towardsdatascience.com/perfect-infinite-precision-game-physics-in-python-part-1-698211c08d95
 Author: Carl Kadie
 License: MIT or Apache-2.0
 Description-Content-Type: text/markdown
 Requires-Dist: sympy
 Requires-Dist: numpy
```

