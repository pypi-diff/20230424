# Comparing `tmp/DGet-0.4.tar.gz` & `tmp/DGet-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DGet-0.4.tar", last modified: Wed Apr 19 05:39:46 2023, max compression
+gzip compressed data, was "DGet-0.5.tar", last modified: Mon Apr 24 07:20:00 2023, max compression
```

## Comparing `DGet-0.4.tar` & `DGet-0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/DGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 05:39:35.000000 DGet-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-19 05:39:46.995087 DGet-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 05:39:35.000000 DGet-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/dget/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 05:39:35.000000 DGet-0.4/dget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-19 05:39:35.000000 DGet-0.4/dget/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-19 05:39:35.000000 DGet-0.4/dget/adduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-19 05:39:35.000000 DGet-0.4/dget/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-19 05:39:35.000000 DGet-0.4/dget/dget.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 05:39:46.995087 DGet-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 05:39:35.000000 DGet-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-19 05:39:35.000000 DGet-0.4/tests/test_adducts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/DGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 07:20:00.000000 DGet-0.5/DGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 07:19:39.000000 DGet-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 07:20:00.135157 DGet-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 07:19:39.000000 DGet-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/dget/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 07:19:39.000000 DGet-0.5/dget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-24 07:19:39.000000 DGet-0.5/dget/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-24 07:19:39.000000 DGet-0.5/dget/adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-24 07:19:39.000000 DGet-0.5/dget/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-04-24 07:19:39.000000 DGet-0.5/dget/dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:20:00.135157 DGet-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-24 07:19:39.000000 DGet-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:20:00.135157 DGet-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-24 07:19:39.000000 DGet-0.5/tests/test_adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-24 07:19:39.000000 DGet-0.5/tests/test_dget.py
```

### Comparing `DGet-0.4/DGet.egg-info/PKG-INFO` & `DGet-0.5/DGet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DGet
-Version: 0.4
+Version: 0.5
 Summary: Calculates compound deuteration from ToF-MS data.
 Home-page: https://github.com/djdt/dget
 Author: djdt
 License: GPL3
 Project-URL: Source, https://github.com/djdt/dget
 Project-URL: Web App, https://djdt.github.io/dget
 Description-Content-Type: text/markdown
```

### Comparing `DGet-0.4/LICENSE` & `DGet-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `DGet-0.4/PKG-INFO` & `DGet-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DGet
-Version: 0.4
+Version: 0.5
 Summary: Calculates compound deuteration from ToF-MS data.
 Home-page: https://github.com/djdt/dget
 Author: djdt
 License: GPL3
 Project-URL: Source, https://github.com/djdt/dget
 Project-URL: Web App, https://djdt.github.io/dget
 Description-Content-Type: text/markdown
```

### Comparing `DGet-0.4/dget/__main__.py` & `DGet-0.5/dget/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 from pathlib import Path
 
-from dget import DGet
+from dget import DGet, __version__
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser("dget")
     parser.add_argument(
         "formula", help="Molecular formula of the compound, see molmass."
     )
@@ -49,14 +49,15 @@
     )
     parser.add_argument(
         "--realign",
         action="store_true",
         help="Force alignment of MS data with predicted spectra, "
         "please just calibrate your MS.",
     )
+    parser.add_argument("--version", action="version", version=__version__)
 
     args = parser.parse_args()
 
     if args.autoadduct:
         args.adduct = "[M]+"
 
     if "D" not in args.formula:
@@ -83,24 +84,18 @@
         dget.formula = adduct
         print(f"Adduct difference from base peak m/z: {diff:.4f}")
         print()
 
     dget.mass_width = args.masswidth
     if args.realign:
         dget.align_tof_with_spectra()
+        print(f"Re-aligned ToF data by shifting {dget.offset_mz:.2f} m/z")
+        print()
 
