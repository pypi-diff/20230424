# Comparing `tmp/spycio-0.2.6.tar.gz` & `tmp/spycio-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spycio-0.2.6.tar", max compression
+gzip compressed data, was "spycio-0.2.7.tar", max compression
```

## Comparing `spycio-0.2.6.tar` & `spycio-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.6/LICENSE
--rw-r--r--   0        0        0     2824 2023-04-05 12:47:50.355077 spycio-0.2.6/README.md
--rw-r--r--   0        0        0     1376 2023-04-23 11:27:01.064906 spycio-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.6/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
--rw-r--r--   0        0        0      377 2023-04-02 20:20:51.957364 spycio-0.2.6/spycio/__init__.py
--rw-r--r--   0        0        0     7374 2023-04-20 22:16:11.949060 spycio-0.2.6/spycio/spycio.py
--rw-r--r--   0        0        0     4279 2023-04-23 11:21:08.123530 spycio-0.2.6/spycio/utils.py
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 spycio-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3088 2023-04-23 21:32:05.272425 spycio-0.2.7/README.md
+-rw-r--r--   0        0        0     1376 2023-04-24 21:14:37.961344 spycio-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.7/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
+-rw-r--r--   0        0        0      412 2023-04-24 21:12:30.128846 spycio-0.2.7/spycio/__init__.py
+-rw-r--r--   0        0        0     7409 2023-04-23 21:33:14.616696 spycio-0.2.7/spycio/spycio.py
+-rw-r--r--   0        0        0     4279 2023-04-23 11:21:08.123530 spycio-0.2.7/spycio/utils.py
+-rw-r--r--   0        0        0     4197 1970-01-01 00:00:00.000000 spycio-0.2.7/PKG-INFO
```

### Comparing `spycio-0.2.6/LICENSE` & `spycio-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spycio-0.2.6/README.md` & `spycio-0.2.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 ```
 
 Minimal example
 ================
 
 ``` {.bash}
 #!/usr/bin/env python
-from numpy import Inf
-from math import pi
+from numpy import pi, Inf
 
 from spycio import distance, travelTime
+from spycio.utils import spherToGeo
 
 def format_distance_without_configuration(A, B, speed, method):
     string_template='A:{origin}, B:{target}, speed:{speed}, method:{on}, distance:{d}, eta:{eta}'
     
     dist=distance(A, B, method)
     duration=travelTime(speed, A, B, method)
     
@@ -41,42 +41,52 @@
     string_template='A:{origin}, B:{target}, speed:{speed}, method:{on}, config:{setup}, distance:{d}, eta:{eta}'
     
     dist=distance(A, B, method, config)
     duration=travelTime(speed, A, B, method, config)
     
     return string_template.format(origin=A,target=B, speed=speed, on=method,setup=config, d=dist, eta=duration)
 
+
 # Default distance calculation: Euclidean
 A=[0, 0]
 B=[1, 1]
+C=[2, 2]
+D=[pi / 2, 0]
 
 speed=1
 
 print('Euclidean distance: '+str(distance(A, B)))
 
 print('\n')
 
 configurations=[
-    ([1, 1], [2, 2], speed, "manhattan"),
-    ([1, 1], [2, 2], speed, "euclidean"),
-    ([1, 1], [2, 2], speed, "max")
+    (B, C, speed, "manhattan"),
+    (B, C, speed, "euclidean"),
+    (B, C, speed, "max"),
+    (B, C, speed, "chebyshev"),
+    (B, C, speed, "manhattan"),
+    (B, C, speed, "cityblock"),
+    (B, C, speed, "cosine"),
+    (B, C, speed, "braycurtis"),
+    (B, C, speed, "canberra")
 ]
 
 print('Format distance without configuration: ')
-for A, B, speed, method in configurations:
-    print(format_distance_without_configuration(A, B, speed, method))
+for origin, target, speed, method in configurations:
+    print(format_distance_without_configuration(origin, target, speed, method))
 
 print('\n')
 
 configurations=[
-    ([1, 1], [2, 2], speed, "pnorm", { "exponent": 2 }),
-    ([1, 1], [2, 2], speed, "pnorm", { "exponent": 3 }),
-    ([1, 1], [2, 2], speed, "pnorm", { "exponent": 4 }),
-    ([1, 1], [2, 2], speed, "pnorm", { "exponent": Inf }),
-    ([0, 0], [pi / 2, 0], speed, "sphere", { "radius": 1 })
+    (B, C, speed, "pnorm", { "exponent": 2 }),
+    (B, C, speed, "pnorm", { "exponent": 3 }),
+    (B, C, speed, "pnorm", { "exponent": 4 }),
+    (B, C, speed, "pnorm", { "exponent": Inf }),
+    (A, D, speed, "sphere", { "radius": 1 }),
+    (spherToGeo(A), spherToGeo(D), speed, "geographical", { "radius": 1 })
 ]
 
 print('Format distance with configuration: ')
 
-for A, B, speed, method, config in configurations:
-    print(format_distance(A, B, speed, method, config))
+for origin, target, speed, method, config in configurations:
+    print(format_distance(origin, target, speed, method, config))
 ```
```

### Comparing `spycio-0.2.6/pyproject.toml` & `spycio-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spycio"
-version = "0.2.6"
+version = "0.2.7"
 description = "Distances in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "spycio"}]
 homepage = "https://pypi.org/project/spycio/"
 repository = "https://github.com/trouchet/spycio"
```

### Comparing `spycio-0.2.6/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb` & `spycio-0.2.7/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `spycio-0.2.6/spycio/spycio.py` & `spycio-0.2.7/spycio/spycio.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,17 @@
       ) 
       )
 
   # Complains on unknown method
   else:
     methods=['pnorm', 'cosine', 'sqeuclidean', 'euclidean', 'manhattan', 
              'cityblock', 'max', 'chebyshev', 'sphere', 'geographical']
-    emsg="There are only the following methods available: {methods}".format(methods=str(methods))
+    emsg="Method \"{method}\" not found among available methods: {methods}".format(\
+      method=method, methods=str(methods)
+    )
     throw(emsg, TypeError)
 
 '''
   @abstract returns the distance of two points based on
  
   @param {Array} coordinate_1
   @param {Array} coordinate_2
```

### Comparing `spycio-0.2.6/spycio/utils.py` & `spycio-0.2.7/spycio/utils.py`

 * *Files identical despite different names*

