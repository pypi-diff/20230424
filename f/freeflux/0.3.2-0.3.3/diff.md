# Comparing `tmp/freeflux-0.3.2.tar.gz` & `tmp/freeflux-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\cwu\Desktop\Software\FreeFlux\pypi\freeflux-0.3.2\dist\.tmp-663xfpld\freeflux-0.3.2.tar", last modified: Mon Apr 24 08:09:51 2023, max compression
+gzip compressed data, was "C:\Users\cwu\Desktop\Software\FreeFlux\pypi\freeflux-0.3.3\dist\.tmp-ho6do_pt\freeflux-0.3.3.tar", last modified: Mon Apr 24 08:23:57 2023, max compression
```

## Comparing `freeflux-0.3.2.tar` & `freeflux-0.3.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.786969 freeflux-0.3.2/
--rw-rw-rw-   0        0        0    35149 2022-08-18 01:02:32.000000 freeflux-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     5239 2023-04-24 08:09:51.787965 freeflux-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4188 2023-04-07 06:00:51.000000 freeflux-0.3.2/README.rst
--rw-rw-rw-   0        0        0       90 2023-04-03 02:02:48.000000 freeflux-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0     1234 2023-04-24 08:09:51.791954 freeflux-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-04-18 21:36:18.000000 freeflux-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.596477 freeflux-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.632383 freeflux-0.3.2/src/freeflux/
--rw-rw-rw-   0        0        0      247 2023-04-24 07:58:25.000000 freeflux-0.3.2/src/freeflux/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.683246 freeflux-0.3.2/src/freeflux/analysis/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.2/src/freeflux/analysis/__init__.py
--rw-rw-rw-   0        0        0    23297 2023-04-18 21:42:54.000000 freeflux-0.3.2/src/freeflux/analysis/fit.py
--rw-rw-rw-   0        0        0    21603 2023-04-18 21:44:20.000000 freeflux-0.3.2/src/freeflux/analysis/inst_fit.py
--rw-rw-rw-   0        0        0     6538 2023-04-18 21:44:44.000000 freeflux-0.3.2/src/freeflux/analysis/inst_simulate.py
--rw-rw-rw-   0        0        0    10165 2023-04-18 21:46:20.000000 freeflux-0.3.2/src/freeflux/analysis/simulate.py
--rw-rw-rw-   0        0        0    12497 2023-04-24 08:02:13.000000 freeflux-0.3.2/src/freeflux/analysis/stats.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.712167 freeflux-0.3.2/src/freeflux/core/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.2/src/freeflux/core/__init__.py
--rw-rw-rw-   0        0        0     4989 2023-04-18 21:49:39.000000 freeflux-0.3.2/src/freeflux/core/emu.py
--rw-rw-rw-   0        0        0    12887 2023-04-24 08:02:34.000000 freeflux-0.3.2/src/freeflux/core/mdv.py
--rw-rw-rw-   0        0        0     2553 2023-03-31 21:40:13.000000 freeflux-0.3.2/src/freeflux/core/metabolite.py
--rw-rw-rw-   0        0        0    35901 2023-04-18 21:53:25.000000 freeflux-0.3.2/src/freeflux/core/model.py
--rw-rw-rw-   0        0        0    11011 2023-04-18 21:49:24.000000 freeflux-0.3.2/src/freeflux/core/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.728126 freeflux-0.3.2/src/freeflux/io/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:20.000000 freeflux-0.3.2/src/freeflux/io/__init__.py
--rw-rw-rw-   0        0        0     3147 2023-04-24 07:59:36.000000 freeflux-0.3.2/src/freeflux/io/inputs.py
--rw-rw-rw-   0        0        0    33246 2023-04-24 08:03:00.000000 freeflux-0.3.2/src/freeflux/io/results.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.739096 freeflux-0.3.2/src/freeflux/optim/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:49.000000 freeflux-0.3.2/src/freeflux/optim/__init__.py
--rw-rw-rw-   0        0        0     9270 2023-04-18 21:54:53.000000 freeflux-0.3.2/src/freeflux/optim/optim.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.755053 freeflux-0.3.2/src/freeflux/solver/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:33:01.000000 freeflux-0.3.2/src/freeflux/solver/__init__.py
--rw-rw-rw-   0        0        0     3375 2023-04-01 23:47:14.000000 freeflux-0.3.2/src/freeflux/solver/lpsolver.py
--rw-rw-rw-   0        0        0    19803 2023-04-24 08:03:20.000000 freeflux-0.3.2/src/freeflux/solver/nlpsolver.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.779987 freeflux-0.3.2/src/freeflux/utils/
--rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.2/src/freeflux/utils/__init__.py
--rw-rw-rw-   0        0        0      496 2023-03-26 22:55:07.000000 freeflux-0.3.2/src/freeflux/utils/context.py
--rw-rw-rw-   0        0        0     1916 2023-04-01 23:41:09.000000 freeflux-0.3.2/src/freeflux/utils/progress.py
--rw-rw-rw-   0        0        0    33624 2023-04-24 08:06:34.000000 freeflux-0.3.2/src/freeflux/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:09:51.653327 freeflux-0.3.2/src/freeflux.egg-info/
--rw-rw-rw-   0        0        0     5239 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 08:09:51.000000 freeflux-0.3.2/src/freeflux.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.231616 freeflux-0.3.3/
+-rw-rw-rw-   0        0        0    35149 2022-08-18 01:02:32.000000 freeflux-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     5239 2023-04-24 08:23:57.232615 freeflux-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4188 2023-04-07 06:00:51.000000 freeflux-0.3.3/README.rst
+-rw-rw-rw-   0        0        0       90 2023-04-03 02:02:48.000000 freeflux-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1232 2023-04-24 08:23:57.237600 freeflux-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-04-18 21:36:18.000000 freeflux-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.057083 freeflux-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.091990 freeflux-0.3.3/src/freeflux/
+-rw-rw-rw-   0        0        0      247 2023-04-24 08:23:21.000000 freeflux-0.3.3/src/freeflux/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.138865 freeflux-0.3.3/src/freeflux/analysis/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.3/src/freeflux/analysis/__init__.py
+-rw-rw-rw-   0        0        0    23297 2023-04-18 21:42:54.000000 freeflux-0.3.3/src/freeflux/analysis/fit.py
+-rw-rw-rw-   0        0        0    21603 2023-04-18 21:44:20.000000 freeflux-0.3.3/src/freeflux/analysis/inst_fit.py
+-rw-rw-rw-   0        0        0     6538 2023-04-18 21:44:44.000000 freeflux-0.3.3/src/freeflux/analysis/inst_simulate.py
+-rw-rw-rw-   0        0        0    10165 2023-04-18 21:46:20.000000 freeflux-0.3.3/src/freeflux/analysis/simulate.py
+-rw-rw-rw-   0        0        0    12497 2023-04-24 08:02:13.000000 freeflux-0.3.3/src/freeflux/analysis/stats.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.166791 freeflux-0.3.3/src/freeflux/core/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.3/src/freeflux/core/__init__.py
+-rw-rw-rw-   0        0        0     4989 2023-04-18 21:49:39.000000 freeflux-0.3.3/src/freeflux/core/emu.py
+-rw-rw-rw-   0        0        0    12887 2023-04-24 08:02:34.000000 freeflux-0.3.3/src/freeflux/core/mdv.py
+-rw-rw-rw-   0        0        0     2553 2023-03-31 21:40:13.000000 freeflux-0.3.3/src/freeflux/core/metabolite.py
+-rw-rw-rw-   0        0        0    35901 2023-04-18 21:53:25.000000 freeflux-0.3.3/src/freeflux/core/model.py
+-rw-rw-rw-   0        0        0    11011 2023-04-18 21:49:24.000000 freeflux-0.3.3/src/freeflux/core/reaction.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.180753 freeflux-0.3.3/src/freeflux/io/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:20.000000 freeflux-0.3.3/src/freeflux/io/__init__.py
+-rw-rw-rw-   0        0        0     3147 2023-04-24 07:59:36.000000 freeflux-0.3.3/src/freeflux/io/inputs.py
+-rw-rw-rw-   0        0        0    33246 2023-04-24 08:03:00.000000 freeflux-0.3.3/src/freeflux/io/results.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.190728 freeflux-0.3.3/src/freeflux/optim/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:49.000000 freeflux-0.3.3/src/freeflux/optim/__init__.py
+-rw-rw-rw-   0        0        0     9270 2023-04-18 21:54:53.000000 freeflux-0.3.3/src/freeflux/optim/optim.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.204690 freeflux-0.3.3/src/freeflux/solver/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:33:01.000000 freeflux-0.3.3/src/freeflux/solver/__init__.py
+-rw-rw-rw-   0        0        0     3375 2023-04-01 23:47:14.000000 freeflux-0.3.3/src/freeflux/solver/lpsolver.py
+-rw-rw-rw-   0        0        0    19803 2023-04-24 08:03:20.000000 freeflux-0.3.3/src/freeflux/solver/nlpsolver.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.225635 freeflux-0.3.3/src/freeflux/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-28 23:32:26.000000 freeflux-0.3.3/src/freeflux/utils/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-03-26 22:55:07.000000 freeflux-0.3.3/src/freeflux/utils/context.py
+-rw-rw-rw-   0        0        0     1916 2023-04-01 23:41:09.000000 freeflux-0.3.3/src/freeflux/utils/progress.py
+-rw-rw-rw-   0        0        0    33624 2023-04-24 08:06:34.000000 freeflux-0.3.3/src/freeflux/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:23:57.110941 freeflux-0.3.3/src/freeflux.egg-info/
+-rw-rw-rw-   0        0        0     5239 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 08:23:57.000000 freeflux-0.3.3/src/freeflux.egg-info/top_level.txt
```

### Comparing `freeflux-0.3.2/LICENSE` & `freeflux-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/PKG-INFO` & `freeflux-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeflux
-Version: 0.3.2
+Version: 0.3.3
 Summary: FreeFlux is a package for 13C metabolic flux analysis
 Home-page: https://github.com/Chaowu88/freeflux
 Author: Chao Wu
 Author-email: chaowu09@gmail.com
 License: GNU General Public License v3.0
 Keywords: 13c,labeling pattern,metabolic flux analysis,metabolism,biology,non-linear programming,optimization,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freeflux-0.3.2/README.rst` & `freeflux-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/setup.cfg` & `freeflux-0.3.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 7265 6566 6c75 780d 0a76 6572   = freeflux..ver
