# Comparing `tmp/freeflux-0.3.1.tar.gz` & `tmp/freeflux-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\cwu\Desktop\Software\FreeFlux\pypi\freeflux-0.3.1\dist\.tmp-iq477cp0\freeflux-0.3.1.tar", last modified: Tue Apr 18 22:29:03 2023, max compression
+gzip compressed data, was "C:\Users\cwu\Desktop\Software\FreeFlux\pypi\freeflux-0.3.2\dist\.tmp-663xfpld\freeflux-0.3.2.tar", last modified: Mon Apr 24 08:09:51 2023, max compression
```

## Comparing `freeflux-0.3.1.tar` & `freeflux-0.3.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.403178 freeflux-0.3.1/
--rw-rw-rw-   0        0        0    35149 2022-08-18 01:02:32.000000 freeflux-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     5239 2023-04-18 22:29:03.414148 freeflux-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4188 2023-04-07 06:00:51.000000 freeflux-0.3.1/README.rst
--rw-rw-rw-   0        0        0       90 2023-04-03 02:02:48.000000 freeflux-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1234 2023-04-18 22:29:03.420132 freeflux-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-04-18 21:36:18.000000 freeflux-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.182766 freeflux-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.209695 freeflux-0.3.1/src/freeflux/
--rw-rw-rw-   0        0        0      247 2023-04-18 22:24:08.000000 freeflux-0.3.1/src/freeflux/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.263552 freeflux-0.3.1/src/freeflux/analysis/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.1/src/freeflux/analysis/__init__.py
--rw-rw-rw-   0        0        0    23297 2023-04-18 21:42:54.000000 freeflux-0.3.1/src/freeflux/analysis/fit.py
--rw-rw-rw-   0        0        0    21603 2023-04-18 21:44:20.000000 freeflux-0.3.1/src/freeflux/analysis/inst_fit.py
--rw-rw-rw-   0        0        0     6538 2023-04-18 21:44:44.000000 freeflux-0.3.1/src/freeflux/analysis/inst_simulate.py
--rw-rw-rw-   0        0        0    10165 2023-04-18 21:46:20.000000 freeflux-0.3.1/src/freeflux/analysis/simulate.py
--rw-rw-rw-   0        0        0    12420 2023-04-18 21:48:46.000000 freeflux-0.3.1/src/freeflux/analysis/stats.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.295466 freeflux-0.3.1/src/freeflux/core/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.1/src/freeflux/core/__init__.py
--rw-rw-rw-   0        0        0     4989 2023-04-18 21:49:39.000000 freeflux-0.3.1/src/freeflux/core/emu.py
--rw-rw-rw-   0        0        0    12810 2023-04-18 21:50:38.000000 freeflux-0.3.1/src/freeflux/core/mdv.py
--rw-rw-rw-   0        0        0     2553 2023-03-31 21:40:13.000000 freeflux-0.3.1/src/freeflux/core/metabolite.py
--rw-rw-rw-   0        0        0    35901 2023-04-18 21:53:25.000000 freeflux-0.3.1/src/freeflux/core/model.py
--rw-rw-rw-   0        0        0    11011 2023-04-18 21:49:24.000000 freeflux-0.3.1/src/freeflux/core/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.310426 freeflux-0.3.1/src/freeflux/io/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:20.000000 freeflux-0.3.1/src/freeflux/io/__init__.py
--rw-rw-rw-   0        0        0     3132 2023-04-03 10:18:57.000000 freeflux-0.3.1/src/freeflux/io/inputs.py
--rw-rw-rw-   0        0        0    33169 2023-04-07 00:30:07.000000 freeflux-0.3.1/src/freeflux/io/results.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.344336 freeflux-0.3.1/src/freeflux/optim/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:49.000000 freeflux-0.3.1/src/freeflux/optim/__init__.py
--rw-rw-rw-   0        0        0     9270 2023-04-18 21:54:53.000000 freeflux-0.3.1/src/freeflux/optim/optim.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.361293 freeflux-0.3.1/src/freeflux/solver/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:33:01.000000 freeflux-0.3.1/src/freeflux/solver/__init__.py
--rw-rw-rw-   0        0        0     3375 2023-04-01 23:47:14.000000 freeflux-0.3.1/src/freeflux/solver/lpsolver.py
--rw-rw-rw-   0        0        0    19726 2023-04-18 21:55:35.000000 freeflux-0.3.1/src/freeflux/solver/nlpsolver.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.390212 freeflux-0.3.1/src/freeflux/utils/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.1/src/freeflux/utils/__init__.py
--rw-rw-rw-   0        0        0      496 2023-03-26 22:55:07.000000 freeflux-0.3.1/src/freeflux/utils/context.py
--rw-rw-rw-   0        0        0     1916 2023-04-01 23:41:09.000000 freeflux-0.3.1/src/freeflux/utils/progress.py
--rw-rw-rw-   0        0        0    32362 2023-04-18 21:58:49.000000 freeflux-0.3.1/src/freeflux/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:29:03.226650 freeflux-0.3.1/src/freeflux.egg-info/
--rw-rw-rw-   0        0        0     5239 2023-04-18 22:29:03.000000 freeflux-0.3.1/src/freeflux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-18 22:29:03.000000 freeflux-0.3.1/src/freeflux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:29:03.000000 freeflux-0.3.1/src/freeflux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-04-18 22:29:03.000000 freeflux-0.3.1/src/freeflux.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 22:29:03.000000 freeflux-0.3.1/src/freeflux.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.786969 freeflux-0.3.2/
+-rw-rw-rw-   0        0        0    35149 2022-08-18 01:02:32.000000 freeflux-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     5239 2023-04-24 08:09:51.787965 freeflux-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4188 2023-04-07 06:00:51.000000 freeflux-0.3.2/README.rst
+-rw-rw-rw-   0        0        0       90 2023-04-03 02:02:48.000000 freeflux-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1234 2023-04-24 08:09:51.791954 freeflux-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-04-18 21:36:18.000000 freeflux-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.596477 freeflux-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.632383 freeflux-0.3.2/src/freeflux/
+-rw-rw-rw-   0        0        0      247 2023-04-24 07:58:25.000000 freeflux-0.3.2/src/freeflux/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.683246 freeflux-0.3.2/src/freeflux/analysis/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.2/src/freeflux/analysis/__init__.py
+-rw-rw-rw-   0        0        0    23297 2023-04-18 21:42:54.000000 freeflux-0.3.2/src/freeflux/analysis/fit.py
+-rw-rw-rw-   0        0        0    21603 2023-04-18 21:44:20.000000 freeflux-0.3.2/src/freeflux/analysis/inst_fit.py
+-rw-rw-rw-   0        0        0     6538 2023-04-18 21:44:44.000000 freeflux-0.3.2/src/freeflux/analysis/inst_simulate.py
+-rw-rw-rw-   0        0        0    10165 2023-04-18 21:46:20.000000 freeflux-0.3.2/src/freeflux/analysis/simulate.py
+-rw-rw-rw-   0        0        0    12497 2023-04-24 08:02:13.000000 freeflux-0.3.2/src/freeflux/analysis/stats.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.712167 freeflux-0.3.2/src/freeflux/core/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.2/src/freeflux/core/__init__.py
+-rw-rw-rw-   0        0        0     4989 2023-04-18 21:49:39.000000 freeflux-0.3.2/src/freeflux/core/emu.py
+-rw-rw-rw-   0        0        0    12887 2023-04-24 08:02:34.000000 freeflux-0.3.2/src/freeflux/core/mdv.py
+-rw-rw-rw-   0        0        0     2553 2023-03-31 21:40:13.000000 freeflux-0.3.2/src/freeflux/core/metabolite.py
+-rw-rw-rw-   0        0        0    35901 2023-04-18 21:53:25.000000 freeflux-0.3.2/src/freeflux/core/model.py
+-rw-rw-rw-   0        0        0    11011 2023-04-18 21:49:24.000000 freeflux-0.3.2/src/freeflux/core/reaction.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.728126 freeflux-0.3.2/src/freeflux/io/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:20.000000 freeflux-0.3.2/src/freeflux/io/__init__.py
+-rw-rw-rw-   0        0        0     3147 2023-04-24 07:59:36.000000 freeflux-0.3.2/src/freeflux/io/inputs.py
+-rw-rw-rw-   0        0        0    33246 2023-04-24 08:03:00.000000 freeflux-0.3.2/src/freeflux/io/results.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.739096 freeflux-0.3.2/src/freeflux/optim/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:49.000000 freeflux-0.3.2/src/freeflux/optim/__init__.py
+-rw-rw-rw-   0        0        0     9270 2023-04-18 21:54:53.000000 freeflux-0.3.2/src/freeflux/optim/optim.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.755053 freeflux-0.3.2/src/freeflux/solver/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:33:01.000000 freeflux-0.3.2/src/freeflux/solver/__init__.py
+-rw-rw-rw-   0        0        0     3375 2023-04-01 23:47:14.000000 freeflux-0.3.2/src/freeflux/solver/lpsolver.py
+-rw-rw-rw-   0        0        0    19803 2023-04-24 08:03:20.000000 freeflux-0.3.2/src/freeflux/solver/nlpsolver.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.779987 freeflux-0.3.2/src/freeflux/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.2/src/freeflux/utils/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-03-26 22:55:07.000000 freeflux-0.3.2/src/freeflux/utils/context.py
+-rw-rw-rw-   0        0        0     1916 2023-04-01 23:41:09.000000 freeflux-0.3.2/src/freeflux/utils/progress.py
+-rw-rw-rw-   0        0        0    33624 2023-04-24 08:06:34.000000 freeflux-0.3.2/src/freeflux/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.653327 freeflux-0.3.2/src/freeflux.egg-info/
+-rw-rw-rw-   0        0        0     5239 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/top_level.txt
```

### Comparing `freeflux-0.3.1/LICENSE` & `freeflux-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/PKG-INFO` & `freeflux-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeflux
-Version: 0.3.1
+Version: 0.3.2
 Summary: FreeFlux is a package for 13C metabolic flux analysis
 Home-page: https://github.com/Chaowu88/freeflux
 Author: Chao Wu
 Author-email: chaowu09@gmail.com
 License: GNU General Public License v3.0
 Keywords: 13c,labeling pattern,metabolic flux analysis,metabolism,biology,non-linear programming,optimization,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freeflux-0.3.1/README.rst` & `freeflux-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/setup.cfg` & `freeflux-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 7265 6566 6c75 780d 0a76 6572   = freeflux..ver
