# Comparing `tmp/equilibrator-pathway-0.4.7.tar.gz` & `tmp/equilibrator-pathway-0.4.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equilibrator-pathway-0.4.7.tar", last modified: Mon Sep 12 14:21:30 2022, max compression
+gzip compressed data, was "equilibrator-pathway-0.4.8b1.tar", last modified: Mon Apr 24 08:14:47 2023, max compression
```

## Comparing `equilibrator-pathway-0.4.7.tar` & `equilibrator-pathway-0.4.8b1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:21:30.313259 equilibrator-pathway-0.4.7/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4065 2022-09-12 14:21:30.313259 equilibrator-pathway-0.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2725 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2007 2022-09-12 14:21:30.314176 equilibrator-pathway-0.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:21:30.305925 equilibrator-pathway-0.4.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:21:30.314176 equilibrator-pathway-0.4.7/src/equilibrator_pathway/
--rw-rw-rw-   0 root         (0) root         (0)     1955 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-09-12 14:21:30.314176 equilibrator-pathway-0.4.7/src/equilibrator_pathway/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7092 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/analysis_solution.py
--rwxrwxrwx   0 root         (0) root         (0)    22788 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/cost_function.py
--rw-rw-rw-   0 root         (0) root         (0)    11760 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/ecm_model.py
--rw-rw-rw-   0 root         (0) root         (0)     9902 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/ecm_solution.py
--rw-rw-rw-   0 root         (0) root         (0)     6545 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/mdf_solution.py
--rwxrwxrwx   0 root         (0) root         (0)     7678 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/mdmc_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    10508 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/pathway.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    10798 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/thermo_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4330 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:21:30.313259 equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4065 2022-09-12 14:21:30.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      832 2022-09-12 14:21:30.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 14:21:30.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      323 2022-09-12 14:21:30.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-12 14:21:30.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 14:21:30.000000 equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)    68615 2022-09-12 14:21:18.000000 equilibrator-pathway-0.4.7/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.251419 equilibrator-pathway-0.4.8b1/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4067 2023-04-24 08:14:47.252419 equilibrator-pathway-0.4.8b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2023-04-24 08:14:47.253419 equilibrator-pathway-0.4.8b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.242418 equilibrator-pathway-0.4.8b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.253419 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-24 08:14:47.253419 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7210 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/analysis_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)    23350 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/cost_function.py
+-rw-rw-rw-   0 root         (0) root         (0)    12964 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10368 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)     6593 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdf_solution.py
+-rwxrwxrwx   0 root         (0) root         (0)     7404 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdmc_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)    10429 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/pathway.py
+-rw-rw-rw-   0 root         (0) root         (0)     4343 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10878 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/thermo_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:14:47.251419 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4067 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      832 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:14:47.000000 equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)    68615 2023-04-24 08:14:32.000000 equilibrator-pathway-0.4.8b1/versioneer.py
```

### Comparing `equilibrator-pathway-0.4.7/LICENSE` & `equilibrator-pathway-0.4.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.7/PKG-INFO` & `equilibrator-pathway-0.4.8b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.4.7
+Version: 0.4.8b1
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
```

### Comparing `equilibrator-pathway-0.4.7/README.md` & `equilibrator-pathway-0.4.8b1/README.md`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.7/setup.cfg` & `equilibrator-pathway-0.4.8b1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 	max-min driving force
 
 [options]
 zip_safe = True
 install_requires = 
 	pint~=0.19
 	numpy~=1.23
+	pandas~=1.4
 	scipy~=1.9
 	seaborn~=0.12
 	uncertainties~=3.1
 	osqp~=0.6
 	cvxpy~=1.2
 	sbtab~=1.0
 	equilibrator-api==0.4.7
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/__init__.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/__init__.py`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/analysis_solution.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/analysis_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def __init__(
         self,
         pathway: Pathway,
         score: float,
         ln_conc: np.ndarray,
         y: Optional[np.array] = None,
     ) -> None:
-        """
+        """Create a PathwayAnalysisSolution object.
 
         Parameters
         ----------
         thermo_model : ThermodynamicModel
         ln_conc : array
             log concentrations at MDF optimum
         """
@@ -151,18 +151,20 @@
             upper_bound
 
         """
         return self._compound_df
 
     @property
     def reaction_ids(self) -> Iterable[str]:
+        """Return the reaction IDs."""
         return self._reaction_df.reaction_id.__iter__()
 
     @property
     def compound_ids(self) -> Iterable[str]:
+        """Return the compound IDs."""
         return self._compound_df.compound_id.__iter__()
 
     def to_sbtab(self) -> SBtab.SBtabDocument:
         """Generate a report (in SBtab format)."""
         sbtabdoc = SBtab.SBtabDocument("report")
 
         # add a table with the optimized metabolite concentrations
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/cost_function.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/cost_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""A module for cost functions."""
 # The MIT License (MIT)
 #
 # Copyright (c) 2013 Weizmann Institute of Science
 # Copyright (c) 2018-2020 Institute for Molecular Systems Biology,
 # ETH Zurich
 # Copyright (c) 2018-2020 Novo Nordisk Foundation Center for Biosustainability,
 # Technical University of Denmark
@@ -21,37 +22,37 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 import itertools
 import logging
-from typing import Iterable, Optional, Tuple
+from typing import Iterable, Optional, Tuple, Union
 
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 from cvxpy.constraints.constraint import Constraint
-from cvxpy.expressions.expression import Expression
-from cvxpy.problems.objective import Objective
 from equilibrator_api import Q_, R, default_T
 from scipy import stats
 
 from .util import ECF_DEFAULTS
 
 
 class EnzymeCostFunction(object):
+    """A class for describing the enzyme cost function."""
 
     ECF_LEVEL_NAMES = [
         "capacity [M]",
         "thermodynamic",
         "saturation",
         "allosteric",
     ]
-    MINIMAL_STDEV = 1e-3  # for metabolites to be considered "fixed"
+    MINIMAL_STDEV = 1e-3  # for metabolites to be considered
+    # "fixed"
     DRIVING_FORCE_LB = 1e-3  # in kJ/mol
 
     def __init__(
         self,
         S: np.ndarray,
         fluxes: Q_,
         kcat: Q_,
@@ -65,15 +66,15 @@
         A_act: Optional[np.ndarray] = None,
         A_inh: Optional[np.ndarray] = None,
         K_act: Optional[Q_] = None,
         K_inh: Optional[Q_] = None,
         idx_water: int = -1,
         params: Optional[dict] = None,
     ):
-        """Create a Cost Function object.
+        """Create an EnzymeCostFunction object.
 
         Parameters
         ----------
         S: ndarray
             stoichiometric matrix [unitless]
         fluxes: Quantity [concentration]/[time]
             steady-state fluxes [flux units]
@@ -136,16 +137,17 @@
 
         # In MDMC we use Z-score to describe distribution within the metabolite
         # so we need to convert the "hard" bounds into a Gaussian distribution
         # where the geometric mean is the middle of the range
         self.ln_conc_mu = (self.ln_conc_ub + self.ln_conc_lb) / 2.0
 
         # and the bounds represent (two-sided) confidence intervals that are
-        # for a chi2 distribution with 1 DoF, and a confidence of self.ln_conc_confidence
-        # therefore, to get ln_conc_sigma, we need to divide by the square root of the PPF:
+        # for a chi2 distribution with 1 DoF, and a confidence of
+        # self.ln_conc_confidence therefore, to get ln_conc_sigma, we need
+        # to divide by the square root of the PPF:
         ci = (self.ln_conc_ub - self.ln_conc_lb) / 2.0
         self.ln_conc_sigma = ci / stats.chi2.ppf(self.ln_conc_confidence, 1) ** (0.5)
 
         self.Nc, self.Nr = S.shape
         assert self.fluxes.shape == (self.Nr,)
         assert self.kcat.shape == (self.Nr,)
         assert self.standard_dg_over_rt.shape == (self.Nr,)
@@ -229,23 +231,23 @@
 
         assert self.params.get("regularization", "volume").lower() == "volume", (
             "Support to regularizations other than 'volume' was dropped when"
             "moving to CVXPY"
         )
         self.ln_capacity = cp.Constant(np.log(self.fluxes / self.kcat))
 
-    def _driving_forces(self, ln_conc: cp.Variable) -> cp.Expression:
-        """
-        calculate the driving force for every reaction in every condition
-        """
+    def _driving_forces(self, ln_conc: Union[np.ndarray, cp.Variable]) -> cp.Expression:
+        """Calculate the driving force for every reaction in every condition."""
         return -self.standard_dg_over_rt - self.S.T @ ln_conc
 
-    def _ln_eta_thermodynamic(self, ln_conc: cp.Variable) -> cp.Expression:
+    def _ln_eta_thermodynamic(
+        self, ln_conc: Union[np.ndarray, cp.Variable]
+    ) -> cp.Expression:
         """Calculate the minus log value of the thermodynamic efficiencies."""
-        return cp.log(1.0 - cp.exp(-self._driving_forces(ln_conc)))
+        return cp.log(cp.Constant(1.0) - cp.exp(-self._driving_forces(ln_conc)))
 
     def _B_matrix(self, col_subs: np.ndarray, col_prod: np.ndarray) -> np.ndarray:
         """Build the B matrix for the eta^kin expression.
 
         row_subs : np.ndarray
             A column from the substrate stoichiometric matrix. We assume
             coefficients represent reactant molecularities so
@@ -280,22 +282,20 @@
                 K_matrix(S_subs.shape[0]) @ S_subs,
                 K_matrix(S_prod.shape[0]) @ S_prod,
             ]
         )
 
         return A - np.ones((A.shape[0], S_subs.shape[0])) @ S_subs
 
-    def _ln_D_CM_minus_ln_D_S(self, i: int, ln_conc: cp.Variable) -> Expression:
+    def _ln_D_CM_minus_ln_D_S(self, i: int, ln_conc: cp.Variable) -> cp.Expression:
         B = self._B_matrix(self.S_subs[:, i], self.S_prod[:, i])
         return cp.log_sum_exp(B @ (ln_conc - np.log(self.KMM[:, i])))
 
-    def _ln_eta_kinetic(self, ln_conc: cp.Variable) -> Expression:
-        """
-        the kinetic part of ECF3 and ECF4
-        """
+    def _ln_eta_kinetic(self, ln_conc: Union[np.ndarray, cp.Variable]) -> cp.Expression:
+        """Calculate the kinetic part of ECF3 and ECF4."""
         ln_KMM = np.log(self.KMM)
         ln_conc_mat = cp.vstack([ln_conc] * self.Nr).T
 
         ln_D_S = self.S_subs.T @ (ln_conc_mat - ln_KMM)
         ln_D_P = self.S_prod.T @ (ln_conc_mat - ln_KMM)
 
         if self.params["denominator"] == "S":
@@ -304,19 +304,21 @@
             return -cp.diag(cp.logistic(-ln_D_S))
         elif self.params["denominator"] == "SP":
             return -cp.diag(cp.logistic(-ln_D_S + ln_D_P))
         elif self.params["denominator"] == "1SP":
             return -cp.diag(cp.logistic(-ln_D_S + cp.logistic(ln_D_P)))
         elif self.params["denominator"] == "CM":
             ln_eta = [-self._ln_D_CM_minus_ln_D_S(i, ln_conc) for i in range(self.Nr)]
