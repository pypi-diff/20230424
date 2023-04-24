# Comparing `tmp/scbs-0.6.1.tar.gz` & `tmp/scbs-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scbs-0.6.1.tar", max compression
+gzip compressed data, was "scbs-0.6.2.tar", max compression
```

## Comparing `scbs-0.6.1.tar` & `scbs-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35147 2022-03-24 15:36:56.224000 scbs-0.6.1/LICENSE
--rwxr-xr-x   0        0        0     4235 2023-03-24 15:56:56.580000 scbs-0.6.1/README.md
--rwxr-xr-x   0        0        0     1371 2023-03-20 13:25:37.476000 scbs-0.6.1/pyproject.toml
--rwxr-xr-x   0        0        0    19471 2022-11-14 17:05:41.660000 scbs-0.6.1/scbs/MINCELLS/cli_MINCELLS.py
--rw-r--r--   0        0        0     3705 2022-11-14 16:11:54.388000 scbs-0.6.1/scbs/MINCELLS/numerics_MINCELLS.py
--rw-r--r--   0        0        0     6819 2022-11-30 09:56:09.808000 scbs-0.6.1/scbs/MINCELLS/scbs_MINCELLS.py
--rw-r--r--   0        0        0     8291 2022-11-21 14:49:13.428000 scbs-0.6.1/scbs/MINCELLS.tar.gz
--rwxr-xr-x   0        0        0       22 2023-03-10 15:46:41.424000 scbs-0.6.1/scbs/__init__.py
--rwxr-xr-x   0        0        0    19458 2023-03-13 10:05:11.584000 scbs-0.6.1/scbs/cli.py
--rwxr-xr-x   0        0        0    19263 2023-03-24 19:47:07.340000 scbs-0.6.1/scbs/diff.py
--rw-r--r--   0        0        0     6141 2023-03-24 20:40:39.984000 scbs-0.6.1/scbs/filter.py
--rw-r--r--   0        0        0     5732 2023-03-10 14:39:39.380000 scbs-0.6.1/scbs/matrix.py
--rw-r--r--   0        0        0     5817 2023-03-24 19:45:31.480000 scbs-0.6.1/scbs/numerics.py
--rw-r--r--   0        0        0    14268 2022-10-24 15:22:10.052000 scbs-0.6.1/scbs/prepare.py
--rw-r--r--   0        0        0     6070 2022-04-14 11:53:01.016000 scbs-0.6.1/scbs/profile.py
--rw-r--r--   0        0        0     7179 2023-03-13 11:03:57.980000 scbs-0.6.1/scbs/scbs.py
--rw-r--r--   0        0        0     3476 2022-04-25 13:54:17.480000 scbs-0.6.1/scbs/smooth.py
--rw-r--r--   0        0        0     3802 2023-03-24 20:41:12.848000 scbs-0.6.1/scbs/utils.py
--rw-r--r--   0        0        0     5297 2023-03-24 20:43:37.776927 scbs-0.6.1/setup.py
--rw-r--r--   0        0        0     5427 2023-03-24 20:43:37.777377 scbs-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-03-24 15:36:56.224000 scbs-0.6.2/LICENSE
+-rwxr-xr-x   0        0        0     4235 2023-03-24 15:56:56.580000 scbs-0.6.2/README.md
+-rwxr-xr-x   0        0        0     1371 2023-04-24 13:32:27.156000 scbs-0.6.2/pyproject.toml
+-rwxr-xr-x   0        0        0    19471 2022-11-14 17:05:41.660000 scbs-0.6.2/scbs/MINCELLS/cli_MINCELLS.py
+-rw-r--r--   0        0        0     3705 2022-11-14 16:11:54.388000 scbs-0.6.2/scbs/MINCELLS/numerics_MINCELLS.py
+-rw-r--r--   0        0        0     6819 2022-11-30 09:56:09.808000 scbs-0.6.2/scbs/MINCELLS/scbs_MINCELLS.py
+-rw-r--r--   0        0        0     8291 2022-11-21 14:49:13.428000 scbs-0.6.2/scbs/MINCELLS.tar.gz
+-rwxr-xr-x   0        0        0       22 2023-04-24 13:32:27.156000 scbs-0.6.2/scbs/__init__.py
+-rwxr-xr-x   0        0        0    19501 2023-04-24 13:32:27.160000 scbs-0.6.2/scbs/cli.py
+-rwxr-xr-x   0        0        0    19851 2023-04-24 15:39:12.964000 scbs-0.6.2/scbs/diff.py
+-rw-r--r--   0        0        0     6141 2023-03-24 20:40:39.984000 scbs-0.6.2/scbs/filter.py
+-rw-r--r--   0        0        0     5732 2023-03-10 14:39:39.380000 scbs-0.6.2/scbs/matrix.py
+-rw-r--r--   0        0        0     5817 2023-03-24 19:45:31.480000 scbs-0.6.2/scbs/numerics.py
+-rw-r--r--   0        0        0    14268 2022-10-24 15:22:10.052000 scbs-0.6.2/scbs/prepare.py
+-rw-r--r--   0        0        0     6070 2022-04-14 11:53:01.016000 scbs-0.6.2/scbs/profile.py
+-rw-r--r--   0        0        0     7179 2023-03-13 11:03:57.980000 scbs-0.6.2/scbs/scbs.py
+-rw-r--r--   0        0        0     3476 2022-04-25 13:54:17.480000 scbs-0.6.2/scbs/smooth.py
+-rw-r--r--   0        0        0     3802 2023-03-24 20:41:12.848000 scbs-0.6.2/scbs/utils.py
+-rw-r--r--   0        0        0     5297 2023-04-24 15:49:37.881707 scbs-0.6.2/setup.py
+-rw-r--r--   0        0        0     5427 2023-04-24 15:49:37.882149 scbs-0.6.2/PKG-INFO
```

### Comparing `scbs-0.6.1/LICENSE` & `scbs-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/README.md` & `scbs-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/pyproject.toml` & `scbs-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scbs"
-version = "0.6.1"
+version = "0.6.2"
 description = "command line tool for the analysis of single-cell bisulfite-sequencing data"
 authors = [
     "Lukas PM Kremer <L-Kremer@web.de>",
     "Leonie Küchenhoff <leonie.kuechenhoff@gmx.de>",
     "Alexey Uvarovskii <a.uvarovskii@uni-heidelberg.de>",
     "Simon Anders <simon.anders@bioquant.uni-heidelberg.de>",
 ]
