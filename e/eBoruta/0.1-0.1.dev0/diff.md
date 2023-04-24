# Comparing `tmp/eboruta-0.1.tar.gz` & `tmp/eboruta-0.1.dev0.tar.gz`

## Comparing `eboruta-0.1.tar` & `eboruta-0.1.dev0.tar`

### file list

```diff
@@ -1,44 +1,15 @@
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 eboruta-0.1/.readthedocs.yaml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eboruta-0.1/setup.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 eboruta-0.1/docs/Makefile
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 eboruta-0.1/docs/build_docs.sh
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 eboruta-0.1/docs/conf.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 eboruta-0.1/docs/eBoruta.rst
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 eboruta-0.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 eboruta-0.1/docs/make.bat
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 eboruta-0.1/docs/modules.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 eboruta-0.1/docs/notebooks.rst
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 eboruta-0.1/docs/ref.bib
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eboruta-0.1/docs/requirements.txt
--rw-r--r--   0        0        0  2190455 2020-02-02 00:00:00.000000 eboruta-0.1/docs/fig/Phosphorylation.png
--rw-r--r--   0        0        0   823048 2020-02-02 00:00:00.000000 eboruta-0.1/docs/fig/juswinderA.png
--rw-r--r--   0        0        0   520158 2020-02-02 00:00:00.000000 eboruta-0.1/docs/fig/juswinderB.png
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 eboruta-0.1/docs/notebooks/demo.ipynb
--rw-r--r--   0        0        0    29552 2020-02-02 00:00:00.000000 eboruta-0.1/docs/notebooks/sequence_determinants_tutorial.ipynb
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/__init__.py
--rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/algorithm.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/base.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/callbacks.py
--rw-r--r--   0        0        0    11665 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/containers.py
--rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/dataprep.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 eboruta-0.1/eBoruta/utils.py
--rw-r--r--   0        0        0  2190455 2020-02-02 00:00:00.000000 eboruta-0.1/fig/Phosphorylation.png
--rw-r--r--   0        0        0   283293 2020-02-02 00:00:00.000000 eboruta-0.1/fig/boruta.svg
--rw-r--r--   0        0        0    71357 2020-02-02 00:00:00.000000 eboruta-0.1/fig/eBoruta_diagram.png
--rw-r--r--   0        0        0   823048 2020-02-02 00:00:00.000000 eboruta-0.1/fig/juswinderA.png
--rw-r--r--   0        0        0   520158 2020-02-02 00:00:00.000000 eboruta-0.1/fig/juswinderB.png
--rw-r--r--   0        0        0    17840 2020-02-02 00:00:00.000000 eboruta-0.1/notebooks/Test oil boruta.ipynb
--rw-r--r--   0        0        0   116100 2020-02-02 00:00:00.000000 eboruta-0.1/notebooks/data_final1.csv
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 eboruta-0.1/notebooks/demo.ipynb
--rw-r--r--   0        0        0    23446 2020-02-02 00:00:00.000000 eboruta-0.1/notebooks/sequence_determinants_tutorial.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eboruta-0.1/test/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 eboruta-0.1/test/conftest.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 eboruta-0.1/test/test.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 eboruta-0.1/test/test_algorithm.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 eboruta-0.1/test/test_containers.py
--rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 eboruta-0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 eboruta-0.1/LICENCE
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 eboruta-0.1/README.md
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 eboruta-0.1/pyproject.toml
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 eboruta-0.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/setup.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/test.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/eBoruta/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/eBoruta/__init__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/eBoruta/base.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/eBoruta/callbacks.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/eBoruta/containers.py
+-rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/eBoruta/eBoruta.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/eBoruta/utils.py
+-rw-r--r--   0        0        0   616688 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/notebooks/demo.ipynb
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/LICENCE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/README.rst
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 eboruta-0.1.dev0/PKG-INFO
```

### Comparing `eboruta-0.1/eBoruta/callbacks.py` & `eboruta-0.1.dev0/eBoruta/callbacks.py`

 * *Files identical despite different names*

### Comparing `eboruta-0.1/eBoruta/containers.py` & `eboruta-0.1.dev0/eBoruta/containers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 Types holding intermediate and final data for the algorithm.
 """
-from __future__ import annotations
-
 import logging
 import typing as t
-from collections import abc, Counter
+from collections import Counter
 from dataclasses import dataclass, field
 
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
+from sklearn.utils import check_array
 
-from eBoruta.base import _X, _Y, ValidationError
-from eBoruta.dataprep import prepare_x, prepare_y, prepare_w, has_missing
-from eBoruta.utils import get_duplicates
+from eBoruta.base import _X, _Y, _W, _E
+from eBoruta.utils import convert_to_array, get_duplicates
 
 LOGGER = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class TrialData(t.Generic[_Y]):
     """
