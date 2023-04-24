# Comparing `tmp/obpgenerator-0.0.15.tar.gz` & `tmp/obpgenerator-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obpgenerator-0.0.15.tar", last modified: Fri Mar 24 15:57:38 2023, max compression
+gzip compressed data, was "obpgenerator-0.0.17.tar", last modified: Fri Apr 21 14:16:37 2023, max compression
```

## Comparing `obpgenerator-0.0.15.tar` & `obpgenerator-0.0.17.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 15:57:38.907253 obpgenerator-0.0.15/
--rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.15/LICENSE
--rw-rw-rw-   0        0        0     2709 2023-03-24 15:57:38.907253 obpgenerator-0.0.15/PKG-INFO
--rw-rw-rw-   0        0        0     2217 2023-03-22 07:53:12.000000 obpgenerator-0.0.15/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 15:57:38.870192 obpgenerator-0.0.15/obpgenerator/
--rw-rw-rw-   0        0        0     3698 2023-03-21 14:05:41.000000 obpgenerator-0.0.15/obpgenerator/Layer.py
--rw-rw-rw-   0        0        0       44 2023-03-20 16:21:07.000000 obpgenerator-0.0.15/obpgenerator/Part.py
--rw-rw-rw-   0        0        0     4363 2023-03-20 16:25:09.000000 obpgenerator-0.0.15/obpgenerator/Shape.py
--rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.15/obpgenerator/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.15/obpgenerator/file_import.py
--rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.15/obpgenerator/generate_obp.py
--rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.15/obpgenerator/layer_sorting.py
--rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.15/obpgenerator/manufacturing_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-24 15:57:38.905252 obpgenerator-0.0.15/obpgenerator/melt_strategies/
--rw-rw-rw-   0        0        0       56 2023-03-21 14:45:26.000000 obpgenerator-0.0.15/obpgenerator/melt_strategies/__init__.py
--rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.15/obpgenerator/melt_strategies/line_melting.py
--rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.15/obpgenerator/melt_strategies/point_melting.py
--rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.15/obpgenerator/shape_melting.py
--rw-rw-rw-   0        0        0     2197 2023-03-20 16:11:59.000000 obpgenerator-0.0.15/obpgenerator/slicer.py
-drwxrwxrwx   0        0        0        0 2023-03-24 15:57:38.899248 obpgenerator-0.0.15/obpgenerator.egg-info/
--rw-rw-rw-   0        0        0     2709 2023-03-24 15:57:38.000000 obpgenerator-0.0.15/obpgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-03-24 15:57:38.000000 obpgenerator-0.0.15/obpgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 15:57:38.000000 obpgenerator-0.0.15/obpgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-24 15:57:38.000000 obpgenerator-0.0.15/obpgenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-24 15:57:38.000000 obpgenerator-0.0.15/obpgenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.15/pyproject.toml
--rw-rw-rw-   0        0        0      646 2023-03-24 15:57:38.910254 obpgenerator-0.0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 14:16:37.087213 obpgenerator-0.0.17/
+-rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.17/LICENSE
+-rw-rw-rw-   0        0        0     2880 2023-04-21 14:16:37.087213 obpgenerator-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     2390 2023-04-21 14:14:58.000000 obpgenerator-0.0.17/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:16:37.013862 obpgenerator-0.0.17/obpgenerator/
+-rw-rw-rw-   0        0        0     3681 2023-04-21 12:27:56.000000 obpgenerator-0.0.17/obpgenerator/Layer.py
+-rw-rw-rw-   0        0        0     5264 2023-04-21 13:56:56.000000 obpgenerator-0.0.17/obpgenerator/Part.py
+-rw-rw-rw-   0        0        0     4647 2023-04-21 13:56:52.000000 obpgenerator-0.0.17/obpgenerator/Shape.py
+-rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.17/obpgenerator/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.17/obpgenerator/file_import.py
+-rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.17/obpgenerator/generate_obp.py
+-rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.17/obpgenerator/layer_sorting.py
+-rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.17/obpgenerator/manufacturing_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:16:37.066648 obpgenerator-0.0.17/obpgenerator/melt_strategies/
+-rw-rw-rw-   0        0        0       56 2023-04-11 11:45:09.000000 obpgenerator-0.0.17/obpgenerator/melt_strategies/__init__.py
+-rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.17/obpgenerator/melt_strategies/line_melting.py
+-rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.17/obpgenerator/melt_strategies/point_melting.py
+-rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.17/obpgenerator/shape_melting.py
+-rw-rw-rw-   0        0        0     3156 2023-04-21 13:57:00.000000 obpgenerator-0.0.17/obpgenerator/slicer.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:16:37.087213 obpgenerator-0.0.17/obpgenerator/visualization/
+-rw-rw-rw-   0        0        0       60 2023-04-12 12:20:29.000000 obpgenerator-0.0.17/obpgenerator/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1155 2023-04-12 14:51:19.000000 obpgenerator-0.0.17/obpgenerator/visualization/obp_to_matplotlib.py
+-rw-rw-rw-   0        0        0     3178 2023-04-12 14:51:18.000000 obpgenerator-0.0.17/obpgenerator/visualization/visualization.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:16:37.040996 obpgenerator-0.0.17/obpgenerator.egg-info/
+-rw-rw-rw-   0        0        0     2880 2023-04-21 14:16:36.000000 obpgenerator-0.0.17/obpgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2023-04-21 14:16:36.000000 obpgenerator-0.0.17/obpgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:16:36.000000 obpgenerator-0.0.17/obpgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-21 14:16:36.000000 obpgenerator-0.0.17/obpgenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 14:16:36.000000 obpgenerator-0.0.17/obpgenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.17/pyproject.toml
+-rw-rw-rw-   0        0        0      662 2023-04-21 14:16:37.087213 obpgenerator-0.0.17/setup.cfg
```

### Comparing `obpgenerator-0.0.15/LICENSE` & `obpgenerator-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/PKG-INFO` & `obpgenerator-0.0.17/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpgenerator
-Version: 0.0.15
+Version: 0.0.17
 Summary: Generation of open beam path files based on different strategies
 Home-page: https://github.com/wiberganton/obpgenerator
 Author: Anton Wiberg
 Author-email: wiberg.anton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,7 +63,13 @@
 my_layer.sorting_settings = ramp_settings
 my_layer.set_melt_strategies("line_snake")
 my_layer.set_nmb_of_scans(3)
 my_layer.sorting_strategy = "ramp_manufacturing_settings"
 
 my_layer.export_obp("output.obp")
 ```
+
+# To package
+- Delete old builds in the \dist folder 
+- Update the version in the setup.cfg file
+- run "python -m build"
+- upload to pip with "twine uplaod dist/*"
```

