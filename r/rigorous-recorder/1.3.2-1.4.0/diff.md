# Comparing `tmp/rigorous_recorder-1.3.2.tar.gz` & `tmp/rigorous_recorder-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigorous_recorder-1.3.2.tar", last modified: Wed Apr 12 13:57:53 2023, max compression
+gzip compressed data, was "rigorous_recorder-1.4.0.tar", last modified: Mon Apr 24 14:15:45 2023, max compression
```

## Comparing `rigorous_recorder-1.3.2.tar` & `rigorous_recorder-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:57:53.680174 rigorous_recorder-1.3.2/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:57:53.680045 rigorous_recorder-1.3.2/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:57:53.679099 rigorous_recorder-1.3.2/rigorous_recorder/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       36 2023-03-19 13:33:17.000000 rigorous_recorder-1.3.2/rigorous_recorder/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    34494 2023-04-12 13:57:30.000000 rigorous_recorder-1.3.2/rigorous_recorder/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-12 13:57:53.679861 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      268 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       59 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-04-12 13:57:53.000000 rigorous_recorder-1.3.2/rigorous_recorder.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-12 13:57:53.680215 rigorous_recorder-1.3.2/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-03-19 13:50:47.000000 rigorous_recorder-1.3.2/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 14:15:45.533557 rigorous_recorder-1.4.0/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-24 14:15:45.533414 rigorous_recorder-1.4.0/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 14:15:45.532658 rigorous_recorder-1.4.0/rigorous_recorder/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       36 2023-03-19 13:33:17.000000 rigorous_recorder-1.4.0/rigorous_recorder/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    35695 2023-04-24 14:13:02.000000 rigorous_recorder-1.4.0/rigorous_recorder/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 14:15:45.533182 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-04-24 14:15:45.000000 rigorous_recorder-1.4.0/rigorous_recorder.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 14:15:45.533597 rigorous_recorder-1.4.0/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1104 2023-04-24 13:58:53.000000 rigorous_recorder-1.4.0/setup.py
```

### Comparing `rigorous_recorder-1.3.2/PKG-INFO` & `rigorous_recorder-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous_recorder
-Version: 1.3.2
+Version: 1.4.0
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `rigorous_recorder-1.3.2/rigorous_recorder/main.py` & `rigorous_recorder-1.4.0/rigorous_recorder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time as now
 from random import random
 import json
 
-import file_system_py as FS
-from super_map import LazyDict
-from super_hash import super_hash
+from .__dependencies__ import file_system_py as FS
+from .__dependencies__.super_map import LazyDict
+from .__dependencies__.super_hash import super_hash
 
 # TODO:
     # have each experiment be given their own pickle file
 
 # 
 # helpers
 # 
@@ -157,19 +157,36 @@
     
     def __setstate__(self, state):
         self.itself, self.ancestors = state
     
     def __json__(self):
         return self.compressed
 
+    def __deep_copy__(self, memo={}):
+        from copy import deepcopy
+        if id(self) in memo:
+            return memo[id(self)]
+        
+        new_itself = {}
+        the_copy = AncestorDict(
+            ancestors=list(self.ancestors),
+            itself=new_itself,
+        )
+        memo[id(self)] = the_copy
+        # cant call deepcopy until id(self) is added to the memo
+        for each_key, each_value in self.itself.items():
+            new_itself[each_key] = deepcopy(each_value, memo)
+        
+        return the_copy
+
 class AncestorMask(dict):
     def __init__(self, *, ancestors, index, frame):
         self.ancestors = ancestors
         if not isinstance(self.ancestors, (list, tuple)):
-            raise Exception('for AncestorDict(), ancestors needs to be a dict')
+            raise Exception('for AncestorDict(), ancestors needs to be a list or tuple')
         if type(frame) != dict:
             raise Exception('for AncestorDict(), frame needs to be a pure dict')
         self.frame = frame
         self.index = index
     
     @property
     def itself(self):
@@ -280,14 +297,33 @@
         return self.index, self.frame, self.ancestors
     
     def __setstate__(self, state):
         self.index, self.frame, self.ancestors = state
     
     def __json__(self):
         return self.compressed
+        
+    def __deep_copy__(self, memo={}):
+        from copy import deepcopy
+        self_id = id(self)
+        if self_id in memo:
+            return memo[self_id]
+        
+        new_frame = {}
+        the_copy = AncestorMask(
+            ancestors=list(self.ancestors),
+            index=self.index,
+            frame=new_frame,
+        )
+        memo[self_id] = the_copy
+        # cant call deepcopy until id(self) is added to the memo
+        for each_key, each_value in self.frame.items():
+            new_frame[each_key] = deepcopy(each_value, memo)
+        
+        return the_copy
 
 class Recorder():
     @classmethod
     def load_from(self, path):
         return large_pickle_load(path)
     
     def __init__(self, data=None, **kwargs):
```

### Comparing `rigorous_recorder-1.3.2/rigorous_recorder.egg-info/PKG-INFO` & `rigorous_recorder-1.4.0/rigorous_recorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous-recorder
-Version: 1.3.2
+Version: 1.4.0
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