-            return cp.reshape(cp.vstack(ln_eta), (self.Nr,))
+            return cp.vstack(ln_eta).flatten()
         else:
             raise ValueError("unsupported denominator: " + self.params["denominator"])
 
-    def _ln_eta_allosteric(self, ln_conc: cp.Variable) -> Expression:
+    def _ln_eta_allosteric(
+        self, ln_conc: Union[np.ndarray, cp.Variable]
+    ) -> cp.Expression:
         ln_K_act = np.log(self.K_act)
         ln_K_inh = np.log(self.K_inh)
         ln_conc_mat = cp.vstack([ln_conc] * self.Nr).T
 
         # original allosteric term:
         # 1 / (1 + prod(k_a/c_a)) / (1 + prod(c_i/k_i))
         # ln_act = self.A_act.T @ (ln_conc_mat - ln_K_act)
@@ -330,78 +332,88 @@
         ln_inh = self.A_inh.T @ cp.logistic(ln_conc_mat - ln_K_inh)
         ln_eta_act = -cp.diag(ln_act)
         ln_eta_inh = -cp.diag(ln_inh)
 
         return ln_eta_act + ln_eta_inh
 
     def is_feasible(self, ln_conc: np.ndarray) -> bool:
+        """Check if the problem is feasible."""
         df = self._driving_forces(ln_conc)
-        return (df > 0).all()
+        return (df > cp.Constant(0.0)).all()
 
-    def get_fluxes(self, ln_conc: np.ndarray, E: np.ndarray) -> np.ndarray:
+    def get_fluxes(
+        self,
+        ln_conc: Union[np.ndarray, cp.Variable],
+        E: Union[np.ndarray, cp.Variable],
+    ) -> np.ndarray:
         """Calculate the fluxes based on metabolite and enzyme conc."""
         assert ln_conc.shape == (self.Nc,)
         assert E.shape == (self.Nr,)
 
         v = self.kcat * E
         v *= np.exp(self._ln_eta_thermodynamic(ln_conc).value)
         v *= np.exp(self._ln_eta_kinetic(ln_conc).value)
         v *= np.exp(self._ln_eta_allosteric(ln_conc))
 
         return v.squeeze()
 
-    def _ECF1(self, ln_conc: cp.Variable) -> Expression:
-        """
+    def _ECF1(self, ln_conc: cp.Variable) -> cp.Expression:
+        """Calculate the level 1 cost.
+
         Arguments:
             A single metabolite ln-concentration vector
 
         Returns:
             The most basic Enzyme Cost Function (only dependent on flux
             and kcat). Gives the predicted enzyme concentrations in [M]
         """
         # ln_conc is not used for ECF1
         return self.ln_capacity
 
-    def _ECF2(self, ln_conc: cp.Variable) -> Expression:
-        """
+    def _ECF2(self, ln_conc: cp.Variable) -> cp.Expression:
+        """Calculate the level 2 cost.
+
         Arguments:
             A single metabolite ln-concentration vector
 
         Returns:
             The thermodynamic-only Enzyme Cost Function.
             Gives the predicted enzyme concentrations in [M].
         """
         return self._ECF1(ln_conc) - self._ln_eta_thermodynamic(ln_conc)
 
-    def _ECF3(self, ln_conc: cp.Variable) -> Expression:
-        """
+    def _ECF3(self, ln_conc: cp.Variable) -> cp.Expression:
+        """Calculate the level 3 cost.
+
         Arguments:
             A single metabolite ln-concentration vector
 
         Returns:
             An Enzyme Cost Function that integrates kinetic and
             thermodynamic data, but no allosteric regulation.
             Gives the predicted enzyme concentrations in [M].
         """
         return self._ECF2(ln_conc) - self._ln_eta_kinetic(ln_conc)
 
-    def _ECF4(self, ln_conc: cp.Variable) -> Expression:
-        """
+    def _ECF4(self, ln_conc: cp.Variable) -> cp.Expression:
+        """Calculate the level 4 cost.
+
         Arguments:
             A single metabolite ln-concentration vector
 
         Returns:
             The full Enzyme Cost Function, i.e. with kinetic, thermodynamic
             and allosteric data.
             Gives the predicted enzyme concentrations in [M].
         """
         return self._ECF3(ln_conc) - self._ln_eta_allosteric(ln_conc)
 
     def get_enzyme_cost_partitions(self, ln_conc: np.ndarray) -> np.ndarray:
-        """
+        """Calculate the cost partitions into the four categories.
+
         Arguments:
             A single metabolite ln-concentration vector
 
         Returns:
             A matrix contining the enzyme costs separated to the 4 ECF
             factors (as columns).
             The first column is the ECF1 predicted concentrations in [M].
