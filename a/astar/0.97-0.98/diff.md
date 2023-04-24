# Comparing `tmp/astar-0.97-py3-none-any.whl.zip` & `tmp/astar-0.98-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 7025 bytes, number of entries: 5
--rw-r--r--  2.0 unx     8774 b- defN 80-Jan-01 00:00 astar/__init__.py
--rw-r--r--  2.0 unx     1496 b- defN 80-Jan-01 00:00 astar-0.97.dist-info/LICENSE
--rw-r--r--  2.0 unx     8619 b- defN 80-Jan-01 00:00 astar-0.97.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 astar-0.97.dist-info/WHEEL
-?rw-r--r--  2.0 unx      356 b- defN 16-Jan-01 00:00 astar-0.97.dist-info/RECORD
-5 files, 19333 bytes uncompressed, 6369 bytes compressed:  67.1%
+Zip file size: 6615 bytes, number of entries: 6
+-rw-r--r--  2.0 fat     6537 b- defN 80-Jan-01 00:00 astar/__init__.py
+-rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 astar/py.typed
+-rw-r--r--  2.0 fat     1496 b- defN 80-Jan-01 00:00 astar-0.98.dist-info/LICENSE
+-rw-r--r--  2.0 fat     8619 b- defN 80-Jan-01 00:00 astar-0.98.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 astar-0.98.dist-info/WHEEL
+?rw-r--r--  2.0 fat      424 b- defN 16-Jan-01 00:00 astar-0.98.dist-info/RECORD
+6 files, 17164 bytes uncompressed, 5855 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
 Filename: astar/__init__.py
 Comment: 
 
-Filename: astar-0.97.dist-info/LICENSE
+Filename: astar/py.typed
 Comment: 
 
-Filename: astar-0.97.dist-info/METADATA
+Filename: astar-0.98.dist-info/LICENSE
 Comment: 
 
-Filename: astar-0.97.dist-info/WHEEL
+Filename: astar-0.98.dist-info/METADATA
 Comment: 
 
-Filename: astar-0.97.dist-info/RECORD
+Filename: astar-0.98.dist-info/WHEEL
+Comment: 
+
+Filename: astar-0.98.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## astar/__init__.py

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 """ generic A-Star path searching algorithm """
 
-import logging
 from abc import ABC, abstractmethod
-from heapq import heapify, heappush, heappop
-from typing import Type, Callable, Dict, Iterable, Union, TypeVar, Generic
+from typing import Callable, Dict, Iterable, Union, TypeVar, Generic
 from math import inf as infinity
+import sortedcontainers # type: ignore
 
 # introduce generic type
 T = TypeVar("T")
 
 
 ################################################################################
 class SearchNode(Generic[T]):
@@ -42,76 +41,15 @@
         return v
 
 
 ################################################################################
 SNType = TypeVar("SNType", bound=SearchNode)
 
 
-class OpenSet(ABC, Generic[SNType]):
-    """As we may have performance issues with the heapq module when an item is
-    re-inserted, we may use other implementations for this feature.
-
-     - By default the HeapQOpenSet class just relies on the heapq module, it does not need any external dependency.
-
-     - The SortedContainersOpenSet class uses the sortedcointainers module. As
-       this module is optional, it will be used only if your own project
-       depends on it.
-
-    """
-
-    @abstractmethod
-    def push(self, item: SNType) -> None:
-        """Add an item to the queue"""
-        raise NotImplementedError
-
-    @abstractmethod
-    def pop(self) -> SNType:
-        """Remove and return the smallest item from the queue"""
-        raise NotImplementedError
-
-    @abstractmethod
-    def remove(self, item: SNType) -> None:
-        """remove an item from the queue, ensuring that the queue is still valid afterwards"""
-        raise NotImplementedError
-
-
-################################################################################
-class HeapQOpenSet(OpenSet[SNType], Generic[SNType]):
-    """just a wrapper around heapq operations"""
-
-    def __init__(self):
-        self.heap = []
-        heapify(self.heap)
-
-    def push(self, item: SNType) -> None:
-        """Add an item to the queue"""
-        item.in_openset = True
-        heappush(self.heap, item)
-
-    def pop(self) -> SNType:
-        """Remove and return the smallest item from the queue"""
-        item = heappop(self.heap)
-        item.in_openset = False
-        return item
-
-    def remove(self, item: SNType):
-        self.heap.remove(item)
-        heapify(
-            self.heap
-        )  # costly operation but necessary as remove operation destroy the structure of the heap
-        item.in_openset = False
-
-
-################################################################################
-OpenSetImpl: Type[OpenSet] = HeapQOpenSet
-
-try:
-    import sortedcontainers
-
-    class SortedContainersOpenSet(OpenSet[SNType], Generic[SNType]):
+class OpenSet(Generic[SNType]):
         def __init__(self):
             self.sortedlist = sortedcontainers.SortedList(key=lambda x: x.fscore)
 
         def push(self, item: SNType) -> None:
             item.in_openset = True
             self.sortedlist.add(item)
 
@@ -120,24 +58,16 @@
             item.in_openset = False
             return item
 
         def remove(self, item: SNType):
             self.sortedlist.remove(item)
             item.in_openset = False
 
-    OpenSetImpl = SortedContainersOpenSet
-    logging.info("using sortedcontainers for heap operations")
-
-except Exception as e:
-    logging.info("sortedcontainers module not loaded, using the default heapq module")
-
-
 ################################################################################*
 
-
 class AStar(ABC, Generic[T]):
     __slots__ = ()
 
     @abstractmethod
     def heuristic_cost_estimate(self, current: T, goal: T) -> float:
         """
         Computes the estimated (rough) distance between a node and the goal.
@@ -185,15 +115,15 @@
 
     def astar(
         self, start: T, goal: T, reversePath: bool = False
     ) -> Union[Iterable[T], None]:
         if self.is_goal_reached(start, goal):
             return [start]
 
-        openSet: OpenSet[SearchNode[T]] = OpenSetImpl()
+        openSet: OpenSet[SearchNode[T]] = OpenSet()
         searchNodes: SearchNodeDict[T] = SearchNodeDict()
         startNode = searchNodes[start] = SearchNode(
             start, gscore=0.0, fscore=self.heuristic_cost_estimate(start, goal)
         )
         openSet.push(startNode)
 
         while openSet:
```

## Comparing `astar-0.97.dist-info/LICENSE` & `astar-0.98.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `astar-0.97.dist-info/METADATA` & `astar-0.98.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astar
-Version: 0.97
+Version: 0.98
 Summary: generic A-Star path searching algorithm
 Home-page: https://github.com/jrialland/python-astar
 License: BSD
 Author: J Rialland
 Author-email: julien.rialland@gmail.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: Intended Audience :: Developers
```