-    print(f"Formula          : {dget.base.empirical}")
-    print(f"Adduct           : {dget.adduct}")
-    print(f"M/Z              : {dget.formula.mz}")
-    print(f"Monoisotopic M/Z : {dget.formula.isotope.mz}")
-    print(f"%D               : {dget.deuteration * 100.0:.2f}")
-    print()
-    print("Deuteration Ratio Spectra")
-    for i, p in enumerate(dget.deuteration_probabilites):
-        print(f"D{i:<2}              : {p:.4f}")
+    dget.print_results()
 
     if args.plot:
         import matplotlib.pyplot as plt
 
         fig, axes = plt.subplots(1, 1)
         dget.plot_predicted_spectra(axes)
         plt.show()
```

### Comparing `DGet-0.4/dget/adduct.py` & `DGet-0.5/dget/adduct.py`

 * *Files identical despite different names*

### Comparing `DGet-0.4/dget/convolve.py` & `DGet-0.5/dget/convolve.py`

 * *Files identical despite different names*

### Comparing `DGet-0.4/dget/dget.py` & `DGet-0.5/dget/dget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List, Tuple
+from typing import List, TextIO, Tuple
 
 import numpy as np
 from molmass import ELEMENTS, Formula, Spectrum
 
 from dget.adduct import adduct_from_formula, formula_from_adduct
 from dget.convolve import deconvolve
 
@@ -22,21 +22,24 @@
     ]
 
     def __init__(
         self,
         formula: str,
         tofdata: Path,
         adduct: str = "[M]+",
+        mass_width: float = 0.5,
         loadtxt_kws: dict | None = None,
     ):
         _loadtxt_kws = {"delimiter": ",", "usecols": (0, 1)}
         if loadtxt_kws is not None:
             _loadtxt_kws.update(loadtxt_kws)
 
-        self.mass_width = 0.5
+        self.mass_width = mass_width
+        self.offset_mz: float | None = None
+
         self._targets: np.ndarray | None = None
         self._probabilities: np.ndarray | None = None
         self._probability_remainders: np.ndarray | None = None
 
         self.base = Formula(formula)  # store original for adduct calcs
         self.formula = formula_from_adduct(formula, adduct)
 
@@ -98,37 +101,41 @@
             self._targets = np.arange(
                 self.spectrum[smin].mz - (self.deuterium_count * diff_HD),
                 self.spectrum[smax].mz + diff_HD,
                 diff_HD,
             )
         return self._targets
 