@@ -411,15 +423,16 @@
         trm = cp.exp(-self._ln_eta_thermodynamic(ln_conc))  # thermodynamics
         kin = cp.exp(-self._ln_eta_kinetic(ln_conc))  # kinetics
         alo = cp.exp(-self._ln_eta_allosteric(ln_conc))
 
         return cp.vstack([cap, trm, kin, alo]).T.value
 
     def get_volumes(self, ln_conc: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-        """
+        """Calculate the volume occupied by every enzyme and metabolite.
+
         Arguments:
             A single metabolite ln-concentration vector
 
         Returns:
             Two arrays containing the enzyme volumes and
             metabolite volumes (at the provided point)
         """
@@ -429,23 +442,23 @@
         met_vols = np.multiply(met_conc, self.mw_met)
 
         # we have to remove the volume of water, otherwise it dominates all
         # other volumes
         met_vols[self.idx_water] = 0.0
         return enz_vols, met_vols
 
-    def _ln_total_enzyme_weight(self, ln_conc: cp.Variable) -> Expression:
+    def _ln_total_enzyme_weight(self, ln_conc: cp.Variable) -> cp.Expression:
         """Calculate the enzyme cost for an input concentration profile."""
         return cp.log_sum_exp(self.ECF(ln_conc) + np.log(self.mw_enz))
 
-    def _ln_total_metabolite_weight(self, ln_conc: cp.Variable) -> Expression:
+    def _ln_total_metabolite_weight(self, ln_conc: cp.Variable) -> cp.Expression:
         """Calculate the enzyme cost for an input concentration profile."""
         return cp.log_sum_exp(ln_conc + np.log(self.mw_met))
 
-    def _create_ecm_problem(self, ln_conc: cp.Variable) -> [Objective, Constraint]:
+    def _create_ecm_problem(self, ln_conc: cp.Variable) -> [cp.Expression, Constraint]:
         obj_enz_wgt = cp.Minimize(self._ln_total_enzyme_weight(ln_conc))
 
         if self.params["objective"] == "enzyme + metabolite":
             obj_met_wgt = cp.Minimize(self._ln_total_metabolite_weight(ln_conc))
             obj_ec = cp.transforms.scalarize.log_sum_exp(
                 [obj_enz_wgt, obj_met_wgt], weights=(1.0, 1.0)
             )
@@ -478,19 +491,21 @@
             return np.exp(prob.value), ln_conc.value
         elif prob.status == cp.OPTIMAL_INACCURATE:
             logging.warning("ECM solution is 'optimal_inaccurate'")
             return np.exp(prob.value), ln_conc.value
         else:
             raise Exception(prob.status)
 
-    def _calc_z_scores(self, ln_conc: cp.Variable) -> Expression:
+    def _calc_z_scores(self, ln_conc: Union[np.ndarray, cp.Variable]) -> cp.Expression:
         """Calculate individual zscores."""
         return (ln_conc - self.ln_conc_mu) / (self.ln_conc_sigma + 1e-9)
 
-    def _metabolic_adjustment(self, ln_conc: np.ndarray) -> float:
+    def _metabolic_adjustment(
+        self, ln_conc: Union[np.ndarray, cp.Variable]
+    ) -> cp.Expression:
         """Calculate metabolic adjustment score.
 
         Essentially, it is the sum of Z-scores for the multivariate Gaussian
         distribution of log-concentrations (described by mu and sigma)
         """
         idx = self.ln_conc_sigma >= self.MINIMAL_STDEV
         return sum(cp.power(self._calc_z_scores(ln_conc)[idx], 2))
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/ecm_model.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""A module for Enzyme Cost models."""
 # The MIT License (MIT)
 #
 # Copyright (c) 2013 Weizmann Institute of Science
 # Copyright (c) 2018-2020 Institute for Molecular Systems Biology,
 # ETH Zurich
 # Copyright (c) 2018-2020 Novo Nordisk Foundation Center for Biosustainability,
 # Technical University of Denmark
@@ -27,16 +28,16 @@
 from typing import Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from equilibrator_api import Q_, ComponentContribution
 from sbtab import SBtab
 
+from .analysis_solution import PathwayAnalysisSolution
 from .cost_function import EnzymeCostFunction
-from .ecm_solution import PathwayEcmSolution
 from .thermo_models import ThermodynamicModel
 from .util import ECF_DEFAULTS
 
 
 class EnzymeCostModel(object):
     """A class for Enzyme Cost Minimization analysis."""
 
@@ -45,14 +46,16 @@
         "Reaction",
         "ConcentrationConstraint",
         "Parameter",
         "Flux",
     }
 
     def __init__(self, thermo_model: ThermodynamicModel, param_df: pd.DataFrame):
+        """Create an EnzymeCostModel object."""
+
         self._thermo_model = thermo_model
         self.config_dict = dict(ECF_DEFAULTS)
         self.config_dict.update(self._thermo_model.config_dict)
 
         # TODO: use the stdev_factor (and the uncertainty estimates for the
         #  Gibbs energies, to somehow weigh the ECF)
         #  stdev_factor = self.config_dict.get("stdev_factor", 1.0)
@@ -148,28 +151,32 @@
         self._enz_conc_unit = Q_("M")
 
     @staticmethod
     def from_sbtab(
         filename: Union[str, SBtab.SBtabDocument],
         comp_contrib: Optional[ComponentContribution] = None,
     ) -> "EnzymeCostModel":
+        """Create an EnzymeCostModel from an SBtab file."""
+
         if isinstance(filename, str):
             sbtabdoc = SBtab.read_csv(filename, "pathway")
         elif isinstance(filename, SBtab.SBtabDocument):
             sbtabdoc = filename
 
         thermo_model = ThermodynamicModel.from_sbtab(sbtabdoc, comp_contrib)
 
         param_sbtab = sbtabdoc.get_sbtab_by_id("Parameter")
         assert param_sbtab, "Missing table 'Parameter' in the SBtab document"
         param_df = param_sbtab.to_data_frame()
 
         return EnzymeCostModel(thermo_model, param_df)
 
     def add_validation_data(self, filename: Union[str, SBtab.SBtabDocument]) -> None:
+        """Load the validation data."""
+
         if isinstance(filename, str):
             sbtabdoc = SBtab.read_csv(filename, "pathway")
         elif isinstance(filename, SBtab.SBtabDocument):
             sbtabdoc = filename
 
         conc_sbtab = sbtabdoc.get_sbtab_by_id("Concentration")
         self._met_conc_unit = Q_(conc_sbtab.get_attribute("Unit"))
