# Comparing `tmp/living-figures-0.1.4.tar.gz` & `tmp/living-figures-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "living-figures-0.1.4.tar", last modified: Wed Apr 19 22:49:37 2023, max compression
+gzip compressed data, was "living-figures-0.1.5.tar", last modified: Mon Apr 24 18:02:55 2023, max compression
```

## Comparing `living-figures-0.1.4.tar` & `living-figures-0.1.5.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-19 22:48:45.000000 living-figures-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 22:48:45.000000 living-figures-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 22:49:37.969930 living-figures-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 22:48:45.000000 living-figures-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-19 22:48:45.000000 living-figures-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 22:48:45.000000 living-figures-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:49:37.969930 living-figures-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 22:48:45.000000 living-figures-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/test_data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/pacbio_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/parse_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/rebase_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27803 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/panepibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/fom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/bio/fom/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/utilities/parse_tax_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures/bio/fom/widgets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/base_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/ordination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/bio/volcano/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/volcano/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/volcano/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/bio/volcano/make_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/src/living_figures/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/parse_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-19 22:48:45.000000 living-figures-0.1.4/src/living_figures/helpers/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.965930 living-figures-0.1.4/src/living_figures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 22:49:37.000000 living-figures-0.1.4/src/living_figures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:49:37.969930 living-figures-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-19 22:48:45.000000 living-figures-0.1.4/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-24 18:01:53.000000 living-figures-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 18:01:53.000000 living-figures-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-24 18:02:55.874375 living-figures-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 18:01:53.000000 living-figures-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-24 18:01:53.000000 living-figures-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 18:01:53.000000 living-figures-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:02:55.874375 living-figures-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 18:01:53.000000 living-figures-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.858375 living-figures-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.858375 living-figures-0.1.5/src/living_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/test_data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/pacbio_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/parse_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/rebase_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27803 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/panepibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.870375 living-figures-0.1.5/src/living_figures/bio/fom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.870375 living-figures-0.1.5/src/living_figures/bio/fom/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/utilities/parse_tax_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.858375 living-figures-0.1.5/src/living_figures/bio/fom/widgets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.870375 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/alpha_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/base_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/ordination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/src/living_figures/bio/volcano/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/volcano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/volcano/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/bio/volcano/make_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/src/living_figures/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/parse_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 18:01:53.000000 living-figures-0.1.5/src/living_figures/helpers/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.862375 living-figures-0.1.5/src/living_figures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 18:02:55.000000 living-figures-0.1.5/src/living_figures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:02:55.874375 living-figures-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-24 18:01:53.000000 living-figures-0.1.5/tests/test_import.py
```

### Comparing `living-figures-0.1.4/LICENSE` & `living-figures-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/PKG-INFO` & `living-figures-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.4
+Version: 0.1.5
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.4/README.md` & `living-figures-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/pyproject.toml` & `living-figures-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py` & `living-figures-0.1.5/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/pacbio_file.py` & `living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/pacbio_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/parse_rebase.py` & `living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/parse_rebase.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/epigenome/utilities/rebase_file.py` & `living-figures-0.1.5/src/living_figures/bio/epigenome/utilities/rebase_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/epigenome/widgets/panepibrowser.py` & `living-figures-0.1.5/src/living_figures/bio/epigenome/widgets/panepibrowser.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/fom/utilities/parse_tax_string.py` & `living-figures-0.1.5/src/living_figures/bio/fom/utilities/parse_tax_string.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py` & `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py`

 * *Files 12% similar despite different names*

```diff
@@ -154,20 +154,32 @@
             pd.DataFrame(dict(
                 Other=abund.drop(index=to_keep).sum()
             )).T
         ])
 
         return abund
 
-    def run_self(self):
+    def get_plotting_data(self):
+        """Return the data used for plotting, using the cache when possible."""
+
+        # If the cache is populated
+        if self.get_cache(self.make_cache_key()) is not None:
+            # Return the cached data
+            return self.get_cache(self.make_cache_key())
+
+        # If the cache is not populated
 
         # Get the abundance data to plot
         abund_df = self.get_abundance_data()
