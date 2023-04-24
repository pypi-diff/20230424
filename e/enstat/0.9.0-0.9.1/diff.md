# Comparing `tmp/enstat-0.9.0.tar.gz` & `tmp/enstat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.9.0.tar", last modified: Mon Apr 24 13:02:28 2023, max compression
+gzip compressed data, was "enstat-0.9.1.tar", last modified: Mon Apr 24 14:28:06 2023, max compression
```

## Comparing `enstat-0.9.0.tar` & `enstat-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.827066 enstat-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 13:02:11.000000 enstat-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 13:02:11.000000 enstat-0.9.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 13:02:11.000000 enstat-0.9.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-24 13:02:11.000000 enstat-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-24 13:02:11.000000 enstat-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:02:11.000000 enstat-0.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 13:02:11.000000 enstat-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-24 13:02:28.827066 enstat-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-24 13:02:11.000000 enstat-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 13:02:11.000000 enstat-0.9.0/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    25589 2023-04-24 13:02:11.000000 enstat-0.9.0/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-24 13:02:11.000000 enstat-0.9.0/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 13:02:11.000000 enstat-0.9.0/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.823066 enstat-0.9.0/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 13:02:28.000000 enstat-0.9.0/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 13:02:11.000000 enstat-0.9.0/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:02:28.827066 enstat-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-24 13:02:11.000000 enstat-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:28.827066 enstat-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/test_binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-24 13:02:11.000000 enstat-0.9.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.883530 enstat-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 14:27:57.000000 enstat-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 14:27:57.000000 enstat-0.9.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 14:27:57.000000 enstat-0.9.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-24 14:27:57.000000 enstat-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 14:27:57.000000 enstat-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 14:27:57.000000 enstat-0.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 14:27:57.000000 enstat-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-24 14:28:06.883530 enstat-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-24 14:27:57.000000 enstat-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    26261 2023-04-24 14:27:57.000000 enstat-0.9.1/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-24 14:27:57.000000 enstat-0.9.1/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 14:27:57.000000 enstat-0.9.1/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.883530 enstat-0.9.1/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 14:27:57.000000 enstat-0.9.1/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-24 14:27:57.000000 enstat-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:28:06.883530 enstat-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.883530 enstat-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/test_main.py
```

### Comparing `enstat-0.9.0/.github/workflows/ci.yml` & `enstat-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/.github/workflows/pre-commit.yml` & `enstat-0.9.1/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/.github/workflows/python-publish.yml` & `enstat-0.9.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/.gitignore` & `enstat-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/.pre-commit-config.yaml` & `enstat-0.9.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 repos:
-- repo: https://github.com/psf/black
-  rev: 23.3.0
-  hooks:
-  - id: black
-    args: [--safe, --quiet, --line-length=100]
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-yaml
+  - id: check-toml
   - id: debug-statements
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
   rev: v2.8.0
   hooks:
   - id: pretty-format-yaml
     args: [--preserve-quotes, --autofix, --indent, '2']
+  - id: pretty-format-toml
+    args: [--autofix]
+- repo: https://github.com/psf/black
+  rev: 23.3.0
+  hooks:
+  - id: black
+    args: [--safe, --quiet, --line-length=100]
 - repo: https://github.com/humitos/mirrors-autoflake.git
   rev: v1.1
   hooks:
   - id: autoflake
     args: [--in-place, --remove-unused-variable, --remove-all-unused-imports]
 - repo: https://github.com/asottile/reorder_python_imports
   rev: v3.9.0
