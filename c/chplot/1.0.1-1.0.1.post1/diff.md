# Comparing `tmp/chplot-1.0.1.tar.gz` & `tmp/chplot-1.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chplot-1.0.1.tar", last modified: Mon Apr 24 15:25:01 2023, max compression
+gzip compressed data, was "chplot-1.0.1.post1.tar", last modified: Mon Apr 24 19:55:52 2023, max compression
```

## Comparing `chplot-1.0.1.tar` & `chplot-1.0.1.post1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:25:01.402002 chplot-1.0.1/
--rw-rw-rw-   0        0        0     1097 2023-02-28 14:01:14.000000 chplot-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    59814 2023-04-24 15:25:01.402002 chplot-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    59387 2023-04-24 15:22:58.000000 chplot-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 15:25:01.335997 chplot-1.0.1/chplot/
--rw-rw-rw-   0        0        0      980 2023-04-24 14:10:24.000000 chplot-1.0.1/chplot/__init__.py
--rw-rw-rw-   0        0        0     8809 2023-04-24 14:33:01.000000 chplot-1.0.1/chplot/__main__.py
--rw-rw-rw-   0        0        0     3207 2023-04-23 13:21:39.000000 chplot-1.0.1/chplot/convert_args.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:25:01.361998 chplot-1.0.1/chplot/functions/
--rw-rw-rw-   0        0        0     2302 2023-04-23 12:24:51.000000 chplot-1.0.1/chplot/functions/__init__.py
--rw-rw-rw-   0        0        0     3844 2023-04-22 12:41:59.000000 chplot-1.0.1/chplot/functions/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:25:01.370998 chplot-1.0.1/chplot/functions/definitions/
--rw-rw-rw-   0        0        0        0 2023-04-23 09:51:17.000000 chplot-1.0.1/chplot/functions/definitions/__init__.py
--rw-rw-rw-   0        0        0      126 2023-04-23 09:57:50.000000 chplot-1.0.1/chplot/functions/definitions/math_functions.py
--rw-rw-rw-   0        0        0       86 2023-04-23 10:00:30.000000 chplot-1.0.1/chplot/functions/definitions/mpmath_functions.py
--rw-rw-rw-   0        0        0     1836 2023-04-24 14:50:10.000000 chplot-1.0.1/chplot/functions/definitions/other_functions.py
--rw-rw-rw-   0        0        0     2857 2023-04-24 14:50:27.000000 chplot-1.0.1/chplot/functions/definitions/probability_functions.py
--rw-rw-rw-   0        0        0      803 2023-04-23 10:27:01.000000 chplot-1.0.1/chplot/functions/definitions/scipy_special_functions.py
--rw-rw-rw-   0        0        0     6057 2023-04-24 14:50:51.000000 chplot-1.0.1/chplot/functions/names.py
--rw-rw-rw-   0        0        0     2930 2023-04-23 09:57:19.000000 chplot-1.0.1/chplot/functions/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:25:01.384997 chplot-1.0.1/chplot/plot/
--rw-rw-rw-   0        0        0       76 2023-04-17 09:20:59.000000 chplot-1.0.1/chplot/plot/__init__.py
--rw-rw-rw-   0        0        0     4945 2023-04-18 15:08:42.000000 chplot-1.0.1/chplot/plot/derivative.py
--rw-rw-rw-   0        0        0     6306 2023-04-20 08:54:04.000000 chplot-1.0.1/chplot/plot/files.py
--rw-rw-rw-   0        0        0     2058 2023-04-24 13:38:31.000000 chplot-1.0.1/chplot/plot/integral.py
--rw-rw-rw-   0        0        0    14663 2023-04-24 14:33:53.000000 chplot-1.0.1/chplot/plot/plot.py
--rw-rw-rw-   0        0        0    10335 2023-04-24 13:06:07.000000 chplot-1.0.1/chplot/plot/plot_parameters.py
--rw-rw-rw-   0        0        0     9336 2023-04-23 12:52:48.000000 chplot-1.0.1/chplot/plot/regression.py
--rw-rw-rw-   0        0        0     1614 2023-04-24 14:14:28.000000 chplot-1.0.1/chplot/plot/utils.py
--rw-rw-rw-   0        0        0     8155 2023-04-18 16:26:23.000000 chplot-1.0.1/chplot/plot/zeros.py
--rw-rw-rw-   0        0        0     4633 2023-04-24 15:00:11.000000 chplot-1.0.1/chplot/rpn.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:25:01.353999 chplot-1.0.1/chplot.egg-info/
--rw-rw-rw-   0        0        0    59814 2023-04-24 15:25:01.000000 chplot-1.0.1/chplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2023-04-24 15:25:01.000000 chplot-1.0.1/chplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:25:01.000000 chplot-1.0.1/chplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-04-24 15:25:01.000000 chplot-1.0.1/chplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 15:25:01.000000 chplot-1.0.1/chplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-03-02 08:00:38.000000 chplot-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-04-24 15:25:01.403998 chplot-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-04-24 15:24:06.000000 chplot-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:25:01.399998 chplot-1.0.1/tests/
--rw-rw-rw-   0        0        0     5941 2023-04-23 13:22:49.000000 chplot-1.0.1/tests/test_cli.py
--rw-rw-rw-   0        0        0     8185 2023-04-23 12:56:26.000000 chplot-1.0.1/tests/test_convert_parameters.py
--rw-rw-rw-   0        0        0     4615 2023-03-21 14:45:08.000000 chplot-1.0.1/tests/test_derivative.py
--rw-rw-rw-   0        0        0     8540 2023-04-20 08:55:39.000000 chplot-1.0.1/tests/test_files.py
--rw-rw-rw-   0        0        0     3404 2023-04-24 13:41:29.000000 chplot-1.0.1/tests/test_integrals.py
--rw-rw-rw-   0        0        0     5869 2023-04-18 16:30:42.000000 chplot-1.0.1/tests/test_plot_graph_lims.py
--rw-rw-rw-   0        0        0      832 2023-04-18 16:30:42.000000 chplot-1.0.1/tests/test_plot_misc.py
--rw-rw-rw-   0        0        0     8341 2023-04-23 12:52:32.000000 chplot-1.0.1/tests/test_regression.py
--rw-rw-rw-   0        0        0     5998 2023-04-23 12:34:35.000000 chplot-1.0.1/tests/test_rpn.py
--rw-rw-rw-   0        0        0     7270 2023-04-23 12:58:03.000000 chplot-1.0.1/tests/test_zeros.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:55:52.292354 chplot-1.0.1.post1/
+-rw-rw-rw-   0        0        0     1097 2023-02-28 14:01:14.000000 chplot-1.0.1.post1/LICENSE
+-rw-rw-rw-   0        0        0    59867 2023-04-24 19:55:52.293340 chplot-1.0.1.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    59434 2023-04-24 19:55:06.000000 chplot-1.0.1.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 19:55:52.218337 chplot-1.0.1.post1/chplot/
+-rw-rw-rw-   0        0        0      980 2023-04-24 14:10:24.000000 chplot-1.0.1.post1/chplot/__init__.py
+-rw-rw-rw-   0        0        0     8809 2023-04-24 14:33:01.000000 chplot-1.0.1.post1/chplot/__main__.py
+-rw-rw-rw-   0        0        0     3207 2023-04-23 13:21:39.000000 chplot-1.0.1.post1/chplot/convert_args.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:55:52.247337 chplot-1.0.1.post1/chplot/functions/
+-rw-rw-rw-   0        0        0     2302 2023-04-23 12:24:51.000000 chplot-1.0.1.post1/chplot/functions/__init__.py
+-rw-rw-rw-   0        0        0     3844 2023-04-22 12:41:59.000000 chplot-1.0.1.post1/chplot/functions/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:55:52.257337 chplot-1.0.1.post1/chplot/functions/definitions/
+-rw-rw-rw-   0        0        0        0 2023-04-23 09:51:17.000000 chplot-1.0.1.post1/chplot/functions/definitions/__init__.py
+-rw-rw-rw-   0        0        0      126 2023-04-23 09:57:50.000000 chplot-1.0.1.post1/chplot/functions/definitions/math_functions.py
+-rw-rw-rw-   0        0        0       86 2023-04-23 10:00:30.000000 chplot-1.0.1.post1/chplot/functions/definitions/mpmath_functions.py
+-rw-rw-rw-   0        0        0     1836 2023-04-24 14:50:10.000000 chplot-1.0.1.post1/chplot/functions/definitions/other_functions.py
+-rw-rw-rw-   0        0        0     2857 2023-04-24 14:50:27.000000 chplot-1.0.1.post1/chplot/functions/definitions/probability_functions.py
+-rw-rw-rw-   0        0        0      803 2023-04-23 10:27:01.000000 chplot-1.0.1.post1/chplot/functions/definitions/scipy_special_functions.py
+-rw-rw-rw-   0        0        0     6057 2023-04-24 14:50:51.000000 chplot-1.0.1.post1/chplot/functions/names.py
+-rw-rw-rw-   0        0        0     2930 2023-04-23 09:57:19.000000 chplot-1.0.1.post1/chplot/functions/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:55:52.274338 chplot-1.0.1.post1/chplot/plot/
+-rw-rw-rw-   0        0        0       76 2023-04-17 09:20:59.000000 chplot-1.0.1.post1/chplot/plot/__init__.py
+-rw-rw-rw-   0        0        0     4945 2023-04-18 15:08:42.000000 chplot-1.0.1.post1/chplot/plot/derivative.py
+-rw-rw-rw-   0        0        0     6306 2023-04-20 08:54:04.000000 chplot-1.0.1.post1/chplot/plot/files.py
+-rw-rw-rw-   0        0        0     2058 2023-04-24 13:38:31.000000 chplot-1.0.1.post1/chplot/plot/integral.py
+-rw-rw-rw-   0        0        0    14663 2023-04-24 14:33:53.000000 chplot-1.0.1.post1/chplot/plot/plot.py
+-rw-rw-rw-   0        0        0    10335 2023-04-24 13:06:07.000000 chplot-1.0.1.post1/chplot/plot/plot_parameters.py
+-rw-rw-rw-   0        0        0     9336 2023-04-23 12:52:48.000000 chplot-1.0.1.post1/chplot/plot/regression.py
+-rw-rw-rw-   0        0        0     1614 2023-04-24 14:14:28.000000 chplot-1.0.1.post1/chplot/plot/utils.py
+-rw-rw-rw-   0        0        0     8155 2023-04-18 16:26:23.000000 chplot-1.0.1.post1/chplot/plot/zeros.py
+-rw-rw-rw-   0        0        0     4633 2023-04-24 15:00:11.000000 chplot-1.0.1.post1/chplot/rpn.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:55:52.240382 chplot-1.0.1.post1/chplot.egg-info/
+-rw-rw-rw-   0        0        0    59867 2023-04-24 19:55:52.000000 chplot-1.0.1.post1/chplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-04-24 19:55:52.000000 chplot-1.0.1.post1/chplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:55:52.000000 chplot-1.0.1.post1/chplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-04-24 19:55:52.000000 chplot-1.0.1.post1/chplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 19:55:52.000000 chplot-1.0.1.post1/chplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-03-02 08:00:38.000000 chplot-1.0.1.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-24 19:55:52.295337 chplot-1.0.1.post1/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-04-24 19:55:11.000000 chplot-1.0.1.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:55:52.291338 chplot-1.0.1.post1/tests/
+-rw-rw-rw-   0        0        0     5941 2023-04-23 13:22:49.000000 chplot-1.0.1.post1/tests/test_cli.py
+-rw-rw-rw-   0        0        0     8185 2023-04-23 12:56:26.000000 chplot-1.0.1.post1/tests/test_convert_parameters.py
+-rw-rw-rw-   0        0        0     4615 2023-03-21 14:45:08.000000 chplot-1.0.1.post1/tests/test_derivative.py
+-rw-rw-rw-   0        0        0     8540 2023-04-20 08:55:39.000000 chplot-1.0.1.post1/tests/test_files.py
+-rw-rw-rw-   0        0        0     3404 2023-04-24 13:41:29.000000 chplot-1.0.1.post1/tests/test_integrals.py
+-rw-rw-rw-   0        0        0     5869 2023-04-18 16:30:42.000000 chplot-1.0.1.post1/tests/test_plot_graph_lims.py
+-rw-rw-rw-   0        0        0      832 2023-04-18 16:30:42.000000 chplot-1.0.1.post1/tests/test_plot_misc.py
+-rw-rw-rw-   0        0        0     8341 2023-04-23 12:52:32.000000 chplot-1.0.1.post1/tests/test_regression.py
+-rw-rw-rw-   0        0        0     5998 2023-04-23 12:34:35.000000 chplot-1.0.1.post1/tests/test_rpn.py
+-rw-rw-rw-   0        0        0     7270 2023-04-23 12:58:03.000000 chplot-1.0.1.post1/tests/test_zeros.py
```

### Comparing `chplot-1.0.1/LICENSE` & `chplot-1.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/PKG-INFO` & `chplot-1.0.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chplot
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: Plot abritrary math expressions, and compute zeros, derivatives, integrals, regression and more!
 Home-page: https://www.github.com/charon25/Chplot
 Download-URL: https://github.com/charon25/Chplot/archive/refs/tags/v1.0.0.tar.gz
 Author: Paul 'charon25' Kern
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -886,15 +886,15 @@
   <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/25.png" width="45%" />
 </p>
 
 ---
 
 #### `-c` parameter
 
