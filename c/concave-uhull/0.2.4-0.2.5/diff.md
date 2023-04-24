# Comparing `tmp/concave_uhull-0.2.4.tar.gz` & `tmp/concave_uhull-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concave_uhull-0.2.4.tar", max compression
+gzip compressed data, was "concave_uhull-0.2.5.tar", max compression
```

## Comparing `concave_uhull-0.2.4.tar` & `concave_uhull-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      321 2023-02-13 23:11:05.234480 concave_uhull-0.2.4/README_pypi.rst
--rw-r--r--   0        0        0        0 2023-02-08 19:07:35.341531 concave_uhull-0.2.4/concave_uhull/__init__.py
--rw-r--r--   0        0        0    12270 2023-02-13 23:04:04.725445 concave_uhull-0.2.4/concave_uhull/alpha_shape.py
--rw-r--r--   0        0        0     3706 2023-02-08 19:07:35.341531 concave_uhull-0.2.4/concave_uhull/geometry.py
--rw-r--r--   0        0        0     7571 2023-02-08 19:07:35.341531 concave_uhull-0.2.4/concave_uhull/graph.py
--rw-r--r--   0        0        0      835 2023-02-13 23:12:10.494693 concave_uhull-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 concave_uhull-0.2.4/setup.py
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 concave_uhull-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      321 2023-02-13 23:11:05.234480 concave_uhull-0.2.5/README_pypi.rst
+-rw-r--r--   0        0        0        0 2023-02-08 19:07:35.341531 concave_uhull-0.2.5/concave_uhull/__init__.py
+-rw-r--r--   0        0        0    12270 2023-02-14 14:11:00.923949 concave_uhull-0.2.5/concave_uhull/alpha_shape.py
+-rw-r--r--   0        0        0     3706 2023-02-08 19:07:35.341531 concave_uhull-0.2.5/concave_uhull/geometry.py
+-rw-r--r--   0        0        0     7621 2023-04-24 15:42:23.043369 concave_uhull-0.2.5/concave_uhull/graph.py
+-rw-r--r--   0        0        0      835 2023-04-24 17:56:42.423275 concave_uhull-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 concave_uhull-0.2.5/setup.py
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 concave_uhull-0.2.5/PKG-INFO
```

### Comparing `concave_uhull-0.2.4/concave_uhull/alpha_shape.py` & `concave_uhull-0.2.5/concave_uhull/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `concave_uhull-0.2.4/concave_uhull/geometry.py` & `concave_uhull-0.2.5/concave_uhull/geometry.py`

 * *Files identical despite different names*

### Comparing `concave_uhull-0.2.4/concave_uhull/graph.py` & `concave_uhull-0.2.5/concave_uhull/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,16 @@
     }
     heap: List = [(distance[edge_source], edge_source)]
     predecessors: Dict = dict()
     while heap:
         distance_node, node = heappop(heap)
         if node == edge_target:
             break
+        if node in explored:
+            continue
         explored.add(node)
         for neighbor in graph[node]:
             distance_neighbor = distance_node + graph.weight[node][neighbor]
             if distance_neighbor < distance[neighbor]:
                 distance[neighbor] = distance_neighbor
                 heappush(heap, (distance[neighbor], neighbor))
                 predecessors[neighbor] = node
```

### Comparing `concave_uhull-0.2.4/pyproject.toml` & `concave_uhull-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "concave_uhull"
-version = "0.2.4"
+version = "0.2.5"
 description = "A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm."
 readme = "README_pypi.rst"
 authors = ["Luan <llvdmoraes@gmail.com>"]
 repository = "https://github.com/luanleonardo/concave_uhull"
 homepage = "https://luanleonardo.github.io/concave_uhull/"
 
 [tool.poetry.dependencies]
```

### Comparing `concave_uhull-0.2.4/setup.py` & `concave_uhull-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.1,<2.0.0', 'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'concave-uhull',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm.',
     'long_description': '==============\nConcave uhull*\n==============\n\nA simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm.\n\nNotes\n-----\n  * uhull! (Brazil) yeah! (expresses joy or celebration)\n\nHomepage\n========\n* `Project Homepage <https://luanleonardo.github.io/concave_uhull/>`_\n',
     'author': 'Luan',
     'author_email': 'llvdmoraes@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://luanleonardo.github.io/concave_uhull/',
```

### Comparing `concave_uhull-0.2.4/PKG-INFO` & `concave_uhull-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concave-uhull
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple (but not simpler) algorithm for concave hull of 2D point sets using an alpha shape algorithm.
 Home-page: https://luanleonardo.github.io/concave_uhull/
 Author: Luan
 Author-email: llvdmoraes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

