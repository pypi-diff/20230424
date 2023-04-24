# Comparing `tmp/numba-kdtree-0.1.6.tar.gz` & `tmp/numba-kdtree-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-kdtree-0.1.6.tar", last modified: Tue Dec 13 14:58:39 2022, max compression
+gzip compressed data, was "numba-kdtree-0.1.7.tar", last modified: Mon Apr 24 18:41:55 2023, max compression
```

## Comparing `numba-kdtree-0.1.6.tar` & `numba-kdtree-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:58:39.350064 numba-kdtree-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-13 14:58:39.350064 numba-kdtree-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:58:39.346064 numba-kdtree-0.1.6/numba_kdtree/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/numba_kdtree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/numba_kdtree/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/numba_kdtree/ckdtree_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/numba_kdtree/kd_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:58:39.346064 numba-kdtree-0.1.6/numba_kdtree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-13 14:58:39.000000 numba-kdtree-0.1.6/numba_kdtree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2022-12-13 14:58:39.000000 numba-kdtree-0.1.6/numba_kdtree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:58:39.000000 numba-kdtree-0.1.6/numba_kdtree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-13 14:58:39.000000 numba-kdtree-0.1.6/numba_kdtree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-13 14:58:39.000000 numba-kdtree-0.1.6/numba_kdtree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:58:39.000000 numba-kdtree-0.1.6/numba_kdtree.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 14:58:39.350064 numba-kdtree-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:58:39.342064 numba-kdtree-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:58:39.350064 numba-kdtree-0.1.6/src/ckdtree/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/README
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/build.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/ckdtree.h
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/ckdtree_decl.h
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/distance.h
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/distance_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/init.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/partial_sort.h
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/query.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/query_radius.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2022-12-13 14:58:18.000000 numba-kdtree-0.1.6/src/ckdtree/rectangle.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:41:55.127469 numba-kdtree-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-24 18:41:55.127469 numba-kdtree-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:41:55.123469 numba-kdtree-0.1.7/numba_kdtree/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/numba_kdtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/numba_kdtree/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/numba_kdtree/ckdtree_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/numba_kdtree/kd_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:41:55.123469 numba-kdtree-0.1.7/numba_kdtree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-24 18:41:55.000000 numba-kdtree-0.1.7/numba_kdtree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 18:41:55.000000 numba-kdtree-0.1.7/numba_kdtree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:41:55.000000 numba-kdtree-0.1.7/numba_kdtree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 18:41:55.000000 numba-kdtree-0.1.7/numba_kdtree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 18:41:55.000000 numba-kdtree-0.1.7/numba_kdtree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:41:54.000000 numba-kdtree-0.1.7/numba_kdtree.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:41:55.127469 numba-kdtree-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:41:55.119469 numba-kdtree-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:41:55.123469 numba-kdtree-0.1.7/src/ckdtree/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/README
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/build.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/ckdtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/ckdtree_decl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/distance_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/init.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/partial_sort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/query.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/query_radius.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/src/ckdtree/rectangle.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:41:55.123469 numba-kdtree-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-04-24 18:41:31.000000 numba-kdtree-0.1.7/tests/test_kdtree.py
```

### Comparing `numba-kdtree-0.1.6/LICENSE` & `numba-kdtree-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/PKG-INFO` & `numba-kdtree-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-kdtree
-Version: 0.1.6
+Version: 0.1.7
 Summary: A kdtree implementation for numba.
 Home-page: https://github.com/mortacious/numba-kdtree
 Author: Felix Igelbrink
 Author-email: felix.igelbrink@uni-osnabrueck.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/numba-kdtree/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `numba-kdtree-0.1.6/README.md` & `numba-kdtree-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/numba_kdtree/ckdtree_ctypes.py` & `numba-kdtree-0.1.7/numba_kdtree/ckdtree_ctypes.py`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/numba_kdtree/kd_tree.py` & `numba-kdtree-0.1.7/numba_kdtree/kd_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,31 +106,24 @@
             # HACK: we are in the process of shutting down the interpreter so calling the external c function
             # might not be possible any more. For now just ignore this
             pass
 
     def free_index(self):
         _KDTree_free(self)
 