-If a constants require another one, define it after:
+If a constant requires another one, define it after:
 ```bash
 python -m chplot a*x+b -c a=2 b=7
 python -m chplot "a*x^2-b*x+1" -c a=8pi/19 "b=a^2-1"
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/26.png" width="45%" />
@@ -928,17 +928,17 @@
 </p>
 
 ---
 
 #### `-d` parameter
 
 ```bash
-python -m chplot x "x(x+1)" "x(x+1)(x+2)/2" "x(x+1)(x+2)(x+3)/6" -s resources\files\saved_data.csv
+python -m chplot x "x(x+1)" "x(x+1)(x+2)/2" "x(x+1)(x+2)(x+3)/6" -d resources\files\saved_data.csv
 ```
-The data can be found in [the saved_data.csv file](resources\files\saved_data.csv).
+The data can be found in [the saved_data.csv file](https://github.com/charon25/Chplot/blob/master/resources/files/saved_data.csv).
 
 ---
 
 #### `-p` parameter
 
 The file `functions.py` must be in the directory from where the command is executed.
 ```bash
```

### Comparing `chplot-1.0.1/README.md` & `chplot-1.0.1.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -874,15 +874,15 @@
   <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/25.png" width="45%" />
 </p>
 
 ---
 
 #### `-c` parameter
 
