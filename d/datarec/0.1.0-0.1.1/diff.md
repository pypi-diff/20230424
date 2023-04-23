# Comparing `tmp/datarec-0.1.0.tar.gz` & `tmp/datarec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarec-0.1.0.tar", last modified: Fri Apr 21 05:41:49 2023, max compression
+gzip compressed data, was "datarec-0.1.1.tar", last modified: Sun Apr 23 23:50:43 2023, max compression
```

## Comparing `datarec-0.1.0.tar` & `datarec-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:41:49.796824 datarec-0.1.0/
--rw-rw-rw-   0        0        0      732 2023-04-21 05:41:49.794827 datarec-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-21 05:32:08.000000 datarec-0.1.0/README.md
--rw-rw-rw-   0        0        0     1083 2023-04-21 05:38:16.000000 datarec-0.1.0/license
--rw-rw-rw-   0        0        0      666 2023-04-21 05:41:19.000000 datarec-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 05:41:49.797826 datarec-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 05:41:49.688800 datarec-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 05:41:49.711805 datarec-0.1.0/src/datarec/
--rw-rw-rw-   0        0        0      100 2023-04-21 01:52:27.000000 datarec-0.1.0/src/datarec/__init__.py
--rw-rw-rw-   0        0        0     3702 2023-04-21 02:40:16.000000 datarec-0.1.0/src/datarec/data.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:41:49.758816 datarec-0.1.0/src/datarec/tables/
--rw-rw-rw-   0        0        0      202 2023-04-20 23:54:12.000000 datarec-0.1.0/src/datarec/tables/__init__.py
--rw-rw-rw-   0        0        0     3354 2023-04-21 01:56:04.000000 datarec-0.1.0/src/datarec/tables/_is_close_numeric.py
--rw-rw-rw-   0        0        0     2369 2023-04-21 01:55:42.000000 datarec-0.1.0/src/datarec/tables/_is_equal.py
--rw-rw-rw-   0        0        0     2391 2023-04-21 01:54:20.000000 datarec-0.1.0/src/datarec/tables/_method_base.py
--rw-rw-rw-   0        0        0     3792 2023-04-21 01:54:05.000000 datarec-0.1.0/src/datarec/tables/_reconciler.py
--rw-rw-rw-   0        0        0     4331 2023-04-21 01:53:36.000000 datarec-0.1.0/src/datarec/tables/_summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:41:49.775820 datarec-0.1.0/src/datarec/utils/
--rw-rw-rw-   0        0        0      145 2023-04-20 10:16:19.000000 datarec-0.1.0/src/datarec/utils/__init__.py
--rw-rw-rw-   0        0        0      321 2023-04-20 10:06:54.000000 datarec-0.1.0/src/datarec/utils/_get_suffixed.py
--rw-rw-rw-   0        0        0      309 2023-04-20 10:06:56.000000 datarec-0.1.0/src/datarec/utils/_set_case.py
--rw-rw-rw-   0        0        0     5627 2023-04-20 11:01:40.000000 datarec-0.1.0/src/datarec/utils/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:41:49.733811 datarec-0.1.0/src/datarec.egg-info/
--rw-rw-rw-   0        0        0      732 2023-04-21 05:41:49.000000 datarec-0.1.0/src/datarec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-04-21 05:41:49.000000 datarec-0.1.0/src/datarec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:41:49.000000 datarec-0.1.0/src/datarec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 05:41:49.000000 datarec-0.1.0/src/datarec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 05:41:49.000000 datarec-0.1.0/src/datarec.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 05:41:49.789823 datarec-0.1.0/tests/
--rw-rw-rw-   0        0        0     1756 2023-04-21 05:20:30.000000 datarec-0.1.0/tests/test_is_close.py
--rw-rw-rw-   0        0        0     1327 2023-04-21 05:23:16.000000 datarec-0.1.0/tests/test_is_equal.py
--rw-rw-rw-   0        0        0     3438 2023-04-21 05:20:14.000000 datarec-0.1.0/tests/test_summarizer.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:50:43.291192 datarec-0.1.1/
+-rw-rw-rw-   0        0        0      732 2023-04-23 23:50:43.290190 datarec-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-04-23 22:56:24.000000 datarec-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1083 2023-04-23 22:56:24.000000 datarec-0.1.1/license
+-rw-rw-rw-   0        0        0      666 2023-04-23 23:46:13.000000 datarec-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 23:50:43.292193 datarec-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 23:50:43.204177 datarec-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 23:50:43.225179 datarec-0.1.1/src/datarec/
+-rw-rw-rw-   0        0        0      106 2023-04-23 22:56:24.000000 datarec-0.1.1/src/datarec/__init__.py
+-rw-rw-rw-   0        0        0     5333 2023-04-23 23:44:40.000000 datarec-0.1.1/src/datarec/data.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:50:43.264185 datarec-0.1.1/src/datarec/tables/
+-rw-rw-rw-   0        0        0      207 2023-04-23 22:56:24.000000 datarec-0.1.1/src/datarec/tables/__init__.py
+-rw-rw-rw-   0        0        0     3467 2023-04-23 22:56:24.000000 datarec-0.1.1/src/datarec/tables/_is_close_numeric.py
+-rw-rw-rw-   0        0        0     2449 2023-04-23 22:56:24.000000 datarec-0.1.1/src/datarec/tables/_is_equal.py
+-rw-rw-rw-   0        0        0     2474 2023-04-23 22:56:24.000000 datarec-0.1.1/src/datarec/tables/_method_base.py
+-rw-rw-rw-   0        0        0     3928 2023-04-23 23:49:47.000000 datarec-0.1.1/src/datarec/tables/_reconciler.py
+-rw-rw-rw-   0        0        0     4479 2023-04-23 22:56:25.000000 datarec-0.1.1/src/datarec/tables/_summarizer.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:50:43.277187 datarec-0.1.1/src/datarec/utils/
+-rw-rw-rw-   0        0        0      150 2023-04-23 22:56:25.000000 datarec-0.1.1/src/datarec/utils/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-04-23 22:56:25.000000 datarec-0.1.1/src/datarec/utils/_get_suffixed.py
+-rw-rw-rw-   0        0        0      319 2023-04-23 22:56:25.000000 datarec-0.1.1/src/datarec/utils/_set_case.py
+-rw-rw-rw-   0        0        0     5821 2023-04-23 22:56:25.000000 datarec-0.1.1/src/datarec/utils/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:50:43.243181 datarec-0.1.1/src/datarec.egg-info/
+-rw-rw-rw-   0        0        0      732 2023-04-23 23:50:43.000000 datarec-0.1.1/src/datarec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-04-23 23:50:43.000000 datarec-0.1.1/src/datarec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 23:50:43.000000 datarec-0.1.1/src/datarec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 23:50:43.000000 datarec-0.1.1/src/datarec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 23:50:43.000000 datarec-0.1.1/src/datarec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 23:50:43.287188 datarec-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1756 2023-04-23 22:56:25.000000 datarec-0.1.1/tests/test_is_close.py
+-rw-rw-rw-   0        0        0     1327 2023-04-23 23:49:12.000000 datarec-0.1.1/tests/test_is_equal.py
+-rw-rw-rw-   0        0        0     3565 2023-04-23 23:45:58.000000 datarec-0.1.1/tests/test_summarizer.py
```

### Comparing `datarec-0.1.0/PKG-INFO` & `datarec-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarec
-Version: 0.1.0
+Version: 0.1.1
 Summary: utilities for reconciling data
 Author-email: Chris Mamon <chrisam1993@live.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datarec-0.1.0/license` & `datarec-0.1.1/license`

 * *Files identical despite different names*

### Comparing `datarec-0.1.0/pyproject.toml` & `datarec-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "datarec"
 description = "utilities for reconciling data"