-    def query(self, X, k=1, p=2.0, eps=0.0, distance_upper_bound=np.inf, workers=1):
-        if workers == 1:
-            return _KDTree_query(self, X, k, p, eps, distance_upper_bound)
-        else:
-            return _KDTree_query_parallel(self, X, k, p, eps, distance_upper_bound, workers=workers)
-
-    def query_radius(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=-1):
-        if workers == 1:
-            return _KDTree_query_radius(self, X, r, p, eps, return_sorted, return_length)
-        else:
-            return _KDTree_query_radius_parallel(self, X, r, p, eps, return_sorted, return_length, workers=workers)
+    def query(self, X, k=1, p=2.0, eps=0.0, distance_upper_bound=np.inf, workers=None):
+        return _KDTree_query(self, X, k, p, eps, distance_upper_bound, workers=workers)
 
+    def query_radius(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=None):
+        return _KDTree_query_radius(self, X, r, p, eps, return_sorted, return_length, workers=workers)
 
 structref.define_proxy(_KDTree, KDTreeType,
                        ["ckdtree", "root_bbox", "data", "idx"])
 
-
+# define wrapper functions for each method of the kdtree
 @nb.njit()
 def _KDTree_get_root_bbox(self):
     return self.root_bbox
 
 
 @nb.njit()
 def _KDTree_get_data(self):
@@ -154,31 +147,21 @@
 
 @nb.njit()
 def _KDTree_free(self):
     self.free_index()
 
 
 @nb.njit()
-def _KDTree_query(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf):
-    return self.query(X, k=k, p=p, eps=eps, distance_upper_bound=distance_upper_bound)
-
-
-@nb.njit()
-def _KDTree_query_parallel(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf, workers=-1):
-    return self.query_parallel(X, k=k, p=p, eps=eps, distance_upper_bound=distance_upper_bound, workers=workers)
-
-
-@nb.njit()
-def _KDTree_query_radius(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False):
-    return self.query_radius(X, r, p, eps, return_sorted, return_length)
+def _KDTree_query(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf, workers=None):
+    return self.query(X, k=k, p=p, eps=eps, distance_upper_bound=distance_upper_bound, workers=workers)
 
 
 @nb.njit()
-def _KDTree_query_radius_parallel(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=1):
-    return self.query_radius_parallel(X, r, p, eps, return_sorted, return_length, workers=workers)
+def _KDTree_query_radius(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=None):
+    return self.query_radius(X, r, p, eps, return_sorted, return_length, workers=workers)
 
 
 @overload_method(KDTreeType, "_size")
 def _ol_size(self):
     dtype = self.field_dict['data'].dtype
     if dtype != nb.types.float32:
         dtype = nb.types.float64
@@ -224,170 +207,152 @@
         compact_ = 1 if compact else 0
         balanced_ = 1 if balanced else 0
         func_build(self.ckdtree, 0, n_data, self.root_bbox[0].ctypes, self.root_bbox[1].ctypes, balanced_, compact_)
 
     return _build_index_impl
 
 
-@overload_method(KDTreeType, "query", jit_options={"nogil": True, "debug": DEBUG, "fastmath": FASTMATH, 'parallel': False})
-def _ol_query(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf):
+@overload_method(KDTreeType, "query", jit_options={"nogil": True, "debug": DEBUG, "fastmath": FASTMATH, 'parallel': True})
+def _ol_query(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf, workers=None):
     # choose the appropriate methods based on the data type
     dtype = self.field_dict['data'].dtype
     if dtype == nb.types.float32:
         dtype_npy = np.float32
     else:
         dtype = nb.types.float64
         dtype_npy = np.float64
 
     func_query_knn = ckdtree_ct.query_knn[dtype]
 