-00000020: 7369 6f6e 203d 2030 2e33 2e31 0d0a 6175  sion = 0.3.1..au
+00000020: 7369 6f6e 203d 2030 2e33 2e32 0d0a 6175  sion = 0.3.2..au
 00000030: 7468 6f72 203d 2043 6861 6f20 5775 0d0a  thor = Chao Wu..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2063  author_email = c
 00000050: 6861 6f77 7530 3940 676d 6169 6c2e 636f  haowu09@gmail.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2046 7265 6546 6c75 7820 6973 2061 2070   FreeFlux is a p
 00000080: 6163 6b61 6765 2066 6f72 2031 3343 206d  ackage for 13C m
 00000090: 6574 6162 6f6c 6963 2066 6c75 7820 616e  etabolic flux an
```

### Comparing `freeflux-0.3.1/src/freeflux/analysis/fit.py` & `freeflux-0.3.2/src/freeflux/analysis/fit.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/analysis/inst_fit.py` & `freeflux-0.3.2/src/freeflux/analysis/inst_fit.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/analysis/inst_simulate.py` & `freeflux-0.3.2/src/freeflux/analysis/inst_simulate.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/analysis/simulate.py` & `freeflux-0.3.2/src/freeflux/analysis/simulate.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/analysis/stats.py` & `freeflux-0.3.2/src/freeflux/analysis/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from os import makedirs
 import numpy as np
 import pandas as pd
 from scipy.stats import t, chi2, probplot, zscore
 from scipy.interpolate import interp1d
 import matplotlib.pyplot as plt