+
+        # If there is no abundance data
         if abund_df is None:
-            return
+            # Note the lack of data in the cache
+            self.set_cache(self.make_cache_key(), (None, None))
+            return None, None
 
         # Get the metadata (if any was provided)
         sample_annots: pd.DataFrame = self._root().sample_annotations()
 
         # Get all of the parameters used for plotting
         params = self.all_values(flatten=True)
 
@@ -180,15 +192,16 @@
             ).dropna()
 
             # If there are no samples with the selected metadata
             if annot_df.shape[0] == 0:
 
                 msg = "No samples available with the selected annotations"
                 self.option("plot_msg").main_empty.warning(msg)
-                return
+                self.set_cache(self.make_cache_key(), (None, None))
+                return None, None
 
             # Only keep the abundances which have annotations
             abund_df = abund_df.reindex(
                 columns=annot_df.index.values
             )
 
         else:
@@ -211,14 +224,30 @@
             # Order the abundances to match
             abund_df = abund_df.reindex(columns=annot_df.index.values)
 
         # Order the annotations to match the abundances
         if annot_df is not None:
             annot_df = annot_df.reindex(index=abund_df.columns.values)
 
+        self.set_cache(self.make_cache_key(), (abund_df, annot_df))
+        return abund_df, annot_df
+
+    def run_self(self):
+
+        # Get the plotting data
+        abund_df, annot_df = self.get_plotting_data()
+
+        # If there is no data
+        if abund_df is None:
+            # Don't make a plot
+            return
+
+        # Get all of the parameters used for plotting
+        params = self.all_values(flatten=True)
+
         # Set up the size of the annotations
         annot_frac = min(
             0.5,
             0.02 + (params["annot_size"] * float(len(params["color_by"])))
         )
         row_heights = [1 - annot_frac, annot_frac]
 
@@ -233,55 +262,82 @@
             shared_xaxes=True
         )
 
         # Plot the heatmap / stacked bars
         fig.add_traces(self.plot_abund(abund_df), rows=1, cols=1)
 
         if params["plot_type"] == "Stacked Bars":
-            fig.update_layout(barmode='stack')
+            fig.update_layout(
+                barmode='stack',
+                yaxis_title="Relative Abundance (%)"
+            )
 
         # Plot the annotations
-        if len(params['color_by']) > 0 and sample_annots is not None:
+        if len(params['color_by']) > 0 and annot_df is not None:
             fig.add_trace(self.plot_annot(annot_df), row=2, col=1)
 
+        # If there is a title
+        if params['title'] is not None and params['title'] != "None":
+            fig.update_layout(title=params['title'])
+
         plot_area = self._get_child("plot")
         plot_area.main_empty.plotly_chart(
             fig,
             use_container_width=True
         )
 
+        # If there is a legend
+        if params['legend'] is not None:
+            self._get_child(
+                "legend_display"
+            ).main_empty.markdown(
+                params['legend']
+            )
+
     def plot_abund(self, abund_df):
 
-        if self.option("plot_type").get_value() == "Heatmap":
+        if self.val("plot_type") == "Heatmap":
             return self.plot_heatmap(abund_df)
         else:
             return self.plot_bars(abund_df)
 