-version     = "0.1.0"
+version     = "0.1.1"
 readme      = "README.md"
 dependencies = [
   "polars",
 ]
 authors         = [
   { name = "Chris Mamon", email = "chrisam1993@live.com" },
 ]
```

### Comparing `datarec-0.1.0/src/datarec/tables/_is_close_numeric.py` & `datarec-0.1.1/src/datarec/tables/_is_close_numeric.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-from typing import Iterable, List
-
-import polars as pl
-
-from ..data import TableReconciliationData
-from ._method_base import _ReconcilerMethodBase
-from ._reconciler import Reconciler
-
-
-class _ReconcilerMethodIsCloseFloat(_ReconcilerMethodBase):
-    def validator(
-        self, test_columns: str, merged: pl.LazyFrame, **kwargs
-    ) -> pl.LazyFrame:
-        get_left = self.methods.get_left
-        get_right = self.methods.get_right
-        setcase = self.methods.setcase
-        a_tol = kwargs["a_tol"]
-        r_tol = kwargs["r_tol"]
-
-        validation = merged.with_columns(
-            [
-                (
-                    (
-                        (pl.col(get_left(c)) - pl.col(get_right(c))).abs()
-                        < a_tol
-                    )
-                    | (
-                        (
-                            (pl.col(get_left(c)) - pl.col(get_right(c)))
-                            / (
-                                (pl.col(get_left(c)) + pl.col(get_right(c)))
-                                / 2
-                                + 1e-20
-                            )
-                        ).abs()
-                        < r_tol
-                    )
-                )
-                .fill_null(pl.lit(False))
-                .alias("%s ~*%s*~" % (c, setcase("validation")))
-                for c in test_columns
-            ]
-        )
-        return validation
-
-
-class _ReconcilerMethodIsCloseFloatNoIndex(_ReconcilerMethodIsCloseFloat):
-    def __call__(
-        self,
-        pl1: pl.LazyFrame,
-        pl2: pl.LazyFrame,
-        columns_to_ignore: List[int],
-        *,
-        a_tol: float,
-        r_tol: float
-    ) -> pl.LazyFrame:
-        test_columns = list(pl1.columns)
-        return super().__call__(
-            pl1, pl2, test_columns, columns_to_ignore, a_tol=a_tol, r_tol=r_tol
-        )
-
-
-class _ReconcilerMethodIsCloseFloatWithIndex(_ReconcilerMethodIsCloseFloat):
-    def __call__(
-        self,
-        pl1: pl.LazyFrame,
-        pl2: pl.LazyFrame,
-        columns_to_ignore: List[int],
-        columns_as_indexes: List[str],
-        *,
-        a_tol: float,
-        r_tol: float
-    ) -> pl.LazyFrame:
-        index_columns = [pl1.columns[i] for i in columns_as_indexes]
-        test_columns = list(
-            filter(lambda x: x not in index_columns, pl1.columns)
-        )
-        return super().__call__(
-            pl1, pl2, test_columns, columns_to_ignore, a_tol=a_tol, r_tol=r_tol
-        )
-
-
-def is_close_numeric(
-    p1: pl.LazyFrame,
-    p2: pl.LazyFrame,
-    pl1_name="left",
-    pl2_name="right",
-    interlaced: bool = True,
-    column_case: str = "upper",
-    show_both_first: bool = True,
-    show_failed_first: bool = True,
-    columns_to_ignore: Iterable[int] = None,
-    column_indexes: Iterable[int] = None,
-    a_tol: float = 10e-3,
-    r_tol: float = 10e-4,
-) -> TableReconciliationData:
-    return Reconciler(
-        _ReconcilerMethodIsCloseFloatNoIndex,
-        _ReconcilerMethodIsCloseFloatWithIndex,
-    )(
-        p1,
-        p2,
-        pl1_name=pl1_name,
-        pl2_name=pl2_name,
-        interlaced=interlaced,
-        column_case=column_case,
-        show_both_first=show_both_first,
-        show_failed_first=show_failed_first,
-        columns_to_ignore=columns_to_ignore,
-        column_indexes=column_indexes,
-        a_tol=a_tol,
-        r_tol=r_tol,
-    )
+from typing import Iterable, List
+
+import polars as pl
+
+from ..data import TableReconciliationData
+from ._method_base import _ReconcilerMethodBase
+from ._reconciler import Reconciler
+
+
+class _ReconcilerMethodIsCloseFloat(_ReconcilerMethodBase):
+    def validator(
+        self, test_columns: str, merged: pl.LazyFrame, **kwargs
+    ) -> pl.LazyFrame:
+        get_left = self.methods.get_left
+        get_right = self.methods.get_right
+        setcase = self.methods.setcase
+        a_tol = kwargs["a_tol"]
+        r_tol = kwargs["r_tol"]
+
+        validation = merged.with_columns(
+            [
+                (
+                    (
+                        (pl.col(get_left(c)) - pl.col(get_right(c))).abs()
+                        < a_tol
+                    )
+                    | (
+                        (
+                            (pl.col(get_left(c)) - pl.col(get_right(c)))
+                            / (
+                                (pl.col(get_left(c)) + pl.col(get_right(c)))
+                                / 2
+                                + 1e-20
+                            )
+                        ).abs()
+                        < r_tol
+                    )
+                )
+                .fill_null(pl.lit(False))
+                .alias("%s ~*%s*~" % (c, setcase("validation")))
+                for c in test_columns
+            ]
+        )
+        return validation
+
+
+class _ReconcilerMethodIsCloseFloatNoIndex(_ReconcilerMethodIsCloseFloat):
+    def __call__(
+        self,
+        pl1: pl.LazyFrame,
+        pl2: pl.LazyFrame,
+        columns_to_ignore: List[int],
+        *,
+        a_tol: float,
+        r_tol: float
+    ) -> pl.LazyFrame:
+        test_columns = list(pl1.columns)
+        return super().__call__(
+            pl1, pl2, test_columns, columns_to_ignore, a_tol=a_tol, r_tol=r_tol
+        )
+
+
+class _ReconcilerMethodIsCloseFloatWithIndex(_ReconcilerMethodIsCloseFloat):
+    def __call__(
+        self,
+        pl1: pl.LazyFrame,
+        pl2: pl.LazyFrame,
+        columns_to_ignore: List[int],
+        columns_as_indexes: List[str],
+        *,
+        a_tol: float,
+        r_tol: float
+    ) -> pl.LazyFrame:
+        index_columns = [pl1.columns[i] for i in columns_as_indexes]
+        test_columns = list(
+            filter(lambda x: x not in index_columns, pl1.columns)
+        )
+        return super().__call__(
+            pl1, pl2, test_columns, columns_to_ignore, a_tol=a_tol, r_tol=r_tol
+        )
+
+
+def is_close_numeric(
+    p1: pl.LazyFrame,
+    p2: pl.LazyFrame,
+    pl1_name="left",
+    pl2_name="right",
+    interlaced: bool = True,
+    column_case: str = "upper",
+    show_both_first: bool = True,
+    show_failed_first: bool = True,
+    columns_to_ignore: Iterable[int] = None,
+    column_indexes: Iterable[int] = None,
+    a_tol: float = 10e-3,
+    r_tol: float = 10e-4,
+) -> TableReconciliationData:
+    return Reconciler(
+        _ReconcilerMethodIsCloseFloatNoIndex,
+        _ReconcilerMethodIsCloseFloatWithIndex,
+    )(
+        p1,
+        p2,
+        pl1_name=pl1_name,
+        pl2_name=pl2_name,
+        interlaced=interlaced,
+        column_case=column_case,
+        show_both_first=show_both_first,
+        show_failed_first=show_failed_first,
+        columns_to_ignore=columns_to_ignore,
+        column_indexes=column_indexes,
+        a_tol=a_tol,
+        r_tol=r_tol,
+    )
```

### Comparing `datarec-0.1.0/src/datarec/tables/_is_equal.py` & `datarec-0.1.1/src/datarec/tables/_is_equal.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import typing as T
-
-import polars as pl
-
-from ..data import TableReconciliationData
-from ._method_base import _ReconcilerMethodBase
-from ._reconciler import Reconciler
-
-
-class _IsEqualReconcilerMethodBase(_ReconcilerMethodBase):
-    def validator(
-        self, test_columns: str, merged: pl.LazyFrame
-    ) -> pl.LazyFrame:
-        get_left = self.methods.get_left
-        get_right = self.methods.get_right
-        setcase = self.methods.setcase
-
-        validation = merged.with_columns(
-            [
-                (pl.col(get_left(c)) == pl.col(get_right(c))).alias(
-                    "%s ~*%s*~" % (c, setcase("validation"))
-                )
-                for c in test_columns
-            ]
-        )
-        return validation
-
-
-class _IsEqualReconcilerMethodeNoIndex(_IsEqualReconcilerMethodBase):
-    def __call__(
-        self,
-        pl1: pl.LazyFrame,
-        pl2: pl.LazyFrame,
-        columns_to_ignore: T.List[int],
-    ) -> pl.LazyFrame:
-        test_columns = list(pl1.columns)
-        return super().__call__(pl1, pl2, test_columns, columns_to_ignore)
-
-
-class _IsEqualReconcilerMethodWithIndex(_IsEqualReconcilerMethodBase):
-    def __call__(
-        self,
-        pl1: pl.LazyFrame,
-        pl2: pl.LazyFrame,
-        columns_to_ignore: T.List[int],
-        columns_as_indexes: T.List[str],
-    ) -> pl.LazyFrame:
-        index_columns = [pl1.columns[i] for i in columns_as_indexes]
-        test_columns = list(
-            filter(lambda x: x not in index_columns, pl1.columns)
-        )
-        return super().__call__(pl1, pl2, test_columns, columns_to_ignore)
-
-
-def is_equal(
-    p1: pl.LazyFrame,
-    p2: pl.LazyFrame,
-    pl1_name="left",
-    pl2_name="right",
-    interlaced: bool = True,
-    column_case: str = "upper",
-    show_both_first: bool = True,
-    show_failed_first: bool = True,
-    columns_to_ignore: T.Iterable[int] = None,
-    column_indexes: T.Iterable[int] = None,
-) -> TableReconciliationData:
-    return Reconciler(
-        _IsEqualReconcilerMethodeNoIndex, _IsEqualReconcilerMethodWithIndex
-    )(
-        p1,
-        p2,
-        pl1_name=pl1_name,
-        pl2_name=pl2_name,
-        interlaced=interlaced,
-        column_case=column_case,
-        show_both_first=show_both_first,
-        show_failed_first=show_failed_first,
-        columns_to_ignore=columns_to_ignore,
-        column_indexes=column_indexes,
-    )
+import typing as T
+
+import polars as pl
+
+from ..data import TableReconciliationData
+from ._method_base import _ReconcilerMethodBase
+from ._reconciler import Reconciler
+
+
+class _IsEqualReconcilerMethodBase(_ReconcilerMethodBase):
+    def validator(
+        self, test_columns: str, merged: pl.LazyFrame
+    ) -> pl.LazyFrame:
+        get_left = self.methods.get_left
+        get_right = self.methods.get_right
+        setcase = self.methods.setcase
+
+        validation = merged.with_columns(
+            [
+                (pl.col(get_left(c)) == pl.col(get_right(c))).alias(
+                    "%s ~*%s*~" % (c, setcase("validation"))
+                )
+                for c in test_columns
+            ]
+        )
+        return validation
+
+
+class _IsEqualReconcilerMethodeNoIndex(_IsEqualReconcilerMethodBase):
+    def __call__(
+        self,
+        pl1: pl.LazyFrame,
+        pl2: pl.LazyFrame,
+        columns_to_ignore: T.List[int],
+    ) -> pl.LazyFrame:
+        test_columns = list(pl1.columns)
+        return super().__call__(pl1, pl2, test_columns, columns_to_ignore)
+
+
+class _IsEqualReconcilerMethodWithIndex(_IsEqualReconcilerMethodBase):
+    def __call__(
+        self,
+        pl1: pl.LazyFrame,
+        pl2: pl.LazyFrame,
+        columns_to_ignore: T.List[int],
+        columns_as_indexes: T.List[str],
+    ) -> pl.LazyFrame:
+        index_columns = [pl1.columns[i] for i in columns_as_indexes]
+        test_columns = list(
+            filter(lambda x: x not in index_columns, pl1.columns)
+        )
+        return super().__call__(pl1, pl2, test_columns, columns_to_ignore)
+
+
+def is_equal(
+    p1: pl.LazyFrame,
+    p2: pl.LazyFrame,
+    pl1_name="left",
+    pl2_name="right",
+    interlaced: bool = True,
+    column_case: str = "upper",
+    show_both_first: bool = True,
+    show_failed_first: bool = True,
+    columns_to_ignore: T.Iterable[int] = None,
+    column_indexes: T.Iterable[int] = None,
+) -> TableReconciliationData:
+    return Reconciler(
+        _IsEqualReconcilerMethodeNoIndex, _IsEqualReconcilerMethodWithIndex
+    )(
+        p1,
+        p2,
+        pl1_name=pl1_name,
+        pl2_name=pl2_name,
+        interlaced=interlaced,
+        column_case=column_case,
+        show_both_first=show_both_first,
+        show_failed_first=show_failed_first,
+        columns_to_ignore=columns_to_ignore,
+        column_indexes=column_indexes,
+    )
```

### Comparing `datarec-0.1.0/src/datarec/tables/_reconciler.py` & `datarec-0.1.1/src/datarec/tables/_reconciler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-import typing as T
-
-from ..data import MethodData, TableReconciliationData
-from ..utils import GetSuffixed, SetCase
-from ..utils.functions import (
-    convert_iterable_to_list,
-    get_formated_ordered_union,
-    group_suffixed,
-    validate_index_columns,
-)
-
-try:
-    from collections.abc import Callable
-except ImportError:
-    from typing import Callable
-
-import polars as pl
-
-
-class Reconciler:
-    def __init__(
-        self, NoIndexConstructor: Callable, WithIndexConstructor: Callable
-    ):
-        self.NoIndexConstructor = NoIndexConstructor
-        self.WithIndexConstructor = WithIndexConstructor
-
-    def __call__(
-        self,
-        pl1: pl.LazyFrame,
-        pl2: pl.LazyFrame,
-        pl1_name: str = "left",
-        pl2_name: str = "right",
-        interlaced: bool = True,
-        column_case: str = "upper",
-        show_both_first: bool = True,
-        show_failed_first: bool = True,
-        columns_to_ignore: T.Iterable = None,
-        column_indexes: T.Iterable = None,
-        **kwargs
-    ) -> TableReconciliationData:
-        assert pl1_name != pl2_name, "tables names must be different"
-
-        setcase = SetCase(column_case)
-        get_left = GetSuffixed(setcase, pl1_name)
-        get_right = GetSuffixed(setcase, pl2_name)
-        methods = MethodData(setcase, get_left, get_right)
-
-        compare_no_index = self.NoIndexConstructor(methods)
-        compare_with_index = self.WithIndexConstructor(methods)
-
-        if column_indexes is None:
-            column_indexes = []
-
-        column_indexes = convert_iterable_to_list(column_indexes)
-
-        if columns_to_ignore is None:
-            columns_to_ignore = []
-
-        columns_to_ignore = convert_iterable_to_list(columns_to_ignore)
-
-        shared_columns = get_formated_ordered_union(
-            pl1.columns, pl2.columns, formatter=setcase
-        )
-
-        pl1 = pl1.rename({c: setcase(c) for c in pl1.columns})
-        pl2 = pl2.rename({c: setcase(c) for c in pl2.columns})
-
-        pl1 = pl1.select([pl.col(c) for c in shared_columns])
-        pl2 = pl2.select([pl.col(c) for c in shared_columns])
-
-        _all_columns = pl1.columns
-        _columns_used_as_indexes = [shared_columns[i] for i in column_indexes]
-        _columns_tested = [
-            c for c in _all_columns if c not in _columns_used_as_indexes
-        ]
-        _columns_ignored = [_columns_tested[i] for i in columns_to_ignore]
-        _index_and_tested = _columns_used_as_indexes + _columns_ignored
-        _tested_columns = [
-            c for c in _all_columns if c not in _index_and_tested
-        ]
-
-        if len(column_indexes) == 0:
-            validation = compare_no_index(
-                pl1, pl2, columns_to_ignore, **kwargs
-            )
-        else:
-            validate_index_columns(pl1.clone(), column_indexes, "left")
-            validate_index_columns(pl2.clone(), column_indexes, "right")
-
-            validation = compare_with_index(
-                pl1, pl2, columns_to_ignore, column_indexes, **kwargs
-            )
-
-        if interlaced:
-            sorted_columns = group_suffixed(validation.columns)
-
-            validation = validation.select([pl.col(c) for c in sorted_columns])
-
-        if show_failed_first:
-            validation_columns = filter(
-                lambda x: setcase("~*validation*~") in x, validation.columns
-            )
-            validation = validation.sort(by=validation_columns)
-
-        if show_both_first:
-            validation = validation.sort(
-                by=setcase("**both**"), descending=True
-            )
-
-        return TableReconciliationData(
-            validation,
-            pl1_name,
-            pl2_name,
-            _all_columns,
-            _columns_used_as_indexes,
-            _columns_ignored,
-            _tested_columns,
-        )
+import typing as T
+
+from ..data import MethodData, TableReconciliationData
+from ..utils import GetSuffixed, SetCase
+from ..utils.functions import (
+    convert_iterable_to_list,
+    get_formated_ordered_union,
+    group_suffixed,
+    validate_index_columns,
+)
+
+try:
+    from collections.abc import Callable
+except ImportError:
+    from typing import Callable
+
+import polars as pl
+
+
+class Reconciler:
+    def __init__(
+        self, NoIndexConstructor: Callable, WithIndexConstructor: Callable
+    ):
+        self.NoIndexConstructor = NoIndexConstructor
+        self.WithIndexConstructor = WithIndexConstructor
+
+    def __call__(
+        self,
+        pl1: pl.LazyFrame,
+        pl2: pl.LazyFrame,
+        pl1_name: str = "left",
+        pl2_name: str = "right",
+        interlaced: bool = True,
+        column_case: str = "upper",
+        show_both_first: bool = True,
+        show_failed_first: bool = True,
+        columns_to_ignore: T.Iterable = None,
+        column_indexes: T.Iterable = None,
+        **kwargs
+    ) -> TableReconciliationData:
+        assert pl1_name != pl2_name, "tables names must be different"
+
+        setcase = SetCase(column_case)
+        get_left = GetSuffixed(setcase, pl1_name)
+        get_right = GetSuffixed(setcase, pl2_name)
+        methods = MethodData(setcase, get_left, get_right)
+
+        compare_no_index = self.NoIndexConstructor(methods)
+        compare_with_index = self.WithIndexConstructor(methods)
+
+        if column_indexes is None:
+            column_indexes = []
+
+        column_indexes = convert_iterable_to_list(column_indexes)
+
+        if columns_to_ignore is None:
+            columns_to_ignore = []
+
+        columns_to_ignore = convert_iterable_to_list(columns_to_ignore)
+
+        shared_columns = get_formated_ordered_union(
+            pl1.columns, pl2.columns, formatter=setcase
+        )
+
+        pl1 = pl1.rename({c: setcase(c) for c in pl1.columns})
+        pl2 = pl2.rename({c: setcase(c) for c in pl2.columns})
+
+        pl1 = pl1.select([pl.col(c) for c in shared_columns])
+        pl2 = pl2.select([pl.col(c) for c in shared_columns])
+
+        _all_columns = pl1.columns
+        _columns_used_as_indexes = [shared_columns[i] for i in column_indexes]
+        _columns_tested = [
+            c for c in _all_columns if c not in _columns_used_as_indexes
+        ]
+        _columns_ignored = [_columns_tested[i] for i in columns_to_ignore]
+        _index_and_tested = _columns_used_as_indexes + _columns_ignored
+        _tested_columns = [
+            c for c in _all_columns if c not in _index_and_tested
+        ]
+
+        if len(column_indexes) == 0:
+            validation = compare_no_index(
+                pl1, pl2, columns_to_ignore, **kwargs
+            )
+        else:
+            validate_index_columns(pl1.clone(), column_indexes, "left")
+            validate_index_columns(pl2.clone(), column_indexes, "right")
+
+            validation = compare_with_index(
+                pl1, pl2, columns_to_ignore, column_indexes, **kwargs
+            )
+
+        if interlaced:
+            sorted_columns = group_suffixed(validation.columns)
+
+            validation = validation.select([pl.col(c) for c in sorted_columns])
+
+        if show_failed_first:
+            validation_columns = filter(
+                lambda x: setcase("~*validation*~") in x, validation.columns
+            )
+            validation = validation.sort(by=validation_columns)
+
+        if show_both_first:
+            validation = validation.sort(
+                by=setcase("**both**"), descending=True
+            )
+
+        return TableReconciliationData(
+            validation,
+            setcase(pl1_name),
+            setcase(pl2_name),
+            _all_columns,
+            _columns_used_as_indexes,
+            _columns_ignored,
+            _tested_columns,
+        )
```

### Comparing `datarec-0.1.0/src/datarec/tables/_summarizer.py` & `datarec-0.1.1/src/datarec/tables/_summarizer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import numpy as np
-from numpy import typing as np_types
-import polars as pl
-from ..data import (
-    TableReconciliationData,
-    TableReconciliationSummarizationData,
-)
-
-
-def _get_validations(lf: pl.LazyFrame) -> pl.LazyFrame:
-    validation_columns = [
-        c for c in lf.columns if "~*validation*~" in c.lower()
-    ]
-    return lf.select([pl.col(c) for c in validation_columns])
-
-
-def _make_2d(arr: np_types.NDArray) -> np_types.NDArray:
-    if len(arr.shape) < 2:
-        return arr.reshape(-1, 1)
-    return arr
-
-
-def _summarizer(arr: np_types.DTypeLike):
-    rows, cols = arr.shape
-    n_entries = rows * cols
-
-    n_entries_passed = arr.sum()
-    n_entries_failed = n_entries - n_entries_passed
-
-    n_rows_passed = (arr.sum(axis=1) == cols).sum()
-    n_rows_partially_passed = (
-        np.logical_and((arr.sum(axis=1) > 0), (arr.sum(axis=1) != cols))
-    ).sum()
-
-    if len(arr) > 0:
-        avg_row_invalidations = (arr == 0).sum(1).mean()
-        std_row_invalidations = (arr == 0).sum(1).std()
-    else:
-        avg_row_invalidations = 0
-        std_row_invalidations = 0
-
-    n_rows_failed = rows - n_rows_passed - n_rows_partially_passed
-
-    try:
-        entry_validation_ratio = n_entries_passed / n_entries
-    except ZeroDivisionError:
-        entry_validation_ratio = 0
-
-    try:
-        row_validation_ratio = n_rows_passed / rows
-    except ZeroDivisionError:
-        row_validation_ratio = 0
-
-    return (
-        rows,
-        cols,
-        n_entries,
-        n_entries_passed,
-        n_entries_failed,
-        n_rows_passed,
-        n_rows_partially_passed,
-        n_rows_failed,
-        entry_validation_ratio,
-        row_validation_ratio,
-        avg_row_invalidations,
-        std_row_invalidations,
-    )
-
-
-def _get_totals(lf: pl.LazyFrame):
-    left_col = [c for c in lf.columns if "**left**" in c.lower()][0]
-    right_col = [c for c in lf.columns if "**right**" in c.lower()][0]
-    intersecting_col = [c for c in lf.columns if "**both**" in c.lower()][0]
-    n_total_rows_left = lf.select(left_col).collect().to_numpy().sum()
-    n_total_rows_right = lf.select(right_col).collect().to_numpy().sum()
-    n_total_rows_intersection = (
-        lf.select(intersecting_col).collect().to_numpy().sum()
-    )
-    n_total_rows_union = len(lf.select(left_col).collect())
-
-    return (
-        n_total_rows_left,
-        n_total_rows_right,
-        n_total_rows_intersection,
-        n_total_rows_union,
-    )
-
-
-def _shared_summarize(
-    lf: pl.LazyFrame, filter_col: str
-) -> TableReconciliationData:
-    lf_original = lf
-    if filter_col is not None:
-        lf = lf.filter(pl.col(filter_col))
-    arr = _make_2d(_get_validations(lf).collect().to_numpy())
-    return TableReconciliationSummarizationData(
-        *_summarizer(arr), *_get_totals(lf_original)
-    )
-
-
-def _left_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
-    filter_col = [c for c in lf.columns if "**left**" in c.lower()][0]
-    return _shared_summarize(lf, filter_col)
-
-
-def _right_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
-    filter_col = [c for c in lf.columns if "**right**" in c.lower()][0]
-    return _shared_summarize(lf, filter_col)
-
-
-def _inner_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
-    filter_col = [c for c in lf.columns if "**both**" in c.lower()][0]
-    return _shared_summarize(lf, filter_col)
-
-
-def _outer_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
-    return _shared_summarize(lf, None)
-
-
-summarizer_map = {
-    "left": _left_summarize,
-    "right": _right_summarize,
-    "inner": _inner_summarize,
-    "outer": _outer_summarize,
-}
-
-
-def summarize_reconciliation(
-    reconciliation: TableReconciliationData, join: str = "outer"
-) -> TableReconciliationSummarizationData:
-    results = reconciliation.results
-    column_indexes = reconciliation.columns_indexes
-    columns_ignored = reconciliation.columns_ignored
-
-    # columns to process
-    processable_columns = [
-        pl.col(c)
-        for c in results.columns
-        if all([c not in t for t in (columns_ignored + column_indexes)])
-    ]
-
-    # grab the validations
-    processable_table = results.select(processable_columns)
-
-    # summarizer method
-    summarizer_method = summarizer_map[join]
-
-    return summarizer_method(processable_table)
+import numpy as np
+from numpy import typing as np_types
+import polars as pl
+from ..data import (
+    TableReconciliationData,
+    TableReconciliationSummarizationData,
+)
+
+
+def _get_validations(lf: pl.LazyFrame) -> pl.LazyFrame:
+    validation_columns = [
+        c for c in lf.columns if "~*validation*~" in c.lower()
+    ]
+    return lf.select([pl.col(c) for c in validation_columns])
+
+
+def _make_2d(arr: np_types.NDArray) -> np_types.NDArray:
+    if len(arr.shape) < 2:
+        return arr.reshape(-1, 1)
+    return arr
+
+
+def _summarizer(arr: np_types.DTypeLike):
+    rows, cols = arr.shape
+    n_entries = rows * cols
+
+    n_entries_passed = arr.sum()
+    n_entries_failed = n_entries - n_entries_passed
+
+    n_rows_passed = (arr.sum(axis=1) == cols).sum()
+    n_rows_partially_passed = (
+        np.logical_and((arr.sum(axis=1) > 0), (arr.sum(axis=1) != cols))
+    ).sum()
+
+    if len(arr) > 0:
+        avg_row_invalidations = (arr == 0).sum(1).mean()
+        std_row_invalidations = (arr == 0).sum(1).std()
+    else:
+        avg_row_invalidations = 0
+        std_row_invalidations = 0
+
+    n_rows_failed = rows - n_rows_passed - n_rows_partially_passed
+
+    try:
+        entry_validation_ratio = n_entries_passed / n_entries
+    except ZeroDivisionError:
+        entry_validation_ratio = 0
+
+    try:
+        row_validation_ratio = n_rows_passed / rows
+    except ZeroDivisionError:
+        row_validation_ratio = 0
+
+    return (
+        rows,
+        cols,
+        n_entries,
+        n_entries_passed,
+        n_entries_failed,
+        n_rows_passed,
+        n_rows_partially_passed,
+        n_rows_failed,
+        entry_validation_ratio,
+        row_validation_ratio,
+        avg_row_invalidations,
+        std_row_invalidations,
+    )
+
+
+def _get_totals(lf: pl.LazyFrame):
+    left_col = [c for c in lf.columns if "**left**" in c.lower()][0]
+    right_col = [c for c in lf.columns if "**right**" in c.lower()][0]
+    intersecting_col = [c for c in lf.columns if "**both**" in c.lower()][0]
+    n_total_rows_left = lf.select(left_col).collect().to_numpy().sum()
+    n_total_rows_right = lf.select(right_col).collect().to_numpy().sum()
+    n_total_rows_intersection = (
+        lf.select(intersecting_col).collect().to_numpy().sum()
+    )
+    n_total_rows_union = len(lf.select(left_col).collect())
+
+    return (
+        n_total_rows_left,
+        n_total_rows_right,
+        n_total_rows_intersection,
+        n_total_rows_union,
+    )
+
+
+def _shared_summarize(
+    lf: pl.LazyFrame, filter_col: str
+) -> TableReconciliationData:
+    lf_original = lf
+    if filter_col is not None:
+        lf = lf.filter(pl.col(filter_col))
+    arr = _make_2d(_get_validations(lf).collect().to_numpy())
+    return TableReconciliationSummarizationData(
+        *_summarizer(arr), *_get_totals(lf_original)
+    )
+
+
+def _left_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
+    filter_col = [c for c in lf.columns if "**left**" in c.lower()][0]
+    return _shared_summarize(lf, filter_col)
+
+
+def _right_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
+    filter_col = [c for c in lf.columns if "**right**" in c.lower()][0]
+    return _shared_summarize(lf, filter_col)
+
+
+def _inner_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
+    filter_col = [c for c in lf.columns if "**both**" in c.lower()][0]
+    return _shared_summarize(lf, filter_col)
+
+
+def _outer_summarize(lf: pl.LazyFrame) -> TableReconciliationSummarizationData:
+    return _shared_summarize(lf, None)
+
+
+summarizer_map = {
+    "left": _left_summarize,
+    "right": _right_summarize,
+    "inner": _inner_summarize,
+    "outer": _outer_summarize,
+}
+
+
+def summarize_reconciliation(
+    reconciliation: TableReconciliationData, join: str = "outer"
+) -> TableReconciliationSummarizationData:
+    results = reconciliation.results
+    column_indexes = reconciliation.columns_indexes
+    columns_ignored = reconciliation.columns_ignored
+
+    # columns to process
+    processable_columns = [
+        pl.col(c)
+        for c in results.columns
+        if all([c not in t for t in (columns_ignored + column_indexes)])
+    ]
+
+    # grab the validations
+    processable_table = results.select(processable_columns)
+
+    # summarizer method
+    summarizer_method = summarizer_map[join]
+
+    return summarizer_method(processable_table)
```

### Comparing `datarec-0.1.0/src/datarec/utils/functions.py` & `datarec-0.1.1/src/datarec/utils/functions.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-import re
-import polars as pl
-from typing import Iterable, Callable, Tuple, List
-from collections import OrderedDict
-
-
-def get_lazyframe_length(lf: pl.LazyFrame) -> int:
-    try:
-        return lf.with_row_count().select("row_nr").last().collect().item() + 1
-    except ValueError:
-        return 0
-
-
-def get_prefixes(suffixed_iterable: Iterable[str], regex: str) -> List[str]:
-    """Extracts the unique prefixes from a given iterable of strings with a
-    given regex.
-
-    Args:
-        suffixed_iterable (Iterable): An iterable of strings to extract prefixes
-        from.
-
-        regex (str): A regex string pattern to use for extracting the prefixes.
-
-    Returns:
-        list[str]: A list of unique prefixes extracted from the given iterable
-        of strings.
-    """
-
-    found = set()
-
-    def set_found(x):
-        prefix = re.sub(regex, "", x)
-        found.add(prefix)
-        return prefix
-
-    base_columns = [
-        set_found(x)
-        for x in suffixed_iterable
-        if re.sub(regex, "", x) not in found
-    ]
-
-    return base_columns
-
-
-def group_suffixed(
-    suffixed_iterable: Iterable[str], regex: str = " ~.+?~"
-) -> List[str]:
-    """Groups a given iterable of strings by their prefixes with a given regex.
-
-    Args:
-        suffixed_iterable (Iterable): An iterable of strings to group by
-        prefixes.
-
-        regex (str, optional): A regex string pattern to use for extracting the
-        prefixes. Defaults to " ~.+?~".
-
-    Returns:
-        list[str]: A list of strings with the given iterable of strings grouped
-        by their prefixes.
-    """
-
-    base_columns = get_prefixes(suffixed_iterable, regex)
-
-    grouped_column_names = OrderedDict()
-
-    for key in base_columns:
-        grouped_column_names[key] = []
-
-    base_suffix_map = {c: re.sub(regex, "", c) for c in suffixed_iterable}
-
-    for new, original in base_suffix_map.items():
-        grouped_column_names[original].append(new)
-
-    sorted_columns = []
-
-    for cols in grouped_column_names.values():
-        sorted_columns.extend(cols)
-
-    return sorted_columns
-
-
-def get_ordered_union(set_1: Iterable[str], set_2: Iterable[str]) -> List[str]:
-    """Computes the ordered union of two given iterables of strings.
-
-    Args:
-        set_1 (Iterable): The first iterable of strings.
-
-        set_2 (Iterable): The second iterable of strings.
-
-    Returns:
-        list[str]: A list of strings with the ordered union of the two given
-        iterables of strings.
-    """
-    union_columns = set(set_1).union(set(set_2))
-    return [col for col in set_1 if col in union_columns]
-
-
-def get_formated_ordered_union(
-    iter_1: Iterable[str],
-    iter_2: Iterable[str],
-    formatter: Callable = lambda x: x,
-) -> List[str]:
-    """Computes the formatted ordered union of two given iterables of objects.
-
-    Args:
-        iter_1 (Iterable): The first iterable of objects.
-
-        iter_2 (Iterable): The second iterable of objects.
-
-        formatter (Callable, optional): A callable object to format each object
-        in the iterables (default identity function).
-
-    Returns:
-        list[str]: A list of objects with the formatted ordered union of the two
-        given iterables of objects.
-    """
-    iter_1 = [formatter(c) for c in iter_1]
-    iter_2 = [formatter(c) for c in iter_2]
-    return get_ordered_union(iter_1, iter_2)
-
-
-def validate_index_columns(
-    df: pl.LazyFrame, index_of_columns: Iterable[int], title: str
-) -> Tuple[int, int]:
-    """Validates that the given columns in a DataFrame are unique.
-
-    Args:
-        df (pl.LazyFrame): A polars DataFrame to validate the columns of.
-
-        index_of_columns (Iterable): An iterable of indices of columns in the
-        DataFrame to validate.
-
-        title (str): A string title of the DataFrame being validated.
-
-    Returns:
-        Tuple[int, int]: A tuple of integers with the number of unique columns
-        and total number of rows in the DataFrame.
-    """
-
-    columns = [df.columns[c] for c in index_of_columns]
-
-    repetitions_columns = (
-        df.select([pl.col(c) for c in columns])
-        .groupby([pl.col(c) for c in columns])
-        .agg(pl.count().alias("group_repetitions"))
-        .with_columns(pl.col("group_repetitions").map(lambda x: x == 1))
-        .select("group_repetitions")
-    ).collect()
-
-    n_unique = repetitions_columns.sum().to_numpy().squeeze()
-    n_rows = len(repetitions_columns)
-
-    assert (
-        n_unique == n_rows
-    ), f"indexes must be unique. there are {n_unique} \
-            unique columns out of a total {n_rows} for the {title} df"
-
-    return n_unique, n_rows
-
-
-def filter_iterable(_l: Iterable[object], c: Iterable[object]) -> List[str]:
-    """Filters a given iterable of objects by excluding the elements at the
-    given indices.
-
-    Args:
-        _l (Iterable): The iterable of objects to filter.
-
-        c (Iterable): An iterable of indices to exclude from the filtered
-        iterable.
-
-    Returns:
-        list[str]: A list of objects with the given iterable of objects filtered
-        by excluding the elements at the given indices.
-    """
-
-    return [_l[i] for i in range(len(_l)) if i not in c]
-
-
-def convert_iterable_to_list(iterable: Iterable[object]) -> List[object]:
-    """Converts an iterable to a list of objects.
-
-    Args:
-        iterable (Iterable): The iterable of objects to convert to a list.
-
-    Returns:
-        list[object]: A list of objects with the given iterable converted to a
-        list.
-    """
-
-    if isinstance(iterable, Iterable):
-        iterable = list(iterable)
-    else:
-        iterable = list([iterable])
-    return iterable
+import re
+import polars as pl
+from typing import Iterable, Callable, Tuple, List
+from collections import OrderedDict
+
+
+def get_lazyframe_length(lf: pl.LazyFrame) -> int:
+    try:
+        return lf.with_row_count().select("row_nr").last().collect().item() + 1
+    except ValueError:
+        return 0
+
+
+def get_prefixes(suffixed_iterable: Iterable[str], regex: str) -> List[str]:
+    """Extracts the unique prefixes from a given iterable of strings with a
+    given regex.
+
+    Args:
+        suffixed_iterable (Iterable): An iterable of strings to extract prefixes
+        from.
+
+        regex (str): A regex string pattern to use for extracting the prefixes.
+
+    Returns:
+        list[str]: A list of unique prefixes extracted from the given iterable
+        of strings.
+    """
+
+    found = set()
+
+    def set_found(x):
+        prefix = re.sub(regex, "", x)
+        found.add(prefix)
+        return prefix
+
+    base_columns = [
+        set_found(x)
+        for x in suffixed_iterable
+        if re.sub(regex, "", x) not in found
+    ]
+
+    return base_columns
+
+
+def group_suffixed(
+    suffixed_iterable: Iterable[str], regex: str = " ~.+?~"
+) -> List[str]:
+    """Groups a given iterable of strings by their prefixes with a given regex.
+
+    Args:
+        suffixed_iterable (Iterable): An iterable of strings to group by
+        prefixes.
+
+        regex (str, optional): A regex string pattern to use for extracting the
+        prefixes. Defaults to " ~.+?~".
+
+    Returns:
+        list[str]: A list of strings with the given iterable of strings grouped
+        by their prefixes.
+    """
+
+    base_columns = get_prefixes(suffixed_iterable, regex)
+
+    grouped_column_names = OrderedDict()
+
+    for key in base_columns:
+        grouped_column_names[key] = []
+
+    base_suffix_map = {c: re.sub(regex, "", c) for c in suffixed_iterable}
+
+    for new, original in base_suffix_map.items():
+        grouped_column_names[original].append(new)
+
+    sorted_columns = []
+
+    for cols in grouped_column_names.values():
+        sorted_columns.extend(cols)
+
+    return sorted_columns
+
+
+def get_ordered_union(set_1: Iterable[str], set_2: Iterable[str]) -> List[str]:
+    """Computes the ordered union of two given iterables of strings.
+
+    Args:
+        set_1 (Iterable): The first iterable of strings.
+
+        set_2 (Iterable): The second iterable of strings.
+
+    Returns:
+        list[str]: A list of strings with the ordered union of the two given
+        iterables of strings.
+    """
+    union_columns = set(set_1).union(set(set_2))
+    return [col for col in set_1 if col in union_columns]
+
+
+def get_formated_ordered_union(
+    iter_1: Iterable[str],
+    iter_2: Iterable[str],
+    formatter: Callable = lambda x: x,
+) -> List[str]:
+    """Computes the formatted ordered union of two given iterables of objects.
+
+    Args:
+        iter_1 (Iterable): The first iterable of objects.
+
+        iter_2 (Iterable): The second iterable of objects.
+
+        formatter (Callable, optional): A callable object to format each object
+        in the iterables (default identity function).
+
+    Returns:
+        list[str]: A list of objects with the formatted ordered union of the two
+        given iterables of objects.
+    """
+    iter_1 = [formatter(c) for c in iter_1]
+    iter_2 = [formatter(c) for c in iter_2]
+    return get_ordered_union(iter_1, iter_2)
+
+
+def validate_index_columns(
+    df: pl.LazyFrame, index_of_columns: Iterable[int], title: str
+) -> Tuple[int, int]:
+    """Validates that the given columns in a DataFrame are unique.
+
+    Args:
+        df (pl.LazyFrame): A polars DataFrame to validate the columns of.
+
+        index_of_columns (Iterable): An iterable of indices of columns in the
+        DataFrame to validate.
+
+        title (str): A string title of the DataFrame being validated.
+
+    Returns:
+        Tuple[int, int]: A tuple of integers with the number of unique columns
+        and total number of rows in the DataFrame.
+    """
+
+    columns = [df.columns[c] for c in index_of_columns]
+
+    repetitions_columns = (
+        df.select([pl.col(c) for c in columns])
+        .groupby([pl.col(c) for c in columns])
+        .agg(pl.count().alias("group_repetitions"))
+        .with_columns(pl.col("group_repetitions").map(lambda x: x == 1))
+        .select("group_repetitions")
+    ).collect()
+
+    n_unique = repetitions_columns.sum().to_numpy().squeeze()
+    n_rows = len(repetitions_columns)
+
+    assert (
+        n_unique == n_rows
+    ), f"indexes must be unique. there are {n_unique} \
+            unique columns out of a total {n_rows} for the {title} df"
+
+    return n_unique, n_rows
+
+
+def filter_iterable(_l: Iterable[object], c: Iterable[object]) -> List[str]:
+    """Filters a given iterable of objects by excluding the elements at the
+    given indices.
+
+    Args:
+        _l (Iterable): The iterable of objects to filter.
+
+        c (Iterable): An iterable of indices to exclude from the filtered
+        iterable.
+
+    Returns:
+        list[str]: A list of objects with the given iterable of objects filtered
+        by excluding the elements at the given indices.
+    """
+
+    return [_l[i] for i in range(len(_l)) if i not in c]
+
+
+def convert_iterable_to_list(iterable: Iterable[object]) -> List[object]:
+    """Converts an iterable to a list of objects.
+
+    Args:
+        iterable (Iterable): The iterable of objects to convert to a list.
+
+    Returns:
+        list[object]: A list of objects with the given iterable converted to a
+        list.
+    """
+
+    if isinstance(iterable, Iterable):
+        iterable = list(iterable)
+    else:
+        iterable = list([iterable])
+    return iterable
```

### Comparing `datarec-0.1.0/src/datarec.egg-info/PKG-INFO` & `datarec-0.1.1/src/datarec.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarec
-Version: 0.1.0
+Version: 0.1.1
 Summary: utilities for reconciling data
 Author-email: Chris Mamon <chrisam1993@live.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datarec-0.1.0/src/datarec.egg-info/SOURCES.txt` & `datarec-0.1.1/src/datarec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datarec-0.1.0/tests/test_is_close.py` & `datarec-0.1.1/tests/test_is_close.py`

 * *Files identical despite different names*

### Comparing `datarec-0.1.0/tests/test_is_equal.py` & `datarec-0.1.1/tests/test_is_equal.py`

 * *Files identical despite different names*

### Comparing `datarec-0.1.0/tests/test_summarizer.py` & `datarec-0.1.1/tests/test_summarizer.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import numpy as np
-import polars as pl
-from dbqq import connectors
-from datarec import tables
-
-
-try:
-    from tests.queries import query1, query2
-except ImportError:
-    import sys
-    import pathlib as pt
-
-    cwd = pt.Path(__file__).parent.absolute()
-    sys.path.append(cwd.parent.absolute().as_posix())
-    from tests.queries import query1, query2
-
-
-def validate_no_index():
-    columns = [
-        "sum_energy",
-        "sum_marketfeevalue",
-        "sum_feerate",
-        "sum_feeunits",
-    ]
-
-    pl_columns = [pl.col(c) for c in columns]
-
-    connector1 = connectors.oracle.improd()
-    connector2 = connectors.databricks.prod()
-
-    p1 = connector1.cache()(query1).select(
-        [pl.col(p.upper()) for p in columns]
-    )
-
-    p2 = connector2.cache()(query2).select(pl_columns)
-
-    return tables.is_close_numeric(
-        p1,
-        p2,
-        show_both_first=True,
-        show_failed_first=True,
-    )
-
-
-def validate_with_index():
-    connector1 = connectors.oracle.improd()
-    connector2 = connectors.databricks.prod()
-
-    p1 = connector1.cache()(query1)
-
-    p2 = connector2.cache()(query2)
-
-    return tables.is_close_numeric(
-        p1,
-        p2,
-        column_indexes=range(0, 6),
-        columns_to_ignore=0,
-        show_both_first=True,
-        show_failed_first=True,
-    )
-
-
-validation_no_index = validate_no_index()
-validation_with_index = validate_with_index()
-
-
-class TestSummarization:
-    def test_left_no_index(self):
-        summary = tables.summarize_reconciliation(validation_no_index, "left")
-        assert summary.validation_ratio_entries == 1, "failed"
-
-    def test_right_no_index(self):
-        summary = tables.summarize_reconciliation(validation_no_index, "right")
-        assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
-        ), "failed"
-
-    def test_inner_no_index(self):
-        summary = tables.summarize_reconciliation(validation_no_index, "inner")
-        assert summary.validation_ratio_entries == 1, "failed"
-
-    def test_outer_no_index(self):
-        summary = tables.summarize_reconciliation(validation_no_index, "outer")
-        assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
-        ), "failed"
-
-    def test_left_with_index(self):
-        summary = tables.summarize_reconciliation(
-            validation_with_index, "left"
-        )
-        assert summary.validation_ratio_entries == 1, "failed"
-
-    def test_right_with_index(self):
-        summary = tables.summarize_reconciliation(
-            validation_with_index, "right"
-        )
-        assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
-        ), "failed"
-
-    def test_inner_with_index(self):
-        summary = tables.summarize_reconciliation(
-            validation_with_index, "inner"
-        )
-        assert summary.validation_ratio_entries == 1, "failed"
-
-    def test_outer_with_index(self):
-        summary = tables.summarize_reconciliation(
-            validation_with_index, "outer"
-        )
-        assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
-        ), "failed"
-
-
-if __name__ == "__main__":
-    T = TestSummarization()
-    T.test_right_no_index()
-    T.test_left_no_index()
-    T.test_inner_no_index()
-    T.test_outer_no_index()
-
-    T.test_right_with_index()
-    T.test_left_with_index()
-    T.test_inner_with_index()
-    T.test_outer_with_index()
+import numpy as np
+import polars as pl
+from dbqq import connectors
+from datarec import tables
+
+
+try:
+    from tests.queries import query1, query2
+except ImportError:
+    import sys
+    import pathlib as pt
+
+    cwd = pt.Path(__file__).parent.absolute()
+    sys.path.append(cwd.parent.absolute().as_posix())
+    from tests.queries import query1, query2
+
+
+def validate_no_index():
+    columns = [
+        "sum_energy",
+        "sum_marketfeevalue",
+        "sum_feerate",
+        "sum_feeunits",
+    ]
+
+    pl_columns = [pl.col(c) for c in columns]
+
+    connector1 = connectors.oracle.improd()
+    connector2 = connectors.databricks.prod()
+
+    p1 = connector1.cache()(query1).select(
+        [pl.col(p.upper()) for p in columns]
+    )
+
+    p2 = connector2.cache()(query2).select(pl_columns)
+
+    return tables.is_close_numeric(
+        p1,
+        p2,
+        show_both_first=True,
+        show_failed_first=True,
+    )
+
+
+def validate_with_index():
+    connector1 = connectors.oracle.improd()
+    connector2 = connectors.databricks.prod()
+
+    p1 = connector1.cache()(query1)
+
+    p2 = connector2.cache()(query2)
+
+    return tables.is_close_numeric(
+        p1,
+        p2,
+        column_indexes=range(0, 6),
+        columns_to_ignore=0,
+        show_both_first=True,
+        show_failed_first=True,
+    )
+
+
+validation_no_index = validate_no_index()
+validation_with_index = validate_with_index()
+
+
+class TestSummarization:
+    def test_left_no_index(self):
+        summary = tables.summarize_reconciliation(validation_no_index, "left")
+        assert summary.validation_ratio_entries == 1, "failed"
+
+    def test_right_no_index(self):
+        summary = tables.summarize_reconciliation(validation_no_index, "right")
+        assert np.isclose(
+            summary.validation_ratio_entries, 0.9523809523809523
+        ), "failed"
+
+    def test_inner_no_index(self):
+        summary = tables.summarize_reconciliation(validation_no_index, "inner")
+        assert summary.validation_ratio_entries == 1, "failed"
+
+    def test_outer_no_index(self):
+        summary = tables.summarize_reconciliation(validation_no_index, "outer")
+        assert np.isclose(
+            summary.validation_ratio_entries, 0.9523809523809523
+        ), "failed"
+
+    def test_left_with_index(self):
+        summary = tables.summarize_reconciliation(
+            validation_with_index, "left"
+        )
+        assert summary.validation_ratio_entries == 1, "failed"
+
+    def test_right_with_index(self):
+        summary = tables.summarize_reconciliation(
+            validation_with_index, "right"
+        )
+        assert np.isclose(
+            summary.validation_ratio_entries, 0.9523809523809523
+        ), "failed"
+
+    def test_inner_with_index(self):
+        summary = tables.summarize_reconciliation(
+            validation_with_index, "inner"
+        )
+        assert summary.validation_ratio_entries == 1, "failed"
+
+    def test_outer_with_index(self):
+        summary = tables.summarize_reconciliation(
+            validation_with_index, "outer"
+        )
+        assert np.isclose(
+            summary.validation_ratio_entries, 0.9523809523809523
+        ), "failed"
+
+
+if __name__ == "__main__":
+    T = TestSummarization()
+    T.test_right_no_index()
+    T.test_left_no_index()
+    T.test_inner_no_index()
+    T.test_outer_no_index()
+
+    T.test_right_with_index()
+    T.test_left_with_index()
+    T.test_inner_with_index()
+    T.test_outer_with_index()
```