-    def _query_impl(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf):
-        n_features = self.data.shape[1]
-        xx = _convert_to_valid_input(X, n_features, dtype_npy)
-        n_queries = xx.shape[0]
-        if p < 1:
-            raise ValueError("Only p-norms with 1<=p<=infinity permitted")
-
-        dd = np.empty((n_queries, k), dtype=dtype_npy)
-        ii = np.full((n_queries, k), fill_value=-1, dtype=INT_TYPE)
-        nn = np.empty((n_queries,), dtype=INT_TYPE)
-
-        for i in range(n_queries):
-            func_query_knn(self.ckdtree, dd[i].ctypes, ii[i].ctypes, nn[i:i+1].ctypes,
-                           xx[i].ctypes, 1, k, eps, p, distance_upper_bound)
-        return dd, ii, nn
-
-    return _query_impl
-
+    # strangely we have to check for all cases of None here...
+    if workers is None or workers is nb.types.none or isinstance(workers, nb.types.Omitted):
+        # single threaded case: ignore the number of workers and just operate sequentially
+        def _query_impl(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf, workers=None):
+            n_features = self.data.shape[1]
+            xx = _convert_to_valid_input(X, n_features, dtype_npy)
+            n_queries = xx.shape[0]
+            if p < 1:
+                raise ValueError("Only p-norms with 1<=p<=infinity permitted")
+
+            dd = np.empty((n_queries, k), dtype=dtype_npy)
+            ii = np.full((n_queries, k), fill_value=-1, dtype=INT_TYPE)
+            nn = np.empty((n_queries,), dtype=INT_TYPE)
+
+            for i in range(n_queries):
+                func_query_knn(self.ckdtree, dd[i].ctypes, ii[i].ctypes, nn[i:i+1].ctypes,
+                               xx[i].ctypes, 1, k, eps, p, distance_upper_bound)
+            return dd, ii, nn
 
-@overload_method(KDTreeType, "query_parallel", jit_options={"nogil": True, "debug": DEBUG, "fastmath": FASTMATH, 'parallel': True})
-def _ol_query_parallel(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf, workers=-1):
-    dtype = self.field_dict['data'].dtype
-    if dtype == nb.types.float32:
-        dtype_npy = np.float32
+        return _query_impl
     else:
-        dtype = nb.types.float64
-        dtype_npy = np.float64
-
-    func_query_knn = ckdtree_ct.query_knn[dtype]
-
-    def _query_parallel_impl(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf, workers=-1):
-        numba_threads_prev = nb.get_num_threads()
-        if workers < 0:
-            nb.set_num_threads(NUMBA_THREADS)
-        else:
-            nb.set_num_threads(workers)
-
-        n_features = self.data.shape[1]
-        xx = _convert_to_valid_input(X, n_features, dtype_npy)
-
-        n_queries = xx.shape[0]
-
-        dd = np.empty((n_queries, k), dtype=dtype_npy)
-        ii = np.full((n_queries, k), fill_value=-1, dtype=INT_TYPE)
-        nn = np.empty((n_queries,), dtype=INT_TYPE)
-
-        for i in nb.prange(n_queries):
-            func_query_knn(self.ckdtree, dd[i].ctypes, ii[i].ctypes, nn[i:i+1].ctypes,
-                           xx[i].ctypes, 1, k, eps, p, distance_upper_bound)
-        nb.set_num_threads(numba_threads_prev)
-        return dd, ii, nn
+        def _query_parallel_impl(self, X, k=1, p=2, eps=0.0, distance_upper_bound=np.inf, workers=None):
+            numba_threads_prev = nb.get_num_threads()
+            if workers < 0:
+                # use all available numba threads
+                nb.set_num_threads(NUMBA_THREADS)
+            else:
+                # only the specified number of threads
+                nb.set_num_threads(int(workers))
+
+            n_features = self.data.shape[1]
+            xx = _convert_to_valid_input(X, n_features, dtype_npy)
+
+            n_queries = xx.shape[0]
+
+            dd = np.empty((n_queries, k), dtype=dtype_npy)
+            ii = np.full((n_queries, k), fill_value=-1, dtype=INT_TYPE)
+            nn = np.empty((n_queries,), dtype=INT_TYPE)
+
+            for i in nb.prange(n_queries):
+                func_query_knn(self.ckdtree, dd[i].ctypes, ii[i].ctypes, nn[i:i + 1].ctypes,
+                               xx[i].ctypes, 1, k, eps, p, distance_upper_bound)
+            # restore the previous number of threads
+            nb.set_num_threads(numba_threads_prev)
+            return dd, ii, nn
 
