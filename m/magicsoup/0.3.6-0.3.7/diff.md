# Comparing `tmp/magicsoup-0.3.6.tar.gz` & `tmp/magicsoup-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.3.6.tar", last modified: Fri Apr 14 20:16:29 2023, max compression
+gzip compressed data, was "magicsoup-0.3.7.tar", last modified: Mon Apr 24 13:55:21 2023, max compression
```

## Comparing `magicsoup-0.3.6.tar` & `magicsoup-0.3.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.920780 magicsoup-0.3.6/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.6/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-14 20:16:29.916780 magicsoup-0.3.6/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.6/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.6/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-14 20:16:29.920780 magicsoup-0.3.6/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-14 20:15:25.000000 magicsoup-0.3.6/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.6/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.6/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.6/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.6/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.6/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.6/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-14 19:52:19.000000 magicsoup-0.3.6/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    30687 2023-04-14 20:12:02.000000 magicsoup-0.3.6/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-04-12 14:59:48.000000 magicsoup-0.3.6/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.6/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    42712 2023-04-14 20:13:45.000000 magicsoup-0.3.6/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.6/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.6/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.6/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.6/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.6/tests/test_world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.7/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-24 13:55:21.286378 magicsoup-0.3.7/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.7/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.7/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-24 13:55:21.286378 magicsoup-0.3.7/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-24 13:55:08.000000 magicsoup-0.3.7/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.7/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.7/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.7/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.7/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.7/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.7/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-14 19:52:19.000000 magicsoup-0.3.7/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    30687 2023-04-14 20:12:02.000000 magicsoup-0.3.7/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-04-12 14:59:48.000000 magicsoup-0.3.7/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.7/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    42780 2023-04-24 13:53:53.000000 magicsoup-0.3.7/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.7/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.7/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.7/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.7/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.7/tests/test_world.py
```

### Comparing `magicsoup-0.3.6/LICENSE` & `magicsoup-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/PKG-INFO` & `magicsoup-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.6
+Version: 0.3.7
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.6/README.md` & `magicsoup-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/pyproject.toml` & `magicsoup-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/constants.py` & `magicsoup-0.3.7/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/containers.py` & `magicsoup-0.3.7/src/magicsoup/containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.3.7/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.3.7/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.3.7/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/genetics.py` & `magicsoup-0.3.7/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/kinetics.py` & `magicsoup-0.3.7/src/magicsoup/kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/mutations.py` & `magicsoup-0.3.7/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/util.py` & `magicsoup-0.3.7/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/src/magicsoup/world.py` & `magicsoup-0.3.7/src/magicsoup/world.py`

 * *Files 0% similar despite different names*

```diff
@@ -825,15 +825,16 @@
             label = names[1].strip() if len(names) > 1 else ""
             self.genomes.append(seq)
             self.labels.append(label)
             genome_idx_pairs.append((seq, idx))
 
         self.n_cells = len(genome_idx_pairs)
 
-        if ignore_cell_params:
+        if not ignore_cell_params:
+            self.kinetics.increase_max_cells(by_n=self.n_cells)
             self.update_cells(genome_idx_pairs=genome_idx_pairs)
 
     def _divide_cells_as_possible(
         self, parent_idxs: list[int]
     ) -> tuple[list[int], list[int], list[torch.Tensor]]:
         run_idx = self.n_cells
         child_idxs = []
```

### Comparing `magicsoup-0.3.6/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.3.7/src/magicsoup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.6
+Version: 0.3.7
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.6/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.3.7/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/tests/test_containers.py` & `magicsoup-0.3.7/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/tests/test_genetics.py` & `magicsoup-0.3.7/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/tests/test_kinetics.py` & `magicsoup-0.3.7/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/tests/test_util.py` & `magicsoup-0.3.7/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.6/tests/test_world.py` & `magicsoup-0.3.7/tests/test_world.py`

 * *Files identical despite different names*

