# Comparing `tmp/enstat-0.8.3.tar.gz` & `tmp/enstat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.8.3.tar", last modified: Fri Apr 21 13:25:27 2023, max compression
+gzip compressed data, was "enstat-0.9.0.tar", last modified: Mon Apr 24 13:02:28 2023, max compression
```

## Comparing `enstat-0.8.3.tar` & `enstat-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:27.099207 enstat-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:27.095207 enstat-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:27.095207 enstat-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-21 13:25:12.000000 enstat-0.8.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-21 13:25:12.000000 enstat-0.8.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-21 13:25:12.000000 enstat-0.8.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-21 13:25:12.000000 enstat-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-21 13:25:12.000000 enstat-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-21 13:25:12.000000 enstat-0.8.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-21 13:25:12.000000 enstat-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-21 13:25:27.099207 enstat-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-21 13:25:12.000000 enstat-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:27.095207 enstat-0.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-21 13:25:12.000000 enstat-0.8.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 13:25:12.000000 enstat-0.8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-21 13:25:12.000000 enstat-0.8.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-21 13:25:12.000000 enstat-0.8.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-21 13:25:12.000000 enstat-0.8.3/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:27.099207 enstat-0.8.3/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    22324 2023-04-21 13:25:12.000000 enstat-0.8.3/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 13:25:26.000000 enstat-0.8.3/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-21 13:25:12.000000 enstat-0.8.3/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-21 13:25:12.000000 enstat-0.8.3/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:27.099207 enstat-0.8.3/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-21 13:25:27.000000 enstat-0.8.3/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-21 13:25:27.000000 enstat-0.8.3/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:25:27.000000 enstat-0.8.3/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 13:25:27.000000 enstat-0.8.3/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 13:25:27.000000 enstat-0.8.3/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 13:25:12.000000 enstat-0.8.3/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:25:27.099207 enstat-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-21 13:25:12.000000 enstat-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:27.099207 enstat-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:25:12.000000 enstat-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-21 13:25:12.000000 enstat-0.8.3/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-21 13:25:12.000000 enstat-0.8.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.827066 enstat-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 13:02:11.000000 enstat-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 13:02:11.000000 enstat-0.9.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 13:02:11.000000 enstat-0.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-24 13:02:11.000000 enstat-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-24 13:02:11.000000 enstat-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:02:11.000000 enstat-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 13:02:11.000000 enstat-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-24 13:02:28.827066 enstat-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-24 13:02:11.000000 enstat-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25589 2023-04-24 13:02:11.000000 enstat-0.9.0/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-24 13:02:11.000000 enstat-0.9.0/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 13:02:11.000000 enstat-0.9.0/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 13:02:11.000000 enstat-0.9.0/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:02:28.827066 enstat-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-24 13:02:11.000000 enstat-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.827066 enstat-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/test_main.py
```

### Comparing `enstat-0.8.3/.github/workflows/ci.yml` & `enstat-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/.github/workflows/pre-commit.yml` & `enstat-0.9.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/.github/workflows/python-publish.yml` & `enstat-0.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/.gitignore` & `enstat-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/.pre-commit-config.yaml` & `enstat-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/LICENSE` & `enstat-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/PKG-INFO` & `enstat-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.8.3
+Version: 0.9.0
 Summary: Ensemble averages
 Home-page: https://github.com/tdegeus/enstat
 Author: Tom de Geus
 Author-email: tom@geus.me
 License: MIT
 Keywords: Statistics,Ensemble
 Description-Content-Type: text/markdown