```

### Comparing `scbs-0.6.1/scbs/MINCELLS/cli_MINCELLS.py` & `scbs-0.6.2/scbs/MINCELLS/cli_MINCELLS.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/MINCELLS/numerics_MINCELLS.py` & `scbs-0.6.2/scbs/MINCELLS/numerics_MINCELLS.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/MINCELLS/scbs_MINCELLS.py` & `scbs-0.6.2/scbs/MINCELLS/scbs_MINCELLS.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/MINCELLS.tar.gz` & `scbs-0.6.2/scbs/MINCELLS.tar.gz`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/cli.py` & `scbs-0.6.2/scbs/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,16 @@
     metavar="INTEGER",
     show_default=True,
     help="Smoothing bandwidth in basepairs.",
 )
 @click.option(
     "--use-weights",
     is_flag=True,
-    help="Use this to weigh each methylation site by log1p(coverage).",
+    help="Use this to weigh each methylation site by log1p(coverage)."
+    "  [default: off]",
 )
 def smooth_cli(**kwargs):
     from .smooth import smooth
 
     timer = Timer(label="smooth")
     _print_kwargs(kwargs)
     smooth(**kwargs)
@@ -455,15 +456,16 @@
     "--write-header",
     is_flag=True,
     help="Write the column names of the output file.  [default: off]",
 )
 @click.option(
     "--debug",
     is_flag=True,
-    help="Use this to to also report DMRs that were identified in permutations.",
+    help="Use this to also report DMRs that were identified in permutations.  "
+    "[default: off]",
 )
 def diff_cli(**kwargs):
     from .diff import diff
 
     timer = Timer(label="diff")
     _print_kwargs(kwargs)
     diff(**kwargs)
```