-00000020: 7369 6f6e 203d 2030 2e33 2e32 0d0a 6175  sion = 0.3.2..au
+00000020: 7369 6f6e 203d 2030 2e33 2e33 0d0a 6175  sion = 0.3.3..au
 00000030: 7468 6f72 203d 2043 6861 6f20 5775 0d0a  thor = Chao Wu..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2063  author_email = c
 00000050: 6861 6f77 7530 3940 676d 6169 6c2e 636f  haowu09@gmail.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2046 7265 6546 6c75 7820 6973 2061 2070   FreeFlux is a p
 00000080: 6163 6b61 6765 2066 6f72 2031 3343 206d  ackage for 13C m
 00000090: 6574 6162 6f6c 6963 2066 6c75 7820 616e  etabolic flux an
@@ -56,23 +56,22 @@
 00000370: 300d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  0....[options]..
 00000380: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 00000390: 3d20 3e3d 2033 2e37 0d0a 696e 7374 616c  = >= 3.7..instal
 000003a0: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
 000003b0: 6e75 6d70 7920 3e3d 2031 2e32 302c 203c  numpy >= 1.20, <
 000003c0: 2031 2e32 330d 0a09 7061 6e64 6173 207e   1.23...pandas ~
 000003d0: 3d20 312e 300d 0a09 7379 6d70 7920 7e3d  = 1.0...sympy ~=
