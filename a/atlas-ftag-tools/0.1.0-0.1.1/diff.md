# Comparing `tmp/atlas-ftag-tools-0.1.0.tar.gz` & `tmp/atlas-ftag-tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-ftag-tools-0.1.0.tar", last modified: Mon Apr 17 15:31:10 2023, max compression
+gzip compressed data, was "atlas-ftag-tools-0.1.1.tar", last modified: Mon Apr 24 14:27:37 2023, max compression
```

## Comparing `atlas-ftag-tools-0.1.0.tar` & `atlas-ftag-tools-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:10.592418 atlas-ftag-tools-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-17 15:31:10.592418 atlas-ftag-tools-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:10.588418 atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-17 15:31:10.000000 atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-17 15:31:10.000000 atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:31:10.000000 atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 15:31:10.000000 atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 15:31:10.000000 atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 15:31:10.000000 atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:10.592418 atlas-ftag-tools-0.1.0/ftag/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/flavour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/flavours.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:10.592418 atlas-ftag-tools-0.1.0/ftag/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/hdf5/h5reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/hdf5/h5utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/hdf5/h5writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/vds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:31:10.592418 atlas-ftag-tools-0.1.0/ftag/wps/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/wps/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/ftag/wps/working_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 15:30:49.000000 atlas-ftag-tools-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:31:10.592418 atlas-ftag-tools-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.902977 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 14:27:37.000000 atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/ftag/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/flavour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/flavours.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/ftag/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/h5reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/h5utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/hdf5/h5writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/vds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/ftag/wps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/wps/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/ftag/wps/working_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-24 14:27:18.000000 atlas-ftag-tools-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:27:37.906977 atlas-ftag-tools-0.1.1/setup.cfg
```

### Comparing `atlas-ftag-tools-0.1.0/PKG-INFO` & `atlas-ftag-tools-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI version](https://badge.fury.io/py/atlas-ftag-tools.svg)](https://badge.fury.io/py/atlas-ftag-tools)
+[![codecov](https://codecov.io/gh/umami-hep/atlas-ftag-tools/branch/main/graph/badge.svg?token=MBHLIYYQ7I)](https://codecov.io/gh/umami-hep/atlas-ftag-tools)
+
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
 The code is intended to be used a [library](https://iscinumpy.dev/post/app-vs-library/) for other projects.
 Please see the [example notebook](ftag/example.ipynb) for usage.
 
 ## Installation
@@ -70,7 +74,18 @@
 
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
 Use `--help` for more options and information.
+
+
+## Tests
+
+To run the tests you can use the `pytest` or `coverage` command, for example
+
+```bash
+coverage run --source ftag -m pytest --show-capture=stdout
+```
+
+Running `coverage report` will display the test coverage.
```

### Comparing `atlas-ftag-tools-0.1.0/README.md` & `atlas-ftag-tools-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI version](https://badge.fury.io/py/atlas-ftag-tools.svg)](https://badge.fury.io/py/atlas-ftag-tools)
+[![codecov](https://codecov.io/gh/umami-hep/atlas-ftag-tools/branch/main/graph/badge.svg?token=MBHLIYYQ7I)](https://codecov.io/gh/umami-hep/atlas-ftag-tools)
+
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
 The code is intended to be used a [library](https://iscinumpy.dev/post/app-vs-library/) for other projects.
 Please see the [example notebook](ftag/example.ipynb) for usage.
 
 ## Installation
@@ -59,7 +63,18 @@
 
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
 Use `--help` for more options and information.
+
+
+## Tests
+
+To run the tests you can use the `pytest` or `coverage` command, for example
+
+```bash
+coverage run --source ftag -m pytest --show-capture=stdout
+```
+
+Running `coverage report` will display the test coverage.
```

### Comparing `atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/PKG-INFO` & `atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI version](https://badge.fury.io/py/atlas-ftag-tools.svg)](https://badge.fury.io/py/atlas-ftag-tools)
+[![codecov](https://codecov.io/gh/umami-hep/atlas-ftag-tools/branch/main/graph/badge.svg?token=MBHLIYYQ7I)](https://codecov.io/gh/umami-hep/atlas-ftag-tools)
+
 # ATLAS FTAG Python Tools
 
 This is a collection of Python tools for working with files produced with the FTAG [ntuple dumper](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-dataset-dumper/).
 The code is intended to be used a [library](https://iscinumpy.dev/post/app-vs-library/) for other projects.
 Please see the [example notebook](ftag/example.ipynb) for usage.
 
 ## Installation
@@ -70,7 +74,18 @@
 
 If you want to use the `ttbar` WPs get the efficiencies and rejections for the `zprime` sample, you can add `--zprime "path/to/zprime/*.h5"` to the command.
 Note that a default selection of $p_T > 250 ~GeV$ to jets in the `zprime` sample.
 
 By default the working points are printed to the terminal, but you can save the results to a YAML file with the `--outfile` option.
 
 Use `--help` for more options and information.
+
+
+## Tests
+
+To run the tests you can use the `pytest` or `coverage` command, for example
+
+```bash
+coverage run --source ftag -m pytest --show-capture=stdout
+```
+
+Running `coverage report` will display the test coverage.
```

### Comparing `atlas-ftag-tools-0.1.0/atlas_ftag_tools.egg-info/SOURCES.txt` & `atlas-ftag-tools-0.1.1/atlas_ftag_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.0/ftag/__init__.py` & `atlas-ftag-tools-0.1.1/ftag/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """atlas-ftag-tools - Common tools for ATLAS flavour tagging software."""
 
 
-__version__ = "v0.1.0"
+__version__ = "v0.1.1"
 
 
 import ftag.hdf5 as hdf5
 from ftag.cuts import Cuts
 from ftag.flavour import Flavour, Flavours
 from ftag.mock import get_mock_file
 from ftag.sample import Sample
```

### Comparing `atlas-ftag-tools-0.1.0/ftag/cuts.py` & `atlas-ftag-tools-0.1.1/ftag/cuts.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.0/ftag/flavour.py` & `atlas-ftag-tools-0.1.1/ftag/flavour.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 class FlavourContainer:
     flavours: dict[str, Flavour]
 
     def __iter__(self) -> Generator:
         yield from self.flavours.values()
 
     def __getitem__(self, key) -> Flavour:
+        if isinstance(key, Flavour):
+            key = key.name
         try:
             return self.flavours[key]
         except KeyError as e:
             raise KeyError(f"Flavour '{key}' not found") from e
 
     def __getattr__(self, name) -> Flavour:
         return self[name]
```

### Comparing `atlas-ftag-tools-0.1.0/ftag/flavours.yaml` & `atlas-ftag-tools-0.1.1/ftag/flavours.yaml`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.0/ftag/hdf5/h5reader.py` & `atlas-ftag-tools-0.1.1/ftag/hdf5/h5reader.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.0/ftag/hdf5/h5utils.py` & `atlas-ftag-tools-0.1.1/ftag/hdf5/h5utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def get_dtype(ds, variables: list[str] | None = None, precision: str | None = None) -> np.dtype:
     """Return a dtype based on an existing dataset and requested variables.
 
     Parameters
     ----------
-    ds : _type_
+    ds : h5py.Dataset
         Input h5 dataset
     variables : list[str] | None, optional
         List of variables to include in dtype, by default None
     precision : str | None, optional
         Precision to cast floats to, "half" or "full", by default None
 
     Returns
@@ -59,15 +59,15 @@
 
     Raises
     ------
     ValueError
         If precision is not "half" or "full"
     """
     t = np.dtype(typestr)
-    if t.kind != "f" or t.itemsize != 2:
+    if t.kind != "f":
         return t
     if precision == "half":
         return np.dtype("f2")
     if precision == "full":
         return np.dtype("f4")
     raise ValueError(f"Invalid precision {precision}")
```

### Comparing `atlas-ftag-tools-0.1.0/ftag/hdf5/h5writer.py` & `atlas-ftag-tools-0.1.1/ftag/hdf5/h5writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
-from subprocess import check_output
 
 import h5py
 import numpy as np
 
+import ftag
 from ftag.hdf5 import get_dtype
 
 
 @dataclass
 class H5Writer:
     src: Path | str
     dst: Path | str
@@ -26,17 +26,15 @@
 
     def __post_init__(self):
         self.src = Path(self.src)
         self.dst = Path(self.dst)
         self.dst.parent.mkdir(parents=True, exist_ok=True)
         self.file = h5py.File(self.dst, "w")
         self.add_attr("srcfile", str(self.src))
-        git_hash = check_output(["git", "rev-parse", "--short", "HEAD"], cwd=Path(__file__).parent)
-        self.git_hash = git_hash.decode("ascii").strip()
-        self.add_attr("writer_hash", self.git_hash)
+        self.add_attr("writer_version", ftag.__version__)
         for name, var in self.variables.items():
             self.create_ds(name, var)
 
     def create_ds(self, name: str, variables: list[str]) -> None:
         with h5py.File(self.src) as f:
             dtype = get_dtype(f[name], variables, self.precision)
             if name == self.jets_name and self.add_flavour_label:
```

### Comparing `atlas-ftag-tools-0.1.0/ftag/mock.py` & `atlas-ftag-tools-0.1.1/ftag/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     return e_x / e_x.sum(axis=axis, keepdims=True)
 
 
 def get_mock_scores(labels: np.ndarray):
     rng = np.random.default_rng(42)
     scores = np.zeros((len(labels), 3))
     for label, count in zip(*np.unique(labels, return_counts=True)):
-        if label == 0:
+        if label == 0 or label == 15:
             scores[labels == label] = rng.normal(loc=[2, 0, 0], scale=1, size=(count, 3))
         elif label == 4:
             scores[labels == label] = rng.normal(loc=[0, 1, 0], scale=2.5, size=(count, 3))
         elif label == 5:
             scores[labels == label] = rng.normal(loc=[0, 0, 3.5], scale=5, size=(count, 3))
     scores = softmax(scores, axis=1)
     cols = [f"MockTagger_p{x}" for x in ["u", "c", "b"]]
@@ -72,15 +72,15 @@
 
 
 def get_mock_file(num_jets=1000, tracks_name: str = "tracks", num_tracks: int = 40):
     # setup jets
     rng = np.random.default_rng(42)
     jets_dtype = np.dtype(JET_VARS)
     jets = u2s(rng.random((num_jets, len(JET_VARS))), jets_dtype)
-    jets["HadronConeExclTruthLabelID"] = rng.choice([0, 4, 5], size=num_jets)
+    jets["HadronConeExclTruthLabelID"] = rng.choice([0, 4, 5, 15], size=num_jets)
     jets["flavour_label"] = rng.choice([0, 4, 5], size=num_jets)
     jets["pt"] *= 400e3
     jets["mass"] *= 50e3
     jets["eta"] = (jets["eta"] - 0.5) * 6.0
     jets["abs_eta"] = np.abs(jets["eta"])
     jets["n_truth_promptLepton"] = 0
```

### Comparing `atlas-ftag-tools-0.1.0/ftag/sample.py` & `atlas-ftag-tools-0.1.1/ftag/sample.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.0/ftag/vds.py` & `atlas-ftag-tools-0.1.1/ftag/vds.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.0/ftag/wps/discriminant.py` & `atlas-ftag-tools-0.1.1/ftag/wps/discriminant.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.0/ftag/wps/working_points.py` & `atlas-ftag-tools-0.1.1/ftag/wps/working_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
         # calculate discriminant
         disc = get_discriminant(jets, tagger, Flavours[args.signal], fx)
         sig_disc = disc[flavs[args.signal].cuts(jets).idx]
 
         # loop over efficiency working points
         for eff in args.effs:
-            d = out[tagger][eff] = {}
+            d = out[tagger][f"{eff:.0f}"] = {}
 
             # calculate working point
             wp = d["cut_value"] = round(float(np.percentile(sig_disc, 100 - eff)), 3)
 
             # calculate eff and rej for each flavour
             d["ttbar"] = get_eff_rej(jets, disc, wp, flavs)
```

### Comparing `atlas-ftag-tools-0.1.0/pyproject.toml` & `atlas-ftag-tools-0.1.1/pyproject.toml`

 * *Files identical despite different names*