### Comparing `scbs-0.6.1/scbs/diff.py` & `scbs-0.6.2/scbs/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,34 @@
         index_g1[i] = True
     for i in permutation[celltype_2]:
         index_g2[i] = True
     return index_g1, index_g2
 
 
 @njit
-def calc_fdr(datatype):
-    fdisc = 0
+def calc_fdr(bools):
+    """
+    Calculates an adjusted p-value for each DMR using the Benjamini-Hochberg method.
+    Input is an array of boolean values, where each value represents a DMR.
+    The array is sorted by absolute t-statistic and the boolean indicates whether the
+    the DMR was found in a permutation (False) or in the real comparison (True).
+    """
+    n_t = bools.sum()  # number of DMRs in the real comparison
+    n_t_null = len(bools) - n_t  # number of DMRs in the permutation
+    fdisc = 0  # number of false discoveries up until a certain threshold
     tdisc = 0
-    adj_p_val_arr = np.empty(datatype.shape, dtype=np.float64)
-    for i in range(len(datatype)):
-        if datatype[i]:
+    adj_p_vals = np.empty(bools.shape, dtype=np.float64)
+    for i in range(len(bools)):
+        if bools[i]:  # it's from the real comparison
             tdisc += 1
-        else:
+        else:  # it's from the permutation
             fdisc += 1