-    def plot_heatmap(self, abund_df):
+    def plot_heatmap(self, abund_df: pd.DataFrame):
+
+        # Color scale used for the heatmap
+        colorscale = self.val("heatmap_cpal")
+
+        # Mouseover text
+        text_df = abund_df.apply(
+            lambda c: [
+                f"Sample: {c.name}<br>Organism: {n}<br>Abundance: {a:.4g}%"
+                for n, a in c.items()
+            ]
+        )
+
         return [
             go.Heatmap(
                 x=abund_df.columns.values,
                 y=abund_df.index.values,
                 z=abund_df.values,
-                # colorscale=formatting["heatmap_cpal"],
-                # text=text_df.values,
-                # hoverinfo="text",
-                colorbar_title="Proportional<br>Abundance"
+                colorscale=colorscale,
+                text=text_df.values,
+                hoverinfo="text",
+                colorbar_title="Relative<br>Abundance<br>(%)"
             )
         ]
 
     def plot_bars(self, abund_df):
 
         return [
             go.Bar(
                 name=org_name,
                 x=org_abund.index.values,
                 y=org_abund.values,
                 hovertext=[
-                    f"{sample}<br>{org_name}: {round(abund * 100., 2)}%"
+                    f"{sample}<br>{org_name}: {abund:.4g}%"
                     for sample, abund in org_abund.items()
                 ]
             )
             for org_name, org_abund in abund_df.iterrows()
         ]
 
     def plot_annot(self, annot_df):
```

### Comparing `living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/base_plots.py` & `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/base_plots.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+from typing import Any
 import widgets.streamlit as wist
 from widgets.streamlit import StResource
 from widgets.base.exceptions import WidgetFunctionException
+from living_figures.bio.fom.widgets.microbiome.base_widget import BaseMicrobiomeExplorer # noqa
 import streamlit as st
 
 
 class MicrobiomePlot(wist.StResource):
     """Base class with helper functions used for microbiome plots."""
 
+    def _root(self) -> BaseMicrobiomeExplorer:
+        return super()._root()
+
     def option(self, id) -> StResource:
         for r in self._find_child(id):
             return r
         raise WidgetFunctionException(f"Cannot find option {id}")
 
+    def val(self, id) -> Any:
+        return self.option(id).get_value()
+
     def update_options(self, options, id):
         """Update the set of options for user-provided metadata."""
 
         # Get the resource by ID
         resource = self.option(id)
 
         # If the options do not already match
@@ -29,12 +37,21 @@
                 update=self.main_container is not None
             )
 
         # Regenerate the plot
         if self.main_container is not None:
             self.run_self()
 
+    def setup_cache(self) -> None:
+        if st.session_state.get(f"{self.id}_cache") is None:
+            st.session_state[f"{self.id}_cache"] = {}
+
     def set_cache(self, cache_key, value) -> None:
+        self.setup_cache()
         st.session_state[f"{self.id}_cache"][cache_key] = value
 
     def get_cache(self, cache_key):
+        self.setup_cache()
         return st.session_state[f"{self.id}_cache"].get(cache_key)