-If a constants require another one, define it after:
+If a constant requires another one, define it after:
 ```bash
 python -m chplot a*x+b -c a=2 b=7
 python -m chplot "a*x^2-b*x+1" -c a=8pi/19 "b=a^2-1"
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/26.png" width="45%" />
@@ -916,17 +916,17 @@
 </p>
 
 ---
 
 #### `-d` parameter
 
 ```bash
-python -m chplot x "x(x+1)" "x(x+1)(x+2)/2" "x(x+1)(x+2)(x+3)/6" -s resources\files\saved_data.csv
+python -m chplot x "x(x+1)" "x(x+1)(x+2)/2" "x(x+1)(x+2)(x+3)/6" -d resources\files\saved_data.csv
 ```
-The data can be found in [the saved_data.csv file](resources\files\saved_data.csv).
+The data can be found in [the saved_data.csv file](https://github.com/charon25/Chplot/blob/master/resources/files/saved_data.csv).
 
 ---
 
 #### `-p` parameter
 
 The file `functions.py` must be in the directory from where the command is executed.
 ```bash
```

### Comparing `chplot-1.0.1/chplot/__init__.py` & `chplot-1.0.1.post1/chplot/__init__.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/__main__.py` & `chplot-1.0.1.post1/chplot/__main__.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/convert_args.py` & `chplot-1.0.1.post1/chplot/convert_args.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/functions/__init__.py` & `chplot-1.0.1.post1/chplot/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/functions/constants.py` & `chplot-1.0.1.post1/chplot/functions/constants.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/functions/definitions/other_functions.py` & `chplot-1.0.1.post1/chplot/functions/definitions/other_functions.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/functions/definitions/probability_functions.py` & `chplot-1.0.1.post1/chplot/functions/definitions/probability_functions.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/functions/definitions/scipy_special_functions.py` & `chplot-1.0.1.post1/chplot/functions/definitions/scipy_special_functions.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/functions/names.py` & `chplot-1.0.1.post1/chplot/functions/names.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/functions/utils.py` & `chplot-1.0.1.post1/chplot/functions/utils.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/derivative.py` & `chplot-1.0.1.post1/chplot/plot/derivative.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/files.py` & `chplot-1.0.1.post1/chplot/plot/files.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/integral.py` & `chplot-1.0.1.post1/chplot/plot/integral.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/plot.py` & `chplot-1.0.1.post1/chplot/plot/plot.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/plot_parameters.py` & `chplot-1.0.1.post1/chplot/plot/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/regression.py` & `chplot-1.0.1.post1/chplot/plot/regression.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/utils.py` & `chplot-1.0.1.post1/chplot/plot/utils.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/plot/zeros.py` & `chplot-1.0.1.post1/chplot/plot/zeros.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot/rpn.py` & `chplot-1.0.1.post1/chplot/rpn.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/chplot.egg-info/PKG-INFO` & `chplot-1.0.1.post1/chplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chplot
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: Plot abritrary math expressions, and compute zeros, derivatives, integrals, regression and more!
 Home-page: https://www.github.com/charon25/Chplot
 Download-URL: https://github.com/charon25/Chplot/archive/refs/tags/v1.0.0.tar.gz
 Author: Paul 'charon25' Kern
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -886,15 +886,15 @@
   <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/25.png" width="45%" />
 </p>
 
 ---
 
 #### `-c` parameter
 