```

### Comparing `enstat-0.9.0/LICENSE` & `enstat-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/PKG-INFO` & `enstat-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.0
-Summary: Ensemble averages
-Home-page: https://github.com/tdegeus/enstat
-Author: Tom de Geus
-Author-email: tom@geus.me
-License: MIT
-Keywords: Statistics,Ensemble
+Version: 0.9.1
+Author-email: Tom de Geus <tom@geus.me>
+Project-URL: Source, https://github.com/tdegeus/enstat
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstat
 
 [![CI](https://github.com/tdegeus/enstat/workflows/CI/badge.svg)](https://github.com/tdegeus/enstat/actions)
 [![Documentation Status](https://readthedocs.org/projects/enstat/badge/?version=latest)](https://enstat.readthedocs.io)
```

### Comparing `enstat-0.9.0/README.md` & `enstat-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/docs/Makefile` & `enstat-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/docs/make.bat` & `enstat-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/docs/module.rst` & `enstat-0.9.1/docs/module.rst`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/enstat/__init__.py` & `enstat-0.9.1/enstat/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -783,81 +783,99 @@
 
     :param bin_edges: The bin-edges.
     :param right: Whether the bin includes the right edge (or the left edge) see numpy.digitize.
     :param bound_error: What to do if a sample falls out of the bin range:
 
         - ``"raise"``: raise an error
         - ``"ignore"``: ignore the data that are out of range
+
+    :param names: The names of the variables to store.
     """
 
-    def __init__(self, bin_edges: ArrayLike, right: bool = False, bound_error: str = "raise"):
-        self.data = []
+    def __init__(
+        self,
+        bin_edges: ArrayLike,
+        right: bool = False,
+        bound_error: str = "raise",
+        names: list[str] = [],
+    ):
         self.hist = histogram(bin_edges, right, bound_error)
+        self.names = names
+        self.data = {name: static(shape=self.hist.bin_edges.size - 1) for name in names}
         if bound_error not in {"raise", "ignore"}:
             raise ValueError(f"Unknown bound_error: {bound_error}")
 
     @classmethod
-    def from_data(cls, *args: ArrayLike, **kwargs):
+    def from_data(cls, *args: ArrayLike, names: list[str] = [], **kwargs):
         r"""
         Construct from data.
 
         :param args:
             Different variables of data to add.
             The binning is done on the first argument and applied to all other arguments.
 
         :param kwargs: Automatic binning settings, see :py:meth:`histogram.from_data`.
         :return: The :py:class:`Histogram` object.
         """
 
         hist = histogram.from_data(args[0], **kwargs)
-        return cls(hist.bin_edges, right=hist.right, bound_error=hist.bound_error).add_sample(*args)
+        return cls(
+            hist.bin_edges, right=hist.right, bound_error=hist.bound_error, names=names
+        ).add_sample(*args)
 
     def __iter__(self):
         return iter(self.data)
 
     def __getitem__(self, index: int):
-        if hasattr(index, "__len__"):
-            raise ValueError("Multi-dimensional indexing is not supported")
-        return self.data[index]
+        if isinstance(index, str):
+            return self.data[index]
+        return self.data[self.names[index]]
 
     def __add__(self, data: ArrayLike):
         self.add_sample(data)
         return self
 
-    def add_sample(self, *args: ArrayLike):
+    def add_sample(self, *args: ArrayLike, **kwargs: ArrayLike):
         """
         Add a sample.
         If you use only one variable, you can also use the ``+`` operator.
 
         :param args:
             Different variables of data to add.
             The binning is done on the first argument and applied to all other arguments.
         """
 
-        if len(args) == 0:
-            raise ValueError("No data given")
-
-        for i in range(len(args) - len(self.data)):
-            self.data.append(static(shape=self.hist.bin_edges.size - 1))
-
-        bin, keep = self.hist._get_bins(args[0], return_selector=True)
-        args = [np.asarray(arg)[keep] for arg in args]
-        sqr = [arg * arg for arg in args]
+        if len(self.names) == 0:
+            self.names = [i for i in range(len(args))]
+            self.data = {name: static(shape=self.hist.bin_edges.size - 1) for name in self.names}
+
+        for i in range(len(args)):
+            name = self.names[i]
+            if name in kwargs:
+                raise ValueError(f"Duplicate argument: {name}")
+            kwargs[name] = args[i]
+
+        if len(kwargs) != len(self.names):
+            raise ValueError("Incorrect number of arguments")
+
+        bin, keep = self.hist._get_bins(kwargs[self.names[0]], return_selector=True)
+        kwargs = {name: np.asarray(arg)[keep] for name, arg in kwargs.items()}
+        sqr = {name: arg * arg for name, arg in kwargs.items()}
 
-        for arg in args:
-            if arg.shape != args[0].shape:
+        for name, arg in kwargs.items():
+            if arg.shape != kwargs[self.names[0]].shape:
                 raise ValueError("All arguments must have the same shape")
 
         for ibin in range(np.max(bin) + 1):
             sel = bin == ibin
             if not np.any(sel):
                 continue
-            for i in range(len(args)):
-                self.data[i].first[ibin] += np.sum(args[i][sel])
-                self.data[i].second[ibin] += np.sum(sqr[i][sel])
-                self.data[i].norm[ibin] += np.sum(sel)
+            for name, arg in kwargs.items():
+                self.data[name].first[ibin] += np.sum(kwargs[name][sel])
+                self.data[name].second[ibin] += np.sum(sqr[name][sel])
+                self.data[name].norm[ibin] += np.sum(sel)
 
         return self
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `enstat-0.9.0/enstat/detail.py` & `enstat-0.9.1/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/enstat/mean.py` & `enstat-0.9.1/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/enstat.egg-info/PKG-INFO` & `enstat-0.9.1/enstat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.0
-Summary: Ensemble averages
-Home-page: https://github.com/tdegeus/enstat
-Author: Tom de Geus
-Author-email: tom@geus.me
-License: MIT
-Keywords: Statistics,Ensemble
+Version: 0.9.1
+Author-email: Tom de Geus <tom@geus.me>
+Project-URL: Source, https://github.com/tdegeus/enstat
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstat
 
 [![CI](https://github.com/tdegeus/enstat/workflows/CI/badge.svg)](https://github.com/tdegeus/enstat/actions)
 [![Documentation Status](https://readthedocs.org/projects/enstat/badge/?version=latest)](https://enstat.readthedocs.io)
```

### Comparing `enstat-0.9.0/enstat.egg-info/SOURCES.txt` & `enstat-0.9.1/enstat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.md
 environment.yaml
-setup.py
+pyproject.toml
 .github/workflows/ci.yml
 .github/workflows/pre-commit.yml
 .github/workflows/python-publish.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
```

### Comparing `enstat-0.9.0/tests/test_binned.py` & `enstat-0.9.1/tests/test_binned.py`

 * *Files 20% similar despite different names*

```diff
@@ -69,22 +69,22 @@
             xmean[ibin] = np.mean(xi)
             ymean[ibin] = np.mean(yi)
             zmean[ibin] = np.mean(zi)
             xerr[ibin] = np.std(xi)
             yerr[ibin] = np.std(yi)
             zerr[ibin] = np.std(zi)
 
-        binned = enstat.binned.from_data(x, y, z, bin_edges=bin_edges)
+        binned = enstat.binned.from_data(x, y, z, names=["x", "y", "z"], bin_edges=bin_edges)
 
-        self.assertTrue(np.allclose(binned[0].mean(), xmean))
-        self.assertTrue(np.allclose(binned[1].mean(), ymean))
-        self.assertTrue(np.allclose(binned[2].mean(), zmean))
-        self.assertTrue(np.allclose(binned[0].std(), xerr, rtol=1e-2, atol=1e-5))
-        self.assertTrue(np.allclose(binned[1].std(), yerr, rtol=1e-2, atol=1e-5))
-        self.assertTrue(np.allclose(binned[2].std(), zerr, rtol=1e-2, atol=1e-5))
+        self.assertTrue(np.allclose(binned["x"].mean(), xmean))
+        self.assertTrue(np.allclose(binned["y"].mean(), ymean))
+        self.assertTrue(np.allclose(binned["z"].mean(), zmean))
+        self.assertTrue(np.allclose(binned["x"].std(), xerr, rtol=1e-2, atol=1e-5))
+        self.assertTrue(np.allclose(binned["y"].std(), yerr, rtol=1e-2, atol=1e-5))
+        self.assertTrue(np.allclose(binned["z"].std(), zerr, rtol=1e-2, atol=1e-5))
 
     def test_ensemble(self):
         """
         Ensemble data, two variables.
         """
         x = np.random.random([123, 10])
         y = np.random.random(x.shape)
@@ -114,10 +114,46 @@
             binned.add_sample(x[i, :], y[i, :])
 
         self.assertTrue(np.allclose(binned[0].mean(), xmean))
         self.assertTrue(np.allclose(binned[1].mean(), ymean))
         self.assertTrue(np.allclose(binned[0].std(), xerr, rtol=1e-2, atol=1e-5))
         self.assertTrue(np.allclose(binned[1].std(), yerr, rtol=1e-2, atol=1e-5))
 
+    def test_named(self):
+        """
+        Ensemble data, two variables.
+        """
+        x = np.random.random([123, 10])
+        y = np.random.random(x.shape)
+        bin_edges = np.linspace(0, 1, 13)
+        bin = np.digitize(x.ravel(), bin_edges) - 1
+        n = bin_edges.size - 1
+
+        xmean = np.NaN * np.ones(n, dtype=float)
+        ymean = np.NaN * np.ones(n, dtype=float)
+        xerr = np.NaN * np.ones(n, dtype=float)
+        yerr = np.NaN * np.ones(n, dtype=float)
+        n = np.zeros(n, dtype=int)
+
+        for ibin in range(np.max(bin) + 1):
+            sel = bin == ibin
+            n[ibin] = np.sum(sel)
+
+            xi = x.ravel()[sel]
+            yi = y.ravel()[sel]
+            xmean[ibin] = np.mean(xi)
+            ymean[ibin] = np.mean(yi)
+            xerr[ibin] = np.std(xi)
+            yerr[ibin] = np.std(yi)
+
+        binned = enstat.binned(bin_edges, names=["x", "y"])
+        for i in range(x.shape[0]):
+            binned.add_sample(y=y[i, :], x=x[i, :])
+
+        self.assertTrue(np.allclose(binned["x"].mean(), xmean))
+        self.assertTrue(np.allclose(binned["y"].mean(), ymean))
+        self.assertTrue(np.allclose(binned["x"].std(), xerr, rtol=1e-2, atol=1e-5))
+        self.assertTrue(np.allclose(binned["y"].std(), yerr, rtol=1e-2, atol=1e-5))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `enstat-0.9.0/tests/test_histogram.py` & `enstat-0.9.1/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.0/tests/test_main.py` & `enstat-0.9.1/tests/test_main.py`

 * *Files identical despite different names*