+import warnings
+warnings.filterwarnings('ignore', category = RuntimeWarning)
 
 
 def _chi2_test(obj_value, dof, confidence_level):
     '''
     Parameters
     ----------
     obj_value: float
```

### Comparing `freeflux-0.3.1/src/freeflux/core/emu.py` & `freeflux-0.3.2/src/freeflux/core/emu.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/core/mdv.py` & `freeflux-0.3.2/src/freeflux/core/mdv.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from collections import OrderedDict, Counter
 from collections.abc import Iterable
 from itertools import combinations_with_replacement
 from numbers import Real
 import numpy as np
 from scipy.special import comb
 from scipy.linalg import inv
+import warnings
+warnings.filterwarnings('ignore', category = RuntimeWarning)
 
 
 natAbuns = {'H': [0.999885, 0.000115],
             'C': [0.9893, 0.0107],
             'N': [0.99632, 0.00368],
             'O': [0.99757, 0.00038, 0.00205],
             'Si': [0.922297, 0.046832, 0.030872],
```

### Comparing `freeflux-0.3.1/src/freeflux/core/metabolite.py` & `freeflux-0.3.2/src/freeflux/core/metabolite.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/core/model.py` & `freeflux-0.3.2/src/freeflux/core/model.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/core/reaction.py` & `freeflux-0.3.2/src/freeflux/core/reaction.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/io/inputs.py` & `freeflux-0.3.2/src/freeflux/io/inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,17 +124,17 @@
             names = ['mean', 'sd'], 
             index_col = indexCols
         )                        
     elif re.search(r'xls', ext):
         data = pd.read_excel(
             file, 
             comment = '#', 
-            header = None, 
-            names = ['mean', 'sd'], 
-            index_col = indexCols
+            header = None
         )
+        data.set_index(indexCols, inplace = True)
+        data.columns = ['mean', 'sd']
     else:
         raise TypeError('can only read from .tsv or excel file')
     
     data = data.dropna()
         
     return data
```

### Comparing `freeflux-0.3.1/src/freeflux/io/results.py` & `freeflux-0.3.2/src/freeflux/io/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import pandas as pd
 from scipy.linalg import pinv2
 from ..core.mdv import MDV
 from ..analysis.stats import (_chi2_test, _normal_probability, _simulated_vs_measured_MDVs, 
                               _simulated_vs_measured_fluxes, _simulated_vs_measured_inst_MDVs,
                               _confidence_intervals_le, _confidence_intervals_mc, _MDV_kinetics,
                               _contribution_matrix, _sensitivity)
+import warnings
+warnings.filterwarnings('ignore', category = RuntimeWarning)
 
 
 class pDict(dict):
 
     def __init__(self, *args, digits = 3, **kwargs):
         
         super().__init__(*args, **kwargs)
```

### Comparing `freeflux-0.3.1/src/freeflux/optim/optim.py` & `freeflux-0.3.2/src/freeflux/optim/optim.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/solver/lpsolver.py` & `freeflux-0.3.2/src/freeflux/solver/lpsolver.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/solver/nlpsolver.py` & `freeflux-0.3.2/src/freeflux/solver/nlpsolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 try:
     from openopt import NLP
 except ModuleNotFoundError:
     OPENOPT_INSTALLED = False
 else:
     OPENOPT_INSTALLED = True
 from ..utils.utils import Calculator
+import warnings
+warnings.filterwarnings('ignore', category = RuntimeWarning)
 
 
 class MFAModel():
     '''
     Parameters
     ----------
     model: Model
