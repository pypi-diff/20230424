# Comparing `tmp/ReplayTables-andnp-2.4.0.tar.gz` & `tmp/ReplayTables-andnp-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReplayTables-andnp-2.4.0.tar", last modified: Fri Apr 21 21:30:06 2023, max compression
+gzip compressed data, was "ReplayTables-andnp-2.5.0.tar", last modified: Mon Apr 24 04:02:34 2023, max compression
```

## Comparing `ReplayTables-andnp-2.4.0.tar` & `ReplayTables-andnp-2.5.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0        0 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/README.md
--rw-r--r--   0        0        0     5174 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/Distributions.py
--rw-r--r--   0        0        0     2140 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/LagBuffer.py
--rw-r--r--   0        0        0     2388 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/PER.py
--rw-r--r--   0        0        0     3622 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/ReplayBuffer.py
--rw-r--r--   0        0        0     8232 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/Table.py
--rw-r--r--   0        0        0        0 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/__init__.py
--rw-r--r--   0        0        0     3416 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/MemoryWriter.py
--rw-r--r--   0        0        0     1772 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/RandDict.py
--rw-r--r--   0        0        0     3816 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/SumTree.py
--rw-r--r--   0        0        0        0 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-21 21:29:29.729979 ReplayTables-andnp-2.4.0/ReplayTables/_utils/jit.py
--rw-r--r--   0        0        0      888 2023-04-21 21:30:05.398145 ReplayTables-andnp-2.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3076 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_LagBuffer.py
--rw-r--r--   0        0        0     2370 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_PER.py
--rw-r--r--   0        0        0     2679 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_ReplayBuffer.py
--rw-r--r--   0        0        0     1537 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_Table.py
--rw-r--r--   0        0        0     5621 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/test_View.py
--rw-r--r--   0        0        0        0 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2987 2023-04-21 21:29:29.733979 ReplayTables-andnp-2.4.0/tests/utils/test_SumTree.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/README.md
+-rw-r--r--   0        0        0     5174 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/Distributions.py
+-rw-r--r--   0        0        0     2140 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/LagBuffer.py
+-rw-r--r--   0        0        0     2388 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/PER.py
+-rw-r--r--   0        0        0     1818 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/PrioritizedHeap.py
+-rw-r--r--   0        0        0     3622 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0        0        0     8236 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/Table.py
+-rw-r--r--   0        0        0        0 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/__init__.py
+-rw-r--r--   0        0        0     3418 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/_utils/MemoryWriter.py
+-rw-r--r--   0        0        0     5813 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/_utils/MinMaxHeap.py
+-rw-r--r--   0        0        0     1772 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0        0        0     3824 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0        0        0        0 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/_utils/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/_utils/jit.py
+-rw-r--r--   0        0        0       58 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/ReplayTables/_utils/logger.py
+-rw-r--r--   0        0        0      888 2023-04-24 04:02:33.309284 ReplayTables-andnp-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3076 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/test_LagBuffer.py
+-rw-r--r--   0        0        0     2370 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/test_PER.py
+-rw-r--r--   0        0        0     2679 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/test_ReplayBuffer.py
+-rw-r--r--   0        0        0     1537 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/test_Table.py
+-rw-r--r--   0        0        0     5621 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/test_View.py
+-rw-r--r--   0        0        0        0 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1217 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/utils/test_MinMaxHeap.py
+-rw-r--r--   0        0        0     2987 2023-04-24 04:01:56.933081 ReplayTables-andnp-2.5.0/tests/utils/test_SumTree.py
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-2.5.0/PKG-INFO
```

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/Distributions.py` & `ReplayTables-andnp-2.5.0/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/LagBuffer.py` & `ReplayTables-andnp-2.5.0/ReplayTables/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/PER.py` & `ReplayTables-andnp-2.5.0/ReplayTables/PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/ReplayBuffer.py` & `ReplayTables-andnp-2.5.0/ReplayTables/ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/Table.py` & `ReplayTables-andnp-2.5.0/ReplayTables/Table.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,18 +222,18 @@
 
         # note this needs to be 2 loops
         # otherwise we change dict while iterating, which is error-prone
         keys = list(to_del())
         for key in keys:
             del self._refs[key]
 
-@try2jit
+@try2jit()
 def rotatedSequence(lo: int, hi: int, mod: int) -> np.ndarray:
     seq = np.arange(lo, hi, dtype=np.int64)
     return seq % mod
 
-@try2jit
+@try2jit()
 def padded(arr: np.ndarray, size: int, mult: int, value: float = np.nan):
     s = int(np.ceil(size / mult) * mult)
     out = np.ones((s, ) + arr.shape[1:], dtype=arr.dtype) * value
     out[:arr.shape[0]] = arr
     return out
```

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/_utils/MemoryWriter.py` & `ReplayTables-andnp-2.5.0/ReplayTables/_utils/MemoryWriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from typing import Any, Dict, Optional
 from numba.typed import List as NList
 from ReplayTables._utils.jit import try2jit
 from concurrent.futures import ThreadPoolExecutor, Future
 
