# Comparing `tmp/bw2analyzer-0.9.dev4.tar.gz` & `tmp/bw2analyzer-0.9.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bw2analyzer-0.9.dev4.tar", last modified: Wed Dec  9 12:48:39 2015, max compression
+gzip compressed data, was "dist/bw2analyzer-0.9.dev5.tar", last modified: Fri Dec 11 15:19:41 2015, max compression
```

## Comparing `bw2analyzer-0.9.dev4.tar` & `bw2analyzer-0.9.dev5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/
--rw-r--r--   0 cmutel     (501) staff       (20)      101 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev4/.hgignore
--rw-r--r--   0 cmutel     (501) staff       (20)      571 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/.hgtags
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer/
--rw-r--r--   0 cmutel     (501) staff       (20)      452 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/bw2analyzer/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8948 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/bw2analyzer/contribution.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2475 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/econ.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1095 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/explorer.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6208 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/health_check.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2306 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/bw2analyzer/lookup.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3658 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/matrix_grapher.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3093 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/bw2analyzer/page_rank.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6181 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/bw2analyzer/report.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9621 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/sc_graph.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)      343 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3335 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/contribution.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1790 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/econ.py
--rw-r--r--   0 cmutel     (501) staff       (20)      717 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/fixtures.py
--rw-r--r--   0 cmutel     (501) staff       (20)      636 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/health_check.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1069 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/matrix_grapher.py
--rw-r--r--   0 cmutel     (501) staff       (20)    17458 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/sc_graph.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3533 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev4/bw2analyzer/tests/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4110 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/bw2analyzer/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)     2909 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)       42 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      844 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       12 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/bw2analyzer.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      957 2015-03-09 12:17:57.000000 bw2analyzer-0.9.dev4/CHANGES.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     7823 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev4/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)      128 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev4/docs/index.rst
--rw-r--r--   0 cmutel     (501) staff       (20)     5106 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev4/docs/make.bat
--rw-r--r--   0 cmutel     (501) staff       (20)     5584 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev4/docs/Makefile
--rw-r--r--   0 cmutel     (501) staff       (20)     1493 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev4/LICENSE.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       88 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev4/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     2909 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      385 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev4/README.rst
--rw-r--r--   0 cmutel     (501) staff       (20)      164 2015-03-09 12:17:57.000000 bw2analyzer-0.9.dev4/requirements.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       59 2015-12-09 12:48:39.000000 bw2analyzer-0.9.dev4/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     1246 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev4/setup.py
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev4/TODO.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/
+-rw-r--r--   0 cmutel     (501) staff       (20)      101 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev5/.hgignore
+-rw-r--r--   0 cmutel     (501) staff       (20)      621 2015-12-11 15:19:25.000000 bw2analyzer-0.9.dev5/.hgtags
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer/
+-rw-r--r--   0 cmutel     (501) staff       (20)      452 2015-12-11 15:18:59.000000 bw2analyzer-0.9.dev5/bw2analyzer/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8948 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev5/bw2analyzer/contribution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2475 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/econ.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1095 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/explorer.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6208 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/health_check.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2306 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev5/bw2analyzer/lookup.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3658 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/matrix_grapher.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3093 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev5/bw2analyzer/page_rank.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6271 2015-12-11 09:43:43.000000 bw2analyzer-0.9.dev5/bw2analyzer/report.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9419 2015-12-11 09:25:13.000000 bw2analyzer-0.9.dev5/bw2analyzer/sc_graph.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)      343 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3335 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/contribution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1790 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/econ.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      717 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/fixtures.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      636 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/health_check.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1069 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/matrix_grapher.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    17432 2015-12-11 09:26:37.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/sc_graph.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3533 2015-10-28 09:02:53.000000 bw2analyzer-0.9.dev5/bw2analyzer/tests/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4110 2015-11-09 08:34:09.000000 bw2analyzer-0.9.dev5/bw2analyzer/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     2909 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)       42 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      844 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       12 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/bw2analyzer.egg-info/top_level.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      957 2015-03-09 12:17:57.000000 bw2analyzer-0.9.dev5/CHANGES.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     7823 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev5/docs/conf.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      128 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev5/docs/index.rst
+-rw-r--r--   0 cmutel     (501) staff       (20)     5106 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev5/docs/make.bat
+-rw-r--r--   0 cmutel     (501) staff       (20)     5584 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev5/docs/Makefile
+-rw-r--r--   0 cmutel     (501) staff       (20)     1493 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev5/LICENSE.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       88 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev5/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     2909 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      385 2014-07-11 12:20:23.000000 bw2analyzer-0.9.dev5/README.rst
+-rw-r--r--   0 cmutel     (501) staff       (20)      164 2015-03-09 12:17:57.000000 bw2analyzer-0.9.dev5/requirements.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2015-12-11 15:19:41.000000 bw2analyzer-0.9.dev5/setup.cfg
+-rw-r--r--   0 cmutel     (501) staff       (20)     1246 2015-12-11 15:19:10.000000 bw2analyzer-0.9.dev5/setup.py
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2014-08-28 16:23:37.000000 bw2analyzer-0.9.dev5/TODO.txt
```

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/contribution.py` & `bw2analyzer-0.9.dev5/bw2analyzer/contribution.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/econ.py` & `bw2analyzer-0.9.dev5/bw2analyzer/econ.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/explorer.py` & `bw2analyzer-0.9.dev5/bw2analyzer/explorer.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/health_check.py` & `bw2analyzer-0.9.dev5/bw2analyzer/health_check.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/lookup.py` & `bw2analyzer-0.9.dev5/bw2analyzer/lookup.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/matrix_grapher.py` & `bw2analyzer-0.9.dev5/bw2analyzer/matrix_grapher.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/page_rank.py` & `bw2analyzer-0.9.dev5/bw2analyzer/page_rank.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/report.py` & `bw2analyzer-0.9.dev5/bw2analyzer/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, unicode_literals, division
 from eight import *
 
 from .contribution import ContributionAnalysis
 from .econ import herfindahl_index, concentration_ratio
 from .sc_graph import GTManipulator
-from brightway2 import JsonWrapper, methods, config, projects
+from brightway2 import JsonWrapper, methods, config, projects, get_activity
 from bw2calc import ParallelMonteCarlo, LCA, GraphTraversal
 from scipy.stats import gaussian_kde
 import numpy as np
 import os
 import requests
 import uuid
 
@@ -45,17 +45,21 @@
         print("herfindahl")
         herfindahl = herfindahl_index(lca.characterized_inventory.data)
         print("concentration")
         concentration = concentration_ratio(lca.characterized_inventory.data)
         print("MC:")
         monte_carlo = self.get_monte_carlo()
 
+        activity_data = []
+        for k, v in self.activity.items():
+            obj = get_activity(k)
+            activity_data.append((obj['name'], "%.2g" % v, obj['unit']))
+
         self.report = {
-            "activity": [(ca.get_name(k), "%.2g" % v, ca.db_names[k[0]][k][
-                "unit"]) for k, v in self.activity.iteritems()],
+            "activity": activity_data,
             "method": {
                 "name": ": ".join(self.method),
                 "unit": methods[self.method]["unit"]
                 },
             "score": float(lca.score),
             "contribution": {
                 "hinton": hinton,
```

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/sc_graph.py` & `bw2analyzer-0.9.dev5/bw2analyzer/sc_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,14 @@
 
 
 def tupify(o):
     """Transform edge from dict to tuples. Multiply impact by -1 because sort by min, not max"""
     return (-1 * o['impact'], o['from'], o['to'], o['amount'], o['exc_amount'])
 
 
