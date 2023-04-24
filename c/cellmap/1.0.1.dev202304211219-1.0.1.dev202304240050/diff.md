# Comparing `tmp/cellmap-1.0.1.dev202304211219-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304240050-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1390449 bytes, number of entries: 6
+Zip file size: 1390535 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    63190 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304211219.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304211219.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304211219.dist-info/RECORD
-6 files, 4512554 bytes uncompressed, 1389563 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    63494 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304240050.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304240050.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304240050.dist-info/RECORD
+6 files, 4512858 bytes uncompressed, 1389649 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304211219.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304240050.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304211219.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304240050.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304211219.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304240050.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 from cellmap.cellmap import *
```

## cellmap/cellmap.py

```diff
@@ -21,25 +21,33 @@
 
 
 
 def create_graph(
     X,
     cutedge_vol = None,
     cutedge_length = None,
-    cut_std = 2.2,
+    cut_std = None,
     return_type = 'edges',
 ):
     tri_ = matplotlib.tri.Triangulation(X[:,0],X[:,1])
     X_src_,X_trg_ = X[tri_.edges[:,0]],X[tri_.edges[:,1]]
     length_edge_ = np.linalg.norm(X_src_-X_trg_,axis=1)
     x1,y1 = X[tri_.triangles[:,0],0],X[tri_.triangles[:,0],1]
     x2,y2 = X[tri_.triangles[:,1],0],X[tri_.triangles[:,1],1]
     x3,y3 = X[tri_.triangles[:,2],0],X[tri_.triangles[:,2],1]
     vol_ = np.abs((x1-x3)*(y2-y3)-(x2-x3)*(y1-y3))
     length_ = np.max([(x1-x2)**2+(y1-y2)**2,(x2-x3)**2+(y2-y3)**2,(x3-x1)**2+(y3-y1)**2],axis=0)
+    if cut_std == None:
+        std_delta_ = 0.1
+        std_min_ = 1
+        cut_std = std_min_
+        while 1:
+            if len(np.unique(tri_.edges[length_edge_ < cut_std*np.std(length_edge_)].reshape(-1,1).T[0])) == X.shape[0]:
+                break
+            cut_std = cut_std + std_delta_
     if cutedge_vol == None:
         judge_vol_tri_ = vol_ < cut_std*np.std(vol_)
     else:
         judge_vol_tri_ = vol_ < np.percentile(vol_,100-cutedge_vol)
     if cutedge_length == None:
         judge_length_edge_ = length_edge_ < cut_std*np.std(length_edge_)
         judge_length_tri_= length_ < cut_std*np.std(length_)
@@ -244,15 +252,15 @@
     graph_key = 'CellMap_graph',
     graph_method = 'Delauney',
     HD_rate = 0.0,
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
-    cut_std = 2,
+    cut_std = None,
     verbose = True,
     logscale_vel = True,
     ):
     """
     Hodge decomposition
 
     Parameters
```

## Comparing `cellmap-1.0.1.dev202304211219.dist-info/METADATA` & `cellmap-1.0.1.dev202304240050.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304211219
+Version: 1.0.1.dev202304240050
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