+
+    def _get_child(self, child_id, *cont) -> 'StResource':
+        return super()._get_child(child_id, *cont)
```

### Comparing `living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/inputs.py` & `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,7 +39,26 @@
         Parse the taxonomic information of the index in the abundance table.
         """
 
         return pd.DataFrame([
             parse_tax_string(org_str)
             for org_str in self.value.index.values
         ], index=self.value.index)
+
+
+class StHashedDataFrame(wist.StDataFrame):
+    """Read in a DataFrame and compute a hash."""
+
+    hash = None
+
+    def parse_files(self, uploaded_file):
+
+        # Read the file
+        self.value: pd.DataFrame = pd.read_csv(
+            uploaded_file,
+            index_col=0,
+            sep="\t" if "tsv" in uploaded_file.name else ",",
+            compression="gzip" if uploaded_file.name.endswith(".gz") else None
+        )
+
+        # Compute the hash of the data
+        self.hash = md5(self.value.to_csv().encode()).hexdigest()
```

### Comparing `living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/main.py` & `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/base_widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,23 @@
-from copy import deepcopy
+from typing import List, Union
 import numpy as np
 import pandas as pd
-from living_figures.bio.fom.widgets.microbiome import MicrobiomeAbund
-from living_figures.bio.fom.widgets.microbiome import Ordination
-from living_figures.bio.fom.widgets.microbiome import AbundantOrgs
-from living_figures.helpers import parse_numeric, is_numeric
-from typing import Union
 import widgets.streamlit as wist
 from widgets.base.exceptions import WidgetFunctionException
+from living_figures.helpers import parse_numeric
+from living_figures.helpers import is_numeric
 
 
-class MicrobiomeExplorer(wist.StreamlitWidget):
-    """
-    Widget used for the analysis of microbiome data.
-
-    Input data:
-        - Microbiome abundance data, from a variety of file formats
-        - Sample annotation metadata
-        - Microbe anotation metadata
-
-    Types of analysis:
-        - Ordination of samples
-        - Visualization of microbial abundances (stacked bars, etc.)
-        - Comparison of the abundance of a single microbe across samples
-        - Testing for significant differences in organism abundances
-          between groups of samples
-    """
-
-    id = "microbiome-explorer"
-    subtitle = "Microbiome Explorer"
-
-    children = [
-
-        wist.StExpander(
-            id="data",
-            label="Input Data",
-            expanded=True,
-            children=[
-                MicrobiomeAbund(id="abund"),
-                wist.StDataFrame(
-                    id="annots",
-                    label="Sample Annotations",
-                    kwargs=dict(index_col=0)
-                ),
-                wist.StDownloadDataFrame(
-                    target="annots",
-                    label="Download Annotations"
-                )
-            ]
-        ),
-        wist.StDuplicator(
-            id='plots',
-            children=[
-                deepcopy(wist.StSelector(
-                    id=f"plot_{i}",
-                    disable_sidebar=True,
-                    options=[
-                        AbundantOrgs(id="abundant_orgs"),
-                        Ordination(id="ordination")
-                    ]
-                ))
-                for i in range(20)
-            ],
-            value=[True] + [False for _ in range(19)]
-        )
-    ]
-
-    requirements = [
-        "living-figures"
-    ]
-
-    extra_imports = [
-        "from living_figures.helpers import parse_numeric, is_numeric",
-        "import numpy as np",
-        "import pandas as pd",
-        "from typing import Union",
-        "from widgets.base.exceptions import WidgetFunctionException"
-    ]
+class BaseMicrobiomeExplorer(wist.StreamlitWidget):
 
     def msg(self, msg):
         """Write to the message container."""
         self.main_container.write(msg)
 
-    def abund(self, level=None, filter='None') -> pd.DataFrame():
+    def abund(self, level=None, filter='None') -> pd.DataFrame:
         """
         Return the abundance table
         """
 
         # Get the abundances
         abund: pd.DataFrame = self.get(["data", "abund"])
 
@@ -147,26 +78,33 @@
                 abund.sum() > 0
             ]
         )
 
         if abund.shape[1] == 0:
             return
 
-        # Normalize all abundances to proportions
-        abund = abund / abund.sum()
+        # Normalize all abundances to percentages
+        abund = 100 * abund / abund.sum()
 
         return abund
 
-    def abund_hash(self) -> pd.DataFrame():
+    def abund_hash(self) -> pd.DataFrame:
         """
         Return the hash of the abundance table
         """
 
         return self.get(["data", "abund"], attr="hash")
 
+    def annot_hash(self) -> pd.DataFrame:
+        """
+        Return the hash of the annotation table
+        """
+
+        return self.get(["data", "annots"], attr="hash")
+
     def sample_annotations(self) -> Union[None, pd.DataFrame]:
         """Return the table of sample annotations."""
 
         # Get the value of the sample annotation resource
         annots: pd.DataFrame = self.get(["data", "annots"])
 
         # If the sample annotations have not been provided
@@ -205,15 +143,15 @@
 
         # Try to convert any values to numeric, if possible
         annots = parse_numeric(annots)
 
         # Return the data which passes this filtering regime
         return annots
 
-    def sample_filters(self, max_categories=10):
+    def sample_filters(self, max_categories=10) -> List[str]:
         """Return the list of possible filters based on sample metadata."""
 
         # Get all of the sample annotations provided by the user
         annots = self.sample_annotations()
 
         # Build a list of possible filters
         filters = ['None']
@@ -242,15 +180,15 @@
 
                 filters.append(
                     f"{cname} == {filter_val}"
                 )
 
         return filters
 
-    def sample_colors(self, max_categories=10, include_none=True):
+    def sample_colors(self, max_categories=10, include_none=True) -> List[str]:
         """Return the list of plot colorings based on sample metadata."""
 
         # Get all of the sample annotations provided by the user
         annots = self.sample_annotations()
 
         # Build a list of possible colors
         colors = ['None'] if include_none else []
@@ -277,33 +215,32 @@
                 if unique_vals.shape[0] <= max_categories:
 
                     # Add it to the list
                     colors.append(cname)
 
         return colors
 
-    def update_options(self):
+    def update_options(self) -> None:
         """Update the menu selection items based on the user inputs."""
 
         # Update the Ordination and Abundant Organism plots
-        for plot_type in ["ordination", "abundant_orgs"]:
+        for plot_type in [
+            "ordination",
+            "abundant_orgs",
+            "alpha_diversity"
+        ]:
 
             # For each of the elements of this type
             for plot_elem in self._find_child(plot_type):
 
                 # Update the 'color_by' and 'filter_by' menu options
+
+                # Update the sample colors
                 plot_elem.update_options(
-                    self.sample_colors(include_none=plot_type == "ordination"),
+                    self.sample_colors(
+                        # Only include a "None" value for ordination
+                        include_none=plot_type != "abundant_orgs"
+                    ),
                     "color_by"
                 )
+                # Update the filter_by for all plot types
                 plot_elem.update_options(self.sample_filters(), "filter_by")
-
-    def run_self(self):
-
-        self.update_options()
-
-        self.clone_button(sidebar=True)
-
-
-if __name__ == "__main__":
-    w = MicrobiomeExplorer()
-    w.run()
```

### Comparing `living-figures-0.1.4/src/living_figures/bio/fom/widgets/microbiome/ordination.py` & `living-figures-0.1.5/src/living_figures/bio/fom/widgets/microbiome/ordination.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from widgets.base.exceptions import WidgetFunctionException
 from living_figures.bio.fom.widgets.microbiome.base_plots import MicrobiomePlot
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE
-import streamlit as st
 from living_figures.helpers.constants import tax_levels
 
 
 class Ordination(MicrobiomePlot):
 
     label = "Ordination (PCA/t-SNE)"
 
@@ -79,40 +78,57 @@
         ),
         wist.StResource(id="plot"),
         wist.StResource(id="ord_msg"),
         wist.StResource(id="legend_display")
     ]
 
     def make_cache_key(self, val_str: str):
-        """Return a cache for the ordination object(s)."""
+        """Return a cache key for the plot data."""
 
         # Get the hash of the input data
-        abund_hash = self._root().abund_hash()
-
-        # Get the plotting options
-        params = self.all_values(flatten=True)
+        abund_hash: str = self._root().abund_hash()
 
         # Set the cache key based on the input data and analysis details
-        cache_key = f"{abund_hash}:{params['tax_level']}:{params['ord_type']}:{2 + params['3D']}D:{params['filter_by']}:{val_str}" # noqa
+        cache_key = ":".join(map(
+            str,
+            [
+                abund_hash,
+                self.val('tax_level'),
+                self.val('ord_type'),
+                self.val('3D'),
+                self.val('filter_by'),
+                val_str
+            ]
+        ))
 
         return cache_key
 
     def run_ordination(self) -> Union[None, pd.DataFrame]:
         """Perform ordination on the abundance data."""
 
-        # Set up the cache
-        if st.session_state.get("ordination_cache") is None:
-            st.session_state["ordination_cache"] = dict()
+        # Get the cache key
+        cache_key = self.make_cache_key("projection")
+
+        # If a value has been computed
+        if self.get_cache(cache_key) is not None:
+
+            # Get the value
+            proj = self.get_cache(cache_key)
+
+            # Return the value
+            if isinstance(proj, str) and proj == "None":
+                return
+            else:
+                return proj
+
+        # The projection needs to be computed
 
         # Get the plotting options
         params = self.all_values(flatten=True)
 
-        # Get the cache key
-        cache_key = self.make_cache_key("projection")
-
         # Get the abundances, filtering to the specified taxonomic level
         # Columns are samples, rows are organisms
         abund: pd.DataFrame = self._root().abund(
             level=params['tax_level'],
             filter=params['filter_by']
         )
 
@@ -127,27 +143,24 @@
         msg = f"Running {params['ord_type']} on {abund.shape[1]:,} samples"
         msg = f"{msg} using {abund.shape[0]:,}"
         msg = f"{msg} {params['tax_level']}-level organisms"
         if params['filter_by'] is not None and params['filter_by'] != 'None':
             msg = msg + "  \n" + f"Filtering to {params['filter_by']}"
         self._get_child("ord_msg").main_empty.write(msg)
 
-        # Only compute if the cache is empty
-        if self.get_cache(cache_key) is None:
-
-            if params['ord_type'] == 'PCA':
-                proj, loadings = self.run_pca(abund)
-            elif params['ord_type'] == 't-SNE':
-                proj, loadings = self.run_tsne(abund)
-            else:
-                msg = "Ordination type not recognized"
-                raise WidgetFunctionException(msg)
+        if params['ord_type'] == 'PCA':
+            proj, loadings = self.run_pca(abund)
+        elif params['ord_type'] == 't-SNE':
+            proj, loadings = self.run_tsne(abund)
+        else:
+            msg = "Ordination type not recognized"
+            raise WidgetFunctionException(msg)
 
-            self.set_cache(cache_key, proj)
-            self.set_cache(self.make_cache_key("loadings"), loadings)
+        self.set_cache(cache_key, proj)
+        self.set_cache(self.make_cache_key("loadings"), loadings)
 
         return self.get_cache(cache_key)
 
     def run_pca(self, abund: pd.DataFrame):
         """Ordinate data using PCA"""
 
         pca = PCA()
@@ -178,15 +191,15 @@
 
         return coords, loadings
 
     def run_tsne(self, abund: pd.DataFrame):
         """Ordinate data using t-SNE"""
 
         tsne = TSNE(
-            n_components=3 if self.option("3D").get_value() else 2
+            n_components=3 if self.val("3D") else 2
         )
         ord_mat = tsne.fit_transform(abund.T)
         coords = pd.DataFrame(
             ord_mat,
             columns=[
                 f"t-SNE {i+1}"
                 for i in range(ord_mat.shape[1])
@@ -212,69 +225,77 @@
             plot_df = plot_df.merge(
                 sample_annots,
                 left_index=True,
                 right_index=True
             )
 
         # Get the coloring column
-        color_by = self.option("color_by").get_value()
+        color_by = self.val("color_by")
         if color_by == 'None':
             color_by = None
 
         # Set up the data which will be used to build the plot
         plot_kwargs = dict(
             data_frame=plot_df,
             x=plot_df.columns.values[0],
             y=plot_df.columns.values[1],
             color=color_by
         )
 
         # If the 3D plot was requested
-        if self.option("3D").get_value():
+        if self.val("3D"):
             plot_f = px.scatter_3d
             plot_kwargs['z'] = plot_df.columns.values[2]
         else:
             plot_f = px.scatter
 
         # Make a plot
         fig = plot_f(**plot_kwargs)
 
         # Add the PCA loadings, if requested
-        self.add_pca_loadings(fig)
+        self.add_pca_loadings(fig, plot_df)
 
         # If there is a title
-        title = self.option("title").get_value()
+        title = self.val("title")
         if title is not None and title != "None":
             fig.update_layout(title=title)
 
         # Add the plot to the display
         self._get_child("plot").main_empty.plotly_chart(fig)
 
         # If there is a legend
-        legend = self.option("legend").get_value()
+        legend = self.val("legend")
         if legend is not None:
             self._get_child(
                 "legend_display"
             ).main_empty.markdown(legend)
 
-    def add_pca_loadings(self, fig):
+    def add_pca_loadings(self, fig, plot_df):
 
-        if not self.option("pca_loadings").get_value():
+        if not self.val("pca_loadings"):
             return
 
         # Get the key used in the cache for the loadings
-        loadings = self.get_cache(
-            self.make_cache_key("loadings")
-        )
+        cache_key = self.make_cache_key("loadings")
+
+        # If there is no value in the cache
+        if self.get_cache(cache_key) is None:
+            # Run the ordination to make sure that the cache
+            # is current
+            _ = self.run_ordination()
 
+        # Get any value in the cache
+        loadings = self.get_cache(cache_key)
+
+        # If no value has been computed
         if loadings is None:
             return
 
         # Number of dimensions
-        ndims = 2 + self.option("3D").get_value()
+        ndims = 2 + self.val("3D")
 
         # Just pick the number of axes used in the plot
         loadings = loadings.head(ndims)
 
         # Score the organisms based on the absolute sum of loadings
         org_score = loadings.abs().sum()
 
@@ -287,23 +308,30 @@
 
         loadings = loadings.reindex(
             columns=org_score.index.values[
                 org_score >= cutoff_score
             ]
         )
 
+        # Scale each loading to fit nicely on the plot
+        loadings = (
+            plot_df.reindex(
+                columns=loadings.index.values
+            ).abs().max() * loadings.T / loadings.T.abs().max()
+        ).T
+
         for org_name, org_coords in loadings.items():
 
             line_props = dict(
                 x=[0, org_coords.values[0]],
                 y=[0, org_coords.values[1]],
                 mode='lines',
                 name=org_name
             )
-            if self.option("3D").get_value():
+            if self.val("3D"):
                 line_props['z'] = [0, org_coords.values[2]]
                 trace_f = go.Scatter3d
             else:
                 trace_f = go.Scatter
 
             fig.add_trace(
                 trace_f(**line_props)
```

### Comparing `living-figures-0.1.4/src/living_figures/bio/volcano/app.py` & `living-figures-0.1.5/src/living_figures/bio/volcano/app.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/bio/volcano/make_test_data.py` & `living-figures-0.1.5/src/living_figures/bio/volcano/make_test_data.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/helpers/parse_numeric.py` & `living-figures-0.1.5/src/living_figures/helpers/parse_numeric.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures/helpers/sorting.py` & `living-figures-0.1.5/src/living_figures/helpers/sorting.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.4/src/living_figures.egg-info/PKG-INFO` & `living-figures-0.1.5/src/living_figures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.4
+Version: 0.1.5
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.4/src/living_figures.egg-info/SOURCES.txt` & `living-figures-0.1.5/src/living_figures.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 src/living_figures/bio/epigenome/widgets/__init__.py
 src/living_figures/bio/epigenome/widgets/panepibrowser.py
 src/living_figures/bio/fom/__init__.py
 src/living_figures/bio/fom/utilities/__init__.py
 src/living_figures/bio/fom/utilities/parse_tax_string.py
 src/living_figures/bio/fom/widgets/microbiome/__init__.py
 src/living_figures/bio/fom/widgets/microbiome/abundant_orgs.py
+src/living_figures/bio/fom/widgets/microbiome/alpha_diversity.py
 src/living_figures/bio/fom/widgets/microbiome/base_plots.py
+src/living_figures/bio/fom/widgets/microbiome/base_widget.py
 src/living_figures/bio/fom/widgets/microbiome/inputs.py
 src/living_figures/bio/fom/widgets/microbiome/main.py
 src/living_figures/bio/fom/widgets/microbiome/ordination.py
 src/living_figures/bio/volcano/__init__.py
 src/living_figures/bio/volcano/app.py
 src/living_figures/bio/volcano/make_test_data.py
 src/living_figures/helpers/__init__.py
```

### Comparing `living-figures-0.1.4/tests/test_import.py` & `living-figures-0.1.5/tests/test_import.py`

 * *Files identical despite different names*