+    def __str__(self) -> str:
+        return f"DGet({self.formula.formula})"
+
     def _read_tofdata(self, path: Path, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         if len(kwargs["usecols"]) != 2:
             raise ValueError(
                 "exactly two columns (mass, signal) must be specified by 'usecols'"
             )
         for kw in ["unpack", "dtype"]:
             if kw in kwargs:
                 kwargs.pop(kw)
                 print(f"warning: removing loadtxt keyword '{kw}'")
         return np.loadtxt(path, unpack=True, dtype=np.float32, **kwargs)  # type: ignore
 
     def align_tof_with_spectra(self) -> None:
         """Shifts ToF data to better align with monoisotopic m/z.
+        Sets the 'offset_mz' attribute.
         Please calibrate your MS instead of using this.
         """
         mz = self.formula.isotope.mz
         start, onmass, end = np.searchsorted(
             self.x, [mz - self.mass_width, mz, mz + self.mass_width]
         )
-        offset = self.x[start + np.argmax(self.y[start:end])] - self.x[onmass]
-        if abs(offset) > 1.0:
+        self.offset_mz = self.x[start + np.argmax(self.y[start:end])] - self.x[onmass]
+        if abs(self.offset_mz) > 1.0:  # type: ignore
             print("warning: calculated alignment offset greater than 0.5 Da!")
-        self.x -= offset
+        self.x -= self.offset_mz
 
     def guess_adduct_from_base_peak(
         self,
         adducts: List[Formula] | None = None,
         mass_range: Tuple[float, float] | None = None,
     ) -> Tuple[Formula, float]:
         """Finds the adduct closest to the m/z of the largest tof peak.
@@ -160,52 +167,70 @@
 
         base = self.x[start:stop][np.argmax(self.y[start:stop])]
         diffs = np.abs(base - masses)
         best = np.argmin(diffs)
         return formulas[best], diffs[best]
 
     def plot_predicted_spectra(
-        self, ax: "matplotlib.axes.Axes", pad_mz: float = 5.0  # noqa: F821
+        self, ax: "matplotlib.axes.Axes", pad_mz: float = 2.0  # noqa: F821
     ) -> None:
         """Plot spectra over mass spectra on `ax`.
 
         Args:
             ax: matplotlib axes
             pad_mz: window around targets to show
         """
-        targets = self.targets
 
-        start, end = np.searchsorted(self.x, [targets[0], targets[-1]])
+        def scale_spectra(x, y, spectra_x, spectra):
+            max = spectra_x[np.argmax(spectra)]
+            start, end = np.searchsorted(x, [max - 0.5, max + 0.5])
+            return spectra * np.amax(y[start:end]) / spectra.max()
+
+        targets = self.targets
+        start, end = np.searchsorted(
+            self.x, [targets[0] - pad_mz, targets[-1] + pad_mz]
+        )
         x, y = self.x[start:end], self.y[start:end]
 
         prediction = np.convolve(self.deuteration_probabilites, self.psf, mode="full")
+
         # Data
         ax.plot(x, y, color="black")
 
         # Scaled prediction
-        if prediction.size == 0 or y.size == 0:
+        if prediction.size == 0:
             return
-        prediction *= y.max() / prediction.max()
+
         ax.stem(
             targets,
-            prediction,
+            scale_spectra(x, y, targets, prediction),
             markerfmt=" ",
             basefmt=" ",
             linefmt="red",
             label="Predicted Specta",
         )
 
         # Scaled PSF
-        psf = self.psf * y.max()
         masses = [i.mass for i in self.spectrum.values()]
         ax.stem(
             masses,
-            psf,
+            scale_spectra(x, y, masses, self.psf),
             markerfmt=" ",
             basefmt=" ",
             linefmt="blue",
             label="Formula Spectra",
         )
         ax.set_title(self.formula.formula)
         ax.set_xlabel("Mass")
         ax.set_ylabel("Signal")
         ax.legend()
+
+    def print_results(self) -> None:
+        print(f"Formula          : {self.base.formula}")
+        print(f"Adduct           : {self.adduct}")
+        print(f"M/Z              : {self.formula.mz}")
+        print(f"Monoisotopic M/Z : {self.formula.isotope.mz}")
+        print(f"%D               : {self.deuteration * 100.0:.2f} %")
+        print()
+        print("Deuteration Ratio Spectra")
+        for i, p in enumerate(self.deuteration_probabilites):
+            print(f"D{i:<2}              : {p * 100.0:5.2f} %")
```

### Comparing `DGet-0.4/setup.py` & `DGet-0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+from pathlib import Path
+
 from setuptools import setup
 
 with open("README.md") as fp:
     long_description = fp.read()
 
+with Path("dget", "__init__.py").open() as fp:
+    version = None
+    for line in fp:
+        if line.startswith("__version__"):
+            version = line.split("=")[1].strip().strip('"')
+    if version is None:
+        raise ValueError("Could not read version from __init__.py")
+
 setup(
     name="DGet",
-    version="0.4",
+    version=version,
     description="Calculates compound deuteration from ToF-MS data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["dget"],
     license="GPL3",
     author="djdt",
     url="https://github.com/djdt/dget",
```

### Comparing `DGet-0.4/tests/test_adducts.py` & `DGet-0.5/tests/test_adduct.py`

 * *Files identical despite different names*

