# Comparing `tmp/richvalues-3.0.9.tar.gz` & `tmp/richvalues-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.0.9.tar", last modified: Tue Apr 11 22:48:32 2023, max compression
+gzip compressed data, was "richvalues-3.1.0.tar", last modified: Mon Apr 24 07:44:48 2023, max compression
```

## Comparing `richvalues-3.0.9.tar` & `richvalues-3.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 22:48:32.340209 richvalues-3.0.9/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 22:48:32.340209 richvalues-3.0.9/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      809 2023-04-10 11:41:38.000000 richvalues-3.0.9/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      515 2023-04-11 22:47:59.000000 richvalues-3.0.9/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 22:48:32.336209 richvalues-3.0.9/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   146680 2023-04-11 22:48:24.000000 richvalues-3.0.9/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-04-11 22:48:32.336209 richvalues-3.0.9/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1308 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-04-11 22:48:32.000000 richvalues-3.0.9/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-04-11 22:48:32.340209 richvalues-3.0.9/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      752 2023-04-11 22:47:54.000000 richvalues-3.0.9/setup.py
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 07:44:48.932227 richvalues-3.1.0/
+-rw-rw-r--   0 andresmegias   (501) staff       (20)     1532 2023-04-20 22:48:48.000000 richvalues-3.1.0/LICENSE
+-rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 07:44:48.931796 richvalues-3.1.0/PKG-INFO
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      848 2023-04-24 07:29:24.000000 richvalues-3.1.0/README.md
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      655 2023-04-24 07:41:47.000000 richvalues-3.1.0/pyproject.toml
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 07:44:48.929056 richvalues-3.1.0/richvalues/
+-rw-rw-r--   0 andresmegias   (501) staff       (20)   155180 2023-04-24 07:25:15.000000 richvalues-3.1.0/richvalues/__init__.py
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 07:44:48.931282 richvalues-3.1.0/richvalues.egg-info/
+-rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/PKG-INFO
+-rw-r--r--   0 andresmegias   (501) staff       (20)      233 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/SOURCES.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)        1 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/dependency_links.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       30 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/requires.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       11 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/top_level.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       38 2023-04-24 07:44:48.932370 richvalues-3.1.0/setup.cfg
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      748 2023-04-24 07:35:45.000000 richvalues-3.1.0/setup.py
```

### Comparing `richvalues-3.0.9/PKG-INFO` & `richvalues-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.9
+Version: 3.1.0
 Summary: Python library for working with uncertainties and upper/lower limits
-Home-page: https://github.com/andresmegias/richvalues
+Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
-Description: # RichValues
-        
-        Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
-        
-        The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. 
+
+With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
+
+The libraries NumPy, Pandas, SciPy and Matplotlib are required by RichValues. An user guide and some examples are available in the GitHub repository: https://github.com/andresmegias/richvalues/.
+
+
```

### Comparing `richvalues-3.0.9/README.md` & `richvalues-3.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-# RichValues
+RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. 
 
-Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
+With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
 
-The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues.
+The libraries NumPy, Pandas, SciPy and Matplotlib are required by RichValues. An user guide and some examples are available in the GitHub repository: https://github.com/andresmegias/richvalues/.
```

### Comparing `richvalues-3.0.9/pyproject.toml` & `richvalues-3.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.0.9"
+version = "3.1.0"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
-    "Operating System :: OS Independent"
-]
+    "Operating System :: OS Independent"]
+homepage = "https://github.com/andresmegias/richvalues/"
+documentation = "https://github.com/andresmegias/richvalues/blob/main/userguide.pdf"
```

### Comparing `richvalues-3.0.9/richvalues/__init__.py` & `richvalues-3.1.0/richvalues/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Rich Values Library
 -------------------
-Version 3.0
+Version 3.1
 
 Copyright (C) 2023 - Andrés Megías Toledano
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
@@ -33,43 +33,43 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.0.9'
+__version__ = '3.1.0'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from scipy.optimize import minimize
 from scipy.stats import linregress
 
 defaultparams = {
     'domain': [-np.inf, np.inf],
-    'size of samples': int(8e3),
+    'size of samples': int(12e3),
     'number of significant figures': 1,
     'limit for extra significant figure': 2.5,
     'minimum exponent for scientific notation': 4,
     'sigmas to define upper/lower limits': 2.,
     'sigmas to use approximate uncertainty propagation': 20.,
     'use 1-sigma combinations to approximate uncertainty propagation': False,
     'fraction of the central value for upper/lower limits': 0.2,
     'number of repetitions to estimate upper/lower limits': 4,
     'decimal exponent to define zero': -90.,
     'decimal exponent to define infinity': 90.,
     'multiplication symbol for scientific notation in LaTeX': '\\cdot',
     'sigmas for overlap': 1.,
-    'sigmas for interval': 3.
+    'sigmas for intervals': 3.
     }
 
 variable_count = 1
 variable_dict = {}
 
 def round_sf(x,
         n=defaultparams['number of significant figures'],
@@ -113,15 +113,15 @@
     base = '{:e}'.format(x).split('e')[0]
     m = n+1 if round(float(base), n) <= extra_sf_lim else n
     y = str(float('{:.{}g}'.format(x, m)))
     base = '{:e}'.format(float(y)).split('e')[0]
     if round(float(base), n) <= extra_sf_lim:
         n += 1
     integers = len(y.split('.')[0])
-    if x > 1 and integers >= n:
+    if x >= 1 and integers >= n:
         y = y.replace('.0','')
     digits = str(y).replace('.','')
     for i in range(len(digits)-1):
         if digits.startswith('0'):
             digits = digits[1:]
     digits = len(digits)
     if n > digits and 'e' not in y:
@@ -209,15 +209,15 @@
                                extra_sf_lim=extra_sf_lim)
             m = len(base_dy.split('.')[1]) if '.' in base_dy else 0
             base_y = '{:.{}f}'.format(float(base_y), m)
             base_dy = '{:.{}f}'.format(float(base_dy), m)
             y = '{}e{}'.format(base_y, exp_y)
             dy = '{}e{}'.format(base_dy, exp_y)
     elif dx == 0:
-        y = round_sf(x, n+1, min_exp, extra_sf_lim)
+        y = round_sf(x, n, min_exp, extra_sf_lim)
         dy = '0e0'
     else:
         y = 'nan'
         dy = 'nan'
     if float(y) != 0 and y != 'nan':
         y = sign + y
     if not use_exp:
@@ -283,15 +283,15 @@
     return y, dy
 
 class RichValue():
     """
     A class to store a value with uncertainties or with upper/lower limits.
     """
     