### Comparing `obpgenerator-0.0.15/README.md` & `obpgenerator-0.0.17/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -48,8 +48,14 @@
 my_layer.set_manufacturing_settings(manufacturing_settings)
 my_layer.sorting_settings = ramp_settings
 my_layer.set_melt_strategies("line_snake")
 my_layer.set_nmb_of_scans(3)
 my_layer.sorting_strategy = "ramp_manufacturing_settings"
 
 my_layer.export_obp("output.obp")
-```
+```
+
+# To package
+- Delete old builds in the \dist folder 
+- Update the version in the setup.cfg file
+- run "python -m build"
+- upload to pip with "twine uplaod dist/*"
```

### Comparing `obpgenerator-0.0.15/obpgenerator/Layer.py` & `obpgenerator-0.0.17/obpgenerator/Layer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import obpgenerator.layer_sorting as sorting
 import obplib as obp
 import obpgenerator.Shape as Shape
 import numpy as np
 
 class Layer:
-    shapes = [] #array of Shape objects
-    shapes_to_export = [] #array with sorted shapes to export
-    sorting_strategy = "shapes_first" #defines the order in which the shapes are manufactured
-    sorting_settings = dict() #appends settings to the sorting algorithm
+    def __init__(self):
+        self.shapes = [] #array of Shape objects
+        self.shapes_to_export = [] #array with sorted shapes to export
+        self.sorting_strategy = "shapes_first" #defines the order in which the shapes are manufactured
+        self.sorting_settings = dict() #appends settings to the sorting algorithm
 
     def create_obp_elements(self):
         self.sort_layers()
         obp_elements = []
         for shape in self.shapes_to_export:
             shape.generate_melt_strategy()
             shape.generate_obp_elements()