-    return _query_parallel_impl
+        return _query_parallel_impl
 
 
 @overload_method(KDTreeType, "query_radius", jit_options={"nogil": True, "debug": DEBUG, "fastmath": FASTMATH, 'parallel': False})
-def _ol_query_radius(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False):
+def _ol_query_radius(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=None):
     # choose the appropriate methods based on the data type
     dtype = self.field_dict['data'].dtype
     if dtype == nb.types.float32:
         dtype_npy = np.float32
     else:
         dtype = nb.types.float64
         dtype_npy = np.float64
 
     func_query_knn = ckdtree_ct.query_radius[dtype]
     radius_result_set_get_size = ckdtree_ct.radius_result_set_get_size
     radius_result_set_copy_and_free = ckdtree_ct.radius_result_set_copy_and_free
 
     result_array_type = types.int64[:]
 
-    # noinspection PyShadowingNames
-    def _query_radius_impl(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False):
-        n_features = self.data.shape[1]
-        xx = _convert_to_valid_input(X, n_features, dtype_npy)
-        n_queries = xx.shape[0]
-
-        if p < 1:
-            raise ValueError("Only p-norms with 1<=p<=infinity permitted")
-
-        # prepare result list
-        results_list = nb.typed.List.empty_list(item_type=result_array_type, allocated=n_queries)
-        results_list.extend([np.empty(0, dtype=np.int64) for i in range(n_queries)])
-
-        for i in range(n_queries):
-            result_set = func_query_knn(self.ckdtree, xx[i].ctypes, 1, r, eps, p, return_length, return_sorted)
-            # copy the result set into a separate buffer owned by python
-            num_results = radius_result_set_get_size(result_set)
-            results = np.empty(num_results, dtype=np.int64)
-            radius_result_set_copy_and_free(result_set, results.ctypes)
-            results_list[i] = results
-
-        return results_list
+    # strangely we have to check for all cases of None here...
+    if workers is None or workers is nb.types.none or isinstance(workers, nb.types.Omitted):
+        # noinspection PyShadowingNames
+        def _query_radius_impl(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=None):
+            n_features = self.data.shape[1]
+            xx = _convert_to_valid_input(X, n_features, dtype_npy)
+            n_queries = xx.shape[0]
+
+            if p < 1:
+                raise ValueError("Only p-norms with 1<=p<=infinity permitted")
+
+            # prepare result list
+            results_list = nb.typed.List.empty_list(item_type=result_array_type, allocated=n_queries)
+            results_list.extend([np.empty(0, dtype=np.int64) for i in range(n_queries)])
+
+            for i in range(n_queries):
+                result_set = func_query_knn(self.ckdtree, xx[i].ctypes, 1, r, eps, p, return_length, return_sorted)
+                # copy the result set into a separate buffer owned by python
+                num_results = radius_result_set_get_size(result_set)
+                results = np.empty(num_results, dtype=np.int64)
+                radius_result_set_copy_and_free(result_set, results.ctypes)
+                results_list[i] = results
 
-    return _query_radius_impl
+            return results_list
 
-
-@overload_method(KDTreeType, "query_radius_parallel", jit_options={"nogil": True, "debug": DEBUG, "fastmath": FASTMATH, 'parallel': True})
-def _ol_query_radius_parallel(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=-1):
-    # choose the appropriate methods based on the data type
-    dtype = self.field_dict['data'].dtype
-    if dtype == nb.types.float32:
-        dtype_npy = np.float32
+        return _query_radius_impl
     else:
-        dtype = nb.types.float64
-        dtype_npy = np.float64
+        # noinspection PyShadowingNames
+        def _query_radius_parallel_impl(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False,
+                                        workers=None):
+            numba_threads_prev = nb.get_num_threads()
+            if workers < 0:
+                # use all available numba threads
+                nb.set_num_threads(NUMBA_THREADS)
+            else:
+                # only the specified number of threads
+                nb.set_num_threads(int(workers))
+
+            n_features = self.data.shape[1]
+            xx = _convert_to_valid_input(X, n_features, dtype_npy)
+            n_queries = xx.shape[0]
+
+            if p < 1:
+                raise ValueError("Only p-norms with 1<=p<=infinity permitted")
+
+            # prepare result list
+            results_list = nb.typed.List.empty_list(item_type=result_array_type, allocated=n_queries)
+            results_list.extend([np.empty(0, dtype=np.int64) for i in range(n_queries)])
+
+            for i in nb.prange(n_queries):
+                result_set = func_query_knn(self.ckdtree, xx[i].ctypes, 1, r, eps, p, return_length, return_sorted)
+                # copy the result set into a separate buffer owned by python
+                num_results = radius_result_set_get_size(result_set)
+                results = np.empty(num_results, dtype=np.int64)
+                radius_result_set_copy_and_free(result_set, results.ctypes)
+                results_list[i] = results
+            nb.set_num_threads(numba_threads_prev)
 
-    func_query_knn = ckdtree_ct.query_radius[dtype]
-    radius_result_set_get_size = ckdtree_ct.radius_result_set_get_size
-    radius_result_set_copy_and_free = ckdtree_ct.radius_result_set_copy_and_free
+            return results_list
 
-    result_array_type = types.int64[:]
-
-    # noinspection PyShadowingNames
-    def _query_radius_parallel_impl(self, X, r, p=2.0, eps=0.0, return_sorted=False, return_length=False, workers=-1):
-        numba_threads_prev = nb.get_num_threads()
-        if workers < 0:
-            nb.set_num_threads(NUMBA_THREADS)
-        else:
-            nb.set_num_threads(workers)
-
-        n_features = self.data.shape[1]
-        xx = _convert_to_valid_input(X, n_features, dtype_npy)
-        n_queries = xx.shape[0]
-
-        if p < 1:
-            raise ValueError("Only p-norms with 1<=p<=infinity permitted")
-
-        # prepare result list
-        results_list = nb.typed.List.empty_list(item_type=result_array_type, allocated=n_queries)
-        results_list.extend([np.empty(0, dtype=np.int64) for i in range(n_queries)])
-
-        for i in nb.prange(n_queries):
-            result_set = func_query_knn(self.ckdtree, xx[i].ctypes, 1, r, eps, p, return_length, return_sorted)
-            # copy the result set into a separate buffer owned by python
-            num_results = radius_result_set_get_size(result_set)
-            results = np.empty(num_results, dtype=np.int64)
-            radius_result_set_copy_and_free(result_set, results.ctypes)
-            results_list[i] = results
-        nb.set_num_threads(numba_threads_prev)
-
-        return results_list
-
-    return _query_radius_parallel_impl
+        return _query_radius_parallel_impl
 
 
 @nb.njit(nogil=True)
 def _make_kdtree(data, root_bbox, idx, leafsize=10, balanced=False, compact=False):
     # create the transparent underlying c object by calling the function appropriate to the data dtype
     ckdtree = np.uint64(0)  # leave the c object empty for now
     kdtree = _KDTree(ckdtree, root_bbox, data, idx)
@@ -413,7 +378,48 @@
     root_bbox = np.ascontiguousarray(root_bbox, dtype=conv_dtype)
 
     idx = np.arange(n_data, dtype=INT_TYPE)
 
     kdtree = _make_kdtree(data, root_bbox, idx, leafsize, compact, balanced)
     return kdtree
 
