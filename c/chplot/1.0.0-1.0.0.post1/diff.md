# Comparing `tmp/chplot-1.0.0.tar.gz` & `tmp/chplot-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chplot-1.0.0.tar", last modified: Mon Apr 24 15:05:37 2023, max compression
+gzip compressed data, was "chplot-1.0.0.post1.tar", last modified: Mon Apr 24 15:14:04 2023, max compression
```

## Comparing `chplot-1.0.0.tar` & `chplot-1.0.0.post1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:05:37.709567 chplot-1.0.0/
--rw-rw-rw-   0        0        0     1097 2023-02-28 14:01:14.000000 chplot-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    57416 2023-04-24 15:05:37.710606 chplot-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    57056 2023-04-24 15:03:13.000000 chplot-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 15:05:37.645623 chplot-1.0.0/chplot/
--rw-rw-rw-   0        0        0      980 2023-04-24 14:10:24.000000 chplot-1.0.0/chplot/__init__.py
--rw-rw-rw-   0        0        0     8809 2023-04-24 14:33:01.000000 chplot-1.0.0/chplot/__main__.py
--rw-rw-rw-   0        0        0     3207 2023-04-23 13:21:39.000000 chplot-1.0.0/chplot/convert_args.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:05:37.670580 chplot-1.0.0/chplot/functions/
--rw-rw-rw-   0        0        0     2302 2023-04-23 12:24:51.000000 chplot-1.0.0/chplot/functions/__init__.py
--rw-rw-rw-   0        0        0     3844 2023-04-22 12:41:59.000000 chplot-1.0.0/chplot/functions/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:05:37.679574 chplot-1.0.0/chplot/functions/definitions/
--rw-rw-rw-   0        0        0        0 2023-04-23 09:51:17.000000 chplot-1.0.0/chplot/functions/definitions/__init__.py
--rw-rw-rw-   0        0        0      126 2023-04-23 09:57:50.000000 chplot-1.0.0/chplot/functions/definitions/math_functions.py
--rw-rw-rw-   0        0        0       86 2023-04-23 10:00:30.000000 chplot-1.0.0/chplot/functions/definitions/mpmath_functions.py
--rw-rw-rw-   0        0        0     1836 2023-04-24 14:50:10.000000 chplot-1.0.0/chplot/functions/definitions/other_functions.py
--rw-rw-rw-   0        0        0     2857 2023-04-24 14:50:27.000000 chplot-1.0.0/chplot/functions/definitions/probability_functions.py
--rw-rw-rw-   0        0        0      803 2023-04-23 10:27:01.000000 chplot-1.0.0/chplot/functions/definitions/scipy_special_functions.py
--rw-rw-rw-   0        0        0     6057 2023-04-24 14:50:51.000000 chplot-1.0.0/chplot/functions/names.py
--rw-rw-rw-   0        0        0     2930 2023-04-23 09:57:19.000000 chplot-1.0.0/chplot/functions/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:05:37.692569 chplot-1.0.0/chplot/plot/
--rw-rw-rw-   0        0        0       76 2023-04-17 09:20:59.000000 chplot-1.0.0/chplot/plot/__init__.py
--rw-rw-rw-   0        0        0     4945 2023-04-18 15:08:42.000000 chplot-1.0.0/chplot/plot/derivative.py
--rw-rw-rw-   0        0        0     6306 2023-04-20 08:54:04.000000 chplot-1.0.0/chplot/plot/files.py
--rw-rw-rw-   0        0        0     2058 2023-04-24 13:38:31.000000 chplot-1.0.0/chplot/plot/integral.py
--rw-rw-rw-   0        0        0    14663 2023-04-24 14:33:53.000000 chplot-1.0.0/chplot/plot/plot.py
--rw-rw-rw-   0        0        0    10335 2023-04-24 13:06:07.000000 chplot-1.0.0/chplot/plot/plot_parameters.py
--rw-rw-rw-   0        0        0     9336 2023-04-23 12:52:48.000000 chplot-1.0.0/chplot/plot/regression.py
--rw-rw-rw-   0        0        0     1614 2023-04-24 14:14:28.000000 chplot-1.0.0/chplot/plot/utils.py
--rw-rw-rw-   0        0        0     8155 2023-04-18 16:26:23.000000 chplot-1.0.0/chplot/plot/zeros.py
--rw-rw-rw-   0        0        0     4633 2023-04-24 15:00:11.000000 chplot-1.0.0/chplot/rpn.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:05:37.664566 chplot-1.0.0/chplot.egg-info/
--rw-rw-rw-   0        0        0    57416 2023-04-24 15:05:37.000000 chplot-1.0.0/chplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-04-24 15:05:37.000000 chplot-1.0.0/chplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:05:37.000000 chplot-1.0.0/chplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-04-24 15:05:37.000000 chplot-1.0.0/chplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 15:05:37.000000 chplot-1.0.0/chplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-03-02 08:00:38.000000 chplot-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-04-24 15:05:37.712567 chplot-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-04-24 15:04:13.000000 chplot-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:05:37.707568 chplot-1.0.0/tests/
--rw-rw-rw-   0        0        0     5941 2023-04-23 13:22:49.000000 chplot-1.0.0/tests/test_cli.py
--rw-rw-rw-   0        0        0     8185 2023-04-23 12:56:26.000000 chplot-1.0.0/tests/test_convert_parameters.py
--rw-rw-rw-   0        0        0     4615 2023-03-21 14:45:08.000000 chplot-1.0.0/tests/test_derivative.py
--rw-rw-rw-   0        0        0     8540 2023-04-20 08:55:39.000000 chplot-1.0.0/tests/test_files.py
--rw-rw-rw-   0        0        0     3404 2023-04-24 13:41:29.000000 chplot-1.0.0/tests/test_integrals.py
--rw-rw-rw-   0        0        0     5869 2023-04-18 16:30:42.000000 chplot-1.0.0/tests/test_plot_graph_lims.py
--rw-rw-rw-   0        0        0      832 2023-04-18 16:30:42.000000 chplot-1.0.0/tests/test_plot_misc.py
--rw-rw-rw-   0        0        0     8341 2023-04-23 12:52:32.000000 chplot-1.0.0/tests/test_regression.py
--rw-rw-rw-   0        0        0     5998 2023-04-23 12:34:35.000000 chplot-1.0.0/tests/test_rpn.py
--rw-rw-rw-   0        0        0     7270 2023-04-23 12:58:03.000000 chplot-1.0.0/tests/test_zeros.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:04.779624 chplot-1.0.0.post1/
+-rw-rw-rw-   0        0        0     1097 2023-02-28 14:01:14.000000 chplot-1.0.0.post1/LICENSE
+-rw-rw-rw-   0        0        0    59759 2023-04-24 15:14:04.780624 chplot-1.0.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    59393 2023-04-24 15:13:12.000000 chplot-1.0.0.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:04.710624 chplot-1.0.0.post1/chplot/
+-rw-rw-rw-   0        0        0      980 2023-04-24 14:10:24.000000 chplot-1.0.0.post1/chplot/__init__.py
+-rw-rw-rw-   0        0        0     8809 2023-04-24 14:33:01.000000 chplot-1.0.0.post1/chplot/__main__.py
+-rw-rw-rw-   0        0        0     3207 2023-04-23 13:21:39.000000 chplot-1.0.0.post1/chplot/convert_args.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:04.737624 chplot-1.0.0.post1/chplot/functions/
+-rw-rw-rw-   0        0        0     2302 2023-04-23 12:24:51.000000 chplot-1.0.0.post1/chplot/functions/__init__.py
+-rw-rw-rw-   0        0        0     3844 2023-04-22 12:41:59.000000 chplot-1.0.0.post1/chplot/functions/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:04.745624 chplot-1.0.0.post1/chplot/functions/definitions/
+-rw-rw-rw-   0        0        0        0 2023-04-23 09:51:17.000000 chplot-1.0.0.post1/chplot/functions/definitions/__init__.py
+-rw-rw-rw-   0        0        0      126 2023-04-23 09:57:50.000000 chplot-1.0.0.post1/chplot/functions/definitions/math_functions.py
+-rw-rw-rw-   0        0        0       86 2023-04-23 10:00:30.000000 chplot-1.0.0.post1/chplot/functions/definitions/mpmath_functions.py
+-rw-rw-rw-   0        0        0     1836 2023-04-24 14:50:10.000000 chplot-1.0.0.post1/chplot/functions/definitions/other_functions.py
+-rw-rw-rw-   0        0        0     2857 2023-04-24 14:50:27.000000 chplot-1.0.0.post1/chplot/functions/definitions/probability_functions.py
+-rw-rw-rw-   0        0        0      803 2023-04-23 10:27:01.000000 chplot-1.0.0.post1/chplot/functions/definitions/scipy_special_functions.py
+-rw-rw-rw-   0        0        0     6057 2023-04-24 14:50:51.000000 chplot-1.0.0.post1/chplot/functions/names.py
+-rw-rw-rw-   0        0        0     2930 2023-04-23 09:57:19.000000 chplot-1.0.0.post1/chplot/functions/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:04.763624 chplot-1.0.0.post1/chplot/plot/
+-rw-rw-rw-   0        0        0       76 2023-04-17 09:20:59.000000 chplot-1.0.0.post1/chplot/plot/__init__.py
+-rw-rw-rw-   0        0        0     4945 2023-04-18 15:08:42.000000 chplot-1.0.0.post1/chplot/plot/derivative.py
+-rw-rw-rw-   0        0        0     6306 2023-04-20 08:54:04.000000 chplot-1.0.0.post1/chplot/plot/files.py
+-rw-rw-rw-   0        0        0     2058 2023-04-24 13:38:31.000000 chplot-1.0.0.post1/chplot/plot/integral.py
+-rw-rw-rw-   0        0        0    14663 2023-04-24 14:33:53.000000 chplot-1.0.0.post1/chplot/plot/plot.py
+-rw-rw-rw-   0        0        0    10335 2023-04-24 13:06:07.000000 chplot-1.0.0.post1/chplot/plot/plot_parameters.py
+-rw-rw-rw-   0        0        0     9336 2023-04-23 12:52:48.000000 chplot-1.0.0.post1/chplot/plot/regression.py
+-rw-rw-rw-   0        0        0     1614 2023-04-24 14:14:28.000000 chplot-1.0.0.post1/chplot/plot/utils.py
+-rw-rw-rw-   0        0        0     8155 2023-04-18 16:26:23.000000 chplot-1.0.0.post1/chplot/plot/zeros.py
+-rw-rw-rw-   0        0        0     4633 2023-04-24 15:00:11.000000 chplot-1.0.0.post1/chplot/rpn.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:04.729624 chplot-1.0.0.post1/chplot.egg-info/
+-rw-rw-rw-   0        0        0    59759 2023-04-24 15:14:04.000000 chplot-1.0.0.post1/chplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-04-24 15:14:04.000000 chplot-1.0.0.post1/chplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:14:04.000000 chplot-1.0.0.post1/chplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-04-24 15:14:04.000000 chplot-1.0.0.post1/chplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 15:14:04.000000 chplot-1.0.0.post1/chplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-03-02 08:00:38.000000 chplot-1.0.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-24 15:14:04.782624 chplot-1.0.0.post1/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-04-24 15:13:54.000000 chplot-1.0.0.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:14:04.778625 chplot-1.0.0.post1/tests/
+-rw-rw-rw-   0        0        0     5941 2023-04-23 13:22:49.000000 chplot-1.0.0.post1/tests/test_cli.py
+-rw-rw-rw-   0        0        0     8185 2023-04-23 12:56:26.000000 chplot-1.0.0.post1/tests/test_convert_parameters.py
+-rw-rw-rw-   0        0        0     4615 2023-03-21 14:45:08.000000 chplot-1.0.0.post1/tests/test_derivative.py
+-rw-rw-rw-   0        0        0     8540 2023-04-20 08:55:39.000000 chplot-1.0.0.post1/tests/test_files.py
+-rw-rw-rw-   0        0        0     3404 2023-04-24 13:41:29.000000 chplot-1.0.0.post1/tests/test_integrals.py
+-rw-rw-rw-   0        0        0     5869 2023-04-18 16:30:42.000000 chplot-1.0.0.post1/tests/test_plot_graph_lims.py
+-rw-rw-rw-   0        0        0      832 2023-04-18 16:30:42.000000 chplot-1.0.0.post1/tests/test_plot_misc.py
+-rw-rw-rw-   0        0        0     8341 2023-04-23 12:52:32.000000 chplot-1.0.0.post1/tests/test_regression.py
+-rw-rw-rw-   0        0        0     5998 2023-04-23 12:34:35.000000 chplot-1.0.0.post1/tests/test_rpn.py
+-rw-rw-rw-   0        0        0     7270 2023-04-23 12:58:03.000000 chplot-1.0.0.post1/tests/test_zeros.py
```

### Comparing `chplot-1.0.0/LICENSE` & `chplot-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/PKG-INFO` & `chplot-1.0.0.post1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-Metadata-Version: 2.1
-Name: chplot
-Version: 1.0.0
-Summary: Fast plot any math expression
-Home-page: https://www.github.com/charon25/Chplot
-Download-URL: https://github.com/charon25/Chplot/archive/refs/tags/v1.0.0.tar.gz
-Author: Paul 'charon25' Kern
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Chplot - Arbitrary functions plotting and computations
 
 Chplot is a Python >= 3.9 module to plot any arbitrary mathematical expressions as well as data series from files, and compute its derivatives and integrals, where it equals zero, linear and non-linear regressions, and much more !
 
 <p align="center">