@@ -46,44 +47,41 @@
         if not type(nmb_of_scans) is list:
             nmb_of_scans = [nmb_of_scans]*len(self.shapes)
         elif not len(nmb_of_scans) == len(self.shapes):
             nmb_of_scans = [nmb_of_scans[0]]*len(self.shapes)
         for i in range(len(self.shapes)):
             self.shapes[i].nmb_of_scans = nmb_of_scans[i]
 
-    def set_shapes(self, spacing, size=300, angle=0):
+    def set_shapes(self, spacing, size=150, angle=0):
         if not type(spacing) is list:
             spacing = [spacing]*len(self.shapes)
         elif not len(spacing) == len(self.shapes):
-            spacing = [spacing[0]]*len(self.shapes)
+            print("error in spacing length")
         if not type(size) is list:
             size = [size]*len(self.shapes)
         elif not len(size) == len(self.shapes):
-            size = [size[0]]*len(self.shapes)
+            print("error in size length")
         if not type(angle) is list:
             angle = [angle]*len(self.shapes)
         elif not len(angle) == len(self.shapes):
-            angle = [angle[0]]*len(self.shapes)
+            print("error in angle length")
 
         for i in range(len(self.shapes)):
             self.shapes[i].generate_matrixes(spacing[i], size[i], angle[i])
             self.shapes[i].check_keep_matrix()
-            
-            x = self.shapes[i].keep_matrix
-            nonZero = np.count_nonzero(x == 2)
-            #print(nonZero)
 
     def sort_layers(self, strategy=None,settings=None):
         if strategy is None:
             strategy = self.sorting_strategy
         if settings is None:
             settings = self.sorting_settings
         self.shapes_to_export = sorting.sort(self.shapes,strategy=strategy,settings=settings)
 
-    def create_from_mplt_paths(self, matplot_paths):
+    def create_from_mplt_paths(self, matplot_paths): 
+        #matplot_paths should be array on form [[path1 path2],[path3]]
         for path in matplot_paths:
             new_shape = Shape.Shape()
             new_shape.paths = path
             self.shapes.append(new_shape)
```

### Comparing `obpgenerator-0.0.15/obpgenerator/Shape.py` & `obpgenerator-0.0.17/obpgenerator/Shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,29 +18,36 @@
     qx = ox + math.cos(angle) * (px - ox) - math.sin(angle) * (py - oy)
     qy = oy + math.sin(angle) * (px - ox) + math.cos(angle) * (py - oy)
     return qx, qy
 
 def check_points_in_path(matplotpaths, points):
     #points N*2 numpy array
     inside_all = np.full((len(points),), False)
-    for path in matplotpaths:
-        inside = path.contains_points(points)
+
+    if type(matplotpaths) is list:
+        for path in matplotpaths:
+            inside = path.contains_points(points)
+            inside_all = np.logical_or(inside_all, inside)
+    else:
+        inside = matplotpaths.contains_points(points)
         inside_all = np.logical_or(inside_all, inside)
+    
     return inside_all
 
 class Shape:
-    paths = [] #array of matplotlib.path
-    keep_matrix = None #matrix defining which mesh elements that should be kept
-    coord_matrix = None #matrix defining the coordinates of the mesh elements
-    obp_points = [] #array with elements that build your obp file, contains arrays with 1, 2, or 4 obp.Points. 1 Point in array = obplib.TimedPoints, 2 points = obplib.Line, 4 points = obp.Curve
-    manufacturing_settings = settings.ManufacturingSetting() #Manufacturing settings
-    obp_elements = [] #array with elements for exports
-    melt_strategy = "point_random" #melting strategy
-    melt_settings = dict() #melting settings
-    nmb_of_scans = 1 #number of times the shape should be scanned
+    def __init__(self):
+        self.paths = [] #array of matplotlib.path
+        self.keep_matrix = None #matrix defining which mesh elements that should be kept
+        self.coord_matrix = None #matrix defining the coordinates of the mesh elements
+        self.obp_points = [] #array with elements that build your obp file, contains arrays with 1, 2, or 4 obp.Points. 1 Point in array = obplib.TimedPoints, 2 points = obplib.Line, 4 points = obp.Curve
+        self.manufacturing_settings = settings.ManufacturingSetting() #Manufacturing settings
+        self.obp_elements = [] #array with elements for exports
+        self.melt_strategy = "point_random" #melting strategy
+        self.melt_settings = dict() #melting settings
+        self.nmb_of_scans = 1 #number of times the shape should be scanned
 
     def generate_matrixes(self, spacing, size=150, angle=0): #spacing and size in mm, angle in degree 
         row_height = math.sqrt(3/4)*spacing
         points_x = math.floor(size/spacing)
         points_y = math.floor(size/row_height)
         self.coord_matrix = np.zeros((points_y, points_x),dtype=np.complex_)
         self.keep_matrix = np.zeros((points_y, points_x))
```

### Comparing `obpgenerator-0.0.15/obpgenerator/file_import.py` & `obpgenerator-0.0.17/obpgenerator/file_import.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/obpgenerator/generate_obp.py` & `obpgenerator-0.0.17/obpgenerator/generate_obp.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/obpgenerator/layer_sorting.py` & `obpgenerator-0.0.17/obpgenerator/layer_sorting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/obpgenerator/manufacturing_settings.py` & `obpgenerator-0.0.17/obpgenerator/manufacturing_settings.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/obpgenerator/melt_strategies/line_melting.py` & `obpgenerator-0.0.17/obpgenerator/melt_strategies/line_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/obpgenerator/melt_strategies/point_melting.py` & `obpgenerator-0.0.17/obpgenerator/melt_strategies/point_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/obpgenerator/shape_melting.py` & `obpgenerator-0.0.17/obpgenerator/shape_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.15/obpgenerator/slicer.py` & `obpgenerator-0.0.17/obpgenerator/slicer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pyvista as pv
 from matplotlib.path import Path
-
+from io import StringIO
 
 def find_min_max_z(mesh): #Finds min and max point in the z-direction
       min_value = 0
       max_value = 0
       for point in mesh.points:
             z_value = point[2]
             if z_value < min_value:
@@ -57,22 +57,52 @@
             codes.append(Path.LINETO)
         codes.pop(1)
         codes[-1] = (Path.CLOSEPOLY)
         mpl_paths.append(Path(path_lines, codes))
 
     return mpl_paths
 
+def combine_arrays(arrays):
+    #create a new array with matplotlibs which adds different sliced stl files into different shapes
+
+    numb_of_layers = 0 #Get the numb of layers based on the file with most layers
+    for array in arrays:
+        if len(array) > numb_of_layers:
+            numb_of_layers = len(array)
+
+    new_array = []
+    for i in range(numb_of_layers):
+        layer_array = []
+        for array in arrays:
+            if len(array)<=i:
+                layer_array.append([])
+            else:
+                layer_array.append(array[i][0])
+        new_array.append(layer_array)
+    
+    return new_array
 
-def slice_stl(path, layer_height):
-    mesh = pv.read(path)
+def slice_stl_file(stl_string, layer_height):
+    mesh = pv.read(stl_string)
     min_z, max_z = find_min_max_z(mesh)
     
     slices = []
     z_pos = min_z+layer_height/2
     while z_pos < max_z:
         single_slice = mesh.slice(normal=[0, 0, 1],origin=(0,0,z_pos))
         mpl_path = py_to_mpl_path(single_slice)
-        slices.append(mpl_path)
+        slices.append([mpl_path])
         z_pos = z_pos + layer_height
     return slices
 
 