```

### Comparing `freeflux-0.3.1/src/freeflux/utils/progress.py` & `freeflux-0.3.2/src/freeflux/utils/progress.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.1/src/freeflux/utils/utils.py` & `freeflux-0.3.2/src/freeflux/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 import warnings
 warnings.filterwarnings('ignore', category = RuntimeWarning) 
 import numpy as np
 from numpy.random import normal
 import pandas as pd
 from scipy.linalg import null_space, pinv2, expm
 from sympy import symbols, lambdify, Matrix, derive_by_array
+try:
+    import jax.numpy as jnp
+    from jax import config, jacfwd
+    config.update('jax_platform_name', 'cpu')
+except ModuleNotFoundError:
+    JAX_INSTALLED = False
+else:
+    JAX_INSTALLED = True
 from multiprocessing import Pool
 from ..core.mdv import MDV, get_natural_MDV, get_substrate_MDV, conv, diff_conv
+import warnings
+warnings.filterwarnings('ignore', category = RuntimeWarning)
+warnings.filterwarnings('ignore', category = DeprecationWarning)
 
     
 class Calculator():
     '''
     Parameters
     ----------
     model: Model
@@ -313,16 +324,33 @@
         
         A = preAB[:preAB.shape[1], :].T
         B = -preAB[preAB.shape[1]:, :].T
         
         matA = Matrix(A)
         matB = Matrix(B)
         
-        matrix_A_der = np.array(derive_by_array(matA, symbols(fluxids)), dtype = float)
-        matrix_B_der = np.array(derive_by_array(matB, symbols(fluxids)), dtype = float)
+        if JAX_INSTALLED:
+            lambA = lambdify(symbols(fluxids), matA, modules = 'jax')
+            lambB = lambdify(symbols(fluxids), matB, modules = 'jax')
+            
+            matrix_A_der = np.array(
+                jacfwd(lambA, range(len(fluxids)))(*jnp.ones(len(fluxids)))
+            )
+            matrix_B_der = np.array(
+                jacfwd(lambB, range(len(fluxids)))(*jnp.ones(len(fluxids)))
+            )
+        else:
+            matrix_A_der = np.array(
+                derive_by_array(matA, symbols(fluxids)), 
+                dtype = float
+            )
+            matrix_B_der = np.array(
+                derive_by_array(matB, symbols(fluxids)), 
+                dtype = float
+            )
         
         return matrix_A_der, matrix_B_der
     
     
     def _calculate_matrix_As_and_Bs_derivatives_u(self, n_jobs):
         '''
         Parameters
