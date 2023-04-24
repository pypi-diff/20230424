# Comparing `tmp/openpile-0.1.0.tar.gz` & `tmp/openpile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-g6d0dqm8/openpile-0.1.0.tar", last modified: Mon Apr 10 19:22:42 2023, max compression
+gzip compressed data, was "/home/runner/work/openpile/openpile/dist/.tmp-95t1783b/openpile-0.2.0.tar", last modified: Mon Apr 24 19:19:03 2023, max compression
```

## Comparing `openpile-0.1.0.tar` & `openpile-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 19:22:26.000000 openpile-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-10 19:22:42.000000 openpile-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-10 19:22:26.000000 openpile-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 19:22:26.000000 openpile-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-10 19:22:42.000000 openpile-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-10 19:22:26.000000 openpile-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/analyses.py
--rw-r--r--   0 runner    (1001) docker     (123)    47018 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/soilmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/Hb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/Mb_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/mt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/py_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/qz_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-10 19:22:26.000000 openpile-0.1.0/src/openpile/utils/tz_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 19:22:42.000000 openpile-0.1.0/src/openpile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:22:42.000000 openpile-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-10 19:22:26.000000 openpile-0.1.0/test/test_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-10 19:22:26.000000 openpile-0.1.0/test/test_pycurves.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-10 19:22:26.000000 openpile-0.1.0/test/test_utils_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 19:18:54.000000 openpile-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 19:19:03.000000 openpile-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-24 19:18:54.000000 openpile-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-24 19:18:54.000000 openpile-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-24 19:19:03.000000 openpile-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 19:18:54.000000 openpile-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/analyses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51654 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18197 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/soilmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/Hb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/Mb_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/mt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/py_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/qz_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-24 19:18:54.000000 openpile-0.2.0/src/openpile/utils/tz_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 19:19:03.000000 openpile-0.2.0/src/openpile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:19:03.000000 openpile-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-24 19:18:54.000000 openpile-0.2.0/test/test_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 19:18:54.000000 openpile-0.2.0/test/test_pycurves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 19:18:54.000000 openpile-0.2.0/test/test_utils_misc.py
```

### Comparing `openpile-0.1.0/LICENSE.txt` & `openpile-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/PKG-INFO` & `openpile-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,44 @@
-Metadata-Version: 2.1
-Name: openpile
-Version: 0.1.0
-Summary: Library for geotechnical pile calculations.
-Home-page: https://github.com/TchilDill/openpile
-Author: Guillaume Melin
-Author-email: guillaume.melin@icloud.com
-License: GPLv3
-Keywords: Offshore Wind,PILE,Geotechnics,monopile,pin-piles,Geotechnical,calculations,PISA,winkler
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
-
-[![Visual Studio](https://badgen.net/badge/icon/visualstudio?icon=visualstudio&label)](https://visualstudio.microsoft.com)
+[![Downloads](https://static.pepy.tech/badge/openpile)](https://pepy.tech/project/openpile)
 
 ![Tests](https://github.com/TchilDill/openpile/actions/workflows/Test.yml/badge.svg) 
 [![Documentation Status](https://readthedocs.org/projects/openpile/badge/?version=latest)](https://openpile.readthedocs.io/en/latest/?badge=latest)
-[![Github All Releases](https://img.shields.io/github/downloads/TchilDill/openpile/total.svg)]()
+
 
 [![issues closed](https://img.shields.io/github/issues-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/issues)
 [![PRs closed](https://img.shields.io/github/issues-pr-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/pulls)
 [![GitHub last commit](https://img.shields.io/github/last-commit/TchilDill/openpile)](https://github.com/TchilDill/openpile/commits/master)
 [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 
 Please see [official documentation](https://openpile.readthedocs.io/en/latest/) for more information.
 
+This package is an open source python library that provides users a tool box for geotechnical pile
+calculations.
+
+This package allows the user to:
+
+* Use basic Euler-Bernoulli beam theory (as well as Timoshenko's variation) to compute 
+  forces, deflection of a beam (or a pile) under adequate loading and 
+  support conditions.
+* Use Winkler's approach of a beam (or a pile) supported by linear or non-linear lateral and/or 
+  rotational springs to compute forces and deflection of the pile based on recognised 
+  soil models such as the widely used traditional API models for sand and clay or more recent models that stem from 
+  the PISA joint-industry project.
+
+This library supports the following versions of python: 3.7-3.10.
+Python 3.11 is not supported!
+
 ## Installation Instructions
 
 **Prerequisites**:
 
 * a version of python is installed on your machine (supported versions: 3.7-3.10)
 * pip is installed in your environment.
 
@@ -53,24 +47,25 @@
 ```
 
 ## Features
 
  * Python 3.7-3.10 support
  * Interactive structure perfectly suited for Jupyter Notebook 
  * Integrated data validation to prevent wrong inputs with pydantic
+ * very fast computations fueled by the Numpy, Numba and Pandas libraries
  * Calculations
    * Beam calculation
    * Winkler model (i.e. beam supported by soil springs)
      * Load-driven analyses
      * Displacement-driven analyses 
    * Out-of-the-box computation of individual soil springs
    <!-- * Axial capacity calculations via integration -->
- * Friendly API interface with  object-oriented approach
- * Fully integrated output with python environment with Matplotlib and Pandas libraries. 
+ * Friendly API interface with object-oriented approach
+ * Matplotlib and Pandas libraries to facilitate post-processing of results. 
 
  ## Please share with the community
 
 This library relies on community interactions. Please consider sharing a post about `OpenPile` and the value it can provide for researcher, academia and professionals.
 
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-reddit-red?logo=reddit)](https://reddit.com/submit?url=https://github.com/TchilDill/openpile&title=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/TchilDill/openpile&t=openpile)
-[![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/TchilDill/openpile&title=openpile)
+[![GitHub Repo stars](https://img.shields.io/badge/share%20on-linkedin-3949AB?logo=linkedin)](https://www.linkedin.com/shareArticle?url=https://github.com/TchilDill/openpile&title=openpile)
```

### Comparing `openpile-0.1.0/setup.cfg` & `openpile-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Operating System :: OS Independent
 
 [options]
 zip_safe = False
 include_package_data = True
 package_dir = 
 	= src
 packages = find:
```

### Comparing `openpile-0.1.0/src/openpile/analyses.py` & `openpile-0.2.0/src/openpile/analyses.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,42 @@
 import openpile.core.misc as misc
 
 
 class PydanticConfig:
     arbitrary_types_allowed = True
 
 
+def springs_mob_to_df(model, d):
+
+    # elevations
+    x = model.nodes_coordinates["x [m]"].values
+    x = kernel.double_inner_njit(x)
+
+    # PY springs
+    # py secant stiffness
+    py_ks = kernel.calculate_py_springs_stiffness(
+        u=d[1::3], springs=model._py_springs, kind="secant"
+    ).flatten()
+    py_u = kernel.double_inner_njit(d[1::3])
+    py_mob = py_u * py_ks
+    # calculate max spring values
+    max_springs_values = model._py_springs[:, :, 0].max(axis=2).flatten()
+
+    # create DataFrame
+    df = pd.DataFrame(
+        data={
+            "Elevation [m]": x,
+            "p_mobilized [kN/m]": np.abs(py_mob),
+            "p_max [kN/m]": max_springs_values,
+        }
+    )
+
+    return df
+
+
 def structural_forces_to_df(model, q):
     x = model.nodes_coordinates["x [m]"].values
     x = misc.repeat_inner(x)
     L = kernel.mesh_to_element_length(model).reshape(-1)
 
     N = np.vstack((-q[0::6], q[3::6])).reshape(-1, order="F")
     V = np.vstack((-q[1::6], q[4::6])).reshape(-1, order="F")
@@ -66,14 +94,15 @@
 
 
 @dataclass(config=PydanticConfig)
 class Result:
     name: str
     displacements: pd.DataFrame
     forces: pd.DataFrame
+    springs_mobilization: pd.DataFrame
 
     class Config:
         frozen = True
 
     @property
     def settlement(self):
         """Retrieves degrees of freedom for settlement
@@ -103,14 +132,25 @@
         Returns
         -------
         pandas.DataFrame
             Table with the nodes elevations along the pile and their rotations
         """
         return self.displacements[["Elevation [m]", "Rotation [rad]"]]
 
+    @property
+    def py_mobilization(self):
+        """Retrieves mobilized resistance of p-y curves.
+
+        Returns
+        -------
+        pandas.DataFrame
+            Table with the nodes elevations along the pile and the mobilized resistance in kN/m.
+        """
+        return self.springs_mobilization[["Elevation [m]", "p_mobilized [kN/m]", "p_max [kN/m]"]]
+
     def plot_deflection(self, assign=False):
         """
         Plots the deflection of the pile.
 
         Parameters
         ----------
         assign : bool, optional
@@ -215,27 +255,25 @@
             displacements=disp_to_df(model, u),
             forces=structural_forces_to_df(model, q_int),
         )
 
         return results
 
 
-def simple_winkler_analysis(model, solver="NR", max_iter: int = 100):
+def simple_winkler_analysis(model, max_iter: int = 100):
     """
     Function where loading or displacement defined in the model boundary conditions
     are used to solve the system of equations, .
 
     #TODO
 
     Parameters
     ----------
     model : `openpile.construct.Model` object
         Model where structure and boundary conditions are defined.
-    solver: str, by default 'MNR'
-        solver. literally 'NR': "Newton-Raphson" or 'MNR': "Modified Newton-Raphson"
     max_iter: int, by defaut 100
         maximum number of iterations for convergence
 
     Returns
     -------
     results : `openpile.analyses.Result` object
         Results of the analysis
@@ -249,30 +287,29 @@
         F = kernel.mesh_to_global_force_dof_vector(model.global_forces)
         # initiliase prescribed displacement vector
         U = kernel.mesh_to_global_disp_dof_vector(model.global_disp)
         # initialise displacement vectors
         d = np.zeros(U.shape)
 
         # initialise global stiffness matrix
-        K = kernel.build_stiffness_matrix(model, u=d, kind="initial")
-
+        K = kernel.build_stiffness_matrix(model, f=None, u=d, kind="initial")
+        # initialise internal forces
+        q_int = np.zeros((model.element_number * 6))
         # initialise global supports vector
         supports = kernel.mesh_to_global_restrained_dof_vector(model.global_restrained)
 
         # validate boundary conditions
         # validation.check_boundary_conditions(model)
 
         # Initialise residual forces
         Rg = F
 
         # incremental calculations to convergence
         iter_no = 0
-        while iter_no <= 100:
-            iter_no += 1
-
+        while iter_no <= max_iter:
             # solve system
             try:
                 u_inc, Q = kernel.solve_equations(K, Rg, U, restraints=supports)
             except np.linalg.LinAlgError:
                 print(
                     """Cannot converge. Failure of the pile-soil system.\n
                       Boundary conditions may not be realistic or values may be too large."""
@@ -282,47 +319,49 @@
             # External forces
             F_ext = F - Q
             control = np.linalg.norm(F_ext)
 
             # add up increment displacements
             d += u_inc
 
-            # internal forces
-            K_secant = kernel.build_stiffness_matrix(model, u=d, kind="secant")
-            F_int = K_secant.dot(d)
+            # calculate internal forces
+            K_secant = kernel.build_stiffness_matrix(model, f=q_int, u=d, kind="secant")
+            F_int = -K_secant.dot(d)
 
             # calculate residual forces
-            Rg = F_ext - F_int
+            Rg = F_ext + F_int
 
             # check if converged
             if np.linalg.norm(Rg[~supports]) < 1e-4 * control:
-                print(f"Converged at iteration no. {iter_no}")
-                break
+                # do not accept convergence without iteration (without a second call to solve equations)
+                if iter_no > 0:
+                    print(f"Converged at iteration no. {iter_no}")
+                    break
 
             if iter_no == 100:
                 print("Not converged after 100 iterations.")
 
+            # Internal forces calculations with dim(nelem,6,6)
+            q_int = kernel.struct_internal_force(model, q_int, d)
+
             # re-calculate global stiffness matrix for next iterations
-            if solver == "NR":
-                K = kernel.build_stiffness_matrix(model, u=d, kind="tangent")
-            elif solver == "MNR":
-                if model.distributed_moment:
-                    pass
-                    # K = kernel.build_stiffness_matrix(model, u=d, kind="initial")
-                else:
-                    pass
+            K = kernel.build_stiffness_matrix(model, f=q_int, u=d, kind="tangent")
 
             # reset prescribed displacements to converge properly in case
             # of displacement-driven analysis
             U[:] = 0.0
 
+            # nump iteration number
+            iter_no += 1
+
         # Internal forces calculations with dim(nelem,6,6)
-        q_int = kernel.struct_internal_force(model, d)
+        q_int = kernel.struct_internal_force(model, q_int, d)
 
         # Final results
         results = Result(
             name=f"{model.name} ({model.pile.name}/{model.soil.name})",
             displacements=disp_to_df(model, d),
             forces=structural_forces_to_df(model, q_int),
+            springs_mobilization=springs_mob_to_df(model, d),
         )
 
         return results
```

### Comparing `openpile-0.1.0/src/openpile/construct.py` & `openpile-0.2.0/src/openpile/construct.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 >>> from openpile.construct import Pile, SoilProfile, Layer, Model
 
 """
 
 import math as m
 import pandas as pd
 import numpy as np
+import warnings
 from typing import List, Dict, Optional, Union
 from typing_extensions import Literal
 from pydantic import (
     BaseModel,
     Field,
     root_validator,
     validator,
     PositiveFloat,
     confloat,
     conlist,
+    constr,
     Extra,
 )
 from pydantic.dataclasses import dataclass
 import matplotlib.pyplot as plt
 
 import openpile.utils.graphics as graphics
 import openpile.core.validation as validation
@@ -47,37 +49,46 @@
 
 from openpile.core.misc import generate_color_string
 
 
 class PydanticConfig:
     arbitrary_types_allowed = True
     extra = Extra.forbid
+    post_init_call = "after_validation"
 
 
 @dataclass(config=PydanticConfig)
 class Pile:
     """
     A class to create the pile.
 
-    Pile instances include the pile geometry and data. Following
-    the initialisation of a pile, a Pandas dataframe is created
-    which can be read by the following command:
-
-    .. note::
-        The classmethod :py:meth:`openpile.construct.Pile.create` shall be used to create a Pile instance.
+    Parameters
+    ----------
+    name : str
+        Pile/Structure's name.
+    top_elevation : float
+        top elevation of the pile. Note that this elevation provides a reference point to
+        know where the pile is located, especially with respect to other object such as a SoilProfile.
+    pile_sections : Dict[str, List[float]]
+        argument that stores the relevant data of each pile segment.
+        Below are the needed keys for the available piles:
+        - kind:'Circular' >> keys:['length', 'diameter', 'wall thickness']
+    kind : Literal["Circular",]
+        type of pile or type of cross-section. by default "Circular"
+    material : Literal["Steel",]
+        material the pile is made of. by default "Steel"
 
-        This method ensures that the post-initialization of the `Pile` instance and post processing is done accordingly.
 
     Example
     -------
 
     >>> from openpile.construct import Pile
 
     >>> # Create a pile instance with two sections of respectively 10m and 30m length.
-    >>> pile = Pile.create(name = "",
+    >>> pile = Pile(name = "",
     >>>         kind='Circular',
     >>>         material='Steel',
     >>>         top_elevation = 0,
     >>>         pile_sections={
     >>>             'length':[10,30],
     >>>             'diameter':[7.5,7.5],
     >>>             'wall thickness':[0.07, 0.08],
@@ -93,15 +104,15 @@
     material: Literal["Steel"]
     #: top elevation of the pile according to general vertical reference set by user
     top_elevation: float
     #: pile geometry made of a dictionary of lists. the structure of the dictionary depends on the type of pile selected.
     #: There can be as many sections as needed by the user. The length of the listsdictates the number of pile sections.
     pile_sections: Dict[str, List[PositiveFloat]]
 
-    def _postinit(self):
+    def __post_init__(self):
         # check that dict is correctly entered
         validation.pile_sections_must_be(self)
 
         # Create material specific specs for given material
         # if steel
         if self.material == "Steel":
             # unit weight
@@ -185,19 +196,15 @@
         kind: Literal[
             "Circular",
         ] = "Circular",
         material: Literal[
             "Steel",
         ] = "Steel",
     ):
-        """A method to create the pile. This function provides a 2-in-1 command where:
-
-        - a `Pile` instance is created
-        - the `._postinit()` method is run and creates all additional pile data necessary.
-
+        """A method to create the pile.
 
         Parameters
         ----------
         name : str
             Pile/Structure's name.
         top_elevation : float
             top elevation of the pile. Note that this elevation provides a reference point to
@@ -220,33 +227,109 @@
         obj = cls(
             name=name,
             kind=kind,
             material=material,
             top_elevation=top_elevation,
             pile_sections=pile_sections,
         )
-        obj._postinit()
+
+        warnings.warn(
+            "\nThe method Pile.create() will be removed in version 1.0.0."
+            "\nPlease use the base class to create a Pile instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+        return obj
+
+    @classmethod
+    def create_tubular(
+        cls,
+        name: str,
+        top_elevation: float,
+        bottom_elevation: float,
+        diameter: float,
+        wt: float,
+        material: str = "Steel",
+    ):
+        """A method to simplify the creation of a Pile instance.
+        This method creates a circular and hollow pile of constant diameter.
+
+        Parameters
+        ----------
+        name : str
+            Pile/Structure's name.
+        top_elevation : float
+            top elevation of the pile [m VREF]
+        bottom_elevation : float
+            bottom elevation of the pile [m VREF]
+        diameter : float
+            pile diameter [m]
+        wt : float
+            pile's wall thickness [m]
+        material : Literal["Steel",]
+            material the pile is made of. by default "Steel"
+
+        Returns
+        -------
+        openpile.construct.Pile
+            a Pile instance.
+        """
+
+        obj = cls(
+            name=name,
+            kind="Circular",
+            material=material,
+            top_elevation=top_elevation,
+            pile_sections={
+                "length": [
+                    (top_elevation - bottom_elevation),
+                ],
+                "wall thickness": [
+                    wt,
+                ],
+                "diameter": [
+                    diameter,
+                ],
+            },
+        )
 
         return obj
 
     @property
     def bottom_elevation(self) -> float:
         """
-        Bottom elevation of the pile.
+        Bottom elevation of the pile [m VREF].
         """
         return self.top_elevation - sum(self.pile_sections["length"])
 
     @property
     def length(self) -> float:
         """
-        Pile length.
+        Pile length [m].
         """
         return sum(self.pile_sections["length"])
 
     @property
+    def volume(self) -> float:
+        """
+        Pile volume [m3].
+        """
+        A = self.data["Area [m2]"].values[1:]
+        L = np.abs(np.diff(self.data["Elevation [m]"].values))
+        return round((A * L).sum(), 2)
+
+    @property
+    def weight(self) -> float:
+        """
+        Pile weight [kN].
+        """
+        return round(self.volume * self._uw, 2)
+
+    @property
     def E(self) -> float:
         """
         Young modulus of the pile material. Thie value does not vary across and along the pile.
         """
         try:
             return self._young_modulus
         except AttributeError:
@@ -264,84 +347,118 @@
             print(e)
 
     @property
     def I(self) -> float:
         """
         Second moment of area of the pile.
 
-        If user-defined, the whole
-        second moment of area of the pile is overriden.
+        The user can use the method :py:meth:`openpile.construct.Pile.set_I` to customise the second
+        moment of area for different sections of the pile.
         """
         try:
-            return self.data["I [m4]"].mean()
+            return self.data["I [m4]"]
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
-    @I.setter
-    def I(self, value: float) -> None:
+    def set_I(self, value: float, section: int) -> None:
+        """set second moment of area for a particular section of the pile.
+
+        Parameters
+        ----------
+        value : float
+            new second moment of area [m4].
+        section : int
+            section number for which to set new second moment of area
+
+        """
         try:
-            self.data.loc[:, "I [m4]"] = value
-            self.data.loc[:, ["Wall thickness [m]"]] = pd.NA
+            length = len(self.data["I [m4]"].values)
+            if section * 2 > length:
+                print("section number is too large")
+            elif section < 1:
+                print("section number must be 1 or above")
+            else:
+                self.data.loc[section * 2 - 2, "I [m4]"] = value
+                self.data.loc[section * 2 - 1, "I [m4]"] = value
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
-            print(e)
+            raise Exception
 
     @property
     def width(self) -> float:
         """
         Width of the pile. (Used to compute soil springs)
         """
         try:
-            return self.data["Diameter [m]"].mean()
+            return self.data.loc[:, "Diameter [m]"]
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
     @width.setter
     def width(self, value: float) -> None:
         try:
             self.data.loc[:, "Diameter [m]"] = value
-            self.data.loc[:, ["Wall thickness [m]"]] = pd.NA
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
     @property
     def area(self) -> float:
+        "Sectional area of the pile"
         try:
-            return self.data["Area [m2]"].mean()
+            return self.data.loc[:, "Area [m2]"]
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
     @area.setter
     def area(self, value: float) -> None:
         try:
             self.data.loc[:, "Area [m2]"] = value
-            self.data.loc[:, ["Wall thickness [m]"]] = pd.NA
         except AttributeError:
             print("Please first create the pile with the Pile.create() method")
         except Exception as e:
             print(e)
 
+    def plot(self, assign=False):
+        fig = graphics.pile_plot(self)
+        return fig if assign else None
+
 
 @dataclass(config=PydanticConfig)
 class Layer:
-    """A class to create a layer. The Layer stores information on the soil parameters
-    of the layer as well as the relevant/representative constitutive model (aka. the soil spring).
+    """A class to create a layer.
+
+    The Layer stores information on the soil parameters of the layer as well
+    as the relevant/representative constitutive model (aka. the soil spring).
 
     Parameters
     ----------
-    #TODO
+    name : str
+        Name of the layer, use for printout
+    top : float
+        top elevation of the layer in [m]
+    bottom : float
+        bottom elevation of the layer in [m]
+    weight : float
+        total unit weight in [kN/m3], cannot be lower than 10 kN/m3
+    lateral_model : ConstitutiveModel
+        Lateral soil model of the layer, by default None
+    axial_model : ConstitutiveModel
+        Axial soil model of the layer, by default None
+    color : str
+        soil layer color in HEX format (e.g. '#000000'), by default None
+
 
     Example
     -------
 
     >>> from openpile.construct import Layer
     >>> from openpile.core.soilmodels import API_clay
 
@@ -374,19 +491,19 @@
     #: unit weight in kN of the layer
     weight: confloat(gt=10.0)
     #: Lateral constitutive model of the layer
     lateral_model: Optional[ConstitutiveModel] = None
     #: Axial constitutive model of the layer
     axial_model: Optional[ConstitutiveModel] = None
     #: Layer's color when plotted
-    color: Optional[str] = None
+    color: Optional[constr(min_length=7, max_length=7)] = None
 
     def __post_init__(self):
         if self.color is None:
-            self.color = generate_color_string()
+            self.color = generate_color_string("earth")
 
     def __str__(self):
         return f"Name: {self.name}\nElevation: ({self.top}) - ({self.bottom}) m\nWeight: {self.weight} kN/m3\nLateral model: {self.lateral_model}\nAxial model: {self.axial_model}"
 
     @root_validator
     def check_elevations(cls, values):  # pylint: disable=no-self-argument
         if not values["top"] > values["bottom"]:
@@ -399,27 +516,44 @@
 @dataclass(config=PydanticConfig)
 class SoilProfile:
     """
     A class to create the soil profile. A soil profile consist of a ground elevation (or top elevation)
     with one or more layers of soil.
 
     Additionally, a soil profile can include discrete information at given elevation such as CPT
-    (Cone Penetration Test) data
+    (Cone Penetration Test) data. Not Implemented yet!
+
+    Parameters
+    ----------
+    name : str
+        Name of the soil profile, used for printout and plots
+    top_elevation : float
+        top elevation of the soil profile in [m VREF]
+    water_line : float
+        elevation of the water table in [m VREF]
+    layers : list[Layer]
+        list of layers for the soil profile
+    cpt_data : np.ndarray
+        cpt data table
+        1st col: elevation [m],
+        2nd col: cone resistance [kPa],
+        3rd col: sleeve friction [kPa]
+        4th col: pore pressure u2 [kPa]
 
     Example
     -------
 
     >>> from openpile.construct import SoilProfile, Layer
     >>> from openpile.core.soilmodels import API_sand, API_clay
 
     >>> # Create a two-layer soil profile
     >>> sp = SoilProfile(
     >>>     name="BH01",
     >>>     top_elevation=0,
-    >>>     water_elevation=0,
+    >>>     water_line=0,
     >>>     layers=[
     >>>         Layer(
     >>>             name='Layer0',
     >>>             top=0,
     >>>             bottom=-20,
     >>>             weight=18,
     >>>             lateral_model= API_sand(phi=30, Neq=100)
@@ -459,20 +593,23 @@
     """
 
     #: name of soil profile / borehole / location
     name: str
     #: top of ground elevation with respect to the model reference elevation datum
     top_elevation: float
     #: water elevation (this can refer to sea elevation of water table)
-    water_elevation: float
+    water_line: float
     #: soil layers to consider in the soil propfile
     layers: List[Layer]
     #: Cone Penetration Test data with folloeing structure:
-    #: 1st col: elevation[m], 2nd col: cone resistance[MPa], 3rd col: pore pressure u2 [MPa]
-    #: (the cpt data cannot be given outside the soil profile boundaries defined by the layers)
+    #: 1st col: elevation[m],
+    #: 2nd col: cone resistance[kPa],
+    #: 3rd col: sleeve friction [kPa]
+    #: 4th col: pore pressure u2 [kPa]
+    #: (the cpt data outside the soil profile boundaries will be ignored)
     cpt_data: Optional[np.ndarray] = None
 
     @root_validator
     def check_layers_elevations(cls, values):  # pylint: disable=no-self-argument
         layers = values["layers"]
 
         top_elevations = np.array([x.top for x in layers], dtype=float)
@@ -488,120 +625,122 @@
 
         for i in range(len(top_sorted) - 1):
             if not m.isclose(top_sorted[i + 1], bottom_sorted[i], abs_tol=0.001):
                 raise ValueError("Layers' elevations overlap.")
 
         return values
 
+    def __post_init__(self):
+        pass
+
     def __str__(self):
         """List all layers in table-like format"""
         out = ""
         i = 0
         for layer in self.layers:
             i += 1
             out += f"Layer {i}\n" + "-" * 30 + "\n"
             out += f"{layer}\n" + "~" * 30 + "\n"
         return out
 
-    def _postinit(self):
-        pass
-
     @property
     def bottom_elevation(self) -> float:
         """
         Bottom elevation of the soil profile.
         """
         return self.top_elevation - sum([abs(x.top - x.bottom) for x in self.layers])
 
-    @classmethod
-    def create(
-        cls,
-        name: str,
-        top_elevation: float,
-        water_elevation: float,
-        layers: List[Layer],
-        cpt_data: Optional[np.ndarray] = None,
-    ):
-        obj = cls(
-            name=name,
-            top_elevation=top_elevation,
-            water_elevation=water_elevation,
-            layers=layers,
-            cpt_data=cpt_data,
-        )
-        obj._postinit()
-
-        return obj
+    def plot(self, assign=False):
+        fig = graphics.soil_plot(self)
+        return fig if assign is True else None
 
 
 @dataclass(config=PydanticConfig)
 class Model:
     """
-    A class to create the Model.
+    A class to create a Model.
 
-    The Model is constructed based on the pile geometry/data primarily.
+    A Model is constructed based on the pile geometry/data primarily.
     Additionally, a soil profile can be fed to the Model, and soil springs can be created.
 
-    .. note::
-        The classmethod :py:meth:`openpile.construct.Model.create` shall be used to create a Model instance.
-
-        This method ensures that the post-initialization of the `Model` instance and post processing is done accordingly.
+    Parameters
+    ----------
+    name : str
+        Name of the model
+    pile : Pile
+        Pile instance to be included in the model
+    soil : Optional[SoilProfile], optional
+        SoilProfile instance, by default None
+    element_type : str, optional
+        can be of ['EulerBernoulli','Timoshenko'], by default 'Timoshenko'
+    x2mesh : List[float], optional
+        additional elevations to be included in the mesh, by default none
+    coarseness : float, optional
+        maximum distance in meters between two nodes of the mesh, by default 0.5
+    distributed_lateral : bool, optional
+        include distributed lateral springs, by default True
+    distributed_moment : bool, optional
+        include distributed moment springs, by default False
+    base_shear : bool, optional
+        include lateral spring at pile toe, by default False
+    base_moment : bool, optional
+        include moment spring at pile toe, by default False
 
 
     Example
     -------
 
     >>> from openpile.construct import Pile, Model, Layer
     >>> from openpile.core.soilmodels import API_sand
 
     >>> # create pile
-    >>> p = Pile.create(name = "WTG01",
+    >>> p = Pile(name = "WTG01",
     >>> 		kind='Circular',
     >>> 		material='Steel',
     >>> 		top_elevation = 0,
     >>> 		pile_sections={
     >>> 			'length':[10,30],
     >>> 			'diameter':[7.5,7.5],
     >>> 			'wall thickness':[0.07, 0.08],
     >>> 		}
     >>> 	)
 
     >>> # Create Soil Profile
     >>> sp = SoilProfile(
     >>> 	name="BH01",
     >>> 	top_elevation=0,
-    >>> 	water_elevation=0,
+    >>> 	water_line=0,
     >>> 	layers=[
     >>> 		Layer(
     >>> 			name='Layer0',
     >>> 			top=0,
     >>> 			bottom=-40,
     >>> 			weight=18,
     >>> 			lateral_model= API_sand(phi=30, Neq=100)
     >>> 		),
     >>> 	]
     >>> )
 
     >>> # Create Model
-    >>> M = Model.create(name="Example", pile=p, soil=sp)
+    >>> M = Model(name="Example", pile=p, soil=sp)
 
     >>> # create Model without soil maximum 5 metres apart.
-    >>> Model_without_soil = Model.create(name = "Example without soil", pile=p, coarseness=5)
+    >>> Model_without_soil = Model(name = "Example without soil", pile=p, coarseness=5)
     >>> # create Model with nodes maximum 1 metre apart with soil profile
-    >>> Model_with_soil = Model.create(name = "Example with soil", pile=p, soil=sp, coarseness=1)
+    >>> Model_with_soil = Model(name = "Example with soil", pile=p, soil=sp, coarseness=1)
 
     """
 
     #: model name
     name: str
     #: pile instance that the Model should consider
     pile: Pile
     #: soil profile instance that the Model should consider
     soil: Optional[SoilProfile] = None
-    #: "EB" for Euler-Bernoulli or "T" for Timoshenko
+    #: type of beam elements
     element_type: Literal["Timoshenko", "EulerBernoulli"] = "Timoshenko"
     #: x coordinates values to mesh as nodes
     x2mesh: List[float] = Field(default_factory=list)
     #: mesh coarseness, represent the maximum accepted length of elements
     coarseness: float = 0.5
     #: whether to include p-y springs in the calculations
     distributed_lateral: bool = True
@@ -612,15 +751,15 @@
     #: whether to include Mb-t spring in the calculations
     base_moment: bool = True
     #: whether to include t-z springs in the calculations
     distributed_axial: bool = False
     #: whether to include Q-z spring in the calculations
     base_axial: bool = False
 
-    @root_validator
+    @root_validator(skip_on_failure=True)
     def soil_and_pile_bottom_elevation_match(cls, values):  # pylint: disable=no-self-argument
         if values["pile"].bottom_elevation < values["soil"].bottom_elevation:
             raise UserWarning("The pile ends deeper than the soil profile.")
         return values
 
     def get_structural_properties(self) -> pd.DataFrame:
         """
@@ -640,15 +779,15 @@
         try:
             return self.soil_properties
         except AttributeError:
             print("Data not found. Please create Model with the Model.create() method.")
         except Exception as e:
             print(e)
 
-    def _postinit(self):
+    def __post_init__(self):
         def check_springs(arr):
             check_nan = np.isnan(arr).any()
             check_negative = (arr < 0).any()
 
             return check_nan or check_negative
 
         def get_coordinates() -> pd.DataFrame:
@@ -792,15 +931,15 @@
                                 (py[i, j, 0], py[i, j, 1]) = layer.lateral_model.py_spring_fct(
                                     sig=sig_v[j],
                                     X=depth_from_ground[j],
                                     layer_height=(layer.top - layer.bottom),
                                     depth_from_top_of_layer=(layer.top - elevation[j]),
                                     D=pile_width,
                                     L=(self.soil.top_elevation - self.pile.bottom_elevation),
-                                    below_water_table=elevation[j] <= self.soil.water_elevation,
+                                    below_water_table=elevation[j] <= self.soil.water_line,
                                     output_length=spring_dim,
                                 )
 
                         if (
                             layer.lateral_model.spring_signature[2] and self.distributed_moment
                         ):  # True if mt spring function exist
 
@@ -809,15 +948,15 @@
                                 (mt[i, j, 0], mt[i, j, 1]) = layer.lateral_model.mt_spring_fct(
                                     sig=sig_v[j],
                                     X=depth_from_ground[j],
                                     layer_height=(layer.top - layer.bottom),
                                     depth_from_top_of_layer=(layer.top - elevation[j]),
                                     D=pile_width,
                                     L=(self.soil.top_elevation - self.pile.bottom_elevation),
-                                    below_water_table=elevation[j] <= self.soil.water_elevation,
+                                    below_water_table=elevation[j] <= self.soil.water_line,
                                     output_length=spring_dim,
                                 )
 
                         # check if pile tip is within layer
                         if (
                             layer.top >= self.pile.bottom_elevation
                             and layer.bottom <= self.pile.bottom_elevation
@@ -835,15 +974,15 @@
                                     layer_height=(layer.top - layer.bottom),
                                     depth_from_top_of_layer=(
                                         layer.top - self.pile.bottom_elevation
                                     ),
                                     D=pile_width,
                                     L=(self.soil.top_elevation - self.pile.bottom_elevation),
                                     below_water_table=self.pile.bottom_elevation
-                                    <= self.soil.water_elevation,
+                                    <= self.soil.water_line,
                                     output_length=spring_dim,
                                 )
 
                             # Mb curve
                             if layer.lateral_model.spring_signature[3] and self.base_moment:
 
                                 (Mb[0, 0, 0], Mb[0, 0, 1]) = layer.lateral_model.Mb_spring_fct(
@@ -852,15 +991,15 @@
                                     layer_height=(layer.top - layer.bottom),
                                     depth_from_top_of_layer=(
                                         layer.top - self.pile.bottom_elevation
                                     ),
                                     D=pile_width,
                                     L=(self.soil.top_elevation - self.pile.bottom_elevation),
                                     below_water_table=self.pile.bottom_elevation
-                                    <= self.soil.water_elevation,
+                                    <= self.soil.water_line,
                                     output_length=spring_dim,
                                 )
 
             if check_springs(py):
                 print("py springs have negative or NaN values.")
                 print(
                     """if using PISA type springs, this can be due to parameters behind out of the parameter space.
@@ -924,15 +1063,15 @@
         self.soil_properties["xg_top [m]"] = (
             self.soil_properties["x_top [m]"] - self.soil.top_elevation
         )
         self.soil_properties["xg_bottom [m]"] = (
             self.soil_properties["x_bottom [m]"] - self.soil.top_elevation
         )
         # add vertical stress at top and bottom of each element
-        condition_below_water_table = self.soil_properties["x_top [m]"] <= self.soil.water_elevation
+        condition_below_water_table = self.soil_properties["x_top [m]"] <= self.soil.water_line
         self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] = (
             self.soil_properties["Unit Weight [kN/m3]"][condition_below_water_table] - 10.0
         )
         s = (
             self.soil_properties["x_top [m]"] - self.soil_properties["x_bottom [m]"]
         ) * self.soil_properties["Unit Weight [kN/m3]"]
         self.soil_properties["sigma_v top [kPa]"] = np.insert(
@@ -1191,18 +1330,15 @@
         distributed_lateral: bool = True,
         distributed_moment: bool = True,
         distributed_axial: bool = False,
         base_shear: bool = True,
         base_moment: bool = True,
         base_axial: bool = False,
     ):
-        """A method to create the Model. This function provides a 2-in-1 command where:
-
-        - a `Model` instance is created
-        - the `._postinit()` method is run and creates all necessary data to perform calculations.
+        """A method to create the Model.
 
         Parameters
         ----------
         name : str
             Name of the model
         pile : Pile
             Pile instance to be included in the model
@@ -1239,41 +1375,51 @@
             distributed_lateral=distributed_lateral,
             distributed_moment=distributed_moment,
             distributed_axial=distributed_axial,
             base_shear=base_shear,
             base_moment=base_moment,
             base_axial=base_axial,
         )
-        obj._postinit()
+
+        warnings.warn(
+            "\nThe method Model.create() will be removed in version 1.0.0."
+            "\nPlease use the base class to create a Pile instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
 
         return obj
 
     def __str__(self):
         return self.element_properties.to_string()
 
     @property
     def py_springs(self) -> pd.DataFrame:
-        """_summary_
-        #TODO
+        """Table with p-y springs computed for the given Model.
 
         Returns
         -------
-        pd.DataFrame
+        pd.DataFrame (or None if no SoilProfile is present)
             Table with p-y springs.
         """
-        return misc.get_springs(
-            springs=self._py_springs,
-            elevations=self.nodes_coordinates["x [m]"].values,
-            kind="p-y",
-        )
+        if self.soil is None:
+            return None
+        else:
+            return misc.get_springs(
+                springs=self._py_springs,
+                elevations=self.nodes_coordinates["x [m]"].values,
+                kind="p-y",
+            )
 
     @property
     def embedment(self) -> float:
-        """_summary_
-        #TODO
+        """Pile embedment length [m].
 
         Returns
         -------
-        float
+        float (or None if no SoilProfile is present)
             Pile embedment
         """
-        return self.soil.top_elevation - self.pile.bottom_elevation
+        if self.soil is None:
+            return None
+        else:
+            return self.soil.top_elevation - self.pile.bottom_elevation
```

### Comparing `openpile-0.1.0/src/openpile/core/kernel.py` & `openpile-0.2.0/src/openpile/core/kernel.py`

 * *Files 3% similar despite different names*

```diff
@@ -450,14 +450,114 @@
             [N, B, D, N, -B, C],
         ]
     ) * (0.5 * ksoil[:, 0] + 0.5 * ksoil[:, 1])
 
     return km
 
 
+def elem_p_delta_stiffness_matrix(model, f):
+    """creates stress stiffness matrix based on axial stress in pile.
+
+    #TODO: proof here
+
+    Parameters
+    ----------
+    model : openpile class object `openpile.construct.Model`
+        includes information on soil/structure, elements, nodes and other model-related data.
+    f: np.ndarray
+        Global displacement vector
+
+    Returns
+    -------
+    k: numpy array (3d)
+        stress stiffness matrix of all elememts related to axial stress
+
+    Raises
+    ------
+    ValueError
+        ndof per node can be either 2 or 3
+
+    """
+
+    # calculate length vector
+    L = mesh_to_element_length(model)
+
+    # internal forces
+    P = f[::6].reshape(-1, 1, 1)
+
+    # elastic properties
+    nu = model.pile._nu
+    E = model.element_properties["E [kPa]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    G = E / (2 + 2 * nu)
+    # cross-section properties
+    I = model.element_properties["I [m4]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    A = model.element_properties["Area [m2]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    d = model.element_properties["Diameter [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+    wt = model.element_properties["Wall thickness [m]"].to_numpy(dtype=float).reshape((-1, 1, 1))
+
+    # calculate shear component in stiffness matrix (if Timorshenko)
+    if model.element_type == "EulerBernoulli":
+        N = 0 * L
+        A = 6 / (5 * L)
+        B = N + 1 / 10
+        C = 2 * L / 15
+        D = -L / 30
+    elif model.element_type == "Timoshenko":
+        if model.pile.kind == "Circular":
+            a = 0.5 * d
+            b = 0.5 * (d - 2 * wt)
+            nom = 6 * (a**2 + b**2) ** 2 * (1 + nu) ** 2
+            denom = (
+                7 * a**4
+                + 34 * a**2 * b**2
+                + 7 * b**4
+                + nu * (12 * a**4 + 48 * a**2 * b**2 + 12 * b**4)
+                + nu**2 * (4 * a**4 + 16 * a**2 * b**2 + 4 * b**4)
+            )
+            kappa = nom / denom
+
+            omega = E * I * kappa / (A * G * L**2)
+
+        else:
+            raise ValueError("Timoshenko beams cannot be used yet for non-circular pile types")
+
+        phi = (12 * omega + 1) ** 2
+
+        N = 0 * L
+        A = 6 * (120 * omega**2 + 20 * omega + 1) / ((5 * L) * phi) + 12 * I / (A * L**3 * phi)
+        B = 1 / (10 * phi) + 6 * I / (A * L**2 * phi)
+        C = (2 * L * (90 * omega**2 + 15 * omega + 1)) / (15 * phi) + 4 * I * (
+            36 * omega**2 + 6 * omega + 1
+        ) / (A * L * phi)
+        D = -L * (360 * omega**2 + 60 * omega + 1) / (30 * phi) - 2 * I * (
+            72 * omega**2 + 12 * omega - 1
+        ) / (A * L * phi)
+
+    else:
+        raise ValueError(
+            "Model.element.type only accepts 'EB' type (for Euler-Bernoulli) of 'T' type (for Timoshenko)"
+        )
+
+    k = (
+        np.block(
+            [
+                [N, N, N, N, N, N],
+                [N, A, B, N, -A, B],
+                [N, B, C, N, -B, D],
+                [N, N, N, N, N, N],
+                [N, -A, -B, N, A, -B],
+                [N, B, D, N, -B, C],
+            ]
+        )
+        * -P
+    )
+
+    return k
+
+
 @njit(parallel=True, cache=True)
 def jit_build(k, ndim, n_elem, node_per_element, ndof_per_node):
     # pre-allocate stiffness matrix
     K = np.zeros((ndim, ndim), dtype=np.float64)
 
     for i in prange(n_elem):
         # dummy stiffness matrix that updates at each iteration
@@ -469,24 +569,26 @@
 
         # update global stiffness matrix
         K += K_temp
 
     return K
 
 
-def build_stiffness_matrix(model, u=None, kind=None, p_mobilised=None):
+def build_stiffness_matrix(model, f, u=None, kind=None):
     """Builds the stiffness matrix based on the model(element and node) properties
 
     Element stiffness matrices are first computed for each element and then loaded in the global stiffness matrix through summation.
     Different element stiffness matrices are computed depending on the specifications found in the Model object.
 
     Parameters
     ----------
     model : obj from openpile library
         stores all information about nodes elements, and other model-related items, see #TODO:link to model class
+    f: np.ndarray, Optional
+        Global internal force vector.
     u: np.ndarray, Optional
         Global displacement vector. Must be given if soil_flag is not None
     p_mobilised: np.ndarray, Optional
         Mobilised p-value. Must be given if soil_flag is not None
     kind: str, Optional
         "initial", "secant" or "tangent". Must be given if soil_flag is not None
 
@@ -503,14 +605,16 @@
     # number of elements in mesh
     n_elem = model.element_number
     # global dimension of the global stiffness matrix can be inferred
     ndim_global = ndof_per_node * n_elem + ndof_per_node
 
     # mechanical stiffness properties
     k = elem_mechanical_stiffness_matrix(model)
+    if f is not None:
+        k += elem_p_delta_stiffness_matrix(model, f=f)
     # add soil contribution
     if model.soil is not None:
         # gives warning if soil is given without displacements or type of stiffness
         if u is None or kind is None:
             UserWarning("'u' and 'kind' must be stipulated.")
         else:
             if model.distributed_lateral:
@@ -551,22 +655,24 @@
 def mesh_to_global_restrained_dof_vector(df: pd.DataFrame) -> np.ndarray:
     # extract each column (one line per node)
     restrained_dof_vector = df[["Tx", "Ty", "Rz"]].values.reshape(-1)
 
     return restrained_dof_vector
 
 
-def struct_internal_force(model, u) -> np.ndarray:
+def struct_internal_force(model, f, u) -> np.ndarray:
     # number of dof per node
     ndof_per_node = 3
     # number of nodes per element
     node_per_element = 2
 
     # create mech consistent stiffness matrix
     k = elem_mechanical_stiffness_matrix(model)
+    if f is not None:
+        k += elem_p_delta_stiffness_matrix(model, f=f)
 
     # add soil contribution
     if model.soil is not None:
         kind = "secant"
         if model.distributed_lateral:
             k += elem_py_stiffness_matrix(model, u, kind)
         elif model.distributed_moment:
```

### Comparing `openpile-0.1.0/src/openpile/core/misc.py` & `openpile-0.2.0/src/openpile/core/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import random
 import numpy as np
 import pandas as pd
 import math as m
 
 from numba import njit
-from matplotlib.colors import CSS4_COLORS
+import matplotlib.colors as mcolors
 
 
 def from_list2x_parse_top_bottom(var):
     """provide top and bottom values of layer based on float or list inputs"""
     if isinstance(var, float) or isinstance(var, int):
         top = var
         bottom = var
@@ -34,16 +34,32 @@
     elif isinstance(var, list):
         var_print = "-".join(str(v) for v in var)
     else:
         raise ValueError("not a float nor list")
     return var_print
 
 
-def generate_color_string():
-    colors = list(CSS4_COLORS.values())
+def generate_color_string(kind=None):
+    if kind is None:
+        colors = list(mcolors.CSS4_COLORS.values())
+    elif kind == "earth":
+        colors = [
+            "#B4A390",
+            "#927E75",
+            "#796363",
+            "#99A885",
+            "#D4DBBA",
+            "#FDEDCF",
+            "#EEEAC3",
+            "#F5D498",
+            "#ECB992",
+            "#DDA175",
+            "#AB7B5E",
+            "#8F6854",
+        ]
     return colors[random.randint(0, len(colors) - 1)]
 
 
 def repeat_inner(arr):
     arr = arr.reshape(-1, 1)
 
     arr_inner = arr[1:-1]
```

### Comparing `openpile-0.1.0/src/openpile/core/txt.py` & `openpile-0.2.0/src/openpile/core/txt.py`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/src/openpile/core/validation.py` & `openpile-0.2.0/src/openpile/core/validation.py`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/src/openpile/soilmodels.py` & `openpile-0.2.0/src/openpile/soilmodels.py`

 * *Files 4% similar despite different names*

```diff
@@ -451,43 +451,38 @@
 class API_sand(LateralModel):
     """A class to establish the API sand model.
 
     Parameters
     ----------
     phi: float or list[top_value, bottom_value]
         internal angle of friction in degrees
-    Neq: float
-        number of equivalent cycles, (Neq=1 means Static, Neq>1 means Cyclic)
+    kind: str, by default "static"
+        types of curves, can be of ("static","cyclic")
     p_multiplier: float
         multiplier for p-values
     y_multiplier: float
         multiplier for y-values
 
     """
 
     #: soil friction angle [deg], if a variation in values, two values can be given.
     phi: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
-    #: Number of equivalent cycles of the curve. 1 = static curve, >1 = cyclic curve.
-    Neq: confloat(ge=1.0, le=100.0)
+    #: types of curves, can be of ("static","cyclic")
+    kind: Literal["static", "cyclic"]
     #: p-multiplier
     p_multiplier: confloat(ge=0.0) = 1.0
     #: y-multiplier
     y_multiplier: confloat(gt=0.0) = 1.0
 
     # spring signature which tells that API sand only has p-y curves
     # signature if of the form [p-y:True, Hb:False, m-t:False, Mb:False]
     spring_signature = np.array([True, False, False, False], dtype=bool)
 
     def __str__(self):
-        if self.Neq == 1:
-            Neq = "Static, N < 1 cycle"
-        else:
-            Neq = "Cyclic, N = 100 cycles"
-
-        return f"\tAPI sand\n\tphi = {var_to_str(self.phi)}°\n\t{Neq}"
+        return f"\tAPI sand\n\tphi = {var_to_str(self.phi)}°\n\t{self.kind} curves"
 
     def py_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -506,15 +501,15 @@
         phi = phi_t + (phi_b - phi_t) * depth_from_top_of_layer / layer_height
 
         p, y = py_curves.api_sand(
             sig=sig,
             X=X,
             phi=phi,
             D=D,
-            Neq=self.Neq,
+            kind=self.kind,
             below_water_table=below_water_table,
             ymax=ymax,
             output_length=output_length,
         )
 
         return p * self.p_multiplier, y * self.y_multiplier
 
@@ -529,49 +524,44 @@
         Undrained shear strength in kPa
     eps50: float or list[top_value, bottom_value]
         strain at 50% failure load [-]
     J: float
         empirical factor varying depending on clay stiffness, varies between 0.25 and 0.50
     stiff_clay_threshold: float
         undrained shear strength [kPa] at which stiff clay curve is computed
-    Neq: float
-        number of equivalent cycles, (Neq=1 means Static, Neq>1 means Cyclic)
+    kind: str, by default "static"
+        types of curves, can be of ("static","cyclic")
     p_multiplier: float
         multiplier for p-values
     y_multiplier: float
         multiplier for y-values
 
     """
 
     #: undrained shear strength [kPa], if a variation in values, two values can be given.
     Su: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
     #: strain at 50% failure load [-], if a variation in values, two values can be given.
     eps50: Union[PositiveFloat, conlist(PositiveFloat, min_items=1, max_items=2)]
-    #: Number of equivalent cycles of the curve. 1 = static curve, >1 = cyclic curve.
-    Neq: confloat(ge=1.0, le=100.0)
+    #: types of curves, can be of ("static","cyclic")
+    kind: Literal["static", "cyclic"]
     #: empirical factor varying depending on clay stiffness
     J: confloat(ge=0.25, le=0.5) = 0.5
     #: undrained shear strength [kPa] at which stiff clay curve is computed
     stiff_clay_threshold: PositiveFloat = 96
     #: p-multiplier
     p_multiplier: confloat(ge=0.0) = 1.0
     #: y-multiplier
     y_multiplier: confloat(gt=0.0) = 1.0
 
     # spring signature which tells that API sand only has p-y curves
     # signature if of the form [p-y:True, Hb:False, m-t:False, Mb:False]
     spring_signature = np.array([True, False, False, False], dtype=bool)
 
     def __str__(self):
-        if self.Neq == 1:
-            Neq = "Static, N < 1 cycle"
-        else:
-            Neq = "Cyclic, N = 100 cycles"
-
-        return f"\tAPI clay\n\tSu = {var_to_str(self.Su)} kPa\n\teps50 = {var_to_str(self.eps50)}\n\t{Neq}"
+        return f"\tAPI clay\n\tSu = {var_to_str(self.Su)} kPa\n\teps50 = {var_to_str(self.eps50)}\n\t{self.kind} curves"
 
     def py_spring_fct(
         self,
         sig: float,
         X: float,
         layer_height: float,
         depth_from_top_of_layer: float,
@@ -597,13 +587,13 @@
             sig=sig,
             X=X,
             Su=Su,
             eps50=eps50,
             D=D,
             J=self.J,
             stiff_clay_threshold=self.stiff_clay_threshold,
-            Neq=self.Neq,
+            kind=self.kind,
             ymax=ymax,
             output_length=output_length,
         )
 
         return p * self.p_multiplier, y * self.y_multiplier
```

### Comparing `openpile-0.1.0/src/openpile/utils/Hb_curves.py` & `openpile-0.2.0/src/openpile/utils/Hb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/src/openpile/utils/Mb_curves.py` & `openpile-0.2.0/src/openpile/utils/Mb_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/src/openpile/utils/graphics.py` & `openpile-0.2.0/src/openpile/utils/graphics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """ general plots for openfile
 
 """
 
 # import libraries
+import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-from matplotlib.patches import FancyArrowPatch
-import numpy as np
+
+from matplotlib.patches import FancyArrowPatch, Rectangle
+from matplotlib.ticker import MultipleLocator, AutoMinorLocator
+from openpile.core.misc import generate_color_string
 
 mpl.rcParams["figure.subplot.wspace"] = 0.4
 
 
 def plot_deflection(result):
     fig, ax = plt.subplots()
 
@@ -54,14 +57,113 @@
     for axis in [ax2, ax3, ax4]:
         axis.set_yticklabels("")
         axis.set_ylabel("")
 
     return fig
 
 
+def soil_plot(SoilProfile):
+    def add_soil_profile(SoilProfile, ax, pile=None):
+        ax.set_title(label=f"Soil Profile overview - {SoilProfile.name}")
+
+        # make data
+        ax.set_xlim(left=0, right=1)
+        offset = 5
+        yBot = SoilProfile.bottom_elevation
+        if pile is None:
+            yTop = max(SoilProfile.top_elevation + offset, SoilProfile.water_line + offset)
+        else:
+            yTop = max(
+                SoilProfile.top_elevation + offset,
+                SoilProfile.water_line + offset,
+                pile.top_elevation + offset,
+            )
+
+        # axes
+        ax.set_ylim(bottom=yBot, top=yTop)
+        ax.set_ylabel("Elevation [m VREF]")
+        ax.set_xticks([])
+
+        for layer in SoilProfile.layers:
+            ax.add_patch(
+                Rectangle(
+                    xy=(0, layer.bottom),
+                    width=1,
+                    height=layer.top - layer.bottom,
+                    facecolor=layer.color,
+                )
+            )
+            ax.text(
+                0.02,
+                0.5 * (layer.top + layer.bottom),
+                layer.name,
+                bbox={"facecolor": [0.98, 0.96, 0.85], "alpha": 1, "edgecolor": "none", "pad": 1},
+            )
+
+        # grid
+        ax.minorticks_on()
+        ax.grid()
+        ax.grid(axis="y", which="minor", color=[0.75, 0.75, 0.75], linestyle="-", linewidth=0.5)
+
+        ax.plot(
+            np.array([-1, 0.1, 2]),
+            SoilProfile.water_line + np.zeros((3)),
+            mfc="dodgerblue",
+            marker=7,
+            linewidth=1,
+            color="dodgerblue",
+        )
+
+        return ax
+
+    fig, ax = plt.subplots()
+    ax = add_soil_profile(SoilProfile, ax, pile=None)
+
+    return fig
+
+
+def pile_plot(pile):
+
+    if pile.kind == "Circular":
+        fig, (ax1, ax2, ax3) = plt.subplots(1, 3)
+
+        fig.suptitle(f"Pile overview - {pile.name}")
+
+        ydata = pile.data["Elevation [m]"]
+
+        xdata = pile.data["Wall thickness [m]"]
+        ax2.plot(xdata, ydata, "-k", lw=2)
+        ax2.set_xlim(left=0, right=xdata.max() * 1.1)
+
+        xdata = pile.data["Area [m2]"]
+        ax3.plot(xdata, ydata, "-k", lw=2)
+        ax3.set_xlim(left=0, right=xdata.max() * 1.1)
+
+        for axis in [ax2, ax3]:
+            axis.set_yticklabels("")
+            axis.set_ylabel("")
+
+        ax1.set_ylabel("Elevation [m VREF]", fontsize=8)
+
+        for (axis, xlab) in zip(
+            [ax1, ax2, ax3], ["Diameter [m]", "Wall thickness [m]", "Area [m2]"]
+        ):
+            xdata = pile.data[xlab]
+            axis.plot(xdata, ydata, "-k", lw=2)
+            axis.set_xlim(left=0, right=xdata.max() * 1.1)
+
+            axis.set_xlabel(xlab, fontsize=8)
+            axis.tick_params(axis="both", labelsize=8)
+            axis.grid()
+            axis.grid(which="minor", color=[0.75, 0.75, 0.75], linestyle="-", linewidth=0.5)
+            axis.xaxis.set_minor_locator(AutoMinorLocator())
+
+    return fig
+
+
 def connectivity_plot(model):
     # TODO docstring
 
     support_color = "b"
     # create 4 subplots with (deflectiom, normal force, shear force, bending moment)
     fig, ax = plt.subplots()
     ax.set_ylabel("x [m]")
```

### Comparing `openpile-0.1.0/src/openpile/utils/mt_curves.py` & `openpile-0.2.0/src/openpile/utils/mt_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/src/openpile/utils/py_curves.py` & `openpile-0.2.0/src/openpile/utils/py_curves.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 # API sand function
 @njit(parallel=True, cache=True)
 def api_sand(
     sig: float,
     X: float,
     phi: float,
     D: float,
-    Neq: float = 1.0,
+    kind: str = "static",
     below_water_table: bool = True,
     ymax: float = 0.0,
     output_length: int = 20,
 ):
     """
     Creates the API sand p-y curve from relevant input.
 
@@ -153,16 +153,16 @@
         Vertical effective stress [unit: kPa]
     X: float
         Depth of the curve w.r.t. mudline [unit: m]
     phi: float
         internal angle of friction of the sand layer [unit: degrees]
     D: float
         Pile width [unit: m]
-    Neq: float, by default 1.0
-        Number of equivalent cycles [unit: -]
+    kind: str, by default "static"
+        types of curves, can be of ("static","cyclic")
     below_water_table: bool, by default False
         switch to calculate initial subgrade modulus below/above water table
     ymax: float, by default 0.0
         maximum value of y, default goes to 99.9% of ultimate resistance
     output_length: int, by default 20
         Number of discrete point along the springs
 
@@ -170,15 +170,15 @@
     -------
     1darray
         p vector [unit: kN/m]
     1darray
         y vector [unit: m]
     """
     # A value - only thing that changes between cyclic or static
-    if Neq == 1:
+    if kind == "static":
         A = max(0.9, 3 - 0.8 * X / D)
     else:
         A = 0.9
 
     # initial subgrade modulus in kpa from fit with API (2014)
     if below_water_table:
         k_phi = max((0.1978 * phi**2 - 10.232 * phi + 136.82) * 1000, 5400)
@@ -236,15 +236,15 @@
     sig: float,
     X: float,
     Su: float,
     eps50: float,
     D: float,
     J: float = 0.5,
     stiff_clay_threshold=96,
-    Neq: float = 1.0,
+    kind: str = "static",
     ymax: float = 0.0,
     output_length: int = 20,
 ):
     """
     Creates the API clay p-y curve from relevant input.
 
     Parameters
@@ -259,16 +259,16 @@
         strain at 50% ultimate resistance [-]
     D: float
         Pile width [unit: m]
     J: float, by default 0.5
         empirical factor varying depending on clay stiffness
     stiff_clay_threshold: float, by default 96.0
         undrained shear strength at which stiff clay curve is computed [unit: kPa]
-    Neq: float, by default 1.0
-        Number of equivalent cycles [unit: -]
+    kind: str, by default "static"
+        types of curves, can be of ("static","cyclic")
     ymax: float, by default 0.0
         maximum value of y, if null the maximum is calculated such that the whole curve is computed
     output_length: int, by default 20
         Number of discrete point along the springs
 
     Returns
     -------
@@ -310,15 +310,15 @@
     y = np.append(y, add_y_values)
     y = np.sort(y)
 
     # define p vector
     p = np.zeros(shape=len(y), dtype=np.float32)
 
     for i in prange(len(y)):
-        if Neq == 1:
+        if kind == "static":
             # derive static curve
             if y[i] > 8 * y50:
                 p[i] = Pmax
             else:
                 p[i] = 0.5 * Pmax * (y[i] / y50) ** 0.33
         else:
             # derive cyclic curve
```

### Comparing `openpile-0.1.0/src/openpile/utils/qz_curves.py` & `openpile-0.2.0/src/openpile/utils/qz_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/src/openpile/utils/tz_curves.py` & `openpile-0.2.0/src/openpile/utils/tz_curves.py`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/src/openpile.egg-info/PKG-INFO` & `openpile-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 Metadata-Version: 2.1
 Name: openpile
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library for geotechnical pile calculations.
 Home-page: https://github.com/TchilDill/openpile
 Author: Guillaume Melin
 Author-email: guillaume.melin@icloud.com
 License: GPLv3
+Project-URL: Documentation, https://openpile.readthedocs.io/en/latest/
+Project-URL: Code, https://github.com/TchilDill/openpile
+Project-URL: Issue tracker, https://github.com/TchilDill/openpile/issues
 Keywords: Offshore Wind,PILE,Geotechnics,monopile,pin-piles,Geotechnical,calculations,PISA,winkler
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # OpenPile
 
 Geotechnical super-toolbox for pile-related calculations.
 
 <!-- [![Python Support](https://img.shields.io/pypi/pyversions/openpile.svg)](https://pypi.org/project/openpile/) -->
 [![License: LGPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
-
-[![Visual Studio](https://badgen.net/badge/icon/visualstudio?icon=visualstudio&label)](https://visualstudio.microsoft.com)
+[![Downloads](https://static.pepy.tech/badge/openpile)](https://pepy.tech/project/openpile)
 
 ![Tests](https://github.com/TchilDill/openpile/actions/workflows/Test.yml/badge.svg) 
 [![Documentation Status](https://readthedocs.org/projects/openpile/badge/?version=latest)](https://openpile.readthedocs.io/en/latest/?badge=latest)
-[![Github All Releases](https://img.shields.io/github/downloads/TchilDill/openpile/total.svg)]()
+
 
 [![issues closed](https://img.shields.io/github/issues-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/issues)
 [![PRs closed](https://img.shields.io/github/issues-pr-closed/TchilDill/openpile)](https://github.com/TchilDill/openpile/pulls)
 [![GitHub last commit](https://img.shields.io/github/last-commit/TchilDill/openpile)](https://github.com/TchilDill/openpile/commits/master)
 [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 
 Please see [official documentation](https://openpile.readthedocs.io/en/latest/) for more information.
 
+This package is an open source python library that provides users a tool box for geotechnical pile
+calculations.
+
+This package allows the user to:
+
+* Use basic Euler-Bernoulli beam theory (as well as Timoshenko's variation) to compute 
+  forces, deflection of a beam (or a pile) under adequate loading and 
+  support conditions.
+* Use Winkler's approach of a beam (or a pile) supported by linear or non-linear lateral and/or 
+  rotational springs to compute forces and deflection of the pile based on recognised 
+  soil models such as the widely used traditional API models for sand and clay or more recent models that stem from 
+  the PISA joint-industry project.
+
+This library supports the following versions of python: 3.7-3.10.
+Python 3.11 is not supported!
+
 ## Installation Instructions
 
 **Prerequisites**:
 
 * a version of python is installed on your machine (supported versions: 3.7-3.10)
 * pip is installed in your environment.
 
@@ -53,23 +72,24 @@
 ```
 
 ## Features
 
  * Python 3.7-3.10 support
  * Interactive structure perfectly suited for Jupyter Notebook 
  * Integrated data validation to prevent wrong inputs with pydantic
+ * very fast computations fueled by the Numpy, Numba and Pandas libraries
  * Calculations
    * Beam calculation
    * Winkler model (i.e. beam supported by soil springs)
      * Load-driven analyses
      * Displacement-driven analyses 
    * Out-of-the-box computation of individual soil springs
    <!-- * Axial capacity calculations via integration -->
- * Friendly API interface with  object-oriented approach
- * Fully integrated output with python environment with Matplotlib and Pandas libraries. 
+ * Friendly API interface with object-oriented approach
+ * Matplotlib and Pandas libraries to facilitate post-processing of results. 
 
  ## Please share with the community
 
 This library relies on community interactions. Please consider sharing a post about `OpenPile` and the value it can provide for researcher, academia and professionals.
 
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-reddit-red?logo=reddit)](https://reddit.com/submit?url=https://github.com/TchilDill/openpile&title=openpile)
 [![GitHub Repo stars](https://img.shields.io/badge/share%20on-twitter-03A9F4?logo=twitter)](https://twitter.com/share?url=https://github.com/TchilDill/openpile&t=openpile)
```

### Comparing `openpile-0.1.0/src/openpile.egg-info/SOURCES.txt` & `openpile-0.2.0/src/openpile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpile-0.1.0/test/test_construct.py` & `openpile-0.2.0/test/test_construct.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestPile:
 
     def test_main_constructor(self):
         """Main constructor of Pile object, check if pile.data 
         has even entries and that steel E value is 210GPa
         """
         # create a steel and circular pile
-        pile = construct.Pile.create(kind='Circular',
+        pile = construct.Pile(kind='Circular',
                             name = "",
                             material='Steel',
                             top_elevation = 0,
                             pile_sections={
                                 'length':[10,30],
                                 'diameter':[7.5,8.5],
                                 'wall thickness':[0.07, 0.08],
@@ -25,43 +25,43 @@
                             )
         # check Young modulus is indeed Steel
         assert pile.E == 210e6
         # check even numbers of row for dataframe
         assert pile.data.values.shape[0] % 2 == 0
 
     def test_pile_width(self):
-        pile = construct.Pile.create(kind='Circular',
+        pile = construct.Pile(kind='Circular',
                             name = "",
                             material='Steel',
                             top_elevation = 0.1,
                             pile_sections={
                                 'length':[20,20],
                                 'diameter':[7.5,8.5],
                                 'wall thickness':[0.07, 0.08],
                             }
                             )
         
-        assert pile.width == 8.00
+        assert pile.width.mean() == 8.00
 
     def test_pile_length(self):
-        pile = construct.Pile.create(kind='Circular',
+        pile = construct.Pile(kind='Circular',
                             name = "",
                             material='Steel',
                             top_elevation = 10,
                             pile_sections={
                                 'length':[22,16],
                                 'diameter':[7.5,8.5],
                                 'wall thickness':[0.07, 0.08],
                             }
                             )
         
         assert pile.length == 38.0
 
     def test_pile_bottom(self):
-        pile = construct.Pile.create(kind='Circular',
+        pile = construct.Pile(kind='Circular',
                             name = "",
                             material='Steel',
                             top_elevation = 10,
                             pile_sections={
                                 'length':[10,30],
                                 'diameter':[7.5,8.5],
                                 'wall thickness':[0.07, 0.08],
@@ -71,91 +71,91 @@
         assert pile.bottom_elevation == -30.0
 
 
     def test_pile_area1(self):
         """check pile area 
         """
         # Create a pile instance with two sections of respectively 10m and 30m length.
-        pile = construct.Pile.create(name = "",
+        pile = construct.Pile(name = "",
                 kind='Circular',
                 material='Steel',
                 top_elevation = 0,
                 pile_sections={
                     'length':[10,30],
                     'diameter':[1.0,1.0],
                     'wall thickness':[0.5, 0.5],
                 }
             )
         
-        assert pile.area == 0.25*m.pi
+        assert pile.area.mean() == 0.25*m.pi
 
     def test_pile_area2(self):
-        pile = construct.Pile.create(name = "",
+        pile = construct.Pile(name = "",
                 kind='Circular',
                 material='Steel',
                 top_elevation = 0,
                 pile_sections={
                     'length':[10,30],
                     'diameter':[1.0,1.0],
                     'wall thickness':[0.001, 0.001],
                 }
             )
         
-        assert m.isclose(pile.area, m.pi*0.001, rel_tol=0.01)
+        assert m.isclose(pile.area.mean(), m.pi*0.001, rel_tol=0.01)
 
 class TestLayer:
     def test_constructor(self):
         try:
             layer = construct.Layer(name='Soft Clay',
                             top=0,
                             bottom=-10,
                             weight=19,
-                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], Neq=100), 
+                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], kind="cyclic"), 
                         )
         except Exception:
             assert False, "Constructor did not work"
 
     def test_wrong_order_top_and_bottom(self):
         with pytest.raises(ValidationError):
             layer = construct.Layer(name='Soft Clay',
                             top=-10,
                             bottom=0,
                             weight=19,
-                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], Neq=100), 
+                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], kind="cyclic"), 
                         )
 
     def test_equal_top_and_bottom(self):
         with pytest.raises(ValidationError):
             layer = construct.Layer(name='Soft Clay',
                             top=-5,
                             bottom=-5,
                             weight=19,
-                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], Neq=100), 
+                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], kind="cyclic"), 
                         )
 
     def test_wrong_unit_weight(self):
         """Constructor should not accept a soil unit weight equal to 10 or less as 
         it would be less dense than water and likely the user made a mistake with 
         the effective unit weight. 
         """
         with pytest.raises(ValidationError):
             layer = construct.Layer(name='Soft Clay',
                             top=0,
                             bottom=-10,
                             weight=10,
-                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], Neq=100), 
+                            lateral_model=API_clay(Su=[30,35], eps50=[0.01, 0.02], kind="static"), 
                         )
             
 class TestSoilProfile:
     def test_wrong_layers_elevations_gap(self):
         with pytest.raises(ValidationError):
             sp = construct.SoilProfile(
                 name = "", 
                 top_elevation=0, 
-                water_elevation=0,
+                water_line=0,
                 layers=[
                     construct.Layer(name= "",
                                     top=0,
                                     bottom=-10,
                                     weight=20,
                                     ),
                     construct.Layer(name= "",
@@ -166,15 +166,15 @@
                 ])
     
     def test_wrong_layers_elevations_overlap(self):
         with pytest.raises(ValidationError):
             sp = construct.SoilProfile(
                 name = "", 
                 top_elevation=0, 
-                water_elevation=0,
+                water_line=0,
                 layers=[
                     construct.Layer(name= "",
                                     top=0,
                                     bottom=-10,
                                     weight=20,
                                     ),
                     construct.Layer(name= "",
@@ -182,18 +182,18 @@
                                     bottom=-30,
                                     weight=20,
                                     ),
                 ])
             
     def test_wrong_top_elevation(self):
         with pytest.raises(ValidationError):
-            sp = construct.SoilProfile.create(
+            sp = construct.SoilProfile(
                 name = "", 
                 top_elevation=10, 
-                water_elevation=0,
+                water_line=0,
                 layers=[
                     construct.Layer(name= "",
                                     top=11,
                                     bottom=-10,
                                     weight=20,
                                     ),
                     construct.Layer(name= "",
@@ -203,15 +203,15 @@
                                     ),
                 ])
     
     def test_wrong_bottom_elevation(self):
         sp = construct.SoilProfile(
             name = "", 
             top_elevation=10, 
-            water_elevation=0,
+            water_line=0,
             layers=[
                 construct.Layer(name= "",
                                 top=10,
                                 bottom=-10,
                                 weight=20,
                                 ),
                 construct.Layer(name= "",
@@ -225,29 +225,31 @@
 
 class TestModel:
 
     def test_constructor_wo_soil_models(self):
         """
         check that model can still be created with no lateral or axial models""" 
         try:
-            model = construct.Model.create(
+            model = construct.Model(
                 name="",
-                pile=construct.Pile.create(
+                pile=construct.Pile(
                     name="",
                     top_elevation=20,
+                    kind="Circular",
+                    material="Steel",
                     pile_sections={
                         'length':[50],
                         'diameter':[7],
                         'wall thickness':[0.08]
                     }
                 ),
-                soil = construct.SoilProfile.create(
+                soil = construct.SoilProfile(
                     name = "", 
                     top_elevation=10, 
-                    water_elevation=0,
+                    water_line=0,
                     layers=[
                         construct.Layer(name= "",
                                         top=10,
                                         bottom=-10,
                                         weight=20,
                                         ),
                         construct.Layer(name= "",
```

### Comparing `openpile-0.1.0/test/test_utils_misc.py` & `openpile-0.2.0/test/test_utils_misc.py`

 * *Files identical despite different names*