+def slice_stl(paths,layer_height):
+    if not type(paths) is list:
+        paths = [paths]
+    slices = []
+    for path in paths:
+       slices.append(slice_stl_file(path,layer_height))
+    combined_slices = combine_arrays(slices)
+    return combined_slices
+
+
+
```

### Comparing `obpgenerator-0.0.15/obpgenerator.egg-info/PKG-INFO` & `obpgenerator-0.0.17/obpgenerator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpgenerator
-Version: 0.0.15
+Version: 0.0.17
 Summary: Generation of open beam path files based on different strategies
 Home-page: https://github.com/wiberganton/obpgenerator
 Author: Anton Wiberg
 Author-email: wiberg.anton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,7 +63,13 @@
 my_layer.sorting_settings = ramp_settings
 my_layer.set_melt_strategies("line_snake")
 my_layer.set_nmb_of_scans(3)
 my_layer.sorting_strategy = "ramp_manufacturing_settings"
 
 my_layer.export_obp("output.obp")
 ```
+
+# To package
+- Delete old builds in the \dist folder 
+- Update the version in the setup.cfg file
+- run "python -m build"
+- upload to pip with "twine uplaod dist/*"
```

### Comparing `obpgenerator-0.0.15/obpgenerator.egg-info/SOURCES.txt` & `obpgenerator-0.0.17/obpgenerator.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 obpgenerator.egg-info/PKG-INFO
 obpgenerator.egg-info/SOURCES.txt
 obpgenerator.egg-info/dependency_links.txt
 obpgenerator.egg-info/requires.txt
 obpgenerator.egg-info/top_level.txt
 obpgenerator/melt_strategies/__init__.py
 obpgenerator/melt_strategies/line_melting.py
-obpgenerator/melt_strategies/point_melting.py
+obpgenerator/melt_strategies/point_melting.py
+obpgenerator/visualization/__init__.py
+obpgenerator/visualization/obp_to_matplotlib.py
+obpgenerator/visualization/visualization.py
```

### Comparing `obpgenerator-0.0.15/setup.cfg` & `obpgenerator-0.0.17/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6270 6765 6e65 7261 746f 720d   = obpgenerator.
 00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
-00000030: 350d 0a61 7574 686f 7220 3d20 416e 746f  5..author = Anto
+00000030: 370d 0a61 7574 686f 7220 3d20 416e 746f  7..author = Anto
 00000040: 6e20 5769 6265 7267 0d0a 6175 7468 6f72  n Wiberg..author
 00000050: 5f65 6d61 696c 203d 2077 6962 6572 672e  _email = wiberg.
 00000060: 616e 746f 6e40 676d 6169 6c2e 636f 6d0d  anton@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2047  .description = G
 00000080: 656e 6572 6174 696f 6e20 6f66 206f 7065  eneration of ope
 00000090: 6e20 6265 616d 2070 6174 6820 6669 6c65  n beam path file
 000000a0: 7320 6261 7365 6420 6f6e 2064 6966 6665  s based on diffe
@@ -28,14 +28,15 @@
 000001b0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
 000001c0: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
 000001d0: 7469 6f6e 735d 0d0a 696e 7374 616c 6c5f  tions]..install_
 000001e0: 7265 7175 6972 6573 203d 200d 0a09 7376  requires = ...sv
 000001f0: 6770 6174 6874 6f6f 6c73 0d0a 096e 756d  gpathtools...num
 00000200: 7079 0d0a 096d 6174 706c 6f74 6c69 620d  py...matplotlib.
 00000210: 0a09 6f62 706c 6962 0d0a 0970 7976 6973  ..obplib...pyvis
-00000220: 7461 0d0a 7079 7468 6f6e 5f72 6571 7569  ta..python_requi
-00000230: 7265 7320 3d20 3e3d 332e 370d 0a69 6e63  res = >=3.7..inc
-00000240: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000250: 6120 3d20 5472 7565 0d0a 0d0a 5b65 6767  a = True....[egg
-00000260: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000270: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000280: 2030 0d0a 0d0a                            0....
+00000220: 7461 0d0a 0979 616d 6c0d 0a09 7079 7961  ta...yaml...pyya
+00000230: 6d6c 0d0a 7079 7468 6f6e 5f72 6571 7569  ml..python_requi
+00000240: 7265 7320 3d20 3e3d 332e 370d 0a69 6e63  res = >=3.7..inc
+00000250: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000260: 6120 3d20 5472 7565 0d0a 0d0a 5b65 6767  a = True....[egg
+00000270: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000280: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000290: 2030 0d0a 0d0a                            0....
```

