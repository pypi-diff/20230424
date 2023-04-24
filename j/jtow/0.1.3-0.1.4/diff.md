# Comparing `tmp/jtow-0.1.3.tar.gz` & `tmp/jtow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtow-0.1.3.tar", last modified: Fri Apr  1 20:07:34 2022, max compression
+gzip compressed data, was "jtow-0.1.4.tar", last modified: Mon Apr 24 16:57:18 2023, max compression
```

## Comparing `jtow-0.1.3.tar` & `jtow-0.1.4.tar`

### file list

```diff
@@ -1,55 +1,72 @@
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.063934 jtow-0.1.3/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      292 2022-01-01 19:36:37.000000 jtow-0.1.3/.editorconfig
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.058962 jtow-0.1.3/.github/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      315 2022-01-01 19:36:37.000000 jtow-0.1.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1196 2022-01-01 19:36:37.000000 jtow-0.1.3/.gitignore
--rw-r--r--   0 everettschlawin   (501) staff       (20)      678 2022-01-01 19:36:37.000000 jtow-0.1.3/.travis.yml
--rw-r--r--   0 everettschlawin   (501) staff       (20)      175 2022-01-01 19:36:37.000000 jtow-0.1.3/AUTHORS.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3466 2022-01-01 19:36:37.000000 jtow-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       89 2022-01-01 19:36:37.000000 jtow-0.1.3/HISTORY.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1075 2022-01-01 19:36:37.000000 jtow-0.1.3/LICENSE
--rw-r--r--   0 everettschlawin   (501) staff       (20)      262 2022-01-01 19:36:37.000000 jtow-0.1.3/MANIFEST.in
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2185 2022-01-01 19:36:37.000000 jtow-0.1.3/Makefile
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1631 2022-04-01 20:07:34.064029 jtow-0.1.3/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)      821 2022-01-01 19:36:37.000000 jtow-0.1.3/README.rst
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.059263 jtow-0.1.3/bin/
--rwxr-xr-x   0 everettschlawin   (501) staff       (20)      725 2022-04-01 19:16:13.000000 jtow-0.1.3/bin/roeba_run
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.061172 jtow-0.1.3/docs/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      605 2022-01-01 19:36:37.000000 jtow-0.1.3/docs/Makefile
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.055920 jtow-0.1.3/docs/_build/
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.055960 jtow-0.1.3/docs/_build/html/
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.061973 jtow-0.1.3/docs/_build/html/_static/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      286 2022-01-01 19:37:20.000000 jtow-0.1.3/docs/_build/html/_static/file.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2022-01-01 19:37:20.000000 jtow-0.1.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2022-01-01 19:37:20.000000 jtow-0.1.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2022-01-01 19:36:37.000000 jtow-0.1.3/docs/authors.rst
--rwxr-xr-x   0 everettschlawin   (501) staff       (20)     4749 2022-04-01 19:20:48.000000 jtow-0.1.3/docs/conf.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)       33 2022-01-01 19:36:37.000000 jtow-0.1.3/docs/contributing.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2022-01-01 19:36:37.000000 jtow-0.1.3/docs/history.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      320 2022-04-01 19:39:37.000000 jtow-0.1.3/docs/index.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1082 2022-01-01 19:36:37.000000 jtow-0.1.3/docs/installation.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      766 2022-01-01 19:36:37.000000 jtow-0.1.3/docs/make.bat
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1373 2022-04-01 19:16:13.000000 jtow-0.1.3/docs/parameters.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      743 2022-04-01 19:59:55.000000 jtow-0.1.3/docs/quickstart.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       27 2022-01-01 19:36:37.000000 jtow-0.1.3/docs/readme.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       23 2022-04-01 19:35:05.000000 jtow-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.062348 jtow-0.1.3/jtow/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      161 2022-04-01 20:05:27.000000 jtow-0.1.3/jtow/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3676 2022-04-01 19:16:13.000000 jtow-0.1.3/jtow/auto_jtow.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    20413 2022-04-01 19:16:13.000000 jtow-0.1.3/jtow/jtow.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.063369 jtow-0.1.3/jtow/params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      488 2022-04-01 19:16:13.000000 jtow-0.1.3/jtow/params/default_params.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.063231 jtow-0.1.3/jtow.egg-info/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1631 2022-04-01 20:07:33.000000 jtow-0.1.3/jtow.egg-info/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)      803 2022-04-01 20:07:34.000000 jtow-0.1.3/jtow.egg-info/SOURCES.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2022-04-01 20:07:33.000000 jtow-0.1.3/jtow.egg-info/dependency_links.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2022-01-20 04:29:53.000000 jtow-0.1.3/jtow.egg-info/not-zip-safe
--rw-r--r--   0 everettschlawin   (501) staff       (20)       21 2022-04-01 20:07:33.000000 jtow-0.1.3/jtow.egg-info/requires.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        5 2022-04-01 20:07:34.000000 jtow-0.1.3/jtow.egg-info/top_level.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)      148 2022-01-01 19:36:37.000000 jtow-0.1.3/requirements_dev.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)      421 2022-04-01 20:07:34.064336 jtow-0.1.3/setup.cfg
--rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1330 2022-04-01 20:03:49.000000 jtow-0.1.3/setup.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-04-01 20:07:34.063798 jtow-0.1.3/tests/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       34 2022-01-01 19:36:37.000000 jtow-0.1.3/tests/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      544 2022-01-01 19:36:37.000000 jtow-0.1.3/tests/test_jtow.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      535 2022-01-01 19:36:37.000000 jtow-0.1.3/tox.ini
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.217445 jtow-0.1.4/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      292 2022-01-01 19:36:37.000000 jtow-0.1.4/.editorconfig
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.209996 jtow-0.1.4/.github/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      315 2022-01-01 19:36:37.000000 jtow-0.1.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1268 2022-11-30 21:57:26.000000 jtow-0.1.4/.gitignore
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      678 2022-01-01 19:36:37.000000 jtow-0.1.4/.travis.yml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      123 2022-07-01 18:10:06.000000 jtow-0.1.4/AUTHORS.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3466 2022-01-01 19:36:37.000000 jtow-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       89 2022-01-01 19:36:37.000000 jtow-0.1.4/HISTORY.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1075 2022-01-01 19:36:37.000000 jtow-0.1.4/LICENSE
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      262 2022-01-01 19:36:37.000000 jtow-0.1.4/MANIFEST.in
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2185 2022-01-01 19:36:37.000000 jtow-0.1.4/Makefile
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1675 2023-04-24 16:57:18.217499 jtow-0.1.4/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      885 2022-06-19 04:16:55.000000 jtow-0.1.4/README.rst
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.210152 jtow-0.1.4/bin/
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)      725 2022-04-01 19:16:13.000000 jtow-0.1.4/bin/roeba_run
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.212315 jtow-0.1.4/docs/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      605 2022-01-01 19:36:37.000000 jtow-0.1.4/docs/Makefile
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.207121 jtow-0.1.4/docs/_build/
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.207164 jtow-0.1.4/docs/_build/html/
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.212965 jtow-0.1.4/docs/_build/html/_static/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      286 2022-01-01 19:37:20.000000 jtow-0.1.4/docs/_build/html/_static/file.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2022-01-01 19:37:20.000000 jtow-0.1.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2022-01-01 19:37:20.000000 jtow-0.1.4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2022-01-01 19:36:37.000000 jtow-0.1.4/docs/authors.rst
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     4749 2022-04-01 19:20:48.000000 jtow-0.1.4/docs/conf.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       33 2022-01-01 19:36:37.000000 jtow-0.1.4/docs/contributing.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      380 2022-06-19 04:16:55.000000 jtow-0.1.4/docs/default_parameters.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2022-01-01 19:36:37.000000 jtow-0.1.4/docs/history.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      342 2022-06-21 18:13:41.000000 jtow-0.1.4/docs/index.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1082 2022-01-01 19:36:37.000000 jtow-0.1.4/docs/installation.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      766 2022-01-01 19:36:37.000000 jtow-0.1.4/docs/make.bat
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     6805 2022-12-17 22:07:24.000000 jtow-0.1.4/docs/parameters.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      743 2022-04-01 19:59:55.000000 jtow-0.1.4/docs/quickstart.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       27 2022-01-01 19:36:37.000000 jtow-0.1.4/docs/readme.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       23 2022-04-01 19:35:05.000000 jtow-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.214856 jtow-0.1.4/jtow/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      161 2023-04-24 16:52:12.000000 jtow-0.1.4/jtow/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3676 2022-04-01 19:16:13.000000 jtow-0.1.4/jtow/auto_jtow.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1516 2022-11-21 22:02:11.000000 jtow-0.1.4/jtow/examine_cubes.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    41215 2023-04-15 04:34:17.000000 jtow-0.1.4/jtow/jtow.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     6197 2023-04-15 04:34:02.000000 jtow-0.1.4/jtow/make_WL_cube.py
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     3081 2022-08-05 07:35:17.000000 jtow-0.1.4/jtow/make_minisegments.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     4157 2022-08-05 17:34:01.000000 jtow-0.1.4/jtow/make_pairwise_cds.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2065 2022-09-29 15:28:16.000000 jtow-0.1.4/jtow/make_ratio_images.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.215875 jtow-0.1.4/jtow/params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      835 2022-12-17 22:07:02.000000 jtow-0.1.4/jtow/params/default_params.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3068 2023-04-24 16:21:26.000000 jtow-0.1.4/jtow/quick_ff_divide.py
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     4448 2022-12-01 17:47:50.000000 jtow-0.1.4/jtow/temporal_clean.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.215761 jtow-0.1.4/jtow.egg-info/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1675 2023-04-24 16:57:18.000000 jtow-0.1.4/jtow.egg-info/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1323 2023-04-24 16:57:18.000000 jtow-0.1.4/jtow.egg-info/SOURCES.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2023-04-24 16:57:18.000000 jtow-0.1.4/jtow.egg-info/dependency_links.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2022-01-20 04:29:53.000000 jtow-0.1.4/jtow.egg-info/not-zip-safe
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       43 2023-04-24 16:57:18.000000 jtow-0.1.4/jtow.egg-info/requires.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        5 2023-04-24 16:57:18.000000 jtow-0.1.4/jtow.egg-info/top_level.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      148 2022-01-01 19:36:37.000000 jtow-0.1.4/requirements_dev.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      421 2023-04-24 16:57:18.217709 jtow-0.1.4/setup.cfg
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1390 2023-04-24 16:51:49.000000 jtow-0.1.4/setup.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:57:18.217347 jtow-0.1.4/tests/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     6148 2023-04-24 16:56:51.000000 jtow-0.1.4/tests/.DS_Store
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       34 2022-01-01 19:36:37.000000 jtow-0.1.4/tests/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3403 2022-06-26 18:32:44.000000 jtow-0.1.4/tests/jtow_nrca1_custBias_None.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3660 2022-06-25 21:14:01.000000 jtow-0.1.4/tests/jtow_nrca1_custBias_cycleBias.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3043 2022-06-25 21:14:01.000000 jtow-0.1.4/tests/jtow_nrca1_custBias_lineIntercept.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3004 2022-06-25 21:14:01.000000 jtow-0.1.4/tests/jtow_nrca1_custBias_selfBias.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2961 2022-06-25 21:14:01.000000 jtow-0.1.4/tests/jtow_nrca5_custBias_None.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3652 2022-06-25 21:14:01.000000 jtow-0.1.4/tests/jtow_nrca5_custBias_cycleBias.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3043 2022-06-25 21:14:01.000000 jtow-0.1.4/tests/jtow_nrca5_custBias_lineIntercept.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3006 2022-06-25 21:14:01.000000 jtow-0.1.4/tests/jtow_nrca5_custBias_selfBias.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      544 2022-01-01 19:36:37.000000 jtow-0.1.4/tests/test_jtow.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      535 2022-01-01 19:36:37.000000 jtow-0.1.4/tox.ini
```

### Comparing `jtow-0.1.3/.gitignore` & `jtow-0.1.4/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -98,8 +98,14 @@
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
 # IDE settings