-000003e0: 2031 2e36 2e31 0d0a 0973 6369 7079 203e   1.6.1...scipy >
-000003f0: 3d20 312e 352c 203c 2031 2e38 0d0a 0970  = 1.5, < 1.8...p
-00000400: 796f 6d6f 203e 3d20 362e 322c 203c 3d20  yomo >= 6.2, <= 
-00000410: 362e 350d 0a09 6d61 7470 6c6f 746c 6962  6.5...matplotlib
-00000420: 203e 3d20 332e 322c 203c 3d20 332e 370d   >= 3.2, <= 3.7.
-00000430: 0a09 7069 6c6c 6f77 0d0a 0978 6c72 6420  ..pillow...xlrd 
-00000440: 3d3d 2031 2e32 2e30 0d0a 096f 7065 6e70  == 1.2.0...openp
-00000450: 7978 6c0d 0a70 6163 6b61 6765 5f64 6972  yxl..package_dir
-00000460: 203d 200d 0a09 3d73 7263 0d0a 7061 636b   = ...=src..pack
-00000470: 6167 6573 203d 2066 696e 643a 0d0a 0d0a  ages = find:....
-00000480: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000490: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-000004a0: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-000004b0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000004c0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000004d0: 0d0a                                     ..
+000003e0: 2031 2e36 0d0a 0973 6369 7079 203e 3d20   1.6...scipy >= 
+000003f0: 312e 352c 203c 2031 2e39 0d0a 0970 796f  1.5, < 1.9...pyo
+00000400: 6d6f 203e 3d20 362e 322c 203c 3d20 362e  mo >= 6.2, <= 6.
+00000410: 350d 0a09 6d61 7470 6c6f 746c 6962 203e  5...matplotlib >
+00000420: 3d20 332e 322c 203c 3d20 332e 370d 0a09  = 3.2, <= 3.7...
+00000430: 7069 6c6c 6f77 0d0a 0978 6c72 6420 3d3d  pillow...xlrd ==
+00000440: 2031 2e32 2e30 0d0a 096f 7065 6e70 7978   1.2.0...openpyx
+00000450: 6c0d 0a70 6163 6b61 6765 5f64 6972 203d  l..package_dir =
+00000460: 200d 0a09 3d73 7263 0d0a 7061 636b 6167   ...=src..packag
+00000470: 6573 203d 2066 696e 643a 0d0a 0d0a 5b6f  es = find:....[o
+00000480: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000490: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+000004a0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
+000004b0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000004c0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `freeflux-0.3.2/src/freeflux/analysis/fit.py` & `freeflux-0.3.3/src/freeflux/analysis/fit.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/analysis/inst_fit.py` & `freeflux-0.3.3/src/freeflux/analysis/inst_fit.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/analysis/inst_simulate.py` & `freeflux-0.3.3/src/freeflux/analysis/inst_simulate.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/analysis/simulate.py` & `freeflux-0.3.3/src/freeflux/analysis/simulate.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/analysis/stats.py` & `freeflux-0.3.3/src/freeflux/analysis/stats.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/core/emu.py` & `freeflux-0.3.3/src/freeflux/core/emu.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/core/mdv.py` & `freeflux-0.3.3/src/freeflux/core/mdv.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/core/metabolite.py` & `freeflux-0.3.3/src/freeflux/core/metabolite.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/core/model.py` & `freeflux-0.3.3/src/freeflux/core/model.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/core/reaction.py` & `freeflux-0.3.3/src/freeflux/core/reaction.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/io/inputs.py` & `freeflux-0.3.3/src/freeflux/io/inputs.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/io/results.py` & `freeflux-0.3.3/src/freeflux/io/results.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/optim/optim.py` & `freeflux-0.3.3/src/freeflux/optim/optim.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/solver/lpsolver.py` & `freeflux-0.3.3/src/freeflux/solver/lpsolver.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/solver/nlpsolver.py` & `freeflux-0.3.3/src/freeflux/solver/nlpsolver.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/utils/progress.py` & `freeflux-0.3.3/src/freeflux/utils/progress.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux/utils/utils.py` & `freeflux-0.3.3/src/freeflux/utils/utils.py`

 * *Files identical despite different names*

### Comparing `freeflux-0.3.2/src/freeflux.egg-info/PKG-INFO` & `freeflux-0.3.3/src/freeflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeflux
-Version: 0.3.2
+Version: 0.3.3
 Summary: FreeFlux is a package for 13C metabolic flux analysis
 Home-page: https://github.com/Chaowu88/freeflux
 Author: Chao Wu
 Author-email: chaowu09@gmail.com
 License: GNU General Public License v3.0
 Keywords: 13c,labeling pattern,metabolic flux analysis,metabolism,biology,non-linear programming,optimization,simulation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freeflux-0.3.2/src/freeflux.egg-info/SOURCES.txt` & `freeflux-0.3.3/src/freeflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