-    def __init__(self, main=None, unc=0, is_lolim=False, is_uplim=False,
+    def __init__(self, main=None, unc=0., is_lolim=False, is_uplim=False,
                  is_range=False, domain=defaultparams['domain'], **kwargs):
         """
         Parameters
         ----------
         main : float
             Central value of the rich value, or value of the upper/lower limit.
         unc : float / list (float), optional
@@ -340,39 +340,37 @@
         
         if type(main) in [list, tuple]:
             is_lolim, is_uplim, is_range = False, False, False
             main = [float(main[0]), float(main[1])]
             if main_or[0] <= domain[0] and main_or[1] < domain[1]:
                 is_uplim = True
                 main = main[1]
-                unc = 0
             elif main_or[1] >= domain[1] and main_or[0] > domain[0]:
                 is_lolim = True
                 main = main[0]
-                unc = 0
             else:
                 is_range = True
             if is_lolim and is_uplim:
                 is_range = True
                 main = domain
             if main == domain:
                 main = np.nan
-                unc = 0
                 is_range = False
             if is_range:
                 unc = (main[1] - main[0]) / 2
                 main = (main[0] + main[1]) / 2
         else:
             main = float(main)
         if not hasattr(unc, '__iter__'):
             unc = [unc, unc]
         if any(np.isinf(unc)):
             main = np.nan
-            unc = [0, 0]
-        unc = np.nan_to_num(unc, nan=0)
+        if is_lolim or is_uplim or not np.isfinite(main):
+            unc = [np.nan]*2
+        
         if not np.isnan(main) and not domain[0] <= main <= domain[1]:
             raise Exception('Invalid main value {} for domain {}.'
                             .format(main, domain))
         unc = list(unc)
         unc = [float(unc[0]), float(unc[1])]
         unc[0] = abs(unc[0])
         if not (is_lolim or is_uplim) and unc[1] < 0:
@@ -421,14 +419,15 @@
         self.unc = unc
         self.is_lolim = is_lolim
         self.is_uplim = is_uplim
         self.is_range = is_range
         self.domain = domain
         self.num_sf = defaultparams['number of significant figures']
         self.min_exp = defaultparams['minimum exponent for scientific notation']
+        self.extra_sf_lim = defaultparams['limit for extra significant figure']
         self.vars = [expression]
         self.expression = expression
         
         global variable_dict
         variable_dict[expression] = self
           
     @property
@@ -451,122 +450,143 @@
         """Central value"""
         cent = self.main if self.is_centr else np.nan
         return cent  
     @property
     def unc_eb(self):
         """Uncertainties with shape (2,1)"""
         unceb = [[self.unc[0]], [self.unc[1]]]
-        return unceb    
+        return unceb
     @property
     def rel_unc(self):
         """Relative uncertainties"""
-        m, s = self.main, self.unc
-        with np.errstate(divide='ignore', invalid='ignore'):
-            runc = list(np.array(s) / abs(m))
+        if self.is_centr:
+            m, s = self.main, self.unc
+            with np.errstate(divide='ignore', invalid='ignore'):
+                runc = list(np.array(s) / abs(m))
+        else:
+            runc = [np.nan]*2
         return runc
     @property
     def signal_noise(self):
         """Signal-to-noise ratios (S/N)"""
-        m, s = self.main, self.unc
-        with np.errstate(divide='ignore', invalid='ignore'):
-            s_n = list(np.nan_to_num(abs(m) / np.array(s),
-                       nan=0, posinf=np.inf))
+        if self.is_centr:
+            m, s = self.main, self.unc
+            with np.errstate(divide='ignore', invalid='ignore'):
+                s_n = list(np.nan_to_num(abs(m) / np.array(s),
+                           nan=0, posinf=np.inf))
+        else:
+            s_n = [np.nan]*2
         return s_n
     @property    
     def ampl(self):
         """Amplitudes"""
         m, b = self.main, self.domain
         a = [m - b[0], b[1] - m]
         return a
-    @property        
+    @property
     def rel_ampl(self):
         """Relative amplitudes"""
-        s, a = self.unc, self.ampl
-        with np.errstate(divide='ignore'):
-            a_s = list(np.array(a) / np.array(s))
+        if self.is_centr:
+            s, a = self.unc, self.ampl
+            with np.errstate(divide='ignore', invalid='ignore'):
+                a_s = list(np.array(a) / np.array(s))
+        else:
+            a_s = [np.nan]*2
         return a_s
     @property
     def norm_unc(self):
         """Normalized uncertainties"""
-        s, a = self.unc, self.ampl
-        s_a = list(np.array(s) / np.array(a))
+        if self.is_centr:
+            s, a = self.unc, self.ampl
+            s_a = list(np.array(s) / np.array(a))
+        else:
+            s_a = [np.nan]*2
         return s_a
     @property
     def prop_score(self):
         """Minimum of the signals-to-noise and the relative amplitudes."""
-        s_n = self.signal_noise
-        a_s = self.rel_ampl
-        pf = np.min([s_n, a_s])
+        if self.is_centr:
+            s_n = self.signal_noise
+            a_s = self.rel_ampl
+            pf = np.min([s_n, a_s])
+        else:
+            pf = 0.
         return pf
     @property
     def is_nan(self):
         """Not a number value."""
-        isnan = (True if np.isnan(self.main) or any(np.isinf(self.unc))
-                 else False)
+        isnan = np.isnan(np.diff(self.interval(sigmas=np.inf)))
         return isnan
     @property
     def is_inf(self):
         """Infinite value."""
-        isinf = (True if np.isinf(self.main) and not any(np.isinf(self.unc))
-                 else False)
+        isinf = np.isinf(np.diff(self.interval(sigmas=np.inf)))
         return isinf
     @property
     def is_finite(self):
         """Finite value."""
-        isfinite = (True if np.isfinite(self.main)
-                    and all(np.isfinite(self.unc)) else False)
+        isfinite = np.isfinite(np.diff(self.interval(sigmas=np.inf)))
         return isfinite
     
-    def interval(self, sigmas=defaultparams['sigmas for interval']):
+    def interval(self, sigmas=defaultparams['sigmas for intervals']):
         """Interval of possible values of the rich value."""
         if not self.is_interv:
-            ampl1 = sigmas * self.unc[0] if self.unc[0] != 0 else 0
-            ampl2 = sigmas * self.unc[1] if self.unc[1] != 0 else 0
-            interv = [max(self.domain[0], self.main - ampl1),
-                      min(self.domain[1], self.main + ampl2)]
+            if np.isfinite(self.main):
+                ampl1 = sigmas * self.unc[0] if self.unc[0] != 0 else 0
+                ampl2 = sigmas * self.unc[1] if self.unc[1] != 0 else 0
+                interv = [max(self.domain[0], self.main - ampl1),
+                          min(self.domain[1], self.main + ampl2)]
+            elif np.isinf(self.main):
+                interv = [self.main, self.main]
+            elif np.isnan(self.main):
+                interv = [np.nan, np.nan]
         else:
             if self.is_uplim and not self.is_lolim:
                 interv = [self.domain[0], self.main]
             elif self.is_lolim and not self.is_uplim:
                 interv = [self.main, self.domain[1]]
             else:
                 interv = [self.main - self.unc[0], self.main + self.unc[1]]
         return interv
     
     def sign(self, sigmas=np.inf):
-        """Sign of the richvalue."""
+        """Sign of the rich value."""
         interv = self.interval(sigmas)
         signs_interv = np.sign(interv)
         if all(signs_interv == 0):
             s = 0
         elif all(signs_interv >= 0):
             s = 1
         elif all(signs_interv <= 0):
             s = -1
         else:
             s = np.nan
         return s
   
-    def set_lims_factor(self, factor=4.):
+    def set_lim_unc(self, factor=4.):
         """Set uncertainties of limits with respect to cetral values."""
-        if self.is_lolim or self.is_uplim:
+        if self.is_lim:
             self.unc = [self.main / factor, self.main / factor]
         
     def _format_as_rich_value(self):
         main = copy.copy(self.main)
         unc = copy.copy(self.unc)
         is_lolim = self.is_lolim
         is_uplim = self.is_uplim
         domain = self.domain
         is_range = self.is_range
-        min_exp = self.min_exp
-        extra_sf_lim = defaultparams['limit for extra significant figure']
+        min_exp = abs(self.min_exp)
+        extra_sf_lim = self.extra_sf_lim
         x = copy.copy(main)
         dx = copy.copy(unc)
         n = copy.copy(self.num_sf)
+        try:
+            range_bound = self.range_bound
+        except:
+            range_bound = False
         use_exp = True
         if ((float(x) > float(max(dx))
              and abs(np.floor(_log10(abs(float(x))))) < min_exp)
              or (float(x) <= float(max(dx))
                  and float('{:e}'.format(max(dx))
                            .split('e')[0]) > extra_sf_lim
                  and any(abs(np.floor(_log10(abs(np.array(dx)))))
@@ -575,15 +595,18 @@
              or (self.is_lim and abs(np.floor(_log10(abs(float(x))))) < min_exp)
              or np.isinf(min_exp)):
             use_exp = False
         if not is_range and not np.isnan(main):
             x = main
             dx1, dx2 = unc
             if not self.is_lim:
-                y, (dy1, dy2) = round_sf_uncs(x, [dx1, dx2], n, min_exp)
+                if dx1 == dx2 == 0 and not range_bound:
+                    n += 1
+                y, (dy1, dy2) = round_sf_uncs(x, [dx1, dx2], n,
+                                              min_exp, extra_sf_lim)
                 if 'e' in y:
                     y, a = y.split('e')
                     a = int(a)
                 else:
                     a = 0
                 if 'e' in dy1:
                     dy1, _ = dy1.split('e')
@@ -595,15 +618,15 @@
                     else:
                         text = '{} e{}'.format(y, a)
                 else:
                     text = '{}-{}+{} e{}'.format(y, dy1, dy2, a)
                 if not use_exp:
                     text = text.replace(' e0','')
             else:
-                y = round_sf(x, n, min_exp)
+                y = round_sf(x, n, min_exp, extra_sf_lim)
                 if 'e' in y:
                     y, a = y.split('e')
                     a = int(a)
                 else:
                     a = 0
                 if is_lolim:
                     sign = '>'
@@ -613,24 +636,27 @@
             if use_exp:
                 text = text.replace('e-0', 'e-')
                 a = int(text.split('e')[1])
                 if abs(a) < min_exp:
                     z = RichValue(x, dx, is_lolim, is_uplim, is_range, domain)
                     z.num_sf = n
                     z.min_exp = np.inf
+                    z.extra_sf_lim = extra_sf_lim
                     text = str(z)
             else:
                 text = text.replace(' e0','')
         elif not is_range and np.isnan(main):
             text = 'nan'
         else:
             x1 = RichValue(main - unc[0], domain=domain)
             x2 = RichValue(main + unc[1], domain=domain)
             x1.min_exp = min_exp
             x2.min_exp = min_exp
+            x1.range_bound = True
+            x2.range_bound = True
             text = '{} -- {}'.format(x1, x2)
         return text
         
     def __repr__(self):
         return self._format_as_rich_value()
     
     def __str__(self):
@@ -640,17 +666,17 @@
                                  + 'symbol for scientific notation in LaTeX']):
         """Display in LaTeX format"""
         main = copy.copy(self.main)
         unc = copy.copy(self.unc)
         domain = self.domain
         is_lolim = self.is_lolim
         is_uplim = self.is_uplim
-        min_exp = self.min_exp
+        min_exp = abs(self.min_exp)
         is_range = self.is_range
-        extra_sf_lim = defaultparams['limit for extra significant figure']
+        extra_sf_lim = self.extra_sf_lim
         use_exp = True
         x = copy.copy(main)
         dx = copy.copy(unc)
         n = copy.copy(self.num_sf)
         if ((float(x) > float(max(dx))
              and abs(np.floor(_log10(abs(float(x))))) < min_exp)
              or (float(x) <= float(max(dx))
@@ -662,56 +688,62 @@
              or np.isinf(min_exp)):
             use_exp = False
         text = ''
         non_numerics = ['nan', 'NaN', 'None', 'inf', '-inf']
         is_numeric = False if str(main) in non_numerics else True
         if is_numeric:
             if not is_range:
-                _, unc_r = round_sf_uncs(x, dx, n)
+                _, unc_r = round_sf_uncs(x, dx, n, min_exp, extra_sf_lim)
                 unc_r = np.array(unc_r, float)
             if not is_range and not use_exp:
                 if not (is_lolim or is_uplim):
                     if unc_r[0] == unc_r[1]:
                         if unc_r[0] == unc_r[1] == 0:
-                            y = round_sf(x, n+1, np.inf)
+                            y = round_sf(x, n+1, np.inf, extra_sf_lim)
                             text = '${}$'.format(y)
                         else:
-                            y, dy = round_sf_unc(x, dx[0], n, min_exp)
+                            y, dy = round_sf_unc(x, dx[0], n,
+                                                 min_exp, extra_sf_lim)
                             text = '${} \pm {}$'.format(y, dy)
                     else:
-                        y, dy = round_sf_uncs(x, dx, n, min_exp)
+                        y, dy = round_sf_uncs(x, dx, n, min_exp, extra_sf_lim)
                         text = '$'+y + '_{-'+dy[0]+'}^{+'+dy[1]+'}$'
                 else:
                     if is_lolim:
                         sign = '>'
                     elif is_uplim:
                         sign = '<'
-                    y = round_sf(x, n, min_exp)
+                    y = round_sf(x, n, min_exp, extra_sf_lim)
                     text = '${} {}$'.format(sign, y)
             elif not is_range and use_exp:
                 if not (is_lolim or is_uplim):
                     if unc_r[0] == unc_r[1]:
                         if unc_r[0] == unc_r[1] == 0:
-                            y = round_sf(x, n+1, min_exp)
-                            y, a = y.split('e') if 'e' in y else y, '0'
+                            y = round_sf(x, n+1, min_exp, extra_sf_lim)
+                            if 'e' in y:
+                                y, a = y.split('e')
+                            else:
+                                a = '0'
                             a = str(int(a))
                             text = ('${} {}'.format(y, mult_symbol)
                                     + ' 10^{'+a+'}$')
                         else:
-                            y, dy = round_sf_unc(x, dx[0], n, min_exp)
+                            y, dy = round_sf_unc(x, dx[0], n,
+                                                 min_exp, extra_sf_lim)
                             if 'e' in y:
                                 y, a = y.split('e')
                                 dy, a = dy.split('e')
                             else:
                                 a = 0
                             a = str(int(a))
                             text = ('$({} \pm {})'.format(y, dy)
                                      + mult_symbol + '10^{'+a+'}$')
                     else:
-                        y, dy = round_sf_uncs(x, [dx[0], dx[1]], n, min_exp)
+                        y, dy = round_sf_uncs(x, [dx[0], dx[1]], n,
+                                              min_exp, extra_sf_lim)
                         if 'e' in y:
                             y, a = y.split('e')
                             dy1, a = dy[0].split('e')
                             dy2, a = dy[1].split('e')
                         else:
                             dy1, dy2 = dy
                             a = 0
@@ -719,27 +751,28 @@
                         text = ('$'+y + '_{-'+dy1+'}^{+'+dy2+'} '
                                 + mult_symbol + ' 10^{'+a+'}' + '$')
                 else:
                     if is_lolim:
                         symbol = '>'
                     elif is_uplim:
                         symbol = '<'
-                    y = round_sf(x, n, min_exp=0)
+                    y = round_sf(x, n, min_exp=0, extra_sf_lim=extra_sf_lim)
                     y, a = y.split('e')
                     a = str(int(a))
                     text = ('${} {} {}'.format(symbol, y, mult_symbol)
                             + ' 10^{'+a+'}$')
                 if use_exp:
                     text = text.replace('e-0', 'e-').replace('e+','e')
                     a = int(text.split('10^{')[1].split('}')[0])
                     if abs(a) < min_exp:
                         y = RichValue(x, dx, is_lolim, is_uplim,
                                       is_range, domain)
                         y.num_sf = n
                         y.min_exp = np.inf
+                        y.extra_sf_lim = extra_sf_lim
                         text = y.latex(dollars, mult_symbol)
             else:
                 x1 = RichValue(main - unc[0], domain=domain)
                 x2 = RichValue(main + unc[1], domain=domain)
                 x1.min_exp = min_exp
                 x2.min_exp = min_exp
                 text = '{} -- {}'.format(x1.latex(dollars, mult_symbol),
@@ -747,17 +780,37 @@
         else:
             text = (str(main).replace('NaN','nan').replace('nan','...')
                     .replace('inf','$\infty$'))
         if not dollars:
             text = text.replace('$','')
         return text
    
+    def __neg__(self):
+        main = copy.copy(self.main)
+        unc = copy.copy(self.unc)
+        domain = copy.copy(self.domain)
+        if not self.is_interv:
+            x = -main
+        else:
+            x1, x2 = self.interval()
+            x = [-x2, -x1]
+        dx = np.abs(unc)
+        domain = [-domain[0], -domain[1]]
+        domain = [min(domain), max(domain)]
+        new_rval = RichValue(x, dx, domain=domain)
+        new_rval.num_sf = self.num_sf
+        new_rval.min_exp = self.min_exp
+        new_rval.extra_sf_lim = self.extra_sf_lim
+        new_rval.vars = self.vars
+        new_rval.expression = '-({})'.format(self.expression)
+        return new_rval
+    
     def __abs__(self):
         sigmas = defaultparams['sigmas to use approximate '
-                       + 'uncertainty propagation']
+                               + 'uncertainty propagation']
         x = copy.copy(self.main)
         dx = copy.copy(self.unc)
         domain = copy.copy(self.domain)
         x1, x2 = self.interval(sigmas=np.inf)
         if all(np.array([x1, x2]) >= 0):
             if (self.is_centr and self.prop_score > sigmas) or self.is_interv:
                 new_rval = self
@@ -774,33 +827,19 @@
                 else:
                     new_rval = self.function(lambda x: abs(x), domain=domain)
             else:
                 x2 = max(np.abs([x1, x2]))
                 x1 = 0
                 new_rval = RichValue([x1, x2], dx, domain=domain)
         new_rval.domain[0] = max(0, new_rval.domain[0])
+        new_rval.num_sf = self.num_sf
+        new_rval.min_exp = self.min_exp
+        new_rval.extra_sf_lim = self.extra_sf_lim
         new_rval.expression = 'abs({})'.format(self.expression)
         return new_rval
-   
-    def __neg__(self):
-        main = copy.copy(self.main)
-        unc = copy.copy(self.unc)
-        domain = copy.copy(self.domain)
-        if not self.is_interv:
-            x = -main
-        else:
-            x1, x2 = self.interval()
-            x = [-x2, -x1]
-        dx = np.abs(unc)
-        domain = [-domain[0], -domain[1]]
-        domain = [min(domain), max(domain)]
-        new_rval = RichValue(x, dx, domain=domain)
-        new_rval.vars = self.vars
-        new_rval.expression = '-({})'.format(self.expression)
-        return new_rval
     
     def __add__(self, other):
         if type(other) in (np.ndarray, RichArray):
             return other + self
         elif type(other) is RichValue:
             other_vars = other.vars
             other_expression = other.expression
@@ -819,14 +858,17 @@
                 if other_ != 0:
                     x = self.main + other_
                     dx = np.abs(self.unc)
                     new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                          self.is_range, self.domain)
                 else:
                     new_rval = RichValue(0, domain=self.domain)
+                new_rval.num_sf = self.num_sf
+                new_rval.min_exp = self.min_exp
+                new_rval.extra_sf_lim = self.extra_sf_lim
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
         new_rval.vars = list(variables)
         new_rval.expression = expression
@@ -874,14 +916,15 @@
                     if not np.isfinite(domain2):
                         domain2 = np.inf
                     domain = [domain1, domain2]
                     new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                          self.is_range, domain)
                     new_rval.num_sf = self.num_sf
                     new_rval.min_exp = self.min_exp
+                    new_rval.extra_sf_lim = self.extra_sf_lim
                 else:
                     new_rval = RichValue(0, domain=self.domain)
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
@@ -922,16 +965,14 @@
                         if not np.isfinite(domain1):
                             domain1 = -np.inf
                         if not np.isfinite(domain2):
                             domain2 = np.inf
                         domain = [domain1, domain2]
                     new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                          self.is_range, domain)
-                    new_rval.num_sf = self.num_sf
-                    new_rval.min_exp = self.min_exp
                 else:
                     if type(other_) is not RichValue:
                         other_domain = (other.domain if type(other)
                                         is RichValue else None)
                         other_ = RichValue(other_, domain=other_domain)
                     zero = other_
                     zero_signs = np.sign(zero.domain)
@@ -946,14 +987,17 @@
                     sign = self.sign() * zero_sign
                     value = sign * np.inf
                     if np.isinf(value):
                         domain = [0, np.inf] if value > 0 else [-np.inf, 0]
                     else:
                         domain = (sign * abs(self)).domain
                     new_rval = RichValue(value, domain=domain)
+                new_rval.num_sf = self.num_sf
+                new_rval.min_exp = self.min_exp
+                new_rval.extra_sf_lim = self.extra_sf_lim
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
         new_rval.vars = list(variables)
         new_rval.expression = expression
@@ -989,18 +1033,19 @@
                         if not np.isfinite(domain1):
                             domain1 = -np.inf
                         if not np.isfinite(domain2):
                             domain2 = np.inf
                         domain = [domain1, domain2]
                     new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                          self.is_range, domain)
-                    new_rval.num_sf = self.num_sf
-                    new_rval.min_exp = self.min_exp
                 else:
                     new_rval = RichValue(0, domain=self.domain)
+                new_rval.num_sf = self.num_sf
+                new_rval.min_exp = self.min_exp
+                new_rval.extra_sf_lim = self.extra_sf_lim
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
         new_rval.vars = list(variables)
         new_rval.expression = expression
@@ -1033,15 +1078,14 @@
                         domain = [0, np.inf]
                     else:
                         domain = self.domain
                     new_rval = function_with_rich_values(lambda a,b: a**b,
                                                 [self, other_], domain=domain)
                 else:
                     new_rval = RichValue(0)
-                    new_rval.num_sf = self.num_sf
             elif (type(other) is not RichValue and self.prop_score > sigmas):
                 x = main ** other
                 dx = np.abs(x * other * np.array(unc) / main)
                 if domain != [-np.inf, np.inf]:
                     if domain[0] != 0 or (domain[0] == 0 and other>0):
                         x1 = domain[0] ** other
                     else:
@@ -1052,20 +1096,22 @@
                         x2 = np.inf
                     domain = [x1, x2]
                     domain = [min(domain), max(domain)]
                 else:
                     domain = [-np.inf, np.inf]
                 new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                      domain=domain)
-                new_rval.num_sf = self.num_sf
             else:
                 if (type(other) is RichValue and other.domain[0] < 0
                         and not np.isinf(other.main)):
                     print('Warning: Domain of exponent should be positive.')
                 new_rval = RichValue(np.nan)
+            new_rval.num_sf = self.num_sf
+            new_rval.min_exp = self.min_exp
+            new_rval.extra_sf_lim = self.extra_sf_lim
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
         new_rval.vars = list(variables)
         new_rval.expression = expression
@@ -1188,24 +1234,29 @@
     
     @property
     def is_finite_range(self): return self.is_range
     @is_finite_range.setter
     def is_finite_range(self, x): self.is_range = x
     
     @property
-    def number_of_scientific_figures(self): return self.num_sf
-    @number_of_scientific_figures.setter
-    def number_of_scientific_figures(self, x): self.num_sf = x 
+    def number_of_significant_figures(self): return self.num_sf
+    @number_of_significant_figures.setter
+    def number_of_significant_figures(self, x): self.num_sf = x
     
     @property
     def minimum_exponent_for_scientific_notation(self): return self.min_exp
     @minimum_exponent_for_scientific_notation.setter
     def minimum_exponent_for_scientific_notation(self, x): self.min_exp = x
     
     @property
+    def limit_for_extra_significant_figure(self): return self.extra_sf_lim
+    @limit_for_extra_significant_figure.setter
+    def limit_for_extra_significant_figure(self, x): self.extra_sf = x
+    
+    @property
     def variables(self): return self.vars
     @variables.setter
     def variables(self, x): self.vars = x
     
     # Attribute acronyms.
     is_limit = is_lim
     is_interval = is_interv
@@ -1216,15 +1267,15 @@
     relative_amplitude = rel_ampl
     normalized_uncertainty = norm_unc
     propagation_score = prop_score
     is_not_a_number = is_nan
     is_infinite = is_inf
     # Method acronyms.
     probability_density_function = pdf
-    set_limits_factor = set_lims_factor
+    set_limit_uncertainty = set_lim_unc
 
 class RichArray(np.ndarray):
     """
     A class to store values with uncertainties or upper/lower limits.
     """
     
     def __new__(cls, mains=None, uncs=None, are_lolims=None, are_uplims=None,
@@ -1270,40 +1321,45 @@
         if 'are_upper_limits' in kwargs:
             are_uplims = kwargs['are_upper_limits']
         if 'are_finite_ranges' in kwargs:
             are_ranges = kwargs['are_finite_ranges']
         
         mains = np.array(mains)
         if uncs is None:
-            uncs = np.zeros((*mains.shape, 2))
+            uncs = 0.
         if are_lolims is None:
-            are_lolims = np.zeros(mains.shape, bool)
+            are_lolims = False
         if are_uplims is None:
-            are_uplims = np.zeros(mains.shape, bool)
+            are_uplims = False
         if are_ranges is None:
-            are_ranges = np.zeros(mains.shape, bool)
+            are_ranges = False
         if domains is None:
             domains = (np.array([[-np.inf, np.inf] for x in mains.flat])
-                       .reshape((*mains.shape, 2)))
-            
+                       .reshape((*mains.shape, 2)))  
         uncs = np.array(uncs)
         are_lolims = np.array(are_lolims)
         are_uplims = np.array(are_uplims)
         are_ranges = np.array(are_ranges)
         domains = np.array(domains)
-        array = np.empty(mains.size, object)
+
         if uncs.size == 1:
-            uncs = uncs * np.ones((*mains.shape, 2))
+            uncs = uncs * np.ones((*mains.shape, 2), float)
         elif len(uncs) == 2 and type(uncs[0]) is not np.ndarray:
             uncs = np.array([uncs[0] * np.ones(mains.shape),
                              uncs[1] * np.ones(mains.shape)])
         elif uncs.shape == (*mains.shape, 2):
             uncs = uncs.transpose()
         elif uncs.shape == mains.shape:
             uncs = np.array([[uncs]]*2).reshape((2, *mains.shape))
+        if are_lolims.size == 1:
+            are_lolims = are_lolims * np.ones(mains.shape, bool)
+        if are_uplims.size == 1:
+            are_uplims = are_uplims * np.ones(mains.shape, bool)
+        if are_ranges.size == 1:
+            are_ranges = are_ranges * np.ones(mains.shape, bool)
         if len(domains) == 2 and type(domains[0]) is not np.ndarray:
             domains = np.array([domains[0] * np.ones(mains.shape),
                                 domains[1] * np.ones(mains.shape)])
         elif domains.shape == (*mains.shape, 2):
             domains = domains.transpose()
         elif domains.flatten().shape == (2,):
             domains = (np.array([domains for x in mains.flat])
@@ -1312,14 +1368,15 @@
         mains_flat = mains.flatten()
         uncs_flat = uncs.flatten()
         are_lolims_flat = are_lolims.flatten()
         are_uplims_flat = are_uplims.flatten()
         are_ranges_flat = are_ranges.flatten()
         domains_flat = domains.flatten()
         offset = len(uncs_flat) // 2
+        array = np.empty(mains.size, RichValue)
         for i in range(mains.size):
             main = mains_flat[i]
             unc = [uncs_flat[i], uncs_flat[i+offset]]
             is_lolim = are_lolims_flat[i]
             is_uplim = are_uplims_flat[i]
             is_range = are_ranges_flat[i]
             domain = [domains_flat[i], domains_flat[i+offset]]
@@ -1350,14 +1407,17 @@
     @property
     def nums_sf(self):
         return np.array([x.num_sf for x in self.flat]).reshape(self.shape)
     @property
     def min_exps(self):
         return np.array([x.min_exp for x in self.flat]).reshape(self.shape)
     @property
+    def extra_sf_lims(self):
+        return np.array([x.extra_sf_lim for x in self.flat]).reshape(self.shape)
+    @property
     def are_lims(self):
         return np.array([x.is_lim for x in self.flat]).reshape(self.shape)
     @property
     def are_intervs(self):
         return np.array([x.is_interv for x in self.flat]).reshape(self.shape)
     @property
     def are_centrs(self):
@@ -1371,49 +1431,56 @@
                 .reshape((*self.shape,2)))
     @property
     def signals_noises(self):
         return (np.array([x.signal_noise for x in self.flat])
                 .reshape((*self.shape,2)))
     @property
     def ampls(self):
-        return (np.array([x.ampls for x in self.flat])
+        return (np.array([x.ampl for x in self.flat])
                 .reshape((*self.shape,2)))
     @property
     def rel_ampls(self):
-        return (np.array([x.rel_ampls for x in self.flat])
+        return (np.array([x.rel_ampl for x in self.flat])
                 .reshape((*self.shape,2)))
     @property
     def norm_uncs(self):
         return (np.array([x.norm_unc for x in self.flat])
-                .reshape((self.shape,2)))
+                .reshape((*self.shape,2)))
     @property
     def prop_scores(self):
         return (np.array([x.prop_score for x in self.flat])
                 .reshape(self.shape))
     @property
     def uncs_eb(self):
         return self.uncs.transpose()
     
-    def intervals(self, sigmas=None):
-        return (np.array([x.interval() for x in self.flat])
+    def intervals(self, sigmas=defaultparams['sigmas for intervals']):
+        return (np.array([x.interval(sigmas) for x in self.flat])
                 .reshape((*self.shape,2)))
+
+    def signs(self, sigmas=np.inf):
+        return (np.array([x.sign(sigmas) for x in self.flat])
+                .reshape(self.shape))
     
     def set_params(self, params):
         """Set the rich value parameters of each entry of the rich array."""
         for x in self.flat:
             if 'domain' in params:
                 x.domain = params['domain']
-            for key in ('num_sf', 'number of scientific figures'):
+            for key in ('num_sf', 'number of significant figures'):
                 if key in params:
                     x.num_sf = params[key]
             for key in ('min_exp', 'minimum exponent for scientific notation'):
                 if key in params:
                     x.min_exp = params[key]
+            for key in ('extra_sf_lim', 'limit for extra significant figure'):
+                if key in params:
+                    x.extra_sf_lim = params[key]
     
-    def set_lims_factor(self, factor=4.):
+    def set_lims_uncs(self, factor=4.):
         """Set uncertainties of limits with respect to central values."""
         c = factor
         if not hasattr(c, '__iter__'):
             c = [c, c]
         cl, cu = c
         if cl == 0:
             cl = 1
@@ -1456,118 +1523,139 @@
 
     # Attribute acronyms.
     main_values = mains
     uncertainties = uncs
     are_lower_limits = are_lolims
     are_upper_limits = are_uplims
     are_finite_ranges = are_ranges
-    numbers_of_scientific_figures = nums_sf
+    numbers_of_significant_figures = nums_sf
     minimum_exponents_for_scientific_notation = min_exps
+    limits_for_extra_significant_figure = extra_sf_lims
     are_limits = are_lims
     are_intervals = are_intervs
     are_centered_values = are_centrs
     relative_uncertainties = rel_uncs
     signals_to_noises = signals_noises
     amplitudes = ampls
     relative_amplitudes = rel_ampls
     normalized_uncertainties = norm_uncs
     propagation_scores = prop_scores
     # Method acronyms.
-    set_limits_factor = set_lims_factor
+    set_limits_uncertainties = set_lims_uncs
     set_parameters = set_params
 
 class RichDataFrame(pd.DataFrame):
     """
     A class to store a dataframe with uncertainties or with upper/lower limits.
     """
     
     @property
     def _constructor(self):
         return RichDataFrame
-    
     @property
     def _constructor_sliced(self):
         return RichSeries
+    @property
+    def values(self):
+        return pd.DataFrame(self).values.view(RichArray)
 
-    def _attribute(self, attribute):
-        """Apply the input RichArray attribute with 1 element."""
+    def _property(self, name):
+        """Apply the input RichArray attribute/method with 1 element."""
         code = [
-            'array = self.values',
-            'shape = array.shape',
-            'types = np.array([type(x) for x in array.flat]).reshape(shape)',
-            'data = np.zeros(shape, object)',
-            'cond = types == RichValue',
-            'data[cond] = rich_array(array[cond]).{}'.format(attribute),
-            'cond = ~cond',
-            'data[cond] = array[cond]',
+            'try:',
+            '    data = self.values.{}'.format(name),
+            'except:',
+            '    array = self.values',
+            '    shape = array.shape',
+            '    types = (np.array([type(x) for x in array.flat])'
+                       + '.reshape(shape))',
+            '    data = np.zeros(shape, object)',
+            '    cond = types == RichValue',
+            '    data[cond] = array[cond].{}'.format(name),
+            '    cond = ~cond',
+            '    data[cond] = array[cond]',
             'df = pd.DataFrame(data, self.index, self.columns)']
         code = '\n'.join(code)
         output = {}
         exec(code, {**{'self': self}, **globals()}, output)
         return output['df']
 
-    def _attribute2(self, attribute):
-        """Apply the input RichArray attribute with 2 elements."""
+    def _property2(self, name):
+        """Apply the input RichArray attribute/method with 2 elements."""
         code = [
             'array = self.values',
             'shape = array.shape',
-            'types = np.array([type(x) for x in array.flat]).reshape(shape)',
+            'types = (np.array([type(x) for x in array.flat])'
+                   + '.reshape(shape))',
             'data = np.zeros(shape, object)',
             'cond = types == RichValue',
-            'new_elements = rich_array(array[cond]).{}'.format(attribute),
+            'new_elements = array[cond].{}'.format(name),
             'new_elements = [[x[0], x[1]] for x in new_elements]',
             'new_subarray = np.frompyfunc(list, 0, 1)'
-            + '(np.empty(cond.sum(), dtype=object))',
+                 + '(np.empty(cond.sum(), dtype=object))',
             'new_subarray[:] = new_elements',
             'data[cond] = new_subarray',
             'cond = ~cond',
             'data[cond] = array[cond]',
             'df = pd.DataFrame(data, self.index, self.columns)']
         code = '\n'.join(code)
         output = {}
         exec(code, {**{'self': self}, **globals()}, output)
         return output['df']
 
     @property    
-    def mains(self): return self._attribute('mains')
+    def mains(self): return self._property('mains')
+    @property
+    def uncs(self): return self._property2('uncs')
+    @property
+    def are_lolims(self): return self._property('are_lolims')
+    @property
+    def are_uplims(self): return self._property('are_uplims')
+    @property
+    def are_ranges(self): return self._property('are_ranges')
     @property
-    def uncs(self): return self._attribute2('uncs')
+    def domains(self): return self._property2('domains')
     @property
-    def are_lolims(self): return self._attribute('are_lolims')
+    def nums_sf(self): return self._property('nums_sf')
     @property
-    def are_uplims(self): return self._attribute('are_uplims')
+    def min_exps(self): return self._property('min_exps')
     @property
-    def are_ranges(self): return self._attribute('are_ranges')
+    def extra_sf_lims(self): return self._property('extra_sf_lims')
     @property
-    def domains(self): return self._attribute2('domains')
+    def are_lims(self): return self._property('are_lims')
     @property
-    def are_lims(self): return self._attribute('are_lims')
+    def are_intervs(self): return self._property('are_intervs')
     @property
-    def are_intervs(self): return self._attribute('are_intervs')
+    def are_centrs(self): return self._property('are_centrs')
     @property
-    def are_centrs(self): return self._attribute('are_centrs')
+    def centers(self): return self._property('centers')
     @property
-    def rel_uncs(self): return self._attribute2('rel_uncs')
+    def rel_uncs(self): return self._property2('rel_uncs')
     @property
-    def signals_noises(self): return self._attribute2('signal_noises')
+    def signals_noises(self): return self._property2('signal_noises')
     @property
-    def ampls(self): return self._attribute2('ampls')
+    def ampls(self): return self._property2('ampls')
     @property
-    def rel_ampls(self): return self._attribute2('rel_ampls')
+    def rel_ampls(self): return self._property2('rel_ampls')
     @property
-    def norm_uncs(self): return self._attribute2('norm_uncs')
+    def norm_uncs(self): return self._property2('norm_uncs')
     @property
-    def prop_scores(self): return self._attribute('prop_scores')
+    def prop_scores(self): return self._property('prop_scores')
 
-    def intervals(self):
-        return self._attribute2('intervals')
+    def intervals(self, sigmas=defaultparams['sigmas for intervals']):
+        sigmas = str(sigmas).replace('inf', 'np.inf')
+        return self._property2('intervals({})'.format(sigmas))
+
+    def signs(self, sigmas=np.inf):
+        sigmas = str(sigmas).replace('inf', 'np.inf')
+        return self._property('signs({})'.format(sigmas))
     
-    def flatten_attribute_output(self, attribute):
-        """Separate the list elements from the output of the given attribute."""
-        df = eval('self.{}'.format(attribute))
+    def flatten_property(self, name):
+        """Separate the list elements from the given attribute/method output."""
+        df = eval('self.{}'.format(name))
         df1, df2 = df.copy(), df.copy()
         columns = df.columns
         are_lists = False
         for i,row in df.iterrows():
             for entry,col in zip(row,columns):
                 if (type(entry) is list and len(entry) == 2
                         and all([type(entry[i]) != str for i in [0,1]])):
@@ -1576,54 +1664,44 @@
                     df2.at[i,col] = entry[1]
                 else:
                     df1.at[i,col] = entry
                     df2.at[i,col] = entry
         output = [df1, df2] if are_lists else df1
         return output
     
-    def get_params(self):
-        """Return the rich value parameters of each column of the dataframe."""
-        domain, num_sf, min_exp = {}, {}, {}
-        for col in self:
-            x = self[col][0]
-            is_rich_value = True if type(x) is RichValue else False
-            domain[col] = (x.domain if is_rich_value
-                           else defaultparams['domain'])
-            num_sf[col] = (x.num_sf if is_rich_value else
-                           defaultparams['number of significant figures'])
-            min_exp[col] = (x.min_exp if is_rich_value
-                            else defaultparams['minimum exponent for '
-                                               + 'scientific notation'])
-        params = {'domain': domain, 'num_sf': num_sf, 'min_exp': min_exp}
-        return params
-    
     def set_params(self, params):
         """Set the rich value parameters of each column of the dataframe."""
-        for param_name in ['domain', 'num_sf', 'min_exp']:
+        for param_name in ['domain', 'num_sf', 'min_exp', 'extra_sf_lim']:
             if param_name in params and type(params[param_name]) is not dict:
                     default_param = params[param_name]
                     params[param_name] = {}
                     for col in self:
                         params[param_name][col] = default_param
         for col in self:
             num_rows = len(self[col])
             is_rich_value = True if type(self[col][0]) is RichValue else False
             if is_rich_value:
                 if 'domain' in params and col in params['domain']:
                     for i in range(num_rows):
                         self[col][i].domain = params['domain'][col]
-                for key in ('num_sf', 'number of scientific figures'):
+                for key in ('num_sf', 'number of significant figures'):
                     if key in params and col in params[key]:
                         for i in range(num_rows):
                             self[col][i].num_sf = params[key][col]
                 for key in ('min_exp',
                             'minimum exponent for scientific notation'):
                     if key in params and col in params[key]:
                         for i in range(num_rows):
                             self[col][i].min_exp = params[key][col]
+                for key in ('extra_sf_lim',
+                            'limit for extra significant figure'):
+                    if key in params and col in params[key]:
+                        for i in range(num_rows):
+                            self[col][i].extra_sf_lim = params[key][col]
+
     
     def create_column(self, function, columns, **kwargs):
         """
         Create a column applying a function to the given columns of the dataframe.
 
         Parameters
         ----------
@@ -1703,30 +1781,31 @@
                         entry = '...'
                     cols += [entry]
                 rows += [' & '.join(cols)]
             text = row_sep.join(rows)
             output = text
         return output
 
-    def set_lims_factors(self, limits_factors={}):
+    def set_lims_uncs(self, factors={}):
         """Set the uncertainties of limits with respect to central values."""
-        if limits_factors == {}:
-            limits_factors = 4.
-        if type(limits_factors) is not dict:
-            limits_factors = {col: limits_factors for col in self}
+        if factors == {}:
+            factors = 4.
+        if type(factors) is not dict:
+            factors = {col: factors for col in self}
         for i,row in self.iterrows():
-            for col in limits_factors:
+            for col in factors:
                 if 'RichValue' in str(type(self.at[i,col])):
                     entry = self.at[i,col]
-                    c = limits_factors[col]
-                    if not hasattr(c, '__iter__'):
-                        c = [c, c]
-                    cl, cu = c
-                    c = cl if entry.is_lolim else cu
-                    self.at[i,col].set_lims_factor(c)
+                    if entry.is_lim:
+                        c = factors[col]
+                        if not hasattr(c, '__iter__'):
+                            c = [c, c]
+                        cl, cu = c
+                        c = cl if entry.is_lolim else cu
+                        self.at[i,col].set_lim_unc(c)
     
     # Attribute acronyms.
     main_values = mains
     uncertainties = uncs
     are_lower_limits = are_lolims
     are_upper_limits = are_uplims
     are_finite_ranges = are_ranges
@@ -1736,108 +1815,113 @@
     relative_uncertainties = rel_uncs
     signals_to_noises = signals_noises
     amplitudes = ampls
     relative_amplitudes = rel_ampls
     normalized_uncertainties = norm_uncs
     propagation_scores = prop_scores
     # Method acronyms.
-    get_parameters = get_params
     set_parameters = set_params
-    set_limits_factors = set_lims_factors
+    set_limits_factors = set_lims_uncs
 
 class RichSeries(pd.Series):
     """A class to store a series with the RichArray methods."""
     
     @property
     def _constructor(self):
         return RichSeries
-    
     @property
     def _constructor_expanddim(self):
         return RichDataFrame
+    @property
+    def values(self):
+        return pd.Series(self).values.view(RichArray)
     
     @property
     def mains(self):
-        return pd.Series(rich_array(self.values).mains, self.index)
+        return pd.Series(self.values.view(RichArray).mains, self.index)
     @property
     def uncs(self):
-        return [pd.Series(rich_array(self.values).uncs.T[i].T,
+        return [pd.Series(self.values.view(RichArray).uncs.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def are_lolims(self):
-        return pd.Series(rich_array(self.values).are_lolims, self.index)
+        return pd.Series(self.values.view(RichArray).are_lolims, self.index)
     @property
     def are_uplims(self):
-        return pd.Series(rich_array(self.values).are_uplims, self.index)
+        return pd.Series(self.values.view(RichArray).are_uplims, self.index)
     @property
     def are_ranges(self):
-        return pd.Series(rich_array(self.values).are_ranges, self.index)
+        return pd.Series(self.values.view(RichArray).are_ranges, self.index)
     @property
     def domains(self):
-        return [pd.Series(rich_array(self.values).domains.T[i].T,
+        return [pd.Series(self.values.view(RichArray).domains.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def nums_sf(self):
-        return pd.Series(rich_array(self.values).num_sf, self.index)
+        return pd.Series(self.values.view(RichArray).num_sf, self.index)
     @property
     def min_exps(self):
-        return pd.Series(rich_array(self.values).min_exps, self.index)
+        return pd.Series(self.values.view(RichArray).min_exps, self.index)
+    def extra_sf_lims(self):
+        return pd.Series(self.values.view(RichArray).extra_sf_lim, self.index)
     @property
     def are_lims(self):
-        return pd.Series(rich_array(self.values).are_lims, self.index)
+        return pd.Series(self.values.view(RichArray).are_lims, self.index)
     @property
     def are_intervs(self):
-        return pd.Series(rich_array(self.values).are_intervs, self.index)
+        return pd.Series(self.values.view(RichArray).are_intervs, self.index)
     @property
     def are_centrs(self):
-        return pd.Series(rich_array(self.values).are_centrs, self.index)
+        return pd.Series(self.values.view(RichArray).are_centrs, self.index)
     @property
     def centers(self):
-        return pd.Series(rich_array(self.values).centers, self.index)
+        return pd.Series(self.values.view(RichArray).centers, self.index)
     @property
     def rel_uncs(self):
-        return [pd.Series(rich_array(self.values).rel_uncs.T[i].T,
+        return [pd.Series(self.values.view(RichArray).rel_uncs.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def signals_noises(self):
-        return [pd.Series(rich_array(self.values).signals_noises.T[i].T,
+        return [pd.Series(self.values.view(RichArray).signals_noises.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def ampls(self):
-        return [pd.Series(rich_array(self.values).ampls.T[i].T,
+        return [pd.Series(self.values.view(RichArray).ampls.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def rel_ampls(self):
-        return [pd.Series(rich_array(self.values).rel_ampls.T[i].T,
+        return [pd.Series(self.values.view(RichArray).rel_ampls.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def norm_uncs(self):
-        return [pd.Series(rich_array(self.values).norm_uncs.T[i].T,
+        return [pd.Series(self.values.view(RichArray).norm_uncs.T[i].T,
                           self.index) for i in (0,1)]
     @property
     def prop_scores(self):
-        return [pd.Series(rich_array(self.values).prop_scores.T[i].T,
-                          self.index) for i in (0,1)]
+        return pd.Series(self.values.view(RichArray).prop_scores, self.index)
     
-    def intervals(self, sigmas=defaultparams['sigmas for interval']):
-        return [pd.Series(rich_array(self.values).intervals(sigmas).T[i].T,
+    def intervals(self, sigmas=defaultparams['sigmas for intervals']):
+        return [pd.Series(self.values.view(RichArray).intervals(sigmas).T[i].T,
                           self.index) for i in (0,1)]
+            
+    def signs(self, sigmas=defaultparams['sigmas for intervals']):
+        return pd.Series(self.values.view(RichArray).signs(sigmas), self.index)
     
     def set_params(self, params):
         data = self.values.view(RichArray)
         data.set_params(params)
         self.update(pd.Series(data, self.index))
     
-    def set_lims_factor(self, factor=4.):
+    def set_lims_uncs(self, factor=4.):
         data = self.values.view(RichArray)
-        data.set_lims_factor(factor)
+        data.set_lims_uncs(factor)
         self.update(pd.Series(data, self.index))
 
     def latex(self, **kwargs):
-        return pd.Series(rich_array(self.values).latex(**kwargs), self.index)
+        return pd.Series(self.values.view(RichArray).latex(**kwargs), self.index)
     
     def function(self, function, **kwargs):
         data = self.values.view(RichArray).function(function, **kwargs)
         return pd.Series(data, self.index)
 
     # Attribute acronyms.
     main_values = mains
@@ -1853,40 +1937,43 @@
     relative_uncertainties = rel_uncs
     signals_to_noises = signals_noises
     amplitudes = ampls
     relative_amplitudes = rel_ampls
     normalized_uncertainties = norm_uncs
     propagation_scores = prop_scores
     # Method acronyms.
-    set_limits_factor = set_lims_factor
+    set_limits_uncertainties = set_lims_uncs
     set_parameters = set_params
     
 
 def add_two_rich_values(x, y):
     """Sum two rich values to get a new one."""
-    num_sf = max(x.num_sf, y.num_sf)
-    min_exp = min(x.min_exp, y.min_exp)
+    num_sf = min(x.num_sf, y.num_sf)
+    min_exp = round(np.mean([x.min_exp, y.min_exp]))
+    extra_sf_lim = max(x.extra_sf_lim, y.extra_sf_lim)
     domain = [x.domain[0] + y.domain[0], x.domain[1] + y.domain[1]]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
     if (not (x.is_interv or y.is_interv)
             and min(x.rel_ampl) > sigmas and min(y.rel_ampl) > sigmas):
         z = x.main + y.main
         dz = (np.array(x.unc)**2 + np.array(y.unc)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a+b, [x, y], domain=domain,
                                       is_vectorizable=True)
     z.num_sf = num_sf
     z.min_exp = min_exp
+    z.extra_sf_lim = extra_sf_lim
     return z
 
 def multiply_two_rich_values(x, y):
     """Multiply two rich values to get a new one."""
-    num_sf = max(x.num_sf, y.num_sf)
-    min_exp = min(x.min_exp, y.min_exp)
+    num_sf = min(x.num_sf, y.num_sf)
+    min_exp = round(np.mean([x.min_exp, y.min_exp]))
+    extra_sf_lim = max(x.extra_sf_lim, y.extra_sf_lim)
     with np.errstate(divide='ignore', invalid='ignore'):
         domain_combs = [x.domain[0] * y.domain[0], x.domain[0] * y.domain[1],
                         x.domain[1] * y.domain[0], x.domain[1] * y.domain[1]]
     domain1, domain2 = min(domain_combs), max(domain_combs)
     if not np.isfinite(domain1):
         domain1 = -np.inf
     if not np.isfinite(domain2):
@@ -1900,20 +1987,22 @@
         dz = abs(z) * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a*b, [x, y], domain=domain,
                                       is_vectorizable=True)
     z.num_sf = num_sf
     z.min_exp = min_exp
+    z.extra_sf_lim = extra_sf_lim
     return z
 
 def divide_two_rich_values(x, y):
     """Divide two rich values to get a new one."""
-    num_sf = max(x.num_sf, y.num_sf)
-    min_exp = min(x.min_exp, y.min_exp)
+    num_sf = min(x.num_sf, y.num_sf)
+    min_exp = round(np.mean([x.min_exp, y.min_exp]))
+    extra_sf_lim = max(x.extra_sf_lim, y.extra_sf_lim)
     with np.errstate(divide='ignore', invalid='ignore'):
         domain_combs = [x.domain[0] * y.domain[0], x.domain[0] * y.domain[1],
                         x.domain[1] * y.domain[0], x.domain[1] * y.domain[1]]
     domain1, domain2 = min(domain_combs), max(domain_combs)
     if not np.isfinite(domain1):
         domain1 = -np.inf
     if not np.isfinite(domain2):
@@ -1927,17 +2016,18 @@
         dz = abs(z) * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a/b, [x, y], domain=domain,
                                   is_vectorizable=True, sigmas=sigmas)
     z.num_sf = num_sf
     z.min_exp = min_exp
+    z.extra_sf_lim = extra_sf_lim
     return z
 
-def greater(x, y, sigmas=defaultparams['sigmas for interval']):
+def greater(x, y, sigmas=defaultparams['sigmas for intervals']):
     """Determine if a rich value/array (x) is greater than another one (y)."""
     are_single_values = all([type(var) is str
                              or not hasattr(var, '__iter__') for var in (x,y)])
     if are_single_values:
         x = x if type(x) is RichValue else rich_value(x)
         y = y if type(y) is RichValue else rich_value(y)
         x1, x2 = x.interval(sigmas=sigmas)
@@ -2006,15 +2096,15 @@
         output = np.empty(0, bool)
         for xi,yi in zip(x.flat, y.flat):
             output = np.append(output, equiv(xi,yi))
         output = output.reshape(x.shape)
     return output
 
 def greater_equiv(x, y,
-                  sigmas_interval=defaultparams['sigmas for interval'],
+                  sigmas_interval=defaultparams['sigmas for intervals'],
                   sigmas_overlap=defaultparams['sigmas for overlap']):
     """Check if a rich value/array is greater or equivalent than another one."""
     are_single_values = all([type(var) is str
                              or not hasattr(var, '__iter__') for var in (x,y)])
     if are_single_values:
         x = x if type(x) is RichValue else rich_value(x)
         y = y if type(y) is RichValue else rich_value(y)
@@ -2031,15 +2121,15 @@
         output = np.empty(0, bool)
         for xi,yi in zip(x.flat, y.flat):
             output = np.append(output, greater_equiv(xi,yi))
         output = output.reshape(x.shape)
     return output
 
 def less_equiv(x, y,
-               sigmas_interval=defaultparams['sigmas for interval'],
+               sigmas_interval=defaultparams['sigmas for intervals'],
                sigmas_overlap=defaultparams['sigmas for overlap']):
     """Check if a rich value/array is less or equivalent than another one."""
     are_single_values = all([type(var) is str
                              or not hasattr(var, '__iter__') for var in (x,y)])
     if are_single_values:
         x = x if type(x) is RichValue else rich_value(x)
         y = y if type(y) is RichValue else rich_value(y)
@@ -2055,34 +2145,40 @@
             raise Exception('Input arrays must have the same shape.')
         output = np.empty(0, bool)
         for xi,yi in zip(x.flat, y.flat):
             output = np.append(output, less_equiv(xi,yi))
         output = output.reshape(x.shape)
     return output
 
-def rich_value(text, domain=None):
+def rich_value(text, domain=None, use_default_extra_sf_lim=False):
     """
     Convert the input text to a rich value.
 
     Parameters
     ----------
     text : str
         String representing a rich value.
     domain : list (float), optional
         The domain of the rich value, that is, the minimum and maximum
-        values that it can take. The default is the union of the domains of all
-        the elements of the resulting rich array.
+        values that it can take. By default, it is the domain written in the
+        input text, but if it is not written it will be [-np.inf, np.inf].
+    use_default_extra_sf_lim : bool, optional
+        If True, the default limit for extra significant figure will be used
+        instead of inferring it from the input text. This will reduce the
+        computation time a little bit.
 
     Returns
     -------
     y : rich value
         Resulting rich value.
     """
-    
+
     domain_or = copy.copy(domain)
+    default_num_sf = defaultparams['number of significant figures']
+    default_extra_sf_lim = defaultparams['limit for extra significant figure']
     
     def parse_as_rich_value(text):
         """Obtain the properties of the input text as a rich value."""
         text = str(text)
         if '[' in text and ']' in text:
             x1, x2 = text.split('[')[1].split(']')[0].split(',')
             x1 = float(x1) if x1 != '-inf' else -np.inf
@@ -2090,21 +2186,26 @@
             domain = [x1, x2]
             text = text.split('[')[0][:-1]
         else:
             domain = [-np.inf, np.inf]
         if not '--' in text:
             if text.startswith('+'):
                 text = text[1:]
-            if 'e' not in text:
+            if ' e' in text:
+                min_exp = abs(int(text.split('e')[1]))
+            else:
+                min_exp = np.inf
                 text = '{} e0'.format(text)
+            min_exp = min(min_exp, defaultparams['minimum exponent for '
+                                                 + 'scientific notation'])
             single_value = True
             for symbol, i0 in zip(['<', '>', '+', '-'], [0, 0, 0, 1]):
                 if symbol in text[i0:]:
                     single_value = False
-            if text in ['nan', 'Nan', 'None']:
+            if text in ['None', 'none', 'NaN', 'nan', 'inf', '-inf']:
                 single_value = False
             if single_value:
                 x, e = text.split(' ')
                 dx = 0
                 text = '{}+/-{} {}'.format(x, dx, e)
             if text.startswith('<'):
                 x = text.replace('<','').replace(' ','')
@@ -2135,103 +2236,167 @@
                         else:
                             x = text.split('-')[0]
                         dx1 = text.split('-')[1].split('+')[0]
                         dx2 = text.split('+')[1].split(' ')[0]
                     else:
                         x = text.split(' ')[0]
                         dx1, dx2 = '0', '0'
-                if x not in ['nan', 'NaN', 'None']:
+                if x in ['None', 'none', 'NaN', 'nan']:
+                    x = 'nan'
+                    dx1, dx2 = '0', '0'
+                elif 'inf' in x:
+                    x = x.replace('e0', '')
+                    dx1, dx2 = '0', '0'
+                else:
                     e = text.split(' ')[1]
                     x = x + e
                     dx1 = dx1 + e
                     dx2 = dx2 + e
+            if not use_default_extra_sf_lim:
+                if (not (is_lolim or is_uplim)
+                        and not (float(dx1) == float(dx2) == 0)):
+                    dx1, dx2 = str(dx1), str(dx2)
+                    dx1_ = dx1.split('e')[0]
+                    dx2_ = dx2.split('e')[0]
+                    for i in reversed(range(len(dx1_))):
+                        dx1_ = dx1_.replace('0.'+'0'*i, '')
+                    dx1_ = dx1_.replace('.','')
+                    for i in reversed(range(len(dx2_))):
+                        dx2_ = dx2_.replace('0.'+'0'*i, '')
+                    dx2_ = dx2_.replace('.','')
+                    n1 = len(dx1_)
+                    n2 = len(dx2_)
+                    num_sf = max(1, n1, n2)
+                    val = np.array([dx1, dx2])[np.argmax([n1, n2])]
                 else:
-                    x = 'nan'
-                    dx1, dx2 = '0', '0'
+                    x_ = x.split('e')[0]
+                    for i in reversed(range(len(x_))):
+                        x_ = x_.replace('0.'+'0'*i, '')
+                    x_ = x_.replace('.','')
+                    n = len(x_)
+                    num_sf = n
+                    val = x
+                num_sf = max(1, num_sf)
+                extra_sf_lim = default_extra_sf_lim
+                base = float('{:e}'.format(float(val)).split('e')[0])
+                if base <= default_extra_sf_lim:
+                    if num_sf < default_num_sf + 1:
+                        extra_sf_lim = base - 1e-8
+            else:
+                extra_sf_lim = default_extra_sf_lim
             x = x.replace('e0','')
             main = float(x)
             unc = [float(dx1), float(dx2)]
             is_range = False
         else:
             text = text.replace(' --','--').replace('-- ','--')
             x1, x2 = text.split('--')
-            x1, _, _, _, _, domain_1 = parse_as_rich_value(x1)
-            x2, _, _, _, _, domain_2 = parse_as_rich_value(x2)
+            x1, _, _, _, _, domain_1, me1, el1 = parse_as_rich_value(x1)
+            x2, _, _, _, _, domain_2, me2, el2 = parse_as_rich_value(x2)
             main = [x1, x2]
             unc = 0
             is_lolim, is_uplim, is_range = False, False, True
             domain = [min(domain_1[0], domain_2[0]),
                       max(domain_1[1], domain_2[1])]
-        return main, unc, is_lolim, is_uplim, is_range, domain
+            min_exp = round(np.mean([me1, me2]))
+            extra_sf_lim = min(el1, el2)
+        return (main, unc, is_lolim, is_uplim, is_range, domain,
+                min_exp, extra_sf_lim)
     
     text = str(text)
-    main, unc, is_lolim, is_uplim, is_range, domain = parse_as_rich_value(text)
+    main, unc, is_lolim, is_uplim, is_range, domain, min_exp, extra_sf_lim = \
+                                                      parse_as_rich_value(text)
     if domain_or is not None:
         domain = domain_or
     y = RichValue(main, unc, is_lolim, is_uplim, is_range, domain)
+    y.min_exp = min_exp
+    y.extra_sf_lim = extra_sf_lim
     return y
 
-def rich_array(array, domain=None):
+def rich_array(array, domain=None, use_default_extra_sf_lim=False):
     """
     Convert the input array to a rich array.
 
     Parameters
     ----------
     array : array / list (str)
         Input array containing text strings representing rich values.
     domain : list (float), optional
-        The domain of al the entries of the rich array, that is, the minimum
-        and maximum values that it can take. If not given, the original domain
-        of each entry of the array will be preserved.
+        The domain of all the entries of the rich array. If not specified,
+        there are two possibilities: if the entry of the input array is already
+        a rich value, its original domain will be preserved; if not, the
+        default domain will be used, that is, [-np.inf, np.inf].
+    use_default_extra_sf_lim : bool, optional
+        If True, the default limit for extra significant figure will be used
+        instead of inferring it from the input text. This will reduce the
+        computation time a little bit.
 
     Returns
     -------
     rich_array : array
         Resulting rich array.
     """
     array = np.array(array)
     shape = array.shape
     mains, uncs, are_lolims, are_uplims, are_ranges, domains = \
         [], [], [], [], [], []
+    min_exps, extra_sf_lims = [], []
     for element in array.flat:
-        x = (element if type(element) is RichValue
-             else rich_value(element, domain))
+        if type(element) is RichValue:
+            x = element
+            if domain is not None:
+                x.domain = domain
+        else:
+            x = rich_value(element, domain, use_default_extra_sf_lim)
         mains += [x.main]
         uncs += [x.unc]
         are_lolims += [x.is_lolim]
         are_uplims += [x.is_uplim]
         are_ranges += [x.is_range]
         domains += [x.domain]
+        min_exps += [x.min_exp]
+        extra_sf_lims += [x.extra_sf_lim]
     mains = np.array(mains).reshape(shape)
     uncs = np.array(uncs)
     uncs = (np.array([uncs[:,0].reshape(shape).tolist(),
-                     uncs[:,1].reshape(shape).tolist()])
+                      uncs[:,1].reshape(shape).tolist()])
             .transpose().reshape((*shape, 2)))
     are_lolims = np.array(are_lolims).reshape(shape)
     are_uplims = np.array(are_uplims).reshape(shape)
     are_ranges = np.array(are_ranges).reshape(shape)
     domains = np.array(domains)
     domains = (np.array([domains[:,0].reshape(shape).tolist(),
                          domains[:,1].reshape(shape).tolist()])
                .transpose().reshape((*shape, 2)))
     new_array = RichArray(mains, uncs, are_lolims, are_uplims, are_ranges,
                           domains)
+    min_exp = round(np.mean(min_exps))
+    extra_sf_lim = min(extra_sf_lims)
+    new_array.set_params({'min_exp': min_exp, 'extra_sf_lim': extra_sf_lim})
     return new_array
 
-def rich_dataframe(df, domains=None):
+def rich_dataframe(df, domains=None, use_default_extra_sf_lim=False):
     """
     Convert the values of the input dataframe of text strings to rich values.
 
     Parameters
     ----------
     df : dataframe (str)
         Input dataframe which contains text strings formatted as rich values.
     domains : dict (list (float)), optional
         Dictionary containing the domain for each column of the dataframe.
-        Instead, a common domain can be directly specified for all the columns.
+        Instead, a common domain for all the columns can be directly specified.
+        If not specified, there are two possibilities: if the entry of the
+        input dataframe is already a rich value, its original domain will be
+        preserved; if not, the default domain will be used, that is,
+        [-np.inf, np.inf].
+    use_default_extra_sf_lim : bool, optional
+        If True, the default limit for extra significant figure will be used
+        instead of inferring it from the input text. This will reduce the
+        computation time a little bit.
 
     Returns
     -------
     new_df : dataframe
         Resulting dataframe of rich values.
     """
     df = pd.DataFrame(df)
@@ -2241,23 +2406,26 @@
     for i,row in new_df.iterrows():
         for col in new_df:
             is_rich_value = (True if type(new_df.at[i,col]) is RichValue
                              else False)
             domain = domains[col] if col in domains else None
             if is_rich_value:
                 x = new_df.at[i,col]
+                if domain is not None:
+                    x.domain = domain
             else:
                 is_number = True
                 text = str(new_df.at[i,col])
                 for char in text.replace(' e', ''):
                     if char.isalpha():
                         is_number = False
                         break
                 if is_number:
-                    x = rich_value(new_df.at[i,col], domain)
+                    x = rich_value(new_df.at[i,col], domain,
+                                   use_default_extra_sf_lim)
             if is_rich_value or is_number:
                 new_df.at[i,col] = x
     new_df = RichDataFrame(new_df)
     return new_df
 
 def bounded_gaussian(x, m=0., s=1., a=np.inf):
     """
@@ -2815,16 +2983,16 @@
             unc = [0, 0]
     
     z = RichValue(main, unc, domain=domain)
             
     return z
 
 def function_with_rich_values(function, args,
-        unc_function=None, is_vectorizable=False,
-        len_samples=None, domain=None, consider_intervs=None,
+        unc_function=None, is_vectorizable=False, len_samples=None,
+        optimize_len_samples=False, consider_intervs=None, domain=None,
         sigmas=defaultparams['sigmas to use approximate '
                              + 'uncertainty propagation'],
         use_sigma_combs=defaultparams['use 1-sigma combinations to '
                                       + 'approximate uncertainty propagation'],
         lims_fraction=defaultparams['fraction of the central value '
                                     + 'for upper/lower limits'],
         num_reps_lims=defaultparams['number of repetitions to estimate'
@@ -2853,22 +3021,26 @@
         first and then the uncertainties, with the same order as in the input
         function.
     is_vectorizable : bool, optional
         If True, the calculations of the function will be optimized making use
         of vectorization. The default is False.
     len_samples : int, optional
         Size of the samples of the arguments. The default is the number of
-        arguments times the default size of samples (8000).
-    domain : list (float), optional
-        Domain of the result. If not specified, it will be estimated
-        automatically.
+        arguments times the default size of samples (12000).
+    optimize_len_samples : bool, optional
+        If True, the samples size will be reduced up to the half if the minimum
+        propagation score of the arguments is high enough.
+        The default is False.
     consider_intervs : bool, optional
         If True, the resulting distribution could be interpreted as an upper/
         lower limit or a constant range of values. The default is None (it is
         False if all of the arguments are centered values).
+    domain : list (float), optional
+        Domain of the result. If not specified, it will be estimated
+        automatically.
     sigmas : float, optional
         Threshold to apply uncertainty propagation. The value is the distance
         to the bounds of the domain relative to the uncertainty.
         The default is 10.
     use_sigma_combs : bool, optional
         If True, the calculation of the uncertainties will be optimized when
         the relative amplitudes are small and there is no uncertainty function
@@ -2901,14 +3073,15 @@
     zero_log = defaultparams['decimal exponent to define zero']
     inf_log = defaultparams['decimal exponent to define infinity']
     
     if type(args) not in (tuple, list):
         args = [args]
     args = [rich_value(arg) if type(arg) is not RichValue else arg
             for arg in args]
+    
     function_or = copy.copy(function)
     if type(function) is str:
         function = function.replace('{}', '({})')
         variables = np.concatenate(tuple(arg.vars for arg in args)).tolist()
         expressions = [arg.expression for arg in args]
         expression = function.format(*expressions).replace(' ', '')
         expression = expression.replace('((', '(').replace('))', ')')
@@ -2917,19 +3090,20 @@
         function = eval('lambda {}: {}'.format(vars_str, expression))
         args = [variable_dict[var] for var in variables]
         common_vars = set(args[0].vars)
         for i in range(len(args)-1):
             common_vars = common_vars & set(args[i+1].vars)
         if len(args) > 1 and len(common_vars) > 0:
             unc_function = None
-    
+            
     if len_samples is None:
         len_samples = int(len(args)**0.5 * defaultparams['size of samples'])
-    num_sf = max([arg.num_sf for arg in args])
-    min_exp = min([arg.min_exp for arg in args])
+    num_sf = min([arg.num_sf for arg in args])
+    min_exp = round(np.mean([arg.min_exp for arg in args]))
+    extra_sf_lim = max([arg.extra_sf_lim for arg in args])
     if consider_intervs is None:
         consider_intervs = (False if all([arg.is_centr for arg in args])
                             else True)
     unc_propagation = (not any([arg.is_interv for arg in args])
                        and all([arg.prop_score > sigmas for arg in args]))
     if use_sigma_combs:
         if (unc_function is None
@@ -2964,25 +3138,21 @@
                 output = line.split('return ')[1]
                 output_size = len(output.split(','))
                 break
         output_type = list if '[' in output else tuple
 
     if output_size > 1:
         is_vectorizable = False
-    if domain is not None and not hasattr(domain[0], '__iter__'):
-        domain = [domain]*output_size
+    if domain is None:
+        domain = [None] * output_size
+    elif domain is not None and not hasattr(domain[0], '__iter__'):
+        domain = [domain] * output_size
     if unc_propagation:
         if output_size == 1:
             main = [main]
-        for k in range(output_size):
-            if domain is not None and domain[k] is None:
-                domain[k] = [-np.inf, np.inf]
-        if domain is None:
-            domain = [[-np.inf, np.inf]]*output_size
-        new_domain = domain
         if unc_function is not None:
             args_unc = [np.array(arg.unc) for arg in args]
             unc = unc_function(*args_main, *args_unc)
             unc = np.abs(unc)
             if not hasattr(unc,'__iter__'):
                 unc = [unc]*output_size
         else:
@@ -2996,69 +3166,78 @@
                 args_combs += [[]]
                 for j, arg in enumerate(args):
                     args_combs[i] += [args_all_vals[j][inds[j]]]
             new_comb = [function(*args_comb) for args_comb in args_combs]
             unc = [[main[k] - np.min(new_comb[:][k]),
                     np.max(new_comb[:][k]) - main[k]]
                    for k in range(output_size)]
-    else:
+    if any([element is None for element in np.array(domain).flat]):
+        domain_args_distr = \
+                 np.array([loguniform_distribution(*arg.domain, len_samples//3)
+                           for arg in args])
+        if is_vectorizable:
+            domain_distr = function(*domain_args_distr)
+        else:
+            domain_distr = np.array([function(*domain_args_distr[:,i])
+                                     for i in range(len_samples//3)])
+        if output_size == 1 and len(domain_distr.shape) == 1:
+            domain_distr = np.array([domain_distr]).transpose()
+    new_domain = []
+    for k in range(output_size):
+        if domain[k] is not None:
+            domain_k = domain[k]
+        else:
+            domain1 = np.min(domain_distr[:,k])
+            domain2 = np.max(domain_distr[:,k])
+            if not np.isfinite(domain1):
+                domain1 = -np.inf
+            if not np.isfinite(domain2):
+                domain2 = np.inf
+            domain1, domain2 = remove_zero_infs([domain1, domain2],
+                                                zero_log, inf_log)
+            domain_k = [float(round_sf(domain1, num_sf+3)),
+                        float(round_sf(domain2, num_sf+3))]
+            domain_k = add_zero_infs(domain_k, zero_log+6, inf_log-6)
+        new_domain += [domain_k]
+    if not unc_propagation:
+        if optimize_len_samples:
+            prop_score = min([arg.prop_score for arg in args])
+            lim1, lim2 = 4., 20.
+            if prop_score > lim1:
+                factor = 1. - 0.5 * (min(prop_score,20.)-lim1) / (lim2-lim1)
+                len_samples = int(factor * len_samples)
         args_distr = np.array([arg.sample(len_samples) for arg in args])
         if is_vectorizable:
             new_distr = function(*args_distr)
         else:
             new_distr = np.array([function(*args_distr[:,i])
                                   for i in range(len_samples)])
         if output_size == 1 and len(new_distr.shape) == 1:
             new_distr = np.array([new_distr]).transpose()
-        main, unc, new_domain = [], [], []
-        if domain is None:
-            domain_args_distr = np.array(
-                [loguniform_distribution(*arg.domain, len_samples//3)
-                 for arg in args])
-            if is_vectorizable:
-                domain_distr = function(*domain_args_distr)
-            else:
-                domain_distr = np.array([function(*domain_args_distr[:,i])
-                                         for i in range(len_samples//3)])
-            if output_size == 1 and len(domain_distr.shape) == 1:
-                domain_distr = np.array([domain_distr]).transpose()
+        main, unc = [], []
         for k in range(output_size):
-            if domain is not None:
-                domain_k = domain[k]
-            else:
-                domain1 = np.min(domain_distr[:,k])
-                domain2 = np.max(domain_distr[:,k])
-                if not np.isfinite(domain1):
-                    domain1 = -np.inf
-                if not np.isfinite(domain2):
-                    domain2 = np.inf
-                domain1, domain2 = remove_zero_infs([domain1, domain2],
-                                                    zero_log, inf_log)
-                domain_k = [float(round_sf(domain1, num_sf+3)),
-                            float(round_sf(domain2, num_sf+3))]
-                domain_k = add_zero_infs(domain_k, zero_log+6, inf_log-6)
             def function_k(*argsk):
                 y = function(*argsk)
                 if output_size > 1:
                     y = y[k]
                 return y
-            rval_k = evaluate_distr(new_distr[:,k], domain_k, function_k,
+            rval_k = evaluate_distr(new_distr[:,k], new_domain[k], function_k,
                         args, len_samples, is_vectorizable, consider_intervs,
                         lims_fraction, num_reps_lims, zero_log, inf_log)
             main_k = rval_k.main if not rval_k.is_interv else rval_k.interval()
             unc_k = rval_k.unc
             main += [main_k]
             unc += [unc_k]
-            new_domain += [domain_k]
         
     output = []
     for k in range(output_size):
         new_rval = RichValue(main[k], unc[k], domain=new_domain[k])
         new_rval.num_sf = num_sf
         new_rval.min_exp = min_exp
+        new_rval.extra_sf_lim = extra_sf_lim
         if type(function_or) is str:
             new_rval.vars = variables
             new_rval.expression = expression
         output += [new_rval]
     if output_size == 1 and output_type not in (tuple, list):
         output = output[0]
     if output_type is tuple:
@@ -3219,15 +3398,14 @@
         Matplotlib's 'errorbar' keyword arguments.
 
     Returns
     -------
     plot : matplotlib.container.ErrorbarContainer
         Matplotib's 'errorbar' output.
     """
-    global num_plots
     def set_kwarg(keyword, default):
         """Set a certain keyword argument with a default value."""
         if keyword in kwargs:
             kwarg = kwargs[keyword]
             del kwargs[keyword]
         else:
             kwarg = default
@@ -3248,16 +3426,16 @@
         lims_factor_x, lims_factor_y = [lims_factor]*2
     elif type(lims_factor) in (list, tuple):
         lims_factor_x, lims_factor_y = lims_factor
     if lims_factor_x is None:
         lims_factor_x = lim_factor(xc)
     if lims_factor_y is None:
         lims_factor_y = lim_factor(yc)
-    xc.set_lims_factor(lims_factor_x)
-    yc.set_lims_factor(lims_factor_y)
+    xc.set_lims_uncs(lims_factor_x)
+    yc.set_lims_uncs(lims_factor_y)
     plt.plot()
     ax = plt.gca()
     color = ax.plot([])[0].get_color()
     color = set_kwarg('color', color)
     ecolor = set_kwarg('ecolor', 'black')
     fmt = set_kwarg('fmt', '.')
     cond = ~ (xc.are_ranges | yc.are_ranges)
@@ -3547,21 +3725,27 @@
     with np.errstate(divide='ignore'):
         y = np.log10(x)
     return y
 
 # Functions for masking arrays.
 def isnan(x):
     x = rich_array(x) if type(x) is not RichArray else x
-    return np.array([xi.is_nan for xi in x]).reshape(x.shape)
+    return np.array([xi.is_nan for xi in x.flat]).reshape(x.shape)
 def isinf(x):
     x = rich_array(x) if type(x) is not RichArray else x
-    return np.array([xi.is_inf for xi in x]).reshape(x.shape)
+    return np.array([xi.is_inf for xi in x.flat]).reshape(x.shape)
 def isfinite(x):
     x = rich_array(x) if type(x) is not RichArray else x
-    return np.array([xi.is_finite for xi in x]).reshape(x.shape)
+    return np.array([xi.is_finite for xi in x.flat]).reshape(x.shape)
+
+# Functions for concatenating arrays.
+def append(arr, values, **kwargs):
+    return np.append(arr, values, **kwargs).view(RichArray)
+def concatenate(arrs, **kwargs):
+    return np.concatenate(arrs, **kwargs).view(RichArray)
 
 # Mathematical functions.
 def sqrt(x):
     function_ = function if type(x) in (str, RichValue) else array_function
     return function_('np.sqrt({})', x, domain=[0,np.inf], elementwise=True,
                      unc_function= lambda x,dx: dx/x**0.5 / 2)
 def exp(x):
@@ -3632,8 +3816,8 @@
 function = function_with_rich_values
 array_function = function_with_rich_arrays
 distribution = distr_with_rich_values
 evaluate_distribution = evaluate_distr
 center_and_uncertainties = center_and_uncs
 is_not_a_number = is_nan = isnan
 is_infinite = is_inf = isinf
-is_finite = is_finite = isfinite
+is_finite = is_finite = isfinite
```

### Comparing `richvalues-3.0.9/richvalues.egg-info/PKG-INFO` & `richvalues-3.1.0/richvalues.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.0.9
+Version: 3.1.0
 Summary: Python library for working with uncertainties and upper/lower limits
-Home-page: https://github.com/andresmegias/richvalues
+Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
-Description: # RichValues
-        
-        Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
-        
-        The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. 
+
+With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
+
+The libraries NumPy, Pandas, SciPy and Matplotlib are required by RichValues. An user guide and some examples are available in the GitHub repository: https://github.com/andresmegias/richvalues/.
+
+
```

### Comparing `richvalues-3.0.9/setup.py` & `richvalues-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.0.9',
+    version = '3.1.0',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
-    url = 'https://github.com/andresmegias/richvalues',
+    url = 'https://github.com/andresmegias/richvalues/',
     install_requires = ['numpy', 'pandas', 'scipy', 'matplotlib'],
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent'
-    ]
+        'Operating System :: OS Independent']
 )
```