-.vscode/
+.vscode/
+
+# emacs backup files
+*~
+
+# ES specific files
+tests/jtow_test_results/
```

### Comparing `jtow-0.1.3/.travis.yml` & `jtow-0.1.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/CONTRIBUTING.rst` & `jtow-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/LICENSE` & `jtow-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/Makefile` & `jtow-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/PKG-INFO` & `jtow-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: jtow
-Version: 0.1.3
+Version: 0.1.4
 Summary: JWST Time series Observation Wrapper.
 Home-page: https://github.com/eas342/jtow
 Author: Everett Schlawin
 Author-email: granfalloontoyballoon@hotmail.com
 License: MIT license
 Keywords: jtow
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -36,23 +35,20 @@
         :alt: Documentation Status
 
 
 
 
 JWST Time series Observation Wrapper.
 
+This code is designed to run the JWST pipeline with some modifications and custom steps.l
 
 * Free software: MIT license
 * Documentation: https://jtow.readthedocs.io.
 
 
-Features
---------
-
-* TODO
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -63,9 +59,7 @@
 History
 =======
 
 0.1.0 (2022-01-01)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `jtow-0.1.3/bin/roeba_run` & `jtow-0.1.4/bin/roeba_run`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/docs/Makefile` & `jtow-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/docs/conf.py` & `jtow-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/docs/installation.rst` & `jtow-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/docs/make.bat` & `jtow-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/docs/quickstart.rst` & `jtow-0.1.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/jtow/auto_jtow.py` & `jtow-0.1.4/jtow/auto_jtow.py`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/jtow.egg-info/PKG-INFO` & `jtow-0.1.4/jtow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: jtow
-Version: 0.1.3
+Version: 0.1.4
 Summary: JWST Time series Observation Wrapper.
 Home-page: https://github.com/eas342/jtow
 Author: Everett Schlawin
 Author-email: granfalloontoyballoon@hotmail.com
 License: MIT license
 Keywords: jtow
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -36,23 +35,20 @@
         :alt: Documentation Status
 
 
 
 
 JWST Time series Observation Wrapper.
 
+This code is designed to run the JWST pipeline with some modifications and custom steps.l
 
 * Free software: MIT license
 * Documentation: https://jtow.readthedocs.io.
 
 
-Features
---------
-
-* TODO
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -63,9 +59,7 @@
 History
 =======
 
 0.1.0 (2022-01-01)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `jtow-0.1.3/setup.py` & `jtow-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ["tshirt >= 0.1dev9",
-                "jwst"]
+requirements = ["tshirt >= 0.2",
+                "jwst",
+                "splintegrate",
+                "scikit-learn"]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Everett Schlawin",
     author_email='granfalloontoyballoon@hotmail.com',
     python_requires='>=3.6',
@@ -37,10 +39,10 @@
     keywords='jtow',
     name='jtow',
     scripts=['bin/roeba_run'],
     packages=find_packages(include=['jtow', 'jtow.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eas342/jtow',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

### Comparing `jtow-0.1.3/tests/test_jtow.py` & `jtow-0.1.4/tests/test_jtow.py`

 * *Files identical despite different names*

### Comparing `jtow-0.1.3/tox.ini` & `jtow-0.1.4/tox.ini`

 * *Files identical despite different names*