-  <img src="resources/images/logo.png">
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/logo.png">
 </p>
 
 ## Installation
 
-You can install `chplot` through Pypi, with the command:
+`chplot` is available [on Pypi](https://pypi.org/project/chplot/#files), and You can install it with the command:
 ```bash
 python -m pip install chplot
 ```
 
 You can also install it by cloning this repo and installing it directly:
 ```bash
 git clone https://github.com/charon25/Chplot.git
@@ -696,147 +684,147 @@
 
 ```bash
 python -m chplot x
 python -m chplot x " -x+1" "x^2"
 ```
 
 <p align="center">
-  <img src="resources/images/01.png" width="45%" />
-  <img src="resources/images/02.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/01.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/02.png" width="45%" />
 </p>
 
 ```bash
 python -m chplot resources/files/equations.txt
 ```
 
 <p align="center">
-  <img src="resources/images/03.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/03.png" width="45%" />
 </p>
 
 ---
 
 #### `-v` parameter
 
 ```bash
 python -m chplot t(t-1) -v t
 python -m chplot sin(var*3) -v var
 ```
 
 <p align="center">
-  <img src="resources/images/04.png" width="45%" />
-  <img src="resources/images/05.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/04.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/05.png" width="45%" />
 </p>
 
 ------
 
 Overriding constant with variable:
 ```bash
 python -m chplot c
 python -m chplot c -v c
 ```
 
 <p align="center">
-  <img src="resources/images/06.png" width="45%" />
-  <img src="resources/images/07.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/06.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/07.png" width="45%" />
 </p>
 
 ---
 
 #### `--no-sn`
 
 The expression in the first command is interpreted as $x\times1.2\cdot10^{-1}=0.12x$, and as $1.2\mathrm{e}\cdot x - 1$ in the second.
 ```bash
 python -m chplot "x*1.2e-1"
 python -m chplot "x*1.2e-1" --no-sn
 ```
 
 <p align="center">
-  <img src="resources/images/38.png" width="45%" />
-  <img src="resources/images/39.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/38.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/39.png" width="45%" />
 </p>
 
 ---
 
 #### `-x`, `-y` parameters
 
 Using expressions in the horizontal axis bounds:
 ```bash
 python -m chplot "x^2+x" -x -3 3
 python -m chplot x -x " -sqrt(2)" "zeta(3)"
 ```
 
 <p align="center">
-  <img src="resources/images/08.png" width="45%" />
-  <img src="resources/images/09.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/08.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/09.png" width="45%" />
 </p>
 
 Using expressions in the vertical axis bounds and restricting the graph:
 ```bash
 python -m chplot fac(x) -x 0 6
 python -m chplot fac(x) -x 0 6 -y 0.5 1.5
 ```
 
 <p align="center">
-  <img src="resources/images/10.png" width="45%" />
-  <img src="resources/images/11.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/10.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/11.png" width="45%" />
 </p>
 
 ---
 
 #### `-n`, `-i`, `--dis` parameters
 
 The `-i` parameter removes the line between points.
 ```bash
 python -m chplot cos(x) -x 0 10 -n 20
 python -m chplot cos(x) -x 0 10 -i
 ```
 
 <p align="center">
-  <img src="resources/images/12.png" width="45%" />
-  <img src="resources/images/13.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/12.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/13.png" width="45%" />
 </p>
 
 ---
 
 ```bash
 python -m chplot sqrt(x) -x 0 100 -i
 python -m chplot sqrt(x) -x 0 10 --dis 10 -n 35
 ```
 
 <p align="center">
-  <img src="resources/images/14.png" width="45%" />
-  <img src="resources/images/15.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/14.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/15.png" width="45%" />
 </p>
 
 ---
 
 #### `-xlog`, `-ylog` parameters
 
 ```bash
 python -m chplot "2^x" -x 1 100 -ylog
 python -m chplot "ln(x)" -x 1 100 -xlog
 ```
 
 <p align="center">
-  <img src="resources/images/16.png" width="45%" />
-  <img src="resources/images/17.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/16.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/17.png" width="45%" />
 </p>
 
 ---
 
 Log axis will adjust the bounds to remove negative points:
 ```bash
 python -m chplot "x^3.5" -x 1 100 -xlog -ylog
 python -m chplot "x" -x -5 5 -xlog
 python -m chplot "x" -x -5 -1 -xlog
 ```
 
 <p align="center">
-  <img src="resources/images/18.png" width="45%" />
-  <img src="resources/images/19.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/18.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/19.png" width="45%" />
 </p>
 
 The second command generates a warning:
 ```
 [CHPLOT] WARNING: x-axis scale is logarithmic, but its lower bound (-5.0) is negative, x-axis will be truncated to positive values
 ```
 The third command generates en error:
@@ -850,85 +838,85 @@
 
 ```bash
 python -m chplot "sin(x)+10" -x 1 10pi
 python -m chplot "sin(x)+10" -x 1 10pi -z
 ```
 
 <p align="center">
-  <img src="resources/images/20.png" width="45%" />
-  <img src="resources/images/21.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/20.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/21.png" width="45%" />
 </p>
 
 ---
 
 #### `-xl`, `-yl`, `-t`, `-rl` parameters
 
 ```bash
 python -m chplot zeta(x) -x 1 10 -y 0 3
 python -m chplot zeta(x) -x 1 10 -y 0 3 -xl "Variable x" -yl "Zeta(x)" -t "Zeta function on [1 ; 10]" -rl
 ```
 
 <p align="center">
-  <img src="resources/images/22.png" width="45%" />
-  <img src="resources/images/23.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/22.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/23.png" width="45%" />
 </p>
 
 ---
 
 #### `-square`, `-lw` parameters
 
 ```bash
 python -m chplot cbrt(x) --square
 python -m chplot cbrt(x) -lw 5
 ```
 
 <p align="center">
-  <img src="resources/images/24.png" width="45%" />
-  <img src="resources/images/25.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/24.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/25.png" width="45%" />
 </p>
 
 ---
 
 #### `-c` parameter
 
 If a constants require another one, define it after:
 ```bash
 python -m chplot a*x+b -c a=2 b=7
 python -m chplot "a*x^2-b*x+1" -c a=8pi/19 "b=a^2-1"
 ```
 
 <p align="center">
-  <img src="resources/images/26.png" width="45%" />
-  <img src="resources/images/27.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/26.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/27.png" width="45%" />
 </p>
 
 ---
 
 Constants can also be an expression, or come from a file:
 ```bash
 python -m chplot cos(a*x) -c "a=(sqrt(2) - zeta(3)) / sin(1.5)" -x 0 50
 python -m chplot "a*x^3+b*x^2+c*x+d" -c resources\files\constants.txt -x -10 10
 ```
 
 <p align="center">
-  <img src="resources/images/28.png" width="45%" />
-  <img src="resources/images/29.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/28.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/29.png" width="45%" />
 </p>
 
 ---
 
 #### `-f` parameter
 
 All the CSV format are summarized in the [CSV files format](#csv-files-format) section.
 ```bash
 python -m chplot -f resources\files\data.csv
 ```
 
 <p align="center">
-  <img src="resources/images/30.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/30.png" width="45%" />
 </p>
 
 ---
 
 #### `-d` parameter
 
 ```bash
@@ -942,15 +930,15 @@
 
 The file `functions.py` must be in the directory from where the command is executed.
 ```bash
 python -m chplot "frac(x)+3" "is_prime(x)" "rnd(x, x/2)" -p functions.py -x 0 10
 ```
 
 <p align="center">
-  <img src="resources/images/31.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/31.png" width="45%" />
 </p>
 
 ---
 
 #### `--zeros`
 
 ```bash
@@ -1021,16 +1009,16 @@
 The second command illustrates the instability of the higher order derivatives.
 ```bash
 python -m chplot "sin(x)" --deriv 1 2 3 4 -x 0 4pi
 python -m chplot "exp(x)" --deriv 1 4 7 -n 100000
 ```
 
 <p align="center">
-  <img src="resources/images/32.png" width="45%" />
-  <img src="resources/images/33.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/32.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/33.png" width="45%" />
 </p>
 
 ---
 
 Synergy between `--deriv` and `--zeros`/`--integral`.
 ```bash
 python -m chplot "x^2+2" -x -3 3 --deriv 1 --zeros --integral
@@ -1066,15 +1054,15 @@
 
 Default keyword usable in the CLI.
 ```bash
 python -m chplot "sin(x)" " -exp(x)" --reg lin
 ```
 
 <p align="center">
-  <img src="resources/images/34.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/34.png" width="45%" />
 </p>
 
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a * x + b
@@ -1111,15 +1099,15 @@
 
 Arbitrary expression for regression (here: $a + \frac{b}{x} + \frac{c}{x^2}$).
 ```bash
 python -m chplot "x" "x^2-3x+2" -x 1 2 --reg "_ra + _rb/x + _rc/x^2" 
 ```
 
 <p align="center">
-  <img src="resources/images/35.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/35.png" width="45%" />
 </p>
 
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a + b/x + c/x^2
@@ -1158,15 +1146,15 @@
 
 Regression on file data.
 ```bash
 python -m chplot -f resources\files\data.csv --reg poly2
 ```
 
 <p align="center">
-  <img src="resources/images/37.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/37.png" width="45%" />
 </p>
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a2 * x^2 + a1 * x + a0
 
@@ -1205,15 +1193,15 @@
 Synergy between `--reg` and `--deriv`/`--zeros`/`--integral`.
 
 ```bash
 python -m chplot log2(x) -x 1 3 --deriv 1 --reg lin --zeros --integral
 ```
 
 <p align="center">
-  <img src="resources/images/36.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/36.png" width="45%" />
 </p>
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a * x + b
```

### Comparing `chplot-1.0.0/README.md` & `chplot-1.0.0.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+Metadata-Version: 2.1
+Name: chplot
+Version: 1.0.0.post1
+Summary: Fast plot any math expression
+Home-page: https://www.github.com/charon25/Chplot
+Download-URL: https://github.com/charon25/Chplot/archive/refs/tags/v1.0.0.tar.gz
+Author: Paul 'charon25' Kern
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Chplot - Arbitrary functions plotting and computations
 
 Chplot is a Python >= 3.9 module to plot any arbitrary mathematical expressions as well as data series from files, and compute its derivatives and integrals, where it equals zero, linear and non-linear regressions, and much more !
 
 <p align="center">
-  <img src="resources/images/logo.png">
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/logo.png">
 </p>
 
 ## Installation
 
-You can install `chplot` through Pypi, with the command:
+`chplot` is available [on Pypi](https://pypi.org/project/chplot/#files), and You can install it with the command:
 ```bash
 python -m pip install chplot
 ```
 
 You can also install it by cloning this repo and installing it directly:
 ```bash
 git clone https://github.com/charon25/Chplot.git
@@ -684,147 +696,147 @@
 
 ```bash
 python -m chplot x
 python -m chplot x " -x+1" "x^2"
 ```
 
 <p align="center">
-  <img src="resources/images/01.png" width="45%" />
-  <img src="resources/images/02.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/01.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/02.png" width="45%" />
 </p>
 
 ```bash
 python -m chplot resources/files/equations.txt
 ```
 
 <p align="center">
-  <img src="resources/images/03.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/03.png" width="45%" />
 </p>
 
 ---
 
 #### `-v` parameter
 
 ```bash
 python -m chplot t(t-1) -v t
 python -m chplot sin(var*3) -v var
 ```
 
 <p align="center">
-  <img src="resources/images/04.png" width="45%" />
-  <img src="resources/images/05.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/04.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/05.png" width="45%" />
 </p>
 
 ------
 
 Overriding constant with variable:
 ```bash
 python -m chplot c
 python -m chplot c -v c
 ```
 
 <p align="center">
-  <img src="resources/images/06.png" width="45%" />
-  <img src="resources/images/07.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/06.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/07.png" width="45%" />
 </p>
 
 ---
 
 #### `--no-sn`
 
 The expression in the first command is interpreted as $x\times1.2\cdot10^{-1}=0.12x$, and as $1.2\mathrm{e}\cdot x - 1$ in the second.
 ```bash
 python -m chplot "x*1.2e-1"
 python -m chplot "x*1.2e-1" --no-sn
 ```
 
 <p align="center">
-  <img src="resources/images/38.png" width="45%" />
-  <img src="resources/images/39.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/38.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/39.png" width="45%" />
 </p>
 
 ---
 
 #### `-x`, `-y` parameters
 
 Using expressions in the horizontal axis bounds:
 ```bash
 python -m chplot "x^2+x" -x -3 3
 python -m chplot x -x " -sqrt(2)" "zeta(3)"
 ```
 
 <p align="center">
-  <img src="resources/images/08.png" width="45%" />
-  <img src="resources/images/09.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/08.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/09.png" width="45%" />
 </p>
 
 Using expressions in the vertical axis bounds and restricting the graph:
 ```bash
 python -m chplot fac(x) -x 0 6
 python -m chplot fac(x) -x 0 6 -y 0.5 1.5
 ```
 
 <p align="center">
-  <img src="resources/images/10.png" width="45%" />
-  <img src="resources/images/11.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/10.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/11.png" width="45%" />
 </p>
 
 ---
 
 #### `-n`, `-i`, `--dis` parameters
 
 The `-i` parameter removes the line between points.
 ```bash
 python -m chplot cos(x) -x 0 10 -n 20
 python -m chplot cos(x) -x 0 10 -i
 ```
 
 <p align="center">
-  <img src="resources/images/12.png" width="45%" />
-  <img src="resources/images/13.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/12.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/13.png" width="45%" />
 </p>
 
 ---
 
 ```bash
 python -m chplot sqrt(x) -x 0 100 -i
 python -m chplot sqrt(x) -x 0 10 --dis 10 -n 35
 ```
 
 <p align="center">
-  <img src="resources/images/14.png" width="45%" />
-  <img src="resources/images/15.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/14.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/15.png" width="45%" />
 </p>
 
 ---
 
 #### `-xlog`, `-ylog` parameters
 
 ```bash
 python -m chplot "2^x" -x 1 100 -ylog
 python -m chplot "ln(x)" -x 1 100 -xlog
 ```
 
 <p align="center">
-  <img src="resources/images/16.png" width="45%" />
-  <img src="resources/images/17.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/16.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/17.png" width="45%" />
 </p>
 
 ---
 
 Log axis will adjust the bounds to remove negative points:
 ```bash
 python -m chplot "x^3.5" -x 1 100 -xlog -ylog
 python -m chplot "x" -x -5 5 -xlog
 python -m chplot "x" -x -5 -1 -xlog
 ```
 
 <p align="center">
-  <img src="resources/images/18.png" width="45%" />
-  <img src="resources/images/19.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/18.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/19.png" width="45%" />
 </p>
 
 The second command generates a warning:
 ```
 [CHPLOT] WARNING: x-axis scale is logarithmic, but its lower bound (-5.0) is negative, x-axis will be truncated to positive values
 ```
 The third command generates en error:
@@ -838,85 +850,85 @@
 
 ```bash
 python -m chplot "sin(x)+10" -x 1 10pi
 python -m chplot "sin(x)+10" -x 1 10pi -z
 ```
 
 <p align="center">
-  <img src="resources/images/20.png" width="45%" />
-  <img src="resources/images/21.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/20.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/21.png" width="45%" />
 </p>
 
 ---
 
 #### `-xl`, `-yl`, `-t`, `-rl` parameters
 
 ```bash
 python -m chplot zeta(x) -x 1 10 -y 0 3
 python -m chplot zeta(x) -x 1 10 -y 0 3 -xl "Variable x" -yl "Zeta(x)" -t "Zeta function on [1 ; 10]" -rl
 ```
 
 <p align="center">
-  <img src="resources/images/22.png" width="45%" />
-  <img src="resources/images/23.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/22.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/23.png" width="45%" />
 </p>
 
 ---
 
 #### `-square`, `-lw` parameters
 
 ```bash
 python -m chplot cbrt(x) --square
 python -m chplot cbrt(x) -lw 5
 ```
 
 <p align="center">
-  <img src="resources/images/24.png" width="45%" />
-  <img src="resources/images/25.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/24.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/25.png" width="45%" />
 </p>
 
 ---
 
 #### `-c` parameter
 
 If a constants require another one, define it after:
 ```bash
 python -m chplot a*x+b -c a=2 b=7
 python -m chplot "a*x^2-b*x+1" -c a=8pi/19 "b=a^2-1"
 ```
 
 <p align="center">
-  <img src="resources/images/26.png" width="45%" />
-  <img src="resources/images/27.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/26.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/27.png" width="45%" />
 </p>
 
 ---
 
 Constants can also be an expression, or come from a file:
 ```bash
 python -m chplot cos(a*x) -c "a=(sqrt(2) - zeta(3)) / sin(1.5)" -x 0 50
 python -m chplot "a*x^3+b*x^2+c*x+d" -c resources\files\constants.txt -x -10 10
 ```
 
 <p align="center">
-  <img src="resources/images/28.png" width="45%" />
-  <img src="resources/images/29.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/28.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/29.png" width="45%" />
 </p>
 
 ---
 
 #### `-f` parameter
 
 All the CSV format are summarized in the [CSV files format](#csv-files-format) section.
 ```bash
 python -m chplot -f resources\files\data.csv
 ```
 
 <p align="center">
-  <img src="resources/images/30.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/30.png" width="45%" />
 </p>
 
 ---
 
 #### `-d` parameter
 
 ```bash
@@ -930,15 +942,15 @@
 
 The file `functions.py` must be in the directory from where the command is executed.
 ```bash
 python -m chplot "frac(x)+3" "is_prime(x)" "rnd(x, x/2)" -p functions.py -x 0 10
 ```
 
 <p align="center">
-  <img src="resources/images/31.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/31.png" width="45%" />
 </p>
 
 ---
 
 #### `--zeros`
 
 ```bash
@@ -1009,16 +1021,16 @@
 The second command illustrates the instability of the higher order derivatives.
 ```bash
 python -m chplot "sin(x)" --deriv 1 2 3 4 -x 0 4pi
 python -m chplot "exp(x)" --deriv 1 4 7 -n 100000
 ```
 
 <p align="center">
-  <img src="resources/images/32.png" width="45%" />
-  <img src="resources/images/33.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/32.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/33.png" width="45%" />
 </p>
 
 ---
 
 Synergy between `--deriv` and `--zeros`/`--integral`.
 ```bash
 python -m chplot "x^2+2" -x -3 3 --deriv 1 --zeros --integral
@@ -1054,15 +1066,15 @@
 
 Default keyword usable in the CLI.
 ```bash
 python -m chplot "sin(x)" " -exp(x)" --reg lin
 ```
 
 <p align="center">
-  <img src="resources/images/34.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/34.png" width="45%" />
 </p>
 
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a * x + b
@@ -1099,15 +1111,15 @@
 
 Arbitrary expression for regression (here: $a + \frac{b}{x} + \frac{c}{x^2}$).
 ```bash
 python -m chplot "x" "x^2-3x+2" -x 1 2 --reg "_ra + _rb/x + _rc/x^2" 
 ```
 
 <p align="center">
-  <img src="resources/images/35.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/35.png" width="45%" />
 </p>
 
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a + b/x + c/x^2
@@ -1146,15 +1158,15 @@
 
 Regression on file data.
 ```bash
 python -m chplot -f resources\files\data.csv --reg poly2
 ```
 
 <p align="center">
-  <img src="resources/images/37.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/37.png" width="45%" />
 </p>
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a2 * x^2 + a1 * x + a0
 
@@ -1193,15 +1205,15 @@
 Synergy between `--reg` and `--deriv`/`--zeros`/`--integral`.
 
 ```bash
 python -m chplot log2(x) -x 1 3 --deriv 1 --reg lin --zeros --integral
 ```
 
 <p align="center">
-  <img src="resources/images/36.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/36.png" width="45%" />
 </p>
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a * x + b
```

### Comparing `chplot-1.0.0/chplot/__init__.py` & `chplot-1.0.0.post1/chplot/__init__.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/__main__.py` & `chplot-1.0.0.post1/chplot/__main__.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/convert_args.py` & `chplot-1.0.0.post1/chplot/convert_args.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/functions/__init__.py` & `chplot-1.0.0.post1/chplot/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/functions/constants.py` & `chplot-1.0.0.post1/chplot/functions/constants.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/functions/definitions/other_functions.py` & `chplot-1.0.0.post1/chplot/functions/definitions/other_functions.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/functions/definitions/probability_functions.py` & `chplot-1.0.0.post1/chplot/functions/definitions/probability_functions.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/functions/definitions/scipy_special_functions.py` & `chplot-1.0.0.post1/chplot/functions/definitions/scipy_special_functions.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/functions/names.py` & `chplot-1.0.0.post1/chplot/functions/names.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/functions/utils.py` & `chplot-1.0.0.post1/chplot/functions/utils.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/derivative.py` & `chplot-1.0.0.post1/chplot/plot/derivative.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/files.py` & `chplot-1.0.0.post1/chplot/plot/files.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/integral.py` & `chplot-1.0.0.post1/chplot/plot/integral.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/plot.py` & `chplot-1.0.0.post1/chplot/plot/plot.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/plot_parameters.py` & `chplot-1.0.0.post1/chplot/plot/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/regression.py` & `chplot-1.0.0.post1/chplot/plot/regression.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/utils.py` & `chplot-1.0.0.post1/chplot/plot/utils.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/plot/zeros.py` & `chplot-1.0.0.post1/chplot/plot/zeros.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot/rpn.py` & `chplot-1.0.0.post1/chplot/rpn.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/chplot.egg-info/PKG-INFO` & `chplot-1.0.0.post1/chplot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: chplot
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Fast plot any math expression
 Home-page: https://www.github.com/charon25/Chplot
 Download-URL: https://github.com/charon25/Chplot/archive/refs/tags/v1.0.0.tar.gz
 Author: Paul 'charon25' Kern
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chplot - Arbitrary functions plotting and computations
 
 Chplot is a Python >= 3.9 module to plot any arbitrary mathematical expressions as well as data series from files, and compute its derivatives and integrals, where it equals zero, linear and non-linear regressions, and much more !
 
 <p align="center">
-  <img src="resources/images/logo.png">
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/logo.png">
 </p>
 
 ## Installation
 
-You can install `chplot` through Pypi, with the command:
+`chplot` is available [on Pypi](https://pypi.org/project/chplot/#files), and You can install it with the command:
 ```bash
 python -m pip install chplot
 ```
 
 You can also install it by cloning this repo and installing it directly:
 ```bash
 git clone https://github.com/charon25/Chplot.git
@@ -696,147 +696,147 @@
 
 ```bash
 python -m chplot x
 python -m chplot x " -x+1" "x^2"
 ```
 
 <p align="center">
-  <img src="resources/images/01.png" width="45%" />
-  <img src="resources/images/02.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/01.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/02.png" width="45%" />
 </p>
 
 ```bash
 python -m chplot resources/files/equations.txt
 ```
 
 <p align="center">
-  <img src="resources/images/03.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/03.png" width="45%" />
 </p>
 
 ---
 
 #### `-v` parameter
 
 ```bash
 python -m chplot t(t-1) -v t
 python -m chplot sin(var*3) -v var
 ```
 
 <p align="center">
-  <img src="resources/images/04.png" width="45%" />
-  <img src="resources/images/05.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/04.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/05.png" width="45%" />
 </p>
 
 ------
 
 Overriding constant with variable:
 ```bash
 python -m chplot c
 python -m chplot c -v c
 ```
 
 <p align="center">
-  <img src="resources/images/06.png" width="45%" />
-  <img src="resources/images/07.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/06.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/07.png" width="45%" />
 </p>
 
 ---
 
 #### `--no-sn`
 
 The expression in the first command is interpreted as $x\times1.2\cdot10^{-1}=0.12x$, and as $1.2\mathrm{e}\cdot x - 1$ in the second.
 ```bash
 python -m chplot "x*1.2e-1"
 python -m chplot "x*1.2e-1" --no-sn
 ```
 
 <p align="center">
-  <img src="resources/images/38.png" width="45%" />
-  <img src="resources/images/39.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/38.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/39.png" width="45%" />
 </p>
 
 ---
 
 #### `-x`, `-y` parameters
 
 Using expressions in the horizontal axis bounds:
 ```bash
 python -m chplot "x^2+x" -x -3 3
 python -m chplot x -x " -sqrt(2)" "zeta(3)"
 ```
 
 <p align="center">
-  <img src="resources/images/08.png" width="45%" />
-  <img src="resources/images/09.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/08.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/09.png" width="45%" />
 </p>
 
 Using expressions in the vertical axis bounds and restricting the graph:
 ```bash
 python -m chplot fac(x) -x 0 6
 python -m chplot fac(x) -x 0 6 -y 0.5 1.5
 ```
 
 <p align="center">
-  <img src="resources/images/10.png" width="45%" />
-  <img src="resources/images/11.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/10.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/11.png" width="45%" />
 </p>
 
 ---
 
 #### `-n`, `-i`, `--dis` parameters
 
 The `-i` parameter removes the line between points.
 ```bash
 python -m chplot cos(x) -x 0 10 -n 20
 python -m chplot cos(x) -x 0 10 -i
 ```
 
 <p align="center">
-  <img src="resources/images/12.png" width="45%" />
-  <img src="resources/images/13.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/12.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/13.png" width="45%" />
 </p>
 
 ---
 
 ```bash
 python -m chplot sqrt(x) -x 0 100 -i
 python -m chplot sqrt(x) -x 0 10 --dis 10 -n 35
 ```
 
 <p align="center">
-  <img src="resources/images/14.png" width="45%" />
-  <img src="resources/images/15.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/14.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/15.png" width="45%" />
 </p>
 
 ---
 
 #### `-xlog`, `-ylog` parameters
 
 ```bash
 python -m chplot "2^x" -x 1 100 -ylog
 python -m chplot "ln(x)" -x 1 100 -xlog
 ```
 
 <p align="center">
-  <img src="resources/images/16.png" width="45%" />
-  <img src="resources/images/17.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/16.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/17.png" width="45%" />
 </p>
 
 ---
 
 Log axis will adjust the bounds to remove negative points:
 ```bash
 python -m chplot "x^3.5" -x 1 100 -xlog -ylog
 python -m chplot "x" -x -5 5 -xlog
 python -m chplot "x" -x -5 -1 -xlog
 ```
 
 <p align="center">
-  <img src="resources/images/18.png" width="45%" />
-  <img src="resources/images/19.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/18.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/19.png" width="45%" />
 </p>
 
 The second command generates a warning:
 ```
 [CHPLOT] WARNING: x-axis scale is logarithmic, but its lower bound (-5.0) is negative, x-axis will be truncated to positive values
 ```
 The third command generates en error:
@@ -850,85 +850,85 @@
 
 ```bash
 python -m chplot "sin(x)+10" -x 1 10pi
 python -m chplot "sin(x)+10" -x 1 10pi -z
 ```
 
 <p align="center">
-  <img src="resources/images/20.png" width="45%" />
-  <img src="resources/images/21.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/20.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/21.png" width="45%" />
 </p>
 
 ---
 
 #### `-xl`, `-yl`, `-t`, `-rl` parameters
 
 ```bash
 python -m chplot zeta(x) -x 1 10 -y 0 3
 python -m chplot zeta(x) -x 1 10 -y 0 3 -xl "Variable x" -yl "Zeta(x)" -t "Zeta function on [1 ; 10]" -rl
 ```
 
 <p align="center">
-  <img src="resources/images/22.png" width="45%" />
-  <img src="resources/images/23.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/22.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/23.png" width="45%" />
 </p>
 
 ---
 
 #### `-square`, `-lw` parameters
 
 ```bash
 python -m chplot cbrt(x) --square
 python -m chplot cbrt(x) -lw 5
 ```
 
 <p align="center">
-  <img src="resources/images/24.png" width="45%" />
-  <img src="resources/images/25.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/24.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/25.png" width="45%" />
 </p>
 
 ---
 
 #### `-c` parameter
 
 If a constants require another one, define it after:
 ```bash
 python -m chplot a*x+b -c a=2 b=7
 python -m chplot "a*x^2-b*x+1" -c a=8pi/19 "b=a^2-1"
 ```
 
 <p align="center">
-  <img src="resources/images/26.png" width="45%" />
-  <img src="resources/images/27.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/26.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/27.png" width="45%" />
 </p>
 
 ---
 
 Constants can also be an expression, or come from a file:
 ```bash
 python -m chplot cos(a*x) -c "a=(sqrt(2) - zeta(3)) / sin(1.5)" -x 0 50
 python -m chplot "a*x^3+b*x^2+c*x+d" -c resources\files\constants.txt -x -10 10
 ```
 
 <p align="center">
-  <img src="resources/images/28.png" width="45%" />
-  <img src="resources/images/29.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/28.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/29.png" width="45%" />
 </p>
 
 ---
 
 #### `-f` parameter
 
 All the CSV format are summarized in the [CSV files format](#csv-files-format) section.
 ```bash
 python -m chplot -f resources\files\data.csv
 ```
 
 <p align="center">
-  <img src="resources/images/30.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/30.png" width="45%" />
 </p>
 
 ---
 
 #### `-d` parameter
 
 ```bash
@@ -942,15 +942,15 @@
 
 The file `functions.py` must be in the directory from where the command is executed.
 ```bash
 python -m chplot "frac(x)+3" "is_prime(x)" "rnd(x, x/2)" -p functions.py -x 0 10
 ```
 
 <p align="center">
-  <img src="resources/images/31.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/31.png" width="45%" />
 </p>
 
 ---
 
 #### `--zeros`
 
 ```bash
@@ -1021,16 +1021,16 @@
 The second command illustrates the instability of the higher order derivatives.
 ```bash
 python -m chplot "sin(x)" --deriv 1 2 3 4 -x 0 4pi
 python -m chplot "exp(x)" --deriv 1 4 7 -n 100000
 ```
 
 <p align="center">
-  <img src="resources/images/32.png" width="45%" />
-  <img src="resources/images/33.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/32.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/33.png" width="45%" />
 </p>
 
 ---
 
 Synergy between `--deriv` and `--zeros`/`--integral`.
 ```bash
 python -m chplot "x^2+2" -x -3 3 --deriv 1 --zeros --integral
@@ -1066,15 +1066,15 @@
 
 Default keyword usable in the CLI.
 ```bash
 python -m chplot "sin(x)" " -exp(x)" --reg lin
 ```
 
 <p align="center">
-  <img src="resources/images/34.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/34.png" width="45%" />
 </p>
 
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a * x + b
@@ -1111,15 +1111,15 @@
 
 Arbitrary expression for regression (here: $a + \frac{b}{x} + \frac{c}{x^2}$).
 ```bash
 python -m chplot "x" "x^2-3x+2" -x 1 2 --reg "_ra + _rb/x + _rc/x^2" 
 ```
 
 <p align="center">
-  <img src="resources/images/35.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/35.png" width="45%" />
 </p>
 
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a + b/x + c/x^2
@@ -1158,15 +1158,15 @@
 
 Regression on file data.
 ```bash
 python -m chplot -f resources\files\data.csv --reg poly2
 ```
 
 <p align="center">
-  <img src="resources/images/37.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/37.png" width="45%" />
 </p>
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a2 * x^2 + a1 * x + a0
 
@@ -1205,15 +1205,15 @@
 Synergy between `--reg` and `--deriv`/`--zeros`/`--integral`.
 
 ```bash
 python -m chplot log2(x) -x 1 3 --deriv 1 --reg lin --zeros --integral
 ```
 
 <p align="center">
-  <img src="resources/images/36.png" width="45%" />
+  <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/36.png" width="45%" />
 </p>
 
 ```bash
 ===== REGRESSION COEFFICIENTS OF THE FUNCTIONS =====
 
 Regression function: reg(x) = a * x + b
```

### Comparing `chplot-1.0.0/chplot.egg-info/SOURCES.txt` & `chplot-1.0.0.post1/chplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/setup.py` & `chplot-1.0.0.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setuptools.setup(
 	name="chplot",
-	version="1.0.0",
+	version="1.0.0-1",
 	author="Paul 'charon25' Kern",
 	description="Fast plot any math expression",
 	long_description=long_description,
     long_description_content_type='text/markdown',
 	python_requires=">=3.9",
 	url="https://www.github.com/charon25/Chplot",
 	license="MIT",
```

### Comparing `chplot-1.0.0/tests/test_cli.py` & `chplot-1.0.0.post1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_convert_parameters.py` & `chplot-1.0.0.post1/tests/test_convert_parameters.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_derivative.py` & `chplot-1.0.0.post1/tests/test_derivative.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_files.py` & `chplot-1.0.0.post1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_integrals.py` & `chplot-1.0.0.post1/tests/test_integrals.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_plot_graph_lims.py` & `chplot-1.0.0.post1/tests/test_plot_graph_lims.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_plot_misc.py` & `chplot-1.0.0.post1/tests/test_plot_misc.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_regression.py` & `chplot-1.0.0.post1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_rpn.py` & `chplot-1.0.0.post1/tests/test_rpn.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.0/tests/test_zeros.py` & `chplot-1.0.0.post1/tests/test_zeros.py`

 * *Files identical despite different names*

