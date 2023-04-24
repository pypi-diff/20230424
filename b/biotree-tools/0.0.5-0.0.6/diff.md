# Comparing `tmp/biotree_tools-0.0.5.tar.gz` & `tmp/biotree_tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotree_tools-0.0.5.tar", last modified: Thu Apr 20 21:06:35 2023, max compression
+gzip compressed data, was "biotree_tools-0.0.6.tar", last modified: Mon Apr 24 14:01:46 2023, max compression
```

## Comparing `biotree_tools-0.0.5.tar` & `biotree_tools-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 21:06:35.619456 biotree_tools-0.0.5/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-03-29 13:25:29.000000 biotree_tools-0.0.5/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1128 2023-04-20 21:06:35.619456 biotree_tools-0.0.5/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      641 2023-04-20 20:13:16.000000 biotree_tools-0.0.5/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 biotree_tools-0.0.5/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      851 2023-04-20 21:06:35.619456 biotree_tools-0.0.5/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 biotree_tools-0.0.5/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 21:06:35.615456 biotree_tools-0.0.5/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 21:06:35.619456 biotree_tools-0.0.5/src/biotree_tools/
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341968 2023-03-29 13:48:02.000000 biotree_tools-0.0.5/src/biotree_tools/MMlib3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      141 2023-04-20 16:25:52.000000 biotree_tools-0.0.5/src/biotree_tools/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-20 21:06:29.000000 biotree_tools-0.0.5/src/biotree_tools/_version.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    24390 2023-04-20 16:23:51.000000 biotree_tools-0.0.5/src/biotree_tools/alignment_tools.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    19769 2023-04-20 16:22:01.000000 biotree_tools-0.0.5/src/biotree_tools/phylo_context.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    43207 2023-04-20 16:16:56.000000 biotree_tools-0.0.5/src/biotree_tools/show_tree.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    71529 2023-04-20 16:36:57.000000 biotree_tools-0.0.5/src/biotree_tools/tree_classes.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7835 2023-04-20 16:14:04.000000 biotree_tools-0.0.5/src/biotree_tools/tree_tools.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-20 21:06:35.619456 biotree_tools-0.0.5/src/biotree_tools.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1128 2023-04-20 21:06:35.000000 biotree_tools-0.0.5/src/biotree_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      512 2023-04-20 21:06:35.000000 biotree_tools-0.0.5/src/biotree_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-20 21:06:35.000000 biotree_tools-0.0.5/src/biotree_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       64 2023-04-20 21:06:35.000000 biotree_tools-0.0.5/src/biotree_tools.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       14 2023-04-20 21:06:35.000000 biotree_tools-0.0.5/src/biotree_tools.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-24 14:01:46.724098 biotree_tools-0.0.6/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-03-29 13:25:29.000000 biotree_tools-0.0.6/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1128 2023-04-24 14:01:46.724098 biotree_tools-0.0.6/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      641 2023-04-20 20:13:16.000000 biotree_tools-0.0.6/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 biotree_tools-0.0.6/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      824 2023-04-24 14:01:46.724098 biotree_tools-0.0.6/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 biotree_tools-0.0.6/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-24 14:01:46.720098 biotree_tools-0.0.6/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-24 14:01:46.724098 biotree_tools-0.0.6/src/biotree_tools/
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341968 2023-03-29 13:48:02.000000 biotree_tools-0.0.6/src/biotree_tools/MMlib3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      141 2023-04-20 16:25:52.000000 biotree_tools-0.0.6/src/biotree_tools/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-24 13:59:21.000000 biotree_tools-0.0.6/src/biotree_tools/_version.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    24390 2023-04-20 16:23:51.000000 biotree_tools-0.0.6/src/biotree_tools/alignment_tools.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    19769 2023-04-20 16:22:01.000000 biotree_tools-0.0.6/src/biotree_tools/phylo_context.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    43207 2023-04-20 16:16:56.000000 biotree_tools-0.0.6/src/biotree_tools/show_tree.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    71529 2023-04-20 16:36:57.000000 biotree_tools-0.0.6/src/biotree_tools/tree_classes.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7835 2023-04-20 16:14:04.000000 biotree_tools-0.0.6/src/biotree_tools/tree_tools.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-24 14:01:46.724098 biotree_tools-0.0.6/src/biotree_tools.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1128 2023-04-24 14:01:46.000000 biotree_tools-0.0.6/src/biotree_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      512 2023-04-24 14:01:46.000000 biotree_tools-0.0.6/src/biotree_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-24 14:01:46.000000 biotree_tools-0.0.6/src/biotree_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       41 2023-04-24 14:01:46.000000 biotree_tools-0.0.6/src/biotree_tools.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       14 2023-04-24 14:01:46.000000 biotree_tools-0.0.6/src/biotree_tools.egg-info/top_level.txt
```

### Comparing `biotree_tools-0.0.5/LICENSE` & `biotree_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/PKG-INFO` & `biotree_tools-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotree_tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Collection of bioinformatics tools related to alignments and phylogenetic trees
 Home-page: https://github.com/pypa/biotree_tools
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `biotree_tools-0.0.5/README.md` & `biotree_tools-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/setup.cfg` & `biotree_tools-0.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	biopython
 	easyterm  >=1.0.0
 	ncbi_db >=0.1.1
-	ete3 == 3.1.1
-	brewer2mpl
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `biotree_tools-0.0.5/src/biotree_tools/MMlib3.py` & `biotree_tools-0.0.6/src/biotree_tools/MMlib3.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/src/biotree_tools/alignment_tools.py` & `biotree_tools-0.0.6/src/biotree_tools/alignment_tools.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/src/biotree_tools/phylo_context.py` & `biotree_tools-0.0.6/src/biotree_tools/phylo_context.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/src/biotree_tools/show_tree.py` & `biotree_tools-0.0.6/src/biotree_tools/show_tree.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/src/biotree_tools/tree_classes.py` & `biotree_tools-0.0.6/src/biotree_tools/tree_classes.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/src/biotree_tools/tree_tools.py` & `biotree_tools-0.0.6/src/biotree_tools/tree_tools.py`

 * *Files identical despite different names*

### Comparing `biotree_tools-0.0.5/src/biotree_tools.egg-info/PKG-INFO` & `biotree_tools-0.0.6/src/biotree_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotree-tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Collection of bioinformatics tools related to alignments and phylogenetic trees
 Home-page: https://github.com/pypa/biotree_tools
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `biotree_tools-0.0.5/src/biotree_tools.egg-info/SOURCES.txt` & `biotree_tools-0.0.6/src/biotree_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