-def iteritems(dct):
-    """Py2 & 3 compatible iteration of key/value pairs in dict"""
-    try:
-        return dct.viewitems()
-    except AttributeError:
-        return dct.items()
-
-
 class GTManipulator(object):
     """Manipulate ``GraphTraversal`` results."""
     @staticmethod
     def unroll_graph(nodes, edges, score, cutoff=0.005, max_links=2500):
         """Unroll a ``GraphTraversal`` result, allowing the same activity to appear in the graph multiple times."""
         input_nodes, input_edges = copy.deepcopy(nodes), copy.deepcopy(edges)
         counter = itertools.count()
@@ -83,15 +75,15 @@
         return nodes, edges, links
 
     @staticmethod
     def add_metadata(nodes, lca):
         """Add metadata to nodes, like name, unit, and category."""
         ra, rp, rb = lca.reverse_dict()
         new_nodes = {}
-        for key, value in iteritems(nodes):
+        for key, value in nodes.items():
             new_value = copy.deepcopy(value)
             if key == -1:
                 new_value.update({
                     'name': "Functional unit",
                     'unit': "unit",
                     'categories': ["Functional unit"]
                 })
@@ -112,15 +104,15 @@
         return new_nodes
 
     @staticmethod
     def d3_force_directed(nodes, edges, score):
         """Reformat to D3 style, which is a list of nodes, and edge ids are node list indices."""
         # Sort node ids by highest cumulative score first
         node_ids = [x[1] for x in sorted(
-            [(v["cum"], k) for k, v in iteritems(nodes)])]
+            [(v["cum"], k) for k, v in nodes.items()])]
         new_nodes = [nodes[i] for i in node_ids]
         lookup = dict([(key, index) for index, key in enumerate(node_ids)])
         new_edges = [{
             "source": lookup[e["to"]],
             "target": lookup[e["from"]],
             "amount": e["impact"]
         } for e in edges]
