# Comparing `tmp/rateslib-0.0.1.tar.gz` & `tmp/rateslib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateslib-0.0.1.tar", last modified: Mon Jan 16 21:28:52 2023, max compression
+gzip compressed data, was "rateslib-0.1.0.tar", last modified: Mon Apr 24 18:45:31 2023, max compression
```

## Comparing `rateslib-0.0.1.tar` & `rateslib-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,37 @@
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-01-16 21:28:52.377163 rateslib-0.0.1/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.0.1/LICENSE
--rw-r--r--   0 Darbyshire   (501) staff       (20)    22764 2023-01-16 21:28:52.376628 rateslib-0.0.1/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)       90 2023-01-16 21:19:41.000000 rateslib-0.0.1/README.md
--rw-r--r--   0 Darbyshire   (501) staff       (20)      775 2023-01-16 21:28:24.000000 rateslib-0.0.1/pyproject.toml
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-01-16 21:28:52.358580 rateslib-0.0.1/rateslib/
--rw-r--r--   0 Darbyshire   (501) staff       (20)        0 2023-01-16 21:19:41.000000 rateslib-0.0.1/rateslib/__init__.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     1067 2023-01-16 21:19:41.000000 rateslib-0.0.1/rateslib/defaults.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-01-16 21:28:52.375999 rateslib-0.0.1/rateslib.egg-info/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    22764 2023-01-16 21:28:52.000000 rateslib-0.0.1/rateslib.egg-info/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)      242 2023-01-16 21:28:52.000000 rateslib-0.0.1/rateslib.egg-info/SOURCES.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-01-16 21:28:52.000000 rateslib-0.0.1/rateslib.egg-info/dependency_links.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)      158 2023-01-16 21:28:52.000000 rateslib-0.0.1/rateslib.egg-info/requires.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-01-16 21:28:52.000000 rateslib-0.0.1/rateslib.egg-info/top_level.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-01-16 21:28:52.377243 rateslib-0.0.1/setup.cfg
--rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.0.1/setup.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.258394 rateslib-0.1.0/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-0.1.0/LICENSE
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-04-24 18:45:31.257970 rateslib-0.1.0/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     1186 2023-04-24 18:38:25.000000 rateslib-0.1.0/README.md
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      799 2023-04-24 18:27:13.000000 rateslib-0.1.0/pyproject.toml
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.091678 rateslib-0.1.0/rateslib/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     4576 2023-04-23 07:34:25.000000 rateslib-0.1.0/rateslib/__init__.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    22387 2023-03-31 16:14:49.000000 rateslib-0.1.0/rateslib/calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    53603 2023-04-24 18:22:38.000000 rateslib-0.1.0/rateslib/curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     3299 2023-04-17 18:48:46.000000 rateslib-0.1.0/rateslib/defaults.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23398 2023-04-17 18:48:46.000000 rateslib-0.1.0/rateslib/dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    64353 2023-04-19 18:21:10.000000 rateslib-0.1.0/rateslib/fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)   207218 2023-04-24 15:23:12.000000 rateslib-0.1.0/rateslib/instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    65006 2023-04-24 04:46:29.000000 rateslib-0.1.0/rateslib/legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    52971 2023-04-24 17:06:01.000000 rateslib-0.1.0/rateslib/periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    45487 2023-03-31 17:09:16.000000 rateslib-0.1.0/rateslib/scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    66561 2023-04-24 16:41:08.000000 rateslib-0.1.0/rateslib/solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    16882 2023-03-31 16:24:01.000000 rateslib-0.1.0/rateslib/splines.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.101595 rateslib-0.1.0/rateslib.egg-info/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    23901 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/PKG-INFO
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      654 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/SOURCES.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/dependency_links.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)      142 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/requires.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2023-04-24 18:45:30.000000 rateslib-0.1.0/rateslib.egg-info/top_level.txt
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2023-04-24 18:45:31.258464 rateslib-0.1.0/setup.cfg
+-rw-r--r--   0 Darbyshire   (501) staff       (20)       37 2022-08-28 05:42:04.000000 rateslib-0.1.0/setup.py
+drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2023-04-24 18:45:31.250350 rateslib-0.1.0/tests/
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     8187 2023-03-05 18:52:18.000000 rateslib-0.1.0/tests/test_calendars.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    18964 2023-03-31 16:52:57.000000 rateslib-0.1.0/tests/test_curves.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    22577 2023-04-17 18:48:46.000000 rateslib-0.1.0/tests/test_dual.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    28832 2023-04-24 16:35:20.000000 rateslib-0.1.0/tests/test_fx.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    63272 2023-04-17 18:48:46.000000 rateslib-0.1.0/tests/test_instruments.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    27553 2023-04-01 10:40:19.000000 rateslib-0.1.0/tests/test_legs.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    32684 2023-04-17 18:48:46.000000 rateslib-0.1.0/tests/test_periods.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    24516 2023-03-20 17:46:32.000000 rateslib-0.1.0/tests/test_scheduling.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)    32047 2023-04-24 17:06:01.000000 rateslib-0.1.0/tests/test_solver.py
+-rw-r--r--   0 Darbyshire   (501) staff       (20)     5430 2023-03-29 17:12:48.000000 rateslib-0.1.0/tests/test_splines.py
```

### Comparing `rateslib-0.0.1/LICENSE` & `rateslib-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rateslib-0.0.1/PKG-INFO` & `rateslib-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.0.1
-Summary: Coding Interest Rate Derivatives
+Version: 0.1.0
+Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
         does not provide legal services or legal advice. Distribution of
