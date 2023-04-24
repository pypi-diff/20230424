# Comparing `tmp/sgw_tools-1.93.tar.gz` & `tmp/sgw_tools-1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgw_tools-1.93.tar", last modified: Tue Mar 28 00:40:08 2023, max compression
+gzip compressed data, was "sgw_tools-1.94.tar", last modified: Mon Apr 24 20:49:09 2023, max compression
```

## Comparing `sgw_tools-1.93.tar` & `sgw_tools-1.94.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-28 00:40:08.971651 sgw_tools-1.93/
--rw-r--r--   0 runner    (1001) docker     (116)     1065 2023-03-28 00:39:32.000000 sgw_tools-1.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      787 2023-03-28 00:40:08.971651 sgw_tools-1.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      391 2023-03-28 00:39:32.000000 sgw_tools-1.93/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-28 00:40:08.971651 sgw_tools-1.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      634 2023-03-28 00:39:32.000000 sgw_tools-1.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-28 00:40:08.971651 sgw_tools-1.93/sgw_tools/
--rw-r--r--   0 runner    (1001) docker     (116)    12418 2023-03-28 00:39:32.000000 sgw_tools-1.93/sgw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2687 2023-03-28 00:39:32.000000 sgw_tools-1.93/sgw_tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (116)    18850 2023-03-28 00:39:32.000000 sgw_tools-1.93/sgw_tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     3431 2023-03-28 00:39:32.000000 sgw_tools-1.93/sgw_tools/graphs.py
--rw-r--r--   0 runner    (1001) docker     (116)     4319 2023-03-28 00:39:32.000000 sgw_tools-1.93/sgw_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-28 00:40:08.971651 sgw_tools-1.93/sgw_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      787 2023-03-28 00:40:08.000000 sgw_tools-1.93/sgw_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      299 2023-03-28 00:40:08.000000 sgw_tools-1.93/sgw_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-28 00:40:08.000000 sgw_tools-1.93/sgw_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-28 00:40:08.000000 sgw_tools-1.93/sgw_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-28 00:40:08.971651 sgw_tools-1.93/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-28 00:39:32.000000 sgw_tools-1.93/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16099 2023-03-28 00:39:32.000000 sgw_tools-1.93/tests/test_biggraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 20:48:38.000000 sgw_tools-1.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-24 20:49:09.693380 sgw_tools-1.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-24 20:48:38.000000 sgw_tools-1.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:49:09.693380 sgw_tools-1.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 20:48:38.000000 sgw_tools-1.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/sgw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-24 20:48:38.000000 sgw_tools-1.94/sgw_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/sgw_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 20:49:09.000000 sgw_tools-1.94/sgw_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:49:09.693380 sgw_tools-1.94/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:48:38.000000 sgw_tools-1.94/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-04-24 20:48:38.000000 sgw_tools-1.94/tests/test_biggraph.py
```

### Comparing `sgw_tools-1.93/LICENSE` & `sgw_tools-1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.93/PKG-INFO` & `sgw_tools-1.94/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw_tools
-Version: 1.93
+Version: 1.94
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.93/setup.py` & `sgw_tools-1.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sgw_tools",
-    version="1.93",
+    version="1.94",
     author="Mark Hale",
     license="MIT",
     description="Spectral graph wavelet tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pulquero/sgw",
     packages=find_packages(),
```

### Comparing `sgw_tools-1.93/sgw_tools/__init__.py` & `sgw_tools-1.94/sgw_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.93/sgw_tools/filters.py` & `sgw_tools-1.94/sgw_tools/filters.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.93/sgw_tools/graph.py` & `sgw_tools-1.94/sgw_tools/graph.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.93/sgw_tools/graphs.py` & `sgw_tools-1.94/sgw_tools/graphs.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
             # check that there are no loops nor parallel edges
             if v1 == v2 or A[v1, v2] == 1:
                 # restart process if needed
                 if edgesTested == N*k:
                     repetition = repetition + 1
                     edgesTested = 0
-                    U = np.kron(np.ones(k), np.arange(N))
+                    U = np.kron(np.ones(k, dtype=np.int32), np.arange(N, dtype=np.int32))
                     A = sparse.lil_matrix(np.zeros((N, N)))
             else:
                 # add edge to graph
                 A[v1, v2] = 1
                 A[v2, v1] = 1
 
                 # remove used half-edges
```

### Comparing `sgw_tools-1.93/sgw_tools/util.py` & `sgw_tools-1.94/sgw_tools/util.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.93/sgw_tools.egg-info/PKG-INFO` & `sgw_tools-1.94/sgw_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw-tools
-Version: 1.93
+Version: 1.94
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.93/tests/test_biggraph.py` & `sgw_tools-1.94/tests/test_biggraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,27 +161,34 @@
             np.testing.assert_equal(G.L.sum(axis=1), 0)
             np.testing.assert_equal(G.L.diagonal(), G.dw)
     
         def test_normalized(G):
             np.testing.assert_equal(G.L.toarray(), G.L.T.toarray())
             np.testing.assert_equal(G.L.diagonal(), 1)
     
+        def test_adjacency(G):
+            np.testing.assert_equal(G.L.diagonal(), 1)
+    
         G = BigGraph.create_from(graphs.ErdosRenyi(100, directed=False))
         self.assertFalse(G.is_directed())
         G.compute_laplacian(lap_type='combinatorial')
         test_combinatorial(G)
         G.compute_laplacian(lap_type='normalized')
         test_normalized(G)
+        G.compute_laplacian(lap_type='adjacency')
+        test_adjacency(G)
     
         G = BigGraph.create_from(graphs.ErdosRenyi(100, directed=True))
         self.assertTrue(G.is_directed())
         G.compute_laplacian(lap_type='combinatorial')
         test_combinatorial(G)
         G.compute_laplacian(lap_type='normalized')
         test_normalized(G)
+        G.compute_laplacian(lap_type='adjacency')
+        test_adjacency(G)
 
     def test_estimate_lmax(self):
         graph = BigGraph.create_from(graphs.Sensor())
         self.assertRaises(ValueError, graph.estimate_lmax, method='unk')
     
         def check_lmax(graph, lmax):
             graph.estimate_lmax(method='bounds')
```