@@ -134,19 +126,19 @@
     def simplify(nodes, edges, score, limit=0.005):
         """Simplify supply chain to include only nodes which individually contribute ``limit * score``.
 
         Only removes and combines edges; doesn't check to make sure amounts add up correctly."""
         if isinstance(limit, int) and limit > 1:
             nodes_to_delete = sorted([
                 (value['amount'] * value['ind'], key)
-                for key, value in iteritems(nodes)
+                for key, value in nodes.items()
                 ], reverse=True)[limit:]
         else:
             nodes_to_delete = [
-                key for key, value in iteritems(nodes)
+                key for key, value in nodes.items()
                 if key != -1
                 and (value['amount'] * value['ind']) < (score * limit)
             ]
         edges_dict = {(edge['to'], edge['from']): edge
             for edge in copy.deepcopy(edges)}
         for node in nodes_to_delete:
             p_edges = [key for key in edges_dict if key[1] == node]
@@ -176,69 +168,69 @@
                         'impact': e_impact
                     }
             # Remove obsolete edges
             for key in p_edges:
                 del edges_dict[key]
             for key in c_edges:
                 del edges_dict[key]
-        nodes = {key: value for key, value in iteritems(nodes)
+        nodes = {key: value for key, value in nodes.items()
             if key not in set(nodes_to_delete)}
         return nodes, edges_dict.values()
 
     @staticmethod
     def simplify_naive(nodes, edges, score, limit=0.0025):
         """Naive simplification which simplifies removes links below an LCA score cutoff. Orphan nodes are also deleted."""
         edges = [e for e in edges if e["impact"] >= (score * limit)]
         good_nodes = set([e["from"] for e in edges]).union(
             set([e["to"] for e in edges]))
-        nodes = dict([(k, v) for k, v in iteritems(nodes) if k in good_nodes])
+        nodes = dict([(k, v) for k, v in nodes.items() if k in good_nodes])
         return nodes, edges
 
     @staticmethod
     def d3_treemap(nodes, edges, lca, add_biosphere=False):
         """Add node data by traversing the graph; assign different metadata to leaf nodes."""
         ra, rp, rb = lca.reverse_dict()
 
         child_nodes = lambda node, edges: [e['from'] for e in edges if e['to'] == node]
 
         counter = itertools.count(1)
 
-        def format_node(node_key, node_data, rt):
+        def format_node(node_key, node_data, ra):
             if node_key == -1:
                 return {
                     'name': 'Functional unit',
                     'unit': 'unit',
                     'location': config.global_location,
                     'categories': "",
-                    'id': counter.next(),
+                    'id': next(counter),
                     'amount': 1.
                 }
 
             if 'row' in node_data:
                 node_key = node_data['row']
             key = ra[node_key]
             ds = Database(key[0]).load()[key]
             return {
                 'name': ds.get('name', "Unknown"),
                 'unit': ds.get('unit', "Unknown"),
                 'location': ds.get('location', "Unknown"),
                 'categories': ", ".join(ds.get('categories', [])),
-                'id': counter.next(),
+                'id': next(counter),
                 'amount': node_data['amount']
             }
 
-        def format_child_node(node_key, node_data, rt, add_biosphere):
-            ds = format_node(node_key, node_data, rt)
+        def format_child_node(node_key, node_data, ra, add_biosphere):
+            ds = format_node(node_key, node_data, ra)
             ds['size'] = node_data['cum']
             ds['variance'] = 0.5
             return ds
 
         def process_node(node):
             cn = child_nodes(node, edges)
             if cn:
-                ds = format_node(node, nodes[node], rt)
+                ds = format_node(node, nodes[node], ra)
                 ds['children'] = [process_node(o) for o in cn]
                 return ds
             else:
-                return format_child_node(node, nodes[node], rt, False)
+                return format_child_node(node, nodes[node], ra, False)
 
         return process_node(-1)
```

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/tests/contribution.py` & `bw2analyzer-0.9.dev5/bw2analyzer/tests/contribution.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/tests/econ.py` & `bw2analyzer-0.9.dev5/bw2analyzer/tests/econ.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/tests/fixtures.py` & `bw2analyzer-0.9.dev5/bw2analyzer/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/tests/health_check.py` & `bw2analyzer-0.9.dev5/bw2analyzer/tests/health_check.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/tests/matrix_grapher.py` & `bw2analyzer-0.9.dev5/bw2analyzer/tests/matrix_grapher.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/tests/sc_graph.py` & `bw2analyzer-0.9.dev5/bw2analyzer/tests/sc_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, unicode_literals, division
 from eight import *
 
-from ..sc_graph import GTManipulator, iteritems
+from ..sc_graph import GTManipulator
 from bw2data import (
     Database,
     databases,
     geomapping,
     mapping,
     methods,
     projects,
@@ -295,15 +295,15 @@
         edges = [
             {'to': 1, 'from': 2, 'amount': 3, 'exc_amount': 2, 'impact': 4},
             {'to': 2, 'from': 3, 'amount': 3, 'exc_amount': 2, 'impact': 5},
         ]
         new_nodes, new_edges = GTManipulator.simplify(nodes, edges, 2, 0.1)
         self.assertEqual(
             new_nodes,
-            {key: value for key, value in iteritems(nodes) if key in (1, 3)}
+            {key: value for key, value in nodes.items() if key in (1, 3)}
         )
         self.assertEqual(
             list(new_edges),
             [{'to': 1, 'from': 3, 'amount': 3, 'exc_amount': 4, 'impact': 5}]
         )
 
     def test_y(self):
@@ -324,15 +324,15 @@
         }
         edges = [
             {'to': 1, 'from': 3, 'amount': 0.2, 'exc_amount': 0.2, 'impact': 1},
             {'to': 2, 'from': 3, 'amount': 0.8, 'exc_amount': 0.2, 'impact': 2},
             {'to': 3, 'from': 4, 'amount': 2, 'exc_amount': 2, 'impact': 3},
         ]
         new_nodes, new_edges = GTManipulator.simplify(nodes, edges, 9, 0.1)
-        expected_nodes = {key: value for key, value in iteritems(nodes)
+        expected_nodes = {key: value for key, value in nodes.items()
             if key in (1, 2, 4)}
         self.assertEqual(expected_nodes, new_nodes)
         expected_edges = [
             {'to': 2, 'from': 4, 'amount': 1.6, 'exc_amount': 0.4, 'impact': 2},
             {'to': 1, 'from': 4, 'amount': 0.4, 'exc_amount': 0.4, 'impact': 1},
         ]
         self.assertEqual(expected_edges, list(new_edges))
@@ -347,15 +347,15 @@
         }
         edges = [
             {'to': 1, 'from': 3, 'amount': 0.2, 'exc_amount': 0.2, 'impact': 1},
             {'to': 2, 'from': 3, 'amount': 0.8, 'exc_amount': 0.2, 'impact': 2},
             {'to': 3, 'from': 4, 'amount': 2, 'exc_amount': 2, 'impact': 3},
         ]
         new_nodes, new_edges = GTManipulator.simplify(nodes, edges, 9, 0.1)
-        expected_nodes = {key: value for key, value in iteritems(nodes)
+        expected_nodes = {key: value for key, value in nodes.items()
             if key in (1, 2, 4)}
         self.assertEqual(expected_nodes, new_nodes)
         expected_edges = [
             {'to': 2, 'from': 4, 'amount': 1.6, 'exc_amount': 0.4, 'impact': 2},
             {'to': 1, 'from': 4, 'amount': 0.4, 'exc_amount': 0.4, 'impact': 1},
         ]
         self.assertEqual(expected_edges, list(new_edges))
@@ -379,15 +379,15 @@
         edges = [
             {'to': 1, 'from': 2, 'amount': 2, 'exc_amount': 1, 'impact': 2},
             {'to': 1, 'from': 3, 'amount': 3, 'exc_amount': 1, 'impact': 3},
             {'to': 2, 'from': 4, 'amount': 2, 'exc_amount': 1, 'impact': 2},
             {'to': 3, 'from': 4, 'amount': 3, 'exc_amount': 1, 'impact': 3},
         ]
         new_nodes, new_edges = GTManipulator.simplify(nodes, edges, 5, 0.1)
-        expected_nodes = {key: value for key, value in iteritems(nodes)
+        expected_nodes = {key: value for key, value in nodes.items()
             if key in (1, 4)}
         self.assertEqual(expected_nodes, new_nodes)
         expected_edges = [
             {'to': 1, 'from': 4, 'amount': 5, 'exc_amount': 2, 'impact': 5}
         ]
         self.assertEqual(expected_edges, list(new_edges))
 
@@ -410,15 +410,15 @@
         edges = [
             {'to': 1, 'from': 3, 'amount': 1, 'exc_amount': 1, 'impact': 17},
             {'to': 2, 'from': 3, 'amount': 2, 'exc_amount': 2, 'impact': 34},
             {'to': 3, 'from': 4, 'amount': 9, 'exc_amount': 3, 'impact': 27},
             {'to': 3, 'from': 5, 'amount': 12, 'exc_amount': 4, 'impact': 24},
         ]
         new_nodes, new_edges = GTManipulator.simplify(nodes, edges, 53, 0.01)
-        expected_nodes = {key: value for key, value in iteritems(nodes)
+        expected_nodes = {key: value for key, value in nodes.items()
             if key in (1, 2, 4, 5)}
         self.assertEqual(expected_nodes, new_nodes)
         expected_edges = [
             {'to': 1, 'from': 4, 'amount': 3, 'exc_amount': 3, 'impact': 9},
             {'to': 1, 'from': 5, 'amount': 4, 'exc_amount': 4, 'impact': 8},
             {'to': 2, 'from': 5, 'amount': 8, 'exc_amount': 8, 'impact': 16},
             {'to': 2, 'from': 4, 'amount': 6, 'exc_amount': 6, 'impact': 18},
```

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/tests/utils.py` & `bw2analyzer-0.9.dev5/bw2analyzer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer/utils.py` & `bw2analyzer-0.9.dev5/bw2analyzer/utils.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer.egg-info/PKG-INFO` & `bw2analyzer-0.9.dev5/bw2analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bw2analyzer
-Version: 0.9.dev4
+Version: 0.9.dev5
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/cmutel/brightway2-analyzer
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: Copyright (c) 2014, Chris Mutel and ETH Zürich
 All rights reserved.
```

### Comparing `bw2analyzer-0.9.dev4/bw2analyzer.egg-info/SOURCES.txt` & `bw2analyzer-0.9.dev5/bw2analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/CHANGES.txt` & `bw2analyzer-0.9.dev5/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/docs/conf.py` & `bw2analyzer-0.9.dev5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/docs/make.bat` & `bw2analyzer-0.9.dev5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/docs/Makefile` & `bw2analyzer-0.9.dev5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/LICENSE.txt` & `bw2analyzer-0.9.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bw2analyzer-0.9.dev4/PKG-INFO` & `bw2analyzer-0.9.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bw2analyzer
-Version: 0.9.dev4
+Version: 0.9.dev5
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/cmutel/brightway2-analyzer
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: Copyright (c) 2014, Chris Mutel and ETH Zürich
 All rights reserved.
```

### Comparing `bw2analyzer-0.9.dev4/setup.py` & `bw2analyzer-0.9.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='bw2analyzer',
-    version="0.9.dev4",
+    version="0.9.dev5",
     packages=["bw2analyzer", "bw2analyzer.tests"],
     author="Chris Mutel",
     author_email="cmutel@gmail.com",
     license=open('LICENSE.txt').read(),
     install_requires=[
         "brightway2>=2.0.dev2",
         "numpy",
```

