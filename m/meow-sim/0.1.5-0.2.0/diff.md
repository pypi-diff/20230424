# Comparing `tmp/meow-sim-0.1.5.tar.gz` & `tmp/meow-sim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.1.5.tar", last modified: Tue Apr  4 14:17:50 2023, max compression
+gzip compressed data, was "meow-sim-0.2.0.tar", last modified: Mon Apr 24 18:58:49 2023, max compression
```

## Comparing `meow-sim-0.1.5.tar` & `meow-sim-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:17:50.250259 meow-sim-0.1.5/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-04-04 14:17:45.000000 meow-sim-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2219 2023-04-04 14:17:50.250259 meow-sim-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1262 2023-04-04 14:17:45.000000 meow-sim-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:17:50.250259 meow-sim-0.1.5/meow/
--rw-r--r--   0 root         (0) root         (0)     1322 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:17:50.250259 meow-sim-0.1.5/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:17:50.250259 meow-sim-0.1.5/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4608 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:17:50.250259 meow-sim-0.1.5/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3440 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)     9206 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10776 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)     9797 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     2677 2023-04-04 14:17:45.000000 meow-sim-0.1.5/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:17:50.250259 meow-sim-0.1.5/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2219 2023-04-04 14:17:50.000000 meow-sim-0.1.5/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      657 2023-04-04 14:17:50.000000 meow-sim-0.1.5/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 14:17:50.000000 meow-sim-0.1.5/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-04 14:17:50.000000 meow-sim-0.1.5/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-04 14:17:50.000000 meow-sim-0.1.5/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1585 2023-04-04 14:17:45.000000 meow-sim-0.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 14:17:50.250259 meow-sim-0.1.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:17:50.250259 meow-sim-0.1.5/tests/
--rw-r--r--   0 root         (0) root         (0)     4008 2023-04-04 14:17:45.000000 meow-sim-0.1.5/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-04-04 14:17:45.000000 meow-sim-0.1.5/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.508033 meow-sim-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-04-24 18:58:44.000000 meow-sim-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3105 2023-04-24 18:58:49.508033 meow-sim-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-04-24 18:58:44.000000 meow-sim-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.496033 meow-sim-0.2.0/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.496033 meow-sim-0.2.0/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.500033 meow-sim-0.2.0/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.500033 meow-sim-0.2.0/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)     9206 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10776 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     9797 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.504033 meow-sim-0.2.0/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3105 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      657 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-04-24 18:58:44.000000 meow-sim-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:58:49.508033 meow-sim-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.508033 meow-sim-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4008 2023-04-24 18:58:44.000000 meow-sim-0.2.0/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-04-24 18:58:44.000000 meow-sim-0.2.0/tests/test_nbs.py
```

### Comparing `meow-sim-0.1.5/LICENSE` & `meow-sim-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/PKG-INFO` & `meow-sim-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.1.5
+Version: 0.2.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -15,30 +15,60 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: min
+Provides-Extra: jax
+Provides-Extra: klu
+Provides-Extra: ipy
+Provides-Extra: gds
+Provides-Extra: dev
+Provides-Extra: full
 License-File: LICENSE
 
 # meow
 
 > **M**odeling of **E**igenmodes and **O**verlaps in **W**aveguides
 
 ![meow](https://flaport.github.io/meow/_static/meow.png)
 
 A simple electromagnetic [EigenMode Expansion (EME)](https://en.wikipedia.org/wiki/Eigenmode_expansion) tool for Python.
 
 ## Installation
 
+### Minimal installation
 ```sh
-pip install meow-sim
+pip install meow-sim[min]
 ```
 
+### Full installation
+```sh
+pip install meow-sim[full]
+```
+
+### Selecting features
+You can select which features to enable during installation as follows:
+```sh
+pip install meow-sim[feature1,feature2,...]
+```
+
+#### Available features
+* `min`: minimal installation (equivalent to not specifying any features)
+* `jax`: use JAX in stead of numpy to calculate the S-matrices
+* `klu`: use `klujax` to speed up S-matric calculations (implies `jax`). Note: you need
+the SuiteSparse headers on your computer for this to work.
+* `gds`: enable GDS creation with GDSFactory (see GDS Taper example).
+* `ipy`: install useful jupyter/ipython packages.
+* `dev`: install dev dependencies
+* `full`: enable all the above features.
+
+
 ## Documentation
 
 - [Examples](https://flaport.github.io/meow/examples.html)
 - [API Docs](https://flaport.github.io/meow/meow.html)
 
 ## Credits
```

### Comparing `meow-sim-0.1.5/meow/__init__.py` & `meow-sim-0.2.0/meow/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.1.5"
+__version__ = "0.2.0"
+
+import warnings
 
 # Silence Excessive Logging...
 
-from loguru import logger
+try:
+    from loguru import logger
 
-logger.disable("gdsfactory")
-from numexpr.utils import log
+    logger.disable("gdsfactory")
+except ImportError:
+    pass
 
-log.setLevel("CRITICAL")
+try:
+    from numexpr.utils import log
 
+    log.setLevel("CRITICAL")
+except ImportError:
+    pass
 
-# disable rich pretty printing enabled by tidy3d (if I want it, I'll enable it myself...)
-from rich import pretty
+try:
+    from rich import pretty
 
-old_install = pretty.install
-pretty.install = lambda *_, **__: None
-import tidy3d
+    old_install = pretty.install
+    pretty.install = lambda *_, **__: None
+    import tidy3d
 
-pretty.install = old_install
+    pretty.install = old_install
+except ImportError:
+    pass
 
-import warnings
 
-warnings.filterwarnings(action="ignore", module="sax")
-import sax
+try:
+    import sax
+
+    warnings.filterwarnings(action="ignore", module="sax")
+except ImportError:
+    pass
 
 # from . import cell as cell
 from . import base_model as base_model
 from . import cross_section as cross_section
 from . import eme as eme
 from . import environment as environment
 from . import fde as fde
```

### Comparing `meow-sim-0.1.5/meow/assets/silicon.csv` & `meow-sim-0.2.0/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/assets/silicon_oxide.csv` & `meow-sim-0.2.0/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/base_model.py` & `meow-sim-0.2.0/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/cache.py` & `meow-sim-0.2.0/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/cell.py` & `meow-sim-0.2.0/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/cross_section.py` & `meow-sim-0.2.0/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/eme/__init__.py` & `meow-sim-0.2.0/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/eme/common.py` & `meow-sim-0.2.0/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/eme/sax.py` & `meow-sim-0.2.0/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/environment.py` & `meow-sim-0.2.0/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/fde/lumerical.py` & `meow-sim-0.2.0/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/fde/tidy3d.py` & `meow-sim-0.2.0/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/gds_structures.py` & `meow-sim-0.2.0/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/geometries.py` & `meow-sim-0.2.0/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/integrate.py` & `meow-sim-0.2.0/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/materials.py` & `meow-sim-0.2.0/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/mesh.py` & `meow-sim-0.2.0/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/mode.py` & `meow-sim-0.2.0/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/structures.py` & `meow-sim-0.2.0/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow/visualize.py` & `meow-sim-0.2.0/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.2.0/meow_sim.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.1.5
+Version: 0.2.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -15,30 +15,60 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: min
+Provides-Extra: jax
+Provides-Extra: klu
+Provides-Extra: ipy
+Provides-Extra: gds
+Provides-Extra: dev
+Provides-Extra: full
 License-File: LICENSE
 
 # meow
 
 > **M**odeling of **E**igenmodes and **O**verlaps in **W**aveguides
 
 ![meow](https://flaport.github.io/meow/_static/meow.png)
 
 A simple electromagnetic [EigenMode Expansion (EME)](https://en.wikipedia.org/wiki/Eigenmode_expansion) tool for Python.
 
 ## Installation
 
+### Minimal installation
 ```sh
-pip install meow-sim
+pip install meow-sim[min]
 ```
 
+### Full installation
+```sh
+pip install meow-sim[full]
+```
+
+### Selecting features
+You can select which features to enable during installation as follows:
+```sh
+pip install meow-sim[feature1,feature2,...]
+```
+
+#### Available features
+* `min`: minimal installation (equivalent to not specifying any features)
+* `jax`: use JAX in stead of numpy to calculate the S-matrices
+* `klu`: use `klujax` to speed up S-matric calculations (implies `jax`). Note: you need
+the SuiteSparse headers on your computer for this to work.
+* `gds`: enable GDS creation with GDSFactory (see GDS Taper example).
+* `ipy`: install useful jupyter/ipython packages.
+* `dev`: install dev dependencies
+* `full`: enable all the above features.
+
+
 ## Documentation
 
 - [Examples](https://flaport.github.io/meow/examples.html)
 - [API Docs](https://flaport.github.io/meow/meow.html)
 
 ## Credits
```

### Comparing `meow-sim-0.1.5/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.2.0/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/pyproject.toml` & `meow-sim-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["build", "pip", "setuptools", "wheel"]
+requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.1.5"
+version = "0.2.0"
 authors = [
-  { name = "Rockley Photonics" },
-  { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
+{ name = "Rockley Photonics" },
+{ name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
   "eigenmodes",
   "eme",
   "fde",
@@ -32,33 +32,33 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
-  "fastprogress",
-  "flatten-dict",
-  "loguru",
-  "mapbox-earcut",
   "matplotlib",
-  "numexpr",
-  "numpy",
-  "orjson",
+  "numpy>=1.24",
   "pydantic",
-  "rich",
   "sax>=0.8.4",
   "scipy",
   "shapely",
-  "tidy3d>2",
-  "tqdm",
-  "triangle",
+  "tidy3d>=2.1",
   "trimesh[easy]",
 ]
 
+[project.optional-dependencies]
+min = ["meow-sim"]
+jax = ["jax", "jaxlib"]
+klu = ["klujax>0.1.2"]
+ipy = ["ipykernel", "ipywidgets", "ipympl", "nbstripout", "tqdm"]
+gds = ["gdsfactory>6.27.0", "klayout>0.28.2"]
+dev = ["bump2version", "nbstripout", "pre-commit", "black", "sphinx", "autodoc-pydantic", "myst-nb>0.17.1"]
+full = ["meow-sim[klu,jax,ipy,gds]"]
+
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["meow*"]
 exclude = []
 namespaces = true
 
 [tool.setuptools.package-data]
```

### Comparing `meow-sim-0.1.5/tests/test_deserialization.py` & `meow-sim-0.2.0/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.1.5/tests/test_nbs.py` & `meow-sim-0.2.0/tests/test_nbs.py`

 * *Files identical despite different names*