```

### Comparing `enstat-0.8.3/README.md` & `enstat-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/docs/Makefile` & `enstat-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/docs/make.bat` & `enstat-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/docs/module.rst` & `enstat-0.9.0/docs/module.rst`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/enstat/__init__.py` & `enstat-0.9.0/enstat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -436,14 +436,17 @@
         self.bound_error = bound_error
         self.count_left = 0
         self.count_right = 0
         self.bound_left = bin_edges[0]
         self.bound_right = bin_edges[-1]
         self.count = np.zeros((len(bin_edges) - 1), np.uint64)
 
+        if bound_error not in {"raise", "ignore", "norm"}:
+            raise ValueError(f"Unknown bound_error: {bound_error}")
+
     def __iter__(self):
         yield "bin_edges", self.bin_edges
         yield "count", self.count
         yield "count_left", self.count_left
         yield "count_right", self.count_right
         yield "bound_left", self.bound_left
         yield "bound_right", self.bound_right
@@ -694,41 +697,49 @@
         self.bin_edges = np.floor(self.bin_edges)
         self.right = False
 
     def __add__(self, data: ArrayLike):
         self.add_sample(data)
         return self
 
-    def add_sample(self, data: ArrayLike):
+    def _get_bins(self, data: ArrayLike, return_selector: bool = False) -> np.ndarray[int]:
         """
-        Add a sample to the histogram.
-        You can also use the ``+`` operator.
+        Get the bins for the data, update out-of-range counts.
         """
 
         data = np.asarray(data)
         bin = np.digitize(data, self.bin_edges, right=self.right) - 1
-
-        left = bin < 0
-        right = bin >= self.count.size
+        left = data < self.bin_edges[0]
+        right = data >= self.bin_edges[-1]
         nleft = np.sum(left)
         nright = np.sum(right)
         self.count_left += nleft
         self.count_right += nright
 
         if nleft:
             self.bound_left = min([self.bound_left, np.min(data[left])])
 
         if nright:
             self.bound_right = max([self.bound_right, np.max(data[right])])
 
         if self.bound_error == "raise" and (nleft or nright):
             raise ValueError("Data out of bin range")
 
-        bin = bin[np.logical_and(~left, ~right)]
-        self.count += np.bincount(bin, minlength=self.count.size).astype(np.uint64)
+        if return_selector:
+            keep = np.logical_and(~left, ~right)
+            return bin[keep], keep
+
+        return bin[np.logical_and(~left, ~right)]
+
+    def add_sample(self, data: ArrayLike):
+        """
+        Add a sample to the histogram.
+        You can also use the ``+`` operator.
+        """
+        self.count += np.bincount(self._get_bins(data), minlength=self.count.size).astype(np.uint64)
         return self
 
     @property
     def x(self) -> ArrayLike:
         """
         The bin centers.
         """
@@ -762,9 +773,91 @@
         """
         Alias for ``(x, density)``.
         """
 
         return (self.x, self.density)
 
 
+class binned:
+    """
+    Ensemble average after binning.
+
+    :param bin_edges: The bin-edges.
+    :param right: Whether the bin includes the right edge (or the left edge) see numpy.digitize.
+    :param bound_error: What to do if a sample falls out of the bin range:
+
+        - ``"raise"``: raise an error
+        - ``"ignore"``: ignore the data that are out of range
+    """
+
+    def __init__(self, bin_edges: ArrayLike, right: bool = False, bound_error: str = "raise"):
+        self.data = []
+        self.hist = histogram(bin_edges, right, bound_error)
+        if bound_error not in {"raise", "ignore"}:
+            raise ValueError(f"Unknown bound_error: {bound_error}")
+
+    @classmethod
+    def from_data(cls, *args: ArrayLike, **kwargs):
+        r"""
+        Construct from data.
+
+        :param args:
+            Different variables of data to add.
+            The binning is done on the first argument and applied to all other arguments.
+
+        :param kwargs: Automatic binning settings, see :py:meth:`histogram.from_data`.
+        :return: The :py:class:`Histogram` object.
+        """
+
+        hist = histogram.from_data(args[0], **kwargs)
+        return cls(hist.bin_edges, right=hist.right, bound_error=hist.bound_error).add_sample(*args)
+
+    def __iter__(self):
+        return iter(self.data)
+
+    def __getitem__(self, index: int):
+        if hasattr(index, "__len__"):
+            raise ValueError("Multi-dimensional indexing is not supported")
+        return self.data[index]
+
+    def __add__(self, data: ArrayLike):
+        self.add_sample(data)
+        return self
+
+    def add_sample(self, *args: ArrayLike):
+        """
+        Add a sample.
+        If you use only one variable, you can also use the ``+`` operator.
+
+        :param args:
+            Different variables of data to add.
+            The binning is done on the first argument and applied to all other arguments.
+        """
+
+        if len(args) == 0:
+            raise ValueError("No data given")
+
+        for i in range(len(args) - len(self.data)):
+            self.data.append(static(shape=self.hist.bin_edges.size - 1))
+
+        bin, keep = self.hist._get_bins(args[0], return_selector=True)
+        args = [np.asarray(arg)[keep] for arg in args]
+        sqr = [arg * arg for arg in args]
+
+        for arg in args:
+            if arg.shape != args[0].shape:
+                raise ValueError("All arguments must have the same shape")
+
+        for ibin in range(np.max(bin) + 1):
+            sel = bin == ibin
+            if not np.any(sel):
+                continue
+            for i in range(len(args)):
+                self.data[i].first[ibin] += np.sum(args[i][sel])
+                self.data[i].second[ibin] += np.sum(sqr[i][sel])
+                self.data[i].norm[ibin] += np.sum(sel)
+
+        return self
+
+
 if __name__ == "__main__":
     pass
```

### Comparing `enstat-0.8.3/enstat/detail.py` & `enstat-0.9.0/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/enstat/mean.py` & `enstat-0.9.0/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/enstat.egg-info/PKG-INFO` & `enstat-0.9.0/enstat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.8.3
+Version: 0.9.0
 Summary: Ensemble averages
 Home-page: https://github.com/tdegeus/enstat
 Author: Tom de Geus
 Author-email: tom@geus.me
 License: MIT
 Keywords: Statistics,Ensemble
 Description-Content-Type: text/markdown
```

### Comparing `enstat-0.8.3/enstat.egg-info/SOURCES.txt` & `enstat-0.9.0/enstat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,9 +19,10 @@
 enstat/mean.py
 enstat.egg-info/PKG-INFO
 enstat.egg-info/SOURCES.txt
 enstat.egg-info/dependency_links.txt
 enstat.egg-info/requires.txt
 enstat.egg-info/top_level.txt
 tests/__init__.py
+tests/test_binned.py
 tests/test_histogram.py
 tests/test_main.py
```

### Comparing `enstat-0.8.3/setup.py` & `enstat-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/tests/test_histogram.py` & `enstat-0.9.0/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `enstat-0.8.3/tests/test_main.py` & `enstat-0.9.0/tests/test_main.py`

 * *Files identical despite different names*

