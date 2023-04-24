# Comparing `tmp/fstflowchat-0.0.2.tar.gz` & `tmp/fstflowchat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstflowchat-0.0.2.tar", last modified: Mon Apr 24 01:32:01 2023, max compression
+gzip compressed data, was "fstflowchat-0.0.3.tar", last modified: Mon Apr 24 01:51:25 2023, max compression
```

## Comparing `fstflowchat-0.0.2.tar` & `fstflowchat-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:32:01.645805 fstflowchat-0.0.2/
--rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.2/LICENSE
--rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.2/MANIFEST.in
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-04-24 01:32:01.645033 fstflowchat-0.0.2/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)     1473 2023-04-24 00:59:35.000000 fstflowchat-0.0.2/README.md
--rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-04-24 01:32:01.645983 fstflowchat-0.0.2/setup.cfg
--rwxr-xr-x   0 kaze7539   (503) staff       (20)     8191 2023-04-24 01:31:41.000000 fstflowchat-0.0.2/setup.py
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:32:01.496198 fstflowchat-0.0.2/src/
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:32:01.587731 fstflowchat-0.0.2/src/fstflowchat/
--rw-r--r--   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:05:43.000000 fstflowchat-0.0.2/src/fstflowchat/__init__.py
--rw-r--r--   0 kaze7539   (503) staff       (20)     7120 2023-04-24 00:06:37.000000 fstflowchat-0.0.2/src/fstflowchat/example.py
--rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.2/src/fstflowchat/quiz.dot
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:32:01.643792 fstflowchat-0.0.2/src/fstflowchat.egg-info/
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-04-24 01:32:01.000000 fstflowchat-0.0.2/src/fstflowchat.egg-info/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-04-24 01:32:01.000000 fstflowchat-0.0.2/src/fstflowchat.egg-info/SOURCES.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-04-24 01:32:01.000000 fstflowchat-0.0.2/src/fstflowchat.egg-info/dependency_links.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-04-24 01:32:01.000000 fstflowchat-0.0.2/src/fstflowchat.egg-info/entry_points.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       11 2023-04-24 01:32:01.000000 fstflowchat-0.0.2/src/fstflowchat.egg-info/requires.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-04-24 01:32:01.000000 fstflowchat-0.0.2/src/fstflowchat.egg-info/top_level.txt
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.436050 fstflowchat-0.0.3/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.3/LICENSE
+-rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.3/MANIFEST.in
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-04-24 01:51:25.435694 fstflowchat-0.0.3/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1473 2023-04-24 00:59:35.000000 fstflowchat-0.0.3/README.md
+-rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-04-24 01:51:25.436110 fstflowchat-0.0.3/setup.cfg
+-rwxr-xr-x   0 kaze7539   (503) staff       (20)     8191 2023-04-24 01:43:27.000000 fstflowchat-0.0.3/setup.py
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.418104 fstflowchat-0.0.3/src/
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.427195 fstflowchat-0.0.3/src/fstflowchat/
+-rw-r--r--   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:05:43.000000 fstflowchat-0.0.3/src/fstflowchat/__init__.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.3/src/fstflowchat/example.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.3/src/fstflowchat/quiz.dot
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-04-24 01:51:25.435243 fstflowchat-0.0.3/src/fstflowchat.egg-info/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/entry_points.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       11 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/requires.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-04-24 01:51:25.000000 fstflowchat-0.0.3/src/fstflowchat.egg-info/top_level.txt
```

### Comparing `fstflowchat-0.0.2/LICENSE` & `fstflowchat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.2/PKG-INFO` & `fstflowchat-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.2
+Version: 0.0.3
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

### Comparing `fstflowchat-0.0.2/README.md` & `fstflowchat-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.2/setup.py` & `fstflowchat-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.2",  # Required
+    version="0.0.3",  # Required
     
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="a small, pedagogical, fst-based dialog toolkit.",  # Optional
     
     # This is an optional longer description of your project that represents
```

### Comparing `fstflowchat-0.0.2/src/fstflowchat/example.py` & `fstflowchat-0.0.3/src/fstflowchat/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import random
 import sys
 import pygraphviz as pgv
+import pathlib
+
 
 
 def get_graph_functions(g: pgv.agraph.AGraph):
     """gets a list of the names of the functions referred to in the
     graph's edges
     """
     fnames_out = []
@@ -204,15 +206,16 @@
 # set up the correct answer counts
 correct_count = 0
 partial_count = 0
                               
 def main():
     # read graph
     try:
-        graph = pgv.AGraph("quiz.dot")
+        here = pathlib.Path(__file__).parent.resolve()
+        graph = pgv.AGraph((here / "quiz.dot"))
     except IndexError:
         print("need to give the name of a dot file graph as input",
               file=sys.stderr)
         exit(-1)
         
     # check if the graph is fully implemented
     fully_implemented = True
```

### Comparing `fstflowchat-0.0.2/src/fstflowchat/quiz.dot` & `fstflowchat-0.0.3/src/fstflowchat/quiz.dot`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.2/src/fstflowchat.egg-info/PKG-INFO` & `fstflowchat-0.0.3/src/fstflowchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.2
+Version: 0.0.3
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