@@ -476,19 +504,28 @@
         return matrix_Ms_der
         
     
     def _calculate_matrix_Ms_derivatives_c(self):
         
         matrix_Ms_der = {}
         for size, EAM in self.model.EAMs.items():            
+            
             matM = Matrix(np.diag(symbols([emu.metabolite_id for emu in EAM.columns])))
-            matrix_M_der = np.array(
-                derive_by_array(matM, symbols(self.model.concids)), 
-                dtype = float
-            )
+            if JAX_INSTALLED:
+                lambM = lambdify(symbols(self.model.concids), matM, modules = 'jax')
+                matrix_M_der = np.array(
+                    jacfwd(lambM, 
+                           range(len(self.model.concids))
+                    )(*jnp.ones(len(self.model.concids)))
+                )
+            else:
+                matrix_M_der = np.array(
+                    derive_by_array(matM, symbols(self.model.concids)), 
+                    dtype = float
+                )
             matrix_Ms_der[size] = matrix_M_der
             
         return matrix_Ms_der
         
         
     def _calculate_matrix_Ms_derivatives_p(self):
```

### Comparing `freeflux-0.3.1/src/freeflux.egg-info/PKG-INFO` & `freeflux-0.3.2/src/freeflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeflux
-Version: 0.3.1
+Version: 0.3.2
 Summary: FreeFlux is a package for 13C metabolic flux analysis
 Home-page: https://github.com/Chaowu88/freeflux
 Author: Chao Wu
 Author-email: chaowu09@gmail.com
 License: GNU General Public License v3.0
 Keywords: 13c,labeling pattern,metabolic flux analysis,metabolism,biology,non-linear programming,optimization,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freeflux-0.3.1/src/freeflux.egg-info/SOURCES.txt` & `freeflux-0.3.2/src/freeflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