-        adj_p_val = fdisc / (fdisc + tdisc)
-        adj_p_val_arr[i] = adj_p_val
-    return adj_p_val_arr
+        adj_p_val = (fdisc / n_t_null) / (tdisc / n_t)
+        adj_p_vals[i] = adj_p_val
+    return adj_p_vals
 
 
 @njit(nogil=True)
 def calc_welch_tstat_df(group1, group2, min_cells):
     """
     Calculates the t-statistic and the degrees of freedom (df) according to Welch's
     t-test for unequal variances.
```

### Comparing `scbs-0.6.1/scbs/filter.py` & `scbs-0.6.2/scbs/filter.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/matrix.py` & `scbs-0.6.2/scbs/matrix.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/numerics.py` & `scbs-0.6.2/scbs/numerics.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/prepare.py` & `scbs-0.6.2/scbs/prepare.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/profile.py` & `scbs-0.6.2/scbs/profile.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/scbs.py` & `scbs-0.6.2/scbs/scbs.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/smooth.py` & `scbs-0.6.2/scbs/smooth.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/scbs/utils.py` & `scbs-0.6.2/scbs/utils.py`

 * *Files identical despite different names*

### Comparing `scbs-0.6.1/setup.py` & `scbs-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'statsmodels>=0.12.2,<1']
 
 entry_points = \
 {'console_scripts': ['scbs = scbs.cli:cli']}
 
 setup_kwargs = {
     'name': 'scbs',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'command line tool for the analysis of single-cell bisulfite-sequencing data',
     'long_description': '[![PyPI](https://img.shields.io/pypi/v/scbs?logo=PyPI)](https://pypi.org/project/scbs)\n[![PyPIDownloads](https://pepy.tech/badge/scbs)](https://pepy.tech/project/scbs)\n[![Stars](https://img.shields.io/github/stars/LKremer/scbs?logo=GitHub&color=yellow)](https://github.com/LKremer/scbs/stargazers)\n\n# `scbs`: A Command Line Tool for the Analysis of Single-Cell Bisulfite-Sequencing Data\n\n## Installation\n\nThis software requires a working installation of [Python 3](https://www.python.org/downloads/) and requires the use of a shell terminal.\nIt was extensively tested on Ubuntu and MacOS, and briefly tested on Windows 10.\n\nYou can install `scbs` from the Python package index as follows:\n```\npython3 -m pip install --upgrade pip  # you need a recent pip version\npython3 -m pip install scbs\n```\nInstallation of `scbs` should take no longer than a few seconds. All required [dependencies](pyproject.toml) are automatically installed, this may take a few minutes.\nAfterwards, restart your terminal. The installation is now finished and the command line interface should now be available when typing the command `scbs` in your terminal.\nIf this is not the case, check the "troubleshooting" section below.  \n\n\n## Updating to the latest version\nJust use `--upgrade` when installing the package, otherwise it\'s the same process as installing:\n```\npython3 -m pip install --upgrade scbs\n```\nAfterwards, make sure that the latest version is correctly installed:\n```\nscbs --version\n```\n\n## [Tutorial](docs/tutorial.md) of a typical `scbs` run\nA tutorial can be found [here](docs/tutorial.md). This gives instructions on how to use `scbs` on a small example data set which we provide.\n\nAlso make sure to read the help by typing `scbs --help` or by checking [this page](docs/commands.md).\n\n\n## What can this package do?\n\n`scbs` takes as input a number of single-cell methylation files and allows you to quickly and easily obtain a cell × region matrix for downstream analysis (e.g. PCA, UMAP or clustering).\nIt also facilitates quality control, allows you to discover variably methylated regions (VMRs), accurately quantifies methylation in genomic intervals, and stores your sc-methylomes in an efficient manner.\nLastly, you can also select two cell populations and identify differentially methylated regions (DMRs) between them.\n\n<picture>\n  <source media="(prefers-color-scheme: dark)" srcset="docs/Fig_workflow2.png">\n  <source media="(prefers-color-scheme: light)" srcset="docs/Fig_workflow.png">\n  <img alt="schematic showing the capabilities of scbs.">\n</picture>\n\nYou can find a list of the available `scbs` commands [here](docs/commands.md).\n\n\n## bioRxiv preprint\n\nFor a detailed explanation of the methods implemented in `scbs`, please check our bioRxiv preprint:\n\n*Analyzing single-cell bisulfite sequencing data with scbs*  \nLukas PM Kremer, Leonie Kuechenhoff, Santiago Cerrizuela, Ana Martin-Villalba, Simon Anders  \nbioRxiv 2022.06.15.496318; doi: [https://doi.org/10.1101/2022.06.15.496318](https://doi.org/10.1101/2022.06.15.496318)\n\n\n## Troubleshooting\n\n#### Installation issues\n\nCarefully check the output log of PIP. Look for a message like `WARNING: The script scbs is installed in \'/home/ubuntu/.local/bin\' which is not on PATH.`, which would indicate that you need to add `/home/ubuntu/.local/bin` to your path. Alternatively, you can copy `/home/ubuntu/.local/bin/scbs` to e.g. `/usr/local/bin`.\n\nIf you encounter other problems during installation, make sure you have Python3.8 or higher, and make sure you have the latest PIP version. If the problem persists, consider installing `scbs` in a clean Python environment (for example using [venv](https://docs.python.org/3/library/venv.html)).\n\n#### Too many open files\nIf you encounter a "too many open files" error during `scbs prepare` (`OSError: [Errno 24] Too many open files`), you need to increase the maximum number of files that can be opened. In Unix systems, try `ulimit -n 9999`.\n\n\n\n## Contributors\n- [Lukas PM Kremer](https://github.com/LKremer)\n- [Martina Braun](https://github.com/martinabraun)\n- [Leonie Küchenhoff](https://github.com/LeonieKuechenhoff)\n- [Alexey Uvarovskii](https://github.com/alexey0308)\n- [Simon Anders](https://github.com/simon-anders)\n',
     'author': 'Lukas PM Kremer',
     'author_email': 'L-Kremer@web.de',
     'maintainer': 'Lukas PM Kremer',
     'maintainer_email': 'L-Kremer@web.de',
     'url': 'https://github.com/LKremer/scbs',
```

### Comparing `scbs-0.6.1/PKG-INFO` & `scbs-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scbs
-Version: 0.6.1
+Version: 0.6.2
 Summary: command line tool for the analysis of single-cell bisulfite-sequencing data
 Home-page: https://github.com/LKremer/scbs
 License: GPL-3.0-or-later
 Keywords: biology,bioinformatics,single cell,methylation,single cell bisulfite sequencing
 Author: Lukas PM Kremer
 Author-email: L-Kremer@web.de
 Maintainer: Lukas PM Kremer
```