@@ -42,84 +40,104 @@
         """
         return (
             f"x_train: {self.x_train.shape}, y_train: {self.y_train.shape}, "
             f"x_test: {self.x_test.shape}, y_test: {self.y_test.shape}"
         )
 
 
-# @dataclass
+@dataclass
 class Dataset(t.Generic[_X, _Y]):
     """
     A container holding permanent data (x, y and weights) for
     training/validation/testing/etc.
     """
 
-    def __init__(self, x: t.Any, y: t.Any, w: t.Any = None, min_features: int = 5):
-        self._x, self._y, self._w = prepare_x(x), prepare_y(y), prepare_w(w)
-        self.min_features = min_features
-
-        if has_missing(self.y):
-            raise ValidationError("Missing values in y")
-        if len(self.x) != len(self.y):
-            raise ValidationError(
-                f"The number of observations in x {len(self.x)} "
-                f"does not match the number in y {len(self.y)}"
-            )
-        if self.w is not None and len(self.x) != len(self.w):
-            raise ValidationError(
-                f"The number of observations in x {len(self.x)} "
-                f"does not match the number in w {len(self.w)}"
-            )
+    x: _X
+    y: _Y
+    w: t.Optional[np.ndarray] = None
+    min_features: t.Optional[int] = 5
 
-    @property
-    def x(self) -> pd.DataFrame:
-        """
-        :return: Variables' dataframe.
-        """
-        return self._x
+    def __post_init__(self):
+        self.x = self.convert_x(self.x)
+        self.y = self.convert_y(self.y)
+        self.w = self.convert_w(self.w)
+        x_missing = self._check_input(self.x)
+        y_missing = self._check_input(self.y)
+
+        if y_missing:
+            raise AttributeError("Missing values in y")
+        if x_missing:
+            LOGGER.warning("Detected missing values in x")
 
-    @property
-    def y(self) -> np.ndarray:
-        """
-        :return: Target variables' array.
-        """
-        return self._y
+    @staticmethod
+    def convert_x(x: _X) -> pd.DataFrame:
+        if isinstance(x, np.ndarray):
+            if len(x.shape) == 1:
+                raise ValueError("Reshape your data: 1D input for x is not allowed")
+            x = pd.DataFrame(x, columns=list(map(str, range(1, x.shape[1] + 1))))
+        elif isinstance(x, pd.DataFrame):
+            x = x.copy().reset_index(drop=True)
+        else:
+            LOGGER.warning("Trying to convert x into an array")
+            x = convert_to_array(x)
+            num_features = x.shape[1] if len(x.shape) == 2 else 1
+            x = pd.DataFrame(x, columns=list(map(str, range(1, num_features + 1))))
+        check_array(
+            x.values, force_all_finite="allow-nan", ensure_2d=False, accept_sparse=False
+        )
+        return x
 
-    @property
-    def w(self) -> np.ndarray | None:
-        """
-        :return: Sample weights' array.
-        """
-        return self._w
+    @staticmethod
+    def convert_y(y: _Y) -> np.ndarray:
+        if isinstance(y, pd.DataFrame):
+            y = y.values
+        elif isinstance(y, pd.Series):
+            y = y.values
+        elif isinstance(y, np.ndarray):
+            pass
+        else:
+            LOGGER.warning("Trying to convert y into an array")
+            y = convert_to_array(y)
+        check_array(y, ensure_2d=False)
+        return y
+
+    @staticmethod
+    def convert_w(w: t.Optional[_W]) -> t.Optional[np.ndarray]:
+        if w is None:
+            return None
+
+        if isinstance(w, pd.Series):
+            w = w.values
+        elif isinstance(w, np.ndarray):
+            pass
+        else:
+            LOGGER.warning("Trying to convert w into an array")
+            w = convert_to_array(w)
+        check_array(w, ensure_2d=False)
+        return w
+
+    @staticmethod
+    def _check_input(a: t.Union[pd.DataFrame, pd.Series, np.ndarray]) -> bool:
+        try:
+            if isinstance(a, pd.DataFrame):
+                return a.isna().any().any()
+            if isinstance(a, pd.Series):
+                return a.isna().any()
+            if isinstance(a, np.ndarray):
+                return np.isnan(a).any()
+            LOGGER.warning(f"Unsupported input array type {type(a)}")
+            return False
+        except Exception as e:
+            LOGGER.exception(e)
+            LOGGER.warning(f"Failed to check input for missing values due to {e}")
+            return False
 
     def generate_trial_sample(
-        self, columns: None | list[str] | np.ndarray = None, **kwargs
+        self, columns: t.Union[None, t.List[str], np.ndarray] = None, **kwargs
     ) -> TrialData:
-        """
-        Generates data for a single Boruta trial based on :attr:`x`, :attr:`y`,
-        and :attr:`w`. Creates a copy of :attr:`x`, permutes rows, and renames
-        columns as "shadow_{original_name}". Concatenates original dataframe
-        and the one with the shadow features to create a copy of the learning
-        data with at least twice as many features.
-
-        If the number of features in :attr:`x` after selecting by ``columns``
-        is below :attr:`min_features`, randomly oversample existing features
-        to account for the difference. Thus, the returned dataframe to always
-        have at least :attr:`min_features` columns.
-
-        :param columns: An optional list or array of columns to select from
-            :attr:`x`.
-        :param kwargs: Keyword args passed to :func:`train_test_split` used to
-            create train/test splits. Enable this feature by passing
-            ``test_size={f}`` where ``f`` is the test size fraction.
-            This allows using different datasets for training and importance
-            computation.
-        :return: A prepared trial data.
-        :raises RuntimeError: If resulting features have duplicate names.
-        """
         if columns is None:
             columns = list(self.x.columns)
         if not isinstance(columns, list):
             columns = list(columns)
 
         x_init = self.x[columns].copy()
         LOGGER.debug(f"Using columns {columns} as features")
@@ -171,128 +189,52 @@
         if self.w is None:
             return TrialData(*train_test_split(x, y, **kwargs))
         return TrialData(*train_test_split(x, y, w, **kwargs))
 
 
 @dataclass
 class Features:
-    # TODO: consider adding slicing on steps and selecting columns pandas-like
-    """
-    A dynamic container representing a set of features used by Boruta
-    throughout the run.
-
-    It's created internally and maintained by :class:`eBoruta.algorithm.eBoruta`.
-    """
-
-    #: An array of feature names.
     names: np.ndarray
     accepted_mask: np.ndarray = field(init=False)
     rejected_mask: np.ndarray = field(init=False)
     tentative_mask: np.ndarray = field(init=False)
     hit_history: pd.DataFrame = field(init=False)
     imp_history: pd.DataFrame = field(init=False)
     dec_history: pd.DataFrame = field(init=False)
-    _history: pd.DataFrame | None = None
+    _history: t.Optional[pd.DataFrame] = None
 
     def __post_init__(self):
         n = len(self.names)
         self.accepted_mask, self.rejected_mask = np.zeros(n).astype(bool), np.zeros(
             n
         ).astype(bool)
         self.tentative_mask = np.ones(n).astype(bool)
         self.hit_history = pd.DataFrame(columns=self.names)
         self.imp_history = pd.DataFrame(columns=self.names)
         self.dec_history = pd.DataFrame(columns=self.names)
 
-    def __len__(self) -> int:
-        return len(self.hit_history)
-
-    def __getitem__(self, item: t.Any) -> t.Self:
-        def get_selectors() -> tuple[int | slice, list]:
-            match item:
-                case [int() | slice(), abc.Sequence()]:
-                    if len(item) != 2:
-                        raise IndexError('Too many indexing items')
-                    return item
-                case slice():
-                    return item, list(self.names)
-                case list():
-                    return slice(1, len(self.names)), item
-                case _:
-                    raise IndexError('Unsupported idx type')
-
-        steps, cols = get_selectors()
-        if isinstance(steps, int):
-            steps = [steps]
-
-        new = Features(np.intersect1d(self.names, cols))
-
-        new.hit_history = self.hit_history.iloc[steps][cols].copy()
-        new.imp_history = self.imp_history.iloc[steps][cols + ['Threshold']].copy()
-        new.dec_history = self.dec_history.iloc[steps][cols].copy()
-
-        decisions = new.dec_history.iloc[-1]
-        new.accepted_mask = decisions == 1
-        new.rejected_mask = decisions == -1
-        new.tentative_mask = decisions == 0
-
-        return new
-
-    @property
-    def shape(self) -> tuple[int, int]:
-        """
-        :return: (# steps, # features)
-        """
-        return len(self), len(self.names)
-
     @property
     def accepted(self) -> np.ndarray:
-        """
-        return: An array of feature names marked as accepted.
-        """
         return self.names[self.accepted_mask]
 
     @property
     def rejected(self) -> np.ndarray:
-        """
-        :return: An array of feature names marked as rejected.
-        """
         return self.names[self.rejected_mask]
 
     @property
     def tentative(self) -> np.ndarray:
-        """
-        :return: An array of feature names marked as tentative.
-        """
         return self.names[self.tentative_mask]
 
     @property
     def history(self) -> pd.DataFrame:
-        """
-        :return: A history dataframe created using :meth:`compose_summary` if
-            it doesn't exist.
-        """
         if self._history is None:
             self._history = self.compose_history()
         return self._history
 
-    def accepted_at_step(self, step: int) -> np.ndarray:
-        """
-        :param step: Step (trial) number.
-        :return: Feature names accepted at `step`.
-        """
-        df = self.history
-        return df[(df.Step == step) & (df.Decision == 'Accepted')]['Feature'].values
-
     def compose_history(self) -> pd.DataFrame:
-        """
-        Access the selection history and compose a summary table.
-
-        :return: A history dataframe.
-        """
         if self._history is not None:
             LOGGER.warning(
                 f"Overwriting existing history with shape {self._history.shape}"
             )
         self.reset_history_index()
         imp = self.melt_history(
             self.imp_history.drop(columns="Threshold"), "Importance"
@@ -328,17 +270,27 @@
             value_vars=columns,
             var_name="Feature",
             value_name=value_name,
         )
         return df
 
     def reset_history_index(self) -> None:
-        """
-        Bulk-:meth:`pd.DataFrame.reset_index`. of importance, decision and
-        hit history dataframes.
-        """
         for df in [self.imp_history, self.dec_history, self.hit_history]:
             df.reset_index(drop=True, inplace=True)
 
 
+class ImportanceGetter(t.Protocol):
+    def __call__(
+        self, estimator: _E, trial_data: t.Optional[TrialData] = None
+    ) -> np.ndarray:
+        ...
+
+
+class CVImportanceGetter:
+    # TODO: A special type of importance getter: `fit` is ommitted in the core loop and instead performed
+    # within this class, computing importances in a CV manner and aggregating the results.
+    # Thus, should be as abstract as possible allowing for custom importance evaluations and CV protocols.
+    pass
+
+
 if __name__ == "__main__":
     raise RuntimeError
```

### Comparing `eboruta-0.1/test/test.py` & `eboruta-0.1.dev0/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pytest
 from sklearn.datasets import make_classification, make_regression
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 from sklearn.utils.estimator_checks import parametrize_with_checks
 
-from eBoruta.algorithm import eBoruta
+from eBoruta.eBoruta import eBoruta
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
 
 
 @pytest.fixture
 def classification_data():
@@ -80,29 +80,29 @@
     for name, model in classifiers:
         try:
             boruta.shap_approximate = name != 'catboost'
             boruta.fit(x, y, model=model)
         except Exception as e:
             assert False, f'Failed to run classifier {name} due to {e}'
     x, y = regression_data
-    boruta = eBoruta(n_iter=20, classification=False, test_stratify=False, verbose=0)
+    boruta = eBoruta(n_iter=20, verbose=0, classification=False, test_stratify=False)
     for name, model in regressors:
         try:
             boruta.shap_approximate = name != 'catboost'
             boruta.fit(x, y, model=model)
         except Exception as e:
             assert False, f'Failed to run regressor {name} due to {e}'
 
 
 def test_params(classification_data):
     x, y = classification_data
     params = [{'shap_importance': False}, {'standardize_imp': True}, {'use_test': False}, {'rough_fix': False}]
     for param_set in params:
         try:
-            boruta = eBoruta(n_iter=10, verbose=0, **param_set)
+            boruta = eBoruta(verbose=0, n_iter=10, **param_set)
             boruta.fit(x, y)
         except Exception as e:
             assert False, f'Failed on param set {param_set} due to {e}'
 
 
 def test_multiobjective(classification_data, classifiers_multiobjective):
     x, y = make_classification()
```

### Comparing `eboruta-0.1/.gitignore` & `eboruta-0.1.dev0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 ### JetBrains template
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
 
 .idea/*
 
-docs/_*
-
-todo.md
-
-catboost_info
-
 # User-specific stuff
 .idea/**/workspace.xml
 .idea/**/tasks.xml
 .idea/**/usage.statistics.xml
 .idea/**/dictionaries
 .idea/**/shelf
```

### Comparing `eboruta-0.1/LICENCE` & `eboruta-0.1.dev0/LICENCE`

 * *Files identical despite different names*

### Comparing `eboruta-0.1/pyproject.toml` & `eboruta-0.1.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "eBoruta"
 description = 'Extended Boruta -- a flexible transparent sklearn-compatible python Boruta implementation'
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
     { name = "Ivan Reveguk", email = "ivan.reveguk@gmail.com" },
 ]
 classifiers = [
@@ -77,17 +77,14 @@
 #module = "toolz.*"
 #ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "sklearn.*"
 ignore_missing_imports = true
 
-[tool.pylint.main]
-ignore = ["test"]
-
 [tool.pylint.format]
 max-line-length = "88"
 good-names = "i, j, k, x, df, l, m, n, f, fn, e"
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "too-few-public-methods",
@@ -95,10 +92,9 @@
     "too-many-arguments",
     "too-many-locals",
     "too-many-instance-attributes",
     "logging-fstring-interpolation",
     "invalid-name",
     "eval-used",
     "exec-used",
-    "broad-except",
-    "attribute-defined-outside-init"
+    "broad-except"
 ]
```