@@ -189,14 +196,16 @@
             sbtab.table_id: sbtab.to_data_frame() for sbtab in sbtabdoc.sbtabs
         }
 
     @staticmethod
     def read_parameters(
         parameter_df: pd.DataFrame, ecf_params: dict
     ) -> Tuple[dict, ...]:
+        """Read the parameter data from a Pandas dataframe."""
+
         cols = ["QuantityType", "Value", "Compound", "Reaction", "Unit"]
 
         rid2mw = dict()
         cid2mw = dict()
         rid2crc_gmean = dict()  # catalytic rate constant geomertic mean
         rid2crc_fwd = dict()  # catalytic rate constant forward
         rid2crc_rev = dict()  # catalytic rate constant reverse
@@ -230,15 +239,15 @@
                     val.ito("Da")
                     rid2mw[rid] = val
                 elif typ == "molecular mass":
                     assert val.check("[mass]"), f"'{typ}' must have mass units"
                     val.ito("Da")
                     cid2mw[cid] = val
                 else:
-                    warnings.warn("unrecognized Parameter: " + typ)
+                    warnings.warn("unrecognized Parameter: " + typ, stacklevel=3)
             except AssertionError:
                 raise ValueError(
                     "Syntax error in Parameter table, row %d - %s" % (i, row)
                 )
         # make sure not to count water as contributing to the volume or
         # cost of a reaction
         return (
@@ -248,40 +257,67 @@
             rid_cid2KMM,
             rid2mw,
             cid2mw,
         )
 
     @staticmethod
     def _generate_KMM(cids: List[str], rids: List[str], rid_cid2KMM: dict) -> np.array:
+        """Generate the KMM matrix (containing the Michaelis constants)."""
+
         KMM = np.ones((len(cids), len(rids)))
         for i, cid in enumerate(cids):
             for j, rid in enumerate(rids):
                 kmm = rid_cid2KMM.get((rid, cid), Q_(1, "M"))
                 KMM[i, j] = kmm.m_as("M")
         return KMM * Q_(1, "M")
 
-    def optimize_ecm(self) -> PathwayEcmSolution:
+    def optimize_ecm(self) -> PathwayAnalysisSolution:
+        """Optimize the ECM model."""
+
+        from .ecm_solution import PathwayEcmSolution
+
         return PathwayEcmSolution(self, *self.ecf.optimize_ecm())
 
     def pareto(self, weights: Iterable[float] = None) -> pd.DataFrame:
+        """Minimize enzyme cost versus metabolic adjustment (Pareto).
+
+        enzyme cost is defined as in standard ECM.
+        metabolic adjustment is the sum of squared Z-scores of the metabolite
+        log-concentrations (relative to the prior Gaussian distribution).
+
+        Arguments
+        ---------
+        weights : Iterable[float]
+            the factor for the upper bounds on the ECM objective. Only
+            non-negative values are allowed
+
+        Returns
+        -------
+        results : DataFrame
+            a summary table of the results of all optimization runs
+        """
         return self.ecf.pareto(weights=weights)
 
     def _get_measured_metabolite_conc(self) -> Q_:
+        """Get the measured metabolite concentrations (validation data)."""
+
         assert (
             self._val_df_dict is not None
         ), "cannot validate results because no validation data was given"
 
         met_conc_df = self._val_df_dict["Concentration"].set_index("Compound")
         met_concentrations = Q_(
             pd.to_numeric(met_conc_df.Value)[self.compound_ids].values,
             self._met_conc_unit,
         )
         return met_concentrations
 
     def _get_measured_enzyme_conc(self) -> Q_:
+        """Get the measured enzyme concentrations (validation data)."""
+
         assert (
             self._val_df_dict is not None
         ), "cannot validate results because no validation data was given"
 
         enz_conc_df = self._val_df_dict["EnzymeConcentration"].set_index("Reaction")
         enz_concentrations = Q_(
             pd.to_numeric(enz_conc_df.Value)[self.reaction_ids].values,
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/ecm_solution.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/ecm_solution.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,34 +30,36 @@
 import pandas as pd
 from equilibrator_api import Q_
 from matplotlib import pyplot as plt
 from sbtab import SBtab
 
 from .analysis_solution import PathwayAnalysisSolution
 from .cost_function import EnzymeCostFunction
+from .ecm_model import EnzymeCostModel
 from .util import PlotCorrelation
 
 
 class PathwayEcmSolution(PathwayAnalysisSolution):
-    """Handle MDF results.
+    """Handle ECM results.
 
     PathwayMDFData is a container class for MDF results, with plotting
     capabilities.
     """
 
     def __init__(
-        self, ecm_model: "EnzymeCostModel", score: float, ln_conc: np.ndarray
+        self, ecm_model: EnzymeCostModel, score: float, ln_conc: np.ndarray
     ) -> None:
-        """
+        """Create a PathwayEcmSolution object.
 
         Parameters
         ----------
         ecm_model : EnzymeCostModel
         ln_conc : ndarray
             log concentrations at ECM optimum
+
         """
         super(PathwayEcmSolution, self).__init__(
             ecm_model._thermo_model, score, ln_conc
         )
         self.ecf = ecm_model.ecf
 
         if ecm_model._val_df_dict is not None:
@@ -92,15 +94,15 @@
         enz_vols : array
         met_vols : array
         """
         return self.ecf.get_volumes(self.ln_conc)
 
     @property
     def costs(self) -> np.ndarray:
-        """
+        """Return the cost array.
 
         Returns
         -------
         costs : array (2D)
             A matrix containing the enzyme costs separated to the 4 ECF
             factors (as columns).
             The first column is the ECF1 predicted concentrations in [M].
@@ -124,31 +126,33 @@
         return (
             enz_vols + met_vols,
             enz_labels + met_labels,
             enz_colors + met_colors,
         )
 
     def plot_volumes(self, ax: plt.axes) -> None:
+        """Create a bar-plot showing the volumes."""
         width = 0.8
         vols, labels, colors = self._get_volume_data_for_plotting()
 
         ax.bar(np.arange(len(vols)), vols, width, color=colors)
         ax.set_xticklabels(labels, size="medium", rotation=90)
         ax.set_ylabel("total weight [g/L]")
 
     def plot_volumes_pie(self, ax: plt.axes) -> None:
+        """Create a pie chart showing the volumes."""
         vols, labels, colors = self._get_volume_data_for_plotting()
         ax.pie(vols, labels=labels, colors=colors)
         ax.set_title(f"total weight = {sum(vols):.3g} [g/L]")
 
     def plot_thermodynamic_profile(self, ax: plt.axes) -> None:
-        """
-        Plot a cumulative line plot of the dG' values given the solution
-        for the metabolite levels. This was originally designed for showing
-        MDF results, but is also a useful tool for ECM.
+        """Plot a cumulative line plot of the dG' values.
+
+        Uses the solution for the metabolite levels. This was originally
+        designed for showing MDF results, but is also a useful tool for ECM.
         """
         dgs = [0] + list((-self.driving_forces).flat)
         cumulative_dgs = np.cumsum(dgs)
 
         xticks = np.arange(0, len(cumulative_dgs)) - 0.5
         xticklabels = [""] + list(self.reaction_ids)
         ax.plot(cumulative_dgs)
@@ -157,15 +161,16 @@
         ax.set_xlim(0, len(cumulative_dgs) - 1)
         ax.set_xlabel("")
         ax.set_ylabel(r"Cumulative $\Delta_r G'$ (kJ/mol)", family="sans-serif")
 
     def plot_enzyme_demand_breakdown(
         self, ax: plt.Axes, top_level: int = 3, plot_measured: bool = True
     ) -> None:
-        """
+        """Create a log-scaled stacked bar-plot of the enzyme demands.
+
         A bar plot in log-scale showing the partitioning of cost between
         the levels of kinetic costs:
         1 - capacity
         2 - thermodynamics
         3 - saturation
         4 - allosteric
         """
@@ -215,14 +220,15 @@
         ax.set_xticks(ind)
         ax.set_xticklabels(self.reaction_ids, size="medium", rotation=90)
         ax.legend(loc="best", framealpha=0.2)
         ax.set_ylabel("enzyme demand [M]")
         ax.set_ylim(bottom=base)
 
     def validate_metabolite_conc(self, ax: plt.Axes, scale: str = "log") -> None:
+        """Create a correlation plot validating the metabolite concentrations."""
         pred_met_conc = self.compound_df.concentration.apply(
             lambda x: x.m_as("M")
         ).values
 
         # remove NaNs and zeros
         mask = np.nan_to_num(self.meas_met_conc) > 0
         mask &= np.nan_to_num(pred_met_conc) > 0
@@ -238,28 +244,31 @@
             mask=mask,
             scale=scale,
         )
         ax.set_xlabel("measured [M]")
         ax.set_ylabel("predicted [M]")
 
     def validate_enzyme_conc(self, ax: plt.Axes, scale: str = "log") -> None:
+        """Create a correlation plot validating the enzyme concentrations."""
+
         pred_enz_conc = self.enzyme_df.concentration.apply(lambda x: x.m_as("M")).values
 
         PlotCorrelation(
             ax,
             self.meas_enz_conc.m_as("M"),
             pred_enz_conc,
             labels=self.enzyme_df.reaction_id,
             scale=scale,
         )
 
         ax.set_xlabel("measured [M]")
         ax.set_ylabel("predicted [M]")
 
     def to_sbtab(self) -> SBtab.SBtabDocument:
+        """Export the results to an SBtab file."""
         sbtabdoc = super(PathwayEcmSolution, self).to_sbtab()
 
         # add another table containing the optimized enzyme concentrations
         enz_df = self.enzyme_df[["reaction_id", "concentration"]].copy()
         enz_df["concentration"] = enz_df.concentration.apply(
             lambda x: f"{x.m_as('M'):.3e}"
         )
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/mdf_solution.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdf_solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,52 +23,54 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 from typing import Optional
 
 import numpy as np
-from equilibrator_api import Q_, ureg
+from equilibrator_api import ureg
 from matplotlib import pyplot as plt
 from matplotlib.collections import LineCollection
 
 from .analysis_solution import PathwayAnalysisSolution
+from .pathway import Pathway
 
 
 class PathwayMdfSolution(PathwayAnalysisSolution):
     """Handle MDF results.
 
     PathwayMDFData is a container class for MDF results, with plotting
     capabilities.
     """
 
     def __init__(
         self,
-        thermo_model: "PathwayThermoModel",
+        thermo_model: Pathway,
         score: float,
         ln_conc: np.array,
         y: np.array,
         reaction_prices: np.array,
         compound_prices: np.array,
     ) -> None:
-        """
+        """Create a PathwayMdfSolution object.
 
         Parameters
         ----------
         thermo_model : ThermodynamicModel
         score : float
             the optimal Max-min Driving Force (in kJ/mol)
         ln_conc : ndarray
             log concentrations at MDF optimum
         y : ndarray
             uncertainty matrix coefficients at MDF optimum
         reaction_prices : ndarray
             shadow prices of reactions
         compound_prices : ndarray
             shadow prices of compound concentrations
+
         """
         super(PathwayMdfSolution, self).__init__(thermo_model, score, ln_conc, y)
         self.reaction_df["shadow_price"] = reaction_prices
         self.compound_df["shadow_price"] = compound_prices
 
     def plot_concentrations(self, ax: Optional[plt.Axes] = None) -> None:
         """Plot compound concentrations.
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/mdmc_solution.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/mdmc_solution.py`

 * *Files 11% similar despite different names*

```diff
@@ -164,29 +164,24 @@
         ax.set_yscale("log")
         ax.set_xlim(self.min_lb - 2, self.max_lb + 2)
         if show_zscores:
             plt.colorbar(sc, label="Z-score")
 
     def plot_metabolite(self, met: str) -> plt.Figure:
         """Plot a single compound's concentration."""
-        from mpl_toolkits.mplot3d import Axes3D
-
         fig = plt.figure()
         ax = fig.add_subplot(1, 1, 1)
-        # ax = fig.gca(projection='3d')
 
         concentrations = self.concentration_df.loc[met, :]
         zscores = self.zscore_df.loc[met, :]
-        sc = ax.scatter(
+        ax.scatter(
             concentrations.index,
             concentrations.values,
             c=zscores.values,
             linewidth=0,
             s=5,
         )
-        # ax.text(self.min_lb - 0.1, concentrations.iat[0], met, ha="right", va="center")
-        # ax.text(self.max_lb + 0.1, concentrations.iat[-1], met, ha="left", va="center")
         ax.set_ylabel("{met} concentration [M]")
         ax.set_xlabel("lower bound on all Driving Forces [kJ/mol]")
         ax.set_yscale("log")
         ax.set_xlim(self.min_lb - 2, self.max_lb + 2)
         return fig
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/pathway.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/pathway.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-from typing import Callable, Dict, List, Optional, Union
+from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 from equilibrator_api import Q_, ComponentContribution, Reaction
 from equilibrator_cache import Compound
 from sbtab import SBtab
 
@@ -49,15 +49,14 @@
         fluxes: Q_,
         comp_contrib: Optional[ComponentContribution] = None,
         standard_dg_primes: Optional[Q_] = None,
         dg_sigma: Optional[Q_] = None,
         bounds: Optional[Bounds] = None,
         config_dict: Optional[Dict[str, str]] = None,
     ) -> None:
-
         """Initialize a Pathway object.
 
         Parameters
         ----------
         S : DataFrame
             stoichiometric matrix, where rows are the compound IDs and columns
             are the reaction IDs
@@ -74,16 +73,14 @@
         dg_sigma : Quantity, optional
             square root of the uncertainty covariance matrix (in kJ/mol)
         bounds : Bounds, optional
             bounds on metabolite concentrations (by default uses the
             "data/cofactors.csv" file in `equilibrator-api`)
         config_dict : dict, optional
             configuration parameters for Pathway analysis
-        compound_id_mapping : callable, optional
-            a function mapping compounds to their names in the model
         """
         super(Pathway, self).__init__(
             S=S,
             compound_dict=compound_dict,
             reaction_dict=reaction_dict,
             comp_contrib=comp_contrib,
             standard_dg_primes=standard_dg_primes,
@@ -94,26 +91,27 @@
 
         assert fluxes.unitless or fluxes.check("[concentration]/[time]")
         self.fluxes = fluxes.flatten()
         assert self.fluxes.shape == (self.Nr,)
         self.I_dir = np.diag(np.sign(self.fluxes.magnitude).flat)
 
     def get_net_reaction_sparse(self) -> Dict[str, int]:
+        """Get the net reaction as a sparse dictionary."""
         net_rxn_stoich = self.S @ self.fluxes.magnitude
         net_rxn_stoich = net_rxn_stoich[net_rxn_stoich != 0]
         return net_rxn_stoich.to_dict()
 
     @property
     def net_reaction(self) -> Reaction:
         """Calculate the sum of all the reactions in the pathway.
 
         :return: the net reaction
         """
         sparse = {
-            self.compound_dict[cid]: coeff
+            self.compound_dict[cid].compound: coeff
             for cid, coeff in self.get_net_reaction_sparse().items()
         }
         return Reaction(sparse)
 
     @property
     def net_reaction_formula(self) -> str:
         """Calculate the sum of all the reactions in the pathway.
@@ -170,15 +168,15 @@
         fluxes: Optional[np.ndarray] = None,
     ) -> "Pathway":
         """Convert a StoichiometricModel into a Pathway.
 
         Assume all fluxes are 1.
         """
         if fluxes is None:
-            fluxes = np.ones(len(stoich_model.reactions)) * Q_(1)
+            fluxes = np.ones(stoich_model.Nr) * Q_(1)
         pp = Pathway(
             S=stoich_model.S,
             compound_dict=stoich_model.compound_dict,
             reaction_dict=stoich_model.reaction_dict,
             fluxes=fluxes,
             comp_contrib=stoich_model.comp_contrib,
             standard_dg_primes=stoich_model.standard_dg_primes,
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/simulator.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""An ODE simulator for the ECM model."""
 # The MIT License (MIT)
 #
 # Copyright (c) 2013 Weizmann Institute of Science
 # Copyright (c) 2018-2020 Institute for Molecular Systems Biology,
 # ETH Zurich
 # Copyright (c) 2018-2020 Novo Nordisk Foundation Center for Biosustainability,
 # Technical University of Denmark
@@ -28,28 +29,32 @@
 import numpy as np
 from scipy.integrate import ode
 
 from .cost_function import EnzymeCostFunction
 
 
 class EnzymeCostSimulator(object):
+    """A class wrapping EnzymeCostFunction, adding simulating functions."""
+
     def __init__(self, ecf: EnzymeCostFunction) -> None:
+        """Create a EnzymeCostSimulator object."""
         self.ecf = ecf
 
         self.idx_fixed = np.where(self.ecf.ln_conc_sigma <= self.ecf.MINIMAL_STDEV)[
             0
         ].tolist()
 
         self.idx_non_fixed = np.where(self.ecf.ln_conc_sigma > self.ecf.MINIMAL_STDEV)[
             0
         ].tolist()
 
         self.E = np.ones(self.ecf.Nr)
 
     def set_enzyme_concentrations(self, E: np.ndarray) -> None:
+        """Set the enzyme concentrations."""
         assert E.shape == (self.ecf.Nr,)
         self.E = E
 
     def _derivaties(self, t, y):
         # we only care about the time derivatives of the internal
         # metabolites (i.e. the first and last one are assumed to be
         # fixed in time)
@@ -62,16 +67,16 @@
     def Simulate(
         self,
         lnC0: np.ndarray,
         t_max: float = 1000.0,
         dt: float = 1.0,
         eps: float = 1e-9,
     ) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Find the steady-state solution for the metabolite concentrations
+        """Find the steady-state solution for the metabolite concentrations.
+
         given the enzyme abundances
 
         Arguments:
             E    - enzyme abundances [gr]
             y0   - initial concentration of internal metabolites
                    (default: MDF solution)
             eps  - the minimal change under which the simulation will stop
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/thermo_models.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/thermo_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,27 +21,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 import logging
-from typing import Callable, Dict, Iterable, List, Optional, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 from cvxpy import Maximize, Minimize, Problem, Variable, norm2
 from cvxpy.constraints.constraint import Constraint
 from cvxpy.problems.objective import Objective
-from equilibrator_api import Q_, ComponentContribution, R, Reaction, default_T
-from equilibrator_cache import Compound
+from equilibrator_api import R, default_T
 from scipy import stats
 
-from . import Bounds
-from .mdf_solution import PathwayMdfSolution
+from .analysis_solution import PathwayAnalysisSolution
 from .mdmc_solution import PathwayMdmcSolution
 from .pathway import Pathway
 
 
 class ThermodynamicModel(Pathway):
     """Container for doing pathway-level thermodynamic analysis."""
 
@@ -141,21 +139,23 @@
             )
             lb = self.ln_conc_mu[j] - ci
             ub = self.ln_conc_mu[j] + ci
             c_lbs += [ln_conc[j] >= lb]
             c_ubs += [ln_conc[j] <= ub]
         return c_lbs, c_ubs
 
-    def mdf_analysis(self) -> PathwayMdfSolution:
+    def mdf_analysis(self) -> PathwayAnalysisSolution:
         """Find the MDF (Max-min Driving Force).
 
         Returns
         -------
         a PathwayMDFData object with the results of MDF analysis.
         """
+        from .mdf_solution import PathwayMdfSolution
+
         # ln-concentration variables (where the units are in M before taking
         # the log)
         ln_conc = Variable(shape=self.Nc, name="log concentrations")
         c_lbs, c_ubs = self._conc_constraints(ln_conc)
 
         # the margin variable representing the MDF in units of kJ/mol
         B = Variable(shape=1, name="minimum driving force")
@@ -169,27 +169,31 @@
             logging.warning("LP status %s", prob.status)
             raise Exception("Cannot solve MDF optimization problem")
 
         reaction_prices = np.array([float(c.dual_value) for c in dg_constraints]).round(
             5
         )
         compound_prices = np.array(
-            [float(u.dual_value - l.dual_value) for l, u in zip(c_lbs, c_ubs)]
+            [
+                float(upper.dual_value - lower.dual_value)
+                for lower, upper in zip(c_lbs, c_ubs)
+            ]
         ).round(5)
 
         return PathwayMdfSolution(
             self,
             score=prob.value,
             ln_conc=ln_conc.value,
             y=y.value if y is not None else None,
             reaction_prices=reaction_prices,
             compound_prices=compound_prices,
         )
 
     def get_zscores(self, ln_conc: Iterable) -> Iterable:
+        """Get the Z-scores for all the log-concentrations."""
         return map(
             lambda x: (x[0] - x[1]) / x[2] if x[2] > self.MINIMAL_STDEV else 0,
             zip(ln_conc, self.ln_conc_mu, self.ln_conc_sigma),
         )
 
     def _make_zscore_objective(self, ln_conc: Variable) -> Objective:
         """Set the Z-score as the new objective."""
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway/util.py` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""General utility functions."""
 # The MIT License (MIT)
 #
 # Copyright (c) 2013 Weizmann Institute of Science
 # Copyright (c) 2018-2020 Institute for Molecular Systems Biology,
 # ETH Zurich
 # Copyright (c) 2018-2020 Novo Nordisk Foundation Center for Biosustainability,
 # Technical University of Denmark
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/PKG-INFO` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equilibrator-pathway
-Version: 0.4.7
+Version: 0.4.8b1
 Summary: Pathway analysis tools by eQuilibrator
 Home-page: https://gitlab.com/equilibrator/equilibrator-pathway/
 Download-URL: https://pypi.org/project/equilibrator-pathway/
 Author: Elad Noor, Moritz E. Beber
 Author-email: eladn@weizmann.ac.il, midnighter@posteo.net
 License: MIT
 Project-URL: Source Code, https://gitlab.com/equilibrator/equilibrator-pathway/
```

### Comparing `equilibrator-pathway-0.4.7/src/equilibrator_pathway.egg-info/SOURCES.txt` & `equilibrator-pathway-0.4.8b1/src/equilibrator_pathway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equilibrator-pathway-0.4.7/versioneer.py` & `equilibrator-pathway-0.4.8b1/versioneer.py`

 * *Files identical despite different names*