@@ -402,20 +402,50 @@
         to any of its public licenses or any other arrangements,
         understandings, or agreements concerning use of licensed material. For
         the avoidance of doubt, this paragraph does not form part of the
         public licenses.
         
         Creative Commons may be contacted at creativecommons.org.
         
-Project-URL: Homepage, https://github.com/attack68/TBD
-Keywords: interest rate,derivatives,swaps
-Requires-Python: >=3.7
+Project-URL: Homepage, https://github.com/attack68/rateslib
+Keywords: interest rate,derivatives,swaps,bonds,fixed income
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Swapslib
+# Rateslib
+
+**This version is beta pre-release. It may change at any point without notice.**
+
+``Rateslib`` is a state-of-the-art **fixed income library** designed for Python.
+Its purpose is to provide advanced, flexible and efficient fixed income analysis
+with a high level, well documented API.
+
+Its design objective is to be able to create a self-consistent, arbitrage free
+framework for pricing all aspects of fixed income trading, such as spot FX, FX forwards,
+single currency securities and derivatives like fixed rate bonds and IRSs, and also
+multi-currency derivatives such as FX swaps and cross-currency swaps. Options,
+swaptions and inflation are also under consideration for future development.
+
+The techniques and object interation within *rateslib* were inspired by
+the requirements of multi-disciplined fixed income teams working, both cooperatively
+and independently, within global investment banks.
+
+
+Licence
+=======
+
+This library is released under a **Creative Commons Attribution, Non-Commercial,
+No-Derivatives 4.0 International Licence**.
+
+
+Get Started
+===========
+
+Read the documentation at 
+[Rateslib Read-the-Docs](https://rateslib.readthedocs.io/en/latest/)
+
+
 
-This package is version 0 of an upcoming release. 
 
-Do not use this package.
```

### Comparing `rateslib-0.0.1/pyproject.toml` & `rateslib-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rateslib"
-version = "0.0.1"
-description = "Coding Interest Rate Derivatives"
+version = "0.1.0"
+description = "A fixed income library for trading interest rates"
 readme = "README.md"
 authors = [{ name = "J H M Darbyshire"}]
 license = { file = "LICENSE" }
-keywords = ["interest rate", "derivatives", "swaps"]
+keywords = ["interest rate", "derivatives", "swaps", "bonds", "fixed income"]
 dependencies = [
     "numpy>=1.21.5",
     "scipy>=1.8.0",
     "matplotlib>=3.5.1",
     "pandas>=1.4.1",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.0.1",
     "jupyterlab>=3.3.1",
-    "matplotlib>=3.5.1",
     "numba>=0.55.1",
-    "pandas>=1.4.1",
     "sphinx>=5.1.1",
+    "coverage>=7.1.0",
 ]
 
 [tool.setuptools]
 packages = ["rateslib"]
 
 [project.urls]
-Homepage = "https://github.com/attack68/TBD"
+Homepage = "https://github.com/attack68/rateslib"
```

### Comparing `rateslib-0.0.1/rateslib.egg-info/PKG-INFO` & `rateslib-0.1.0/rateslib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rateslib
-Version: 0.0.1
-Summary: Coding Interest Rate Derivatives
+Version: 0.1.0
+Summary: A fixed income library for trading interest rates
 Author: J H M Darbyshire
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
         does not provide legal services or legal advice. Distribution of
@@ -402,20 +402,50 @@
         to any of its public licenses or any other arrangements,
         understandings, or agreements concerning use of licensed material. For
         the avoidance of doubt, this paragraph does not form part of the
         public licenses.
         
         Creative Commons may be contacted at creativecommons.org.
         
-Project-URL: Homepage, https://github.com/attack68/TBD
-Keywords: interest rate,derivatives,swaps
-Requires-Python: >=3.7
+Project-URL: Homepage, https://github.com/attack68/rateslib
+Keywords: interest rate,derivatives,swaps,bonds,fixed income
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Swapslib
+# Rateslib
+
+**This version is beta pre-release. It may change at any point without notice.**
+
+``Rateslib`` is a state-of-the-art **fixed income library** designed for Python.
+Its purpose is to provide advanced, flexible and efficient fixed income analysis
+with a high level, well documented API.
+
+Its design objective is to be able to create a self-consistent, arbitrage free
+framework for pricing all aspects of fixed income trading, such as spot FX, FX forwards,
+single currency securities and derivatives like fixed rate bonds and IRSs, and also
+multi-currency derivatives such as FX swaps and cross-currency swaps. Options,
+swaptions and inflation are also under consideration for future development.
+
+The techniques and object interation within *rateslib* were inspired by
+the requirements of multi-disciplined fixed income teams working, both cooperatively
+and independently, within global investment banks.
+
+
+Licence
+=======
+
+This library is released under a **Creative Commons Attribution, Non-Commercial,
+No-Derivatives 4.0 International Licence**.
+
+
+Get Started
+===========
+
+Read the documentation at 
+[Rateslib Read-the-Docs](https://rateslib.readthedocs.io/en/latest/)
+
+
 
-This package is version 0 of an upcoming release. 
 
-Do not use this package.
```