-@try2jit
+@try2jit()
 def _update(tree: NList[np.ndarray], dim: int, idxs: np.ndarray, values: np.ndarray):
     for idx, value in zip(idxs, values):
         sub_idx = idx
         old = tree[0][dim, idx]
 
         for i in range(len(tree)):
             tree[i][dim, sub_idx] += value - old
```

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/_utils/RandDict.py` & `ReplayTables-andnp-2.5.0/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/_utils/SumTree.py` & `ReplayTables-andnp-2.5.0/ReplayTables/_utils/SumTree.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 from numba.typed import List as NList
 from ReplayTables._utils.jit import try2jit, try2vectorize
 from ReplayTables._utils.MemoryWriter import MemoryWriter, ThreadedWriter
 
 W = Optional[np.ndarray]
 
 
-@try2jit
+@try2jit()
 def _nearestPowerOf2(x: float):
     i = np.log2(x)
     u = np.ceil(i)
     return int(2**u)
 
-@try2jit
+@try2jit()
 def _update(tree: NList[np.ndarray], dim: int, idxs: np.ndarray, values: np.ndarray):
     for idx, value in zip(idxs, values):
         sub_idx = idx
         old = tree[0][dim, idx]
 
         for i in range(len(tree)):
             tree[i][dim, sub_idx] += value - old
             sub_idx = int(sub_idx // 2)
 
 @try2vectorize
 def _bound(x: int, ma: int):
     return min(x, ma)
 
-@try2jit
+@try2jit()
 def _query(tree: NList[np.ndarray], size: int, weights: np.ndarray, values: np.ndarray):
     totals = np.zeros(len(values))
     idxs = np.zeros(len(values), dtype=np.int64)
     for i in range(len(tree) - 2, -1, -1):
         layer = tree[i]
 
         idxs = idxs * 2
@@ -122,14 +122,14 @@
         }
 
     def __setstate__(self, state):
         self.__init__(state['size'], state['dims'], _defer_build=True)
         self._tree = NList(state['memory'])
         self._writer._mem = self._tree
 
-@try2jit
+@try2jit()
 def _safe_invert(arr: np.ndarray):
     out = np.empty_like(arr)
     for i in range(len(arr)):
         out[i] = 0 if arr[i] == 0 else 1 / arr[i]
 
     return out
```

### Comparing `ReplayTables-andnp-2.4.0/ReplayTables/_utils/jit.py` & `ReplayTables-andnp-2.5.0/ReplayTables/_utils/jit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import logging
 from typing import Any, Callable, TypeVar, Protocol, cast
 import numpy.typing as npt
 
 _has_warned = False
 T = TypeVar('T', bound=Callable[..., Any])
 
-def try2jit(f: T) -> T:
-    try:
-        from numba import njit
-        return njit(f, cache=True, nogil=True, fastmath=True)
-    except Exception:
-        global _has_warned
-        if not _has_warned:
-            _has_warned = True
-            logging.getLogger('ReplayTables').warn('Could not jit compile --- expect slow performance')
+def try2jit(fastmath: bool = True, inline: Any = 'never'):
+    def _inner(f: T) -> T:
+        try:
+            from numba import njit
+            return njit(f, cache=True, nogil=True, fastmath=fastmath, inline=inline)
+        except Exception:
+            global _has_warned
+            if not _has_warned:
+                _has_warned = True
+                logging.getLogger('ReplayTables').warn('Could not jit compile --- expect slow performance')
 
-        return f
+            return f
+
+    return _inner
 
 
 class Vectorized(Protocol):
     def __call__(self, *args: npt.ArrayLike) -> npt.ArrayLike:
         ...
 
 def try2vectorize(f: Any) -> Vectorized:
```

### Comparing `ReplayTables-andnp-2.4.0/pyproject.toml` & `ReplayTables-andnp-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.4.0"
+version = "2.5.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -22,15 +22,15 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "ReplayTables-andnp"
-version = "2.4.0"
+version = "2.5.0"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.56.4",
     "numpy>=1.23.5",
```

### Comparing `ReplayTables-andnp-2.4.0/tests/test_LagBuffer.py` & `ReplayTables-andnp-2.5.0/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/tests/test_PER.py` & `ReplayTables-andnp-2.5.0/tests/test_PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/tests/test_ReplayBuffer.py` & `ReplayTables-andnp-2.5.0/tests/test_ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/tests/test_Table.py` & `ReplayTables-andnp-2.5.0/tests/test_Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/tests/test_View.py` & `ReplayTables-andnp-2.5.0/tests/test_View.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-2.4.0/tests/utils/test_SumTree.py` & `ReplayTables-andnp-2.5.0/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