-If a constants require another one, define it after:
+If a constant requires another one, define it after:
 ```bash
 python -m chplot a*x+b -c a=2 b=7
 python -m chplot "a*x^2-b*x+1" -c a=8pi/19 "b=a^2-1"
 ```
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/charon25/Chplot/master/resources/images/26.png" width="45%" />
@@ -928,17 +928,17 @@
 </p>
 
 ---
 
 #### `-d` parameter
 
 ```bash
-python -m chplot x "x(x+1)" "x(x+1)(x+2)/2" "x(x+1)(x+2)(x+3)/6" -s resources\files\saved_data.csv
+python -m chplot x "x(x+1)" "x(x+1)(x+2)/2" "x(x+1)(x+2)(x+3)/6" -d resources\files\saved_data.csv
 ```
-The data can be found in [the saved_data.csv file](resources\files\saved_data.csv).
+The data can be found in [the saved_data.csv file](https://github.com/charon25/Chplot/blob/master/resources/files/saved_data.csv).
 
 ---
 
 #### `-p` parameter
 
 The file `functions.py` must be in the directory from where the command is executed.
 ```bash
```

### Comparing `chplot-1.0.1/chplot.egg-info/SOURCES.txt` & `chplot-1.0.1.post1/chplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/setup.py` & `chplot-1.0.1.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setuptools.setup(
 	name="chplot",
-	version="1.0.1",
+	version="1.0.1-1",
 	author="Paul 'charon25' Kern",
 	description="Plot abritrary math expressions, and compute zeros, derivatives, integrals, regression and more!",
 	long_description=long_description,
     long_description_content_type='text/markdown',
 	python_requires=">=3.9",
 	url="https://www.github.com/charon25/Chplot",
 	license="MIT",
```

### Comparing `chplot-1.0.1/tests/test_cli.py` & `chplot-1.0.1.post1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_convert_parameters.py` & `chplot-1.0.1.post1/tests/test_convert_parameters.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_derivative.py` & `chplot-1.0.1.post1/tests/test_derivative.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_files.py` & `chplot-1.0.1.post1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_integrals.py` & `chplot-1.0.1.post1/tests/test_integrals.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_plot_graph_lims.py` & `chplot-1.0.1.post1/tests/test_plot_graph_lims.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_plot_misc.py` & `chplot-1.0.1.post1/tests/test_plot_misc.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_regression.py` & `chplot-1.0.1.post1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_rpn.py` & `chplot-1.0.1.post1/tests/test_rpn.py`

 * *Files identical despite different names*

### Comparing `chplot-1.0.1/tests/test_zeros.py` & `chplot-1.0.1.post1/tests/test_zeros.py`

 * *Files identical despite different names*

