# Comparing `tmp/aamaze-0.3.1.tar.gz` & `tmp/aamaze-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aamaze-0.3.1.tar", max compression
+gzip compressed data, was "aamaze-0.3.2.tar", max compression
```

## Comparing `aamaze-0.3.1.tar` & `aamaze-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      186 2023-04-03 07:43:57.148079 aamaze-0.3.1/aamaze/__init__.py
--rw-r--r--   0        0        0     8177 2023-03-23 09:20:21.587036 aamaze-0.3.1/aamaze/base_maze.py
--rw-r--r--   0        0        0      260 2023-03-31 18:07:30.949375 aamaze-0.3.1/aamaze/generation/__init__.py
--rw-r--r--   0        0        0     4124 2023-03-31 18:05:40.713952 aamaze-0.3.1/aamaze/generation/eller.py
--rw-r--r--   0        0        0     2807 2023-04-24 07:12:39.837365 aamaze-0.3.1/aamaze/generation/growing_tree.py
--rw-r--r--   0        0        0     3288 2023-03-31 18:05:38.606297 aamaze-0.3.1/aamaze/generation/kruskals.py
--rw-r--r--   0        0        0     2014 2023-03-31 18:05:37.271506 aamaze-0.3.1/aamaze/generation/prims.py
--rw-r--r--   0        0        0     1483 2023-03-31 18:05:26.549723 aamaze-0.3.1/aamaze/generation/recursive_backtracker.py
--rw-r--r--   0        0        0     2216 2023-03-31 18:05:33.456326 aamaze-0.3.1/aamaze/generation/recursive_divisior.py
--rw-r--r--   0        0        0     3699 2023-03-31 18:07:31.882718 aamaze-0.3.1/aamaze/generation/wilsons.py
--rw-r--r--   0        0        0      160 2023-03-30 12:11:36.991366 aamaze-0.3.1/aamaze/graphics/__init__.py
--rw-r--r--   0        0        0     8879 2023-04-17 06:44:13.978585 aamaze-0.3.1/aamaze/graphics/app.py
--rw-r--r--   0        0        0      763 2023-03-30 12:07:47.044163 aamaze-0.3.1/aamaze/graphics/defaults.py
--rw-r--r--   0        0        0     7494 2023-03-30 12:27:00.782446 aamaze-0.3.1/aamaze/graphics/draw_maze.py
--rw-r--r--   0        0        0      119 2023-03-31 18:08:58.935015 aamaze-0.3.1/aamaze/solving/__init__.py
--rw-r--r--   0        0        0     4686 2023-03-31 18:08:49.792390 aamaze-0.3.1/aamaze/solving/a_star.py
--rw-r--r--   0        0        0     3620 2023-03-31 18:08:59.816974 aamaze-0.3.1/aamaze/solving/dijkstra.py
--rw-r--r--   0        0        0     2297 2023-03-31 18:09:18.754733 aamaze-0.3.1/aamaze/solving/flood_fill.py
--rw-r--r--   0        0        0     1101 2023-03-31 13:19:38.969419 aamaze-0.3.1/LICENSE
--rw-r--r--   0        0        0      587 2023-03-31 13:50:32.610572 aamaze-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3657 2023-04-10 08:26:02.253903 aamaze-0.3.1/README.md
--rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 aamaze-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-04-03 07:43:57.148079 aamaze-0.3.2/aamaze/__init__.py
+-rw-r--r--   0        0        0     8177 2023-03-23 09:20:21.587036 aamaze-0.3.2/aamaze/base_maze.py
+-rw-r--r--   0        0        0      260 2023-03-31 18:07:30.949375 aamaze-0.3.2/aamaze/generation/__init__.py
+-rw-r--r--   0        0        0     4124 2023-03-31 18:05:40.713952 aamaze-0.3.2/aamaze/generation/eller.py
+-rw-r--r--   0        0        0     2807 2023-04-24 07:12:39.837365 aamaze-0.3.2/aamaze/generation/growing_tree.py
+-rw-r--r--   0        0        0     3288 2023-03-31 18:05:38.606297 aamaze-0.3.2/aamaze/generation/kruskals.py
+-rw-r--r--   0        0        0     2014 2023-03-31 18:05:37.271506 aamaze-0.3.2/aamaze/generation/prims.py
+-rw-r--r--   0        0        0     1483 2023-03-31 18:05:26.549723 aamaze-0.3.2/aamaze/generation/recursive_backtracker.py
+-rw-r--r--   0        0        0     2216 2023-03-31 18:05:33.456326 aamaze-0.3.2/aamaze/generation/recursive_divisior.py
+-rw-r--r--   0        0        0     3699 2023-03-31 18:07:31.882718 aamaze-0.3.2/aamaze/generation/wilsons.py
+-rw-r--r--   0        0        0      160 2023-03-30 12:11:36.991366 aamaze-0.3.2/aamaze/graphics/__init__.py
+-rw-r--r--   0        0        0     8879 2023-04-17 06:44:13.978585 aamaze-0.3.2/aamaze/graphics/app.py
+-rw-r--r--   0        0        0      763 2023-03-30 12:07:47.044163 aamaze-0.3.2/aamaze/graphics/defaults.py
+-rw-r--r--   0        0        0     7494 2023-03-30 12:27:00.782446 aamaze-0.3.2/aamaze/graphics/draw_maze.py
+-rw-r--r--   0        0        0      119 2023-03-31 18:08:58.935015 aamaze-0.3.2/aamaze/solving/__init__.py
+-rw-r--r--   0        0        0     4686 2023-03-31 18:08:49.792390 aamaze-0.3.2/aamaze/solving/a_star.py
+-rw-r--r--   0        0        0     3620 2023-03-31 18:08:59.816974 aamaze-0.3.2/aamaze/solving/dijkstra.py
+-rw-r--r--   0        0        0     2297 2023-03-31 18:09:18.754733 aamaze-0.3.2/aamaze/solving/flood_fill.py
+-rw-r--r--   0        0        0     1101 2023-03-31 13:19:38.969419 aamaze-0.3.2/LICENSE
+-rw-r--r--   0        0        0      587 2023-04-24 07:59:58.594156 aamaze-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9877 2023-04-24 07:59:29.336298 aamaze-0.3.2/README.md
+-rw-r--r--   0        0        0    10342 1970-01-01 00:00:00.000000 aamaze-0.3.2/PKG-INFO
```

### Comparing `aamaze-0.3.1/aamaze/base_maze.py` & `aamaze-0.3.2/aamaze/base_maze.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/generation/eller.py` & `aamaze-0.3.2/aamaze/generation/eller.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/generation/growing_tree.py` & `aamaze-0.3.2/aamaze/generation/growing_tree.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/generation/kruskals.py` & `aamaze-0.3.2/aamaze/generation/kruskals.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/generation/prims.py` & `aamaze-0.3.2/aamaze/generation/prims.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/generation/recursive_backtracker.py` & `aamaze-0.3.2/aamaze/generation/recursive_backtracker.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/generation/recursive_divisior.py` & `aamaze-0.3.2/aamaze/generation/recursive_divisior.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/generation/wilsons.py` & `aamaze-0.3.2/aamaze/generation/wilsons.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/graphics/app.py` & `aamaze-0.3.2/aamaze/graphics/app.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/graphics/defaults.py` & `aamaze-0.3.2/aamaze/graphics/defaults.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/graphics/draw_maze.py` & `aamaze-0.3.2/aamaze/graphics/draw_maze.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/solving/a_star.py` & `aamaze-0.3.2/aamaze/solving/a_star.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/solving/dijkstra.py` & `aamaze-0.3.2/aamaze/solving/dijkstra.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/aamaze/solving/flood_fill.py` & `aamaze-0.3.2/aamaze/solving/flood_fill.py`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/LICENSE` & `aamaze-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aamaze-0.3.1/pyproject.toml` & `aamaze-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aamaze"
-version = "0.3.1"
+version = "0.3.2"
 description = "A python package for generating, solving and displaying mazes."
 authors = ["aaFurze <aafurze@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aaFurze/aamaze"
 keywords = ["maze", "algorithm", "maze generation", "maze solution", "display", "draw"]
```