+
+# constructor method
+@nb.extending.overload(KDTree, jit_options={'nogil': True, 'fastmath': True})
+def KDTree_numba(data, leafsize: int = 10, compact: bool = False, balanced: bool = False, root_bbox=None):
+    if data.dtype == nb.types.float32:
+        conv_dtype = nb.types.float32
+        finfo = np.finfo(np.float32)
+
+    else:
+        conv_dtype = nb.types.float64
+        finfo = np.finfo(np.float64)
+
+    cmax = finfo.max
+    cmin = finfo.min
+
+    def KDTree_impl(data, leafsize=10, compact=False, balanced=False, root_bbox=None):
+        data = np.ascontiguousarray(data).astype(conv_dtype)
+        n_data, n_features = data.shape
+
+        if root_bbox is None:
+            root_bbox = np.empty((2, 3), dtype=data.dtype)
+            root_bbox[0] = cmax
+            root_bbox[1] = cmin
+
+            for i in range(data.shape[0]):
+                for j in range(data.shape[1]):
+                    if data[i, j] < root_bbox[0, j]:
+                        root_bbox[0, j] = data[i, j]
+                    if data[i, j] > root_bbox[1, j]:
+                        root_bbox[1, j] = data[i, j]
+            # compute the bounding box
+        root_bbox = np.ascontiguousarray(root_bbox).astype(conv_dtype)
+
+        idx = np.arange(n_data, dtype=INT_TYPE)
+
+        kdtree = _make_kdtree(data, root_bbox, idx, leafsize, compact, balanced)
+
+        return kdtree
+
+    return KDTree_impl
+
```

### Comparing `numba-kdtree-0.1.6/numba_kdtree.egg-info/PKG-INFO` & `numba-kdtree-0.1.7/numba_kdtree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-kdtree
-Version: 0.1.6
+Version: 0.1.7
 Summary: A kdtree implementation for numba.
 Home-page: https://github.com/mortacious/numba-kdtree
 Author: Felix Igelbrink
 Author-email: felix.igelbrink@uni-osnabrueck.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/numba-kdtree/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `numba-kdtree-0.1.6/numba_kdtree.egg-info/SOURCES.txt` & `numba-kdtree-0.1.7/numba_kdtree.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 src/ckdtree/ckdtree_decl.h
 src/ckdtree/distance.h
 src/ckdtree/distance_base.h
 src/ckdtree/init.cpp
 src/ckdtree/partial_sort.h
 src/ckdtree/query.cpp
 src/ckdtree/query_radius.cpp
-src/ckdtree/rectangle.h
+src/ckdtree/rectangle.h
+tests/test_kdtree.py
```

### Comparing `numba-kdtree-0.1.6/setup.py` & `numba-kdtree-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/README` & `numba-kdtree-0.1.7/src/ckdtree/README`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/build.cpp` & `numba-kdtree-0.1.7/src/ckdtree/build.cpp`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/ckdtree.h` & `numba-kdtree-0.1.7/src/ckdtree/ckdtree.h`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/ckdtree_decl.h` & `numba-kdtree-0.1.7/src/ckdtree/ckdtree_decl.h`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/distance.h` & `numba-kdtree-0.1.7/src/ckdtree/distance.h`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/distance_base.h` & `numba-kdtree-0.1.7/src/ckdtree/distance_base.h`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/init.cpp` & `numba-kdtree-0.1.7/src/ckdtree/init.cpp`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/partial_sort.h` & `numba-kdtree-0.1.7/src/ckdtree/partial_sort.h`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/query.cpp` & `numba-kdtree-0.1.7/src/ckdtree/query.cpp`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/query_radius.cpp` & `numba-kdtree-0.1.7/src/ckdtree/query_radius.cpp`

 * *Files identical despite different names*

### Comparing `numba-kdtree-0.1.6/src/ckdtree/rectangle.h` & `numba-kdtree-0.1.7/src/ckdtree/rectangle.h`

 * *Files identical despite different names*

