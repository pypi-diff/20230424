# Comparing `tmp/mopac_step-2023.3.31.1.tar.gz` & `tmp/mopac_step-2023.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopac_step-2023.3.31.1.tar", last modified: Fri Mar 31 23:22:47 2023, max compression
+gzip compressed data, was "mopac_step-2023.4.24.tar", last modified: Mon Apr 24 19:42:33 2023, max compression
```

## Comparing `mopac_step-2023.3.31.1.tar` & `mopac_step-2023.4.24.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.520989 mopac_step-2023.3.31.1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-03-31 23:22:47.520989 mopac_step-2023.3.31.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.500989 mopac_step-2023.3.31.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.500989 mopac_step-2023.3.31.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.504989 mopac_step-2023.3.31.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.504989 mopac_step-2023.3.31.1/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.504989 mopac_step-2023.3.31.1/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.504989 mopac_step-2023.3.31.1/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.520989 mopac_step-2023.3.31.1/mopac_step/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-31 23:22:47.520989 mopac_step-2023.3.31.1/mopac_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.520989 mopac_step-2023.3.31.1/mopac_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/data/seamm-mopac.yml
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/forceconstants_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/forceconstants_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/ir_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/ir_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/lewis_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/lewis_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/mopac_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/thermodynamics_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/thermodynamics_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/tk_forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/tk_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/tk_lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/tk_mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/mopac_step/tk_thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.516989 mopac_step-2023.3.31.1/mopac_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-03-31 23:22:47.000000 mopac_step-2023.3.31.1/mopac_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-31 23:22:47.000000 mopac_step-2023.3.31.1/mopac_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:22:47.000000 mopac_step-2023.3.31.1/mopac_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-31 23:22:47.000000 mopac_step-2023.3.31.1/mopac_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 23:22:47.000000 mopac_step-2023.3.31.1/mopac_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 23:22:47.000000 mopac_step-2023.3.31.1/mopac_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:22:37.000000 mopac_step-2023.3.31.1/mopac_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-31 23:22:47.520989 mopac_step-2023.3.31.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:22:47.520989 mopac_step-2023.3.31.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/tests/test_mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-31 23:22:35.000000 mopac_step-2023.3.31.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.049124 mopac_step-2023.4.24/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-24 19:42:33.049124 mopac_step-2023.4.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.037124 mopac_step-2023.4.24/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.041124 mopac_step-2023.4.24/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.041124 mopac_step-2023.4.24/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.041124 mopac_step-2023.4.24/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.041124 mopac_step-2023.4.24/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.041124 mopac_step-2023.4.24/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.053124 mopac_step-2023.4.24/mopac_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 19:42:33.053124 mopac_step-2023.4.24/mopac_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.049124 mopac_step-2023.4.24/mopac_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/data/seamm-mopac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/forceconstants_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/forceconstants_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/ir_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/ir_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/lewis_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/lewis_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/mopac_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/thermodynamics_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/thermodynamics_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/tk_forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/tk_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/tk_lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/tk_mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/mopac_step/tk_thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.049124 mopac_step-2023.4.24/mopac_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-24 19:42:33.000000 mopac_step-2023.4.24/mopac_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 19:42:33.000000 mopac_step-2023.4.24/mopac_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:42:33.000000 mopac_step-2023.4.24/mopac_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-24 19:42:33.000000 mopac_step-2023.4.24/mopac_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 19:42:33.000000 mopac_step-2023.4.24/mopac_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 19:42:33.000000 mopac_step-2023.4.24/mopac_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:42:13.000000 mopac_step-2023.4.24/mopac_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 19:42:33.053124 mopac_step-2023.4.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:33.049124 mopac_step-2023.4.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/tests/test_mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-24 19:42:08.000000 mopac_step-2023.4.24/versioneer.py
```

### Comparing `mopac_step-2023.3.31.1/CONTRIBUTING.rst` & `mopac_step-2023.4.24/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/HISTORY.rst` & `mopac_step-2023.4.24/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2023.4.24 -- Bugfixes for Lewis structure
+  * Correctly handle periodic systems in Lewis structure.
+  * Fixed and issue with the Lewis structure GUI not displaying all the widgets.
+    
 2023.3.31 -- Bugfix
   Lewis structure could reference a variable before it was set, and crash.
   
 2023.3.15 -- Bugfix
   A copy of the input and output files for MOPAC was inadvertently written to the main
   job directory. This has been fixed.
```

### Comparing `mopac_step-2023.3.31.1/LICENSE` & `mopac_step-2023.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/PKG-INFO` & `mopac_step-2023.4.24/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac_step
-Version: 2023.3.31.1
+Version: 2023.4.24
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.4.24 -- Bugfixes for Lewis structure
+  * Correctly handle periodic systems in Lewis structure.
+  * Fixed and issue with the Lewis structure GUI not displaying all the widgets.
+    
 2023.3.31 -- Bugfix
   Lewis structure could reference a variable before it was set, and crash.
   
 2023.3.15 -- Bugfix
   A copy of the input and output files for MOPAC was inadvertently written to the main
   job directory. This has been fixed.
```

### Comparing `mopac_step-2023.3.31.1/README.rst` & `mopac_step-2023.4.24/README.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/Makefile` & `mopac_step-2023.4.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/_static/SEAMM inverted.png` & `mopac_step-2023.4.24/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/_static/SEAMM logo.png` & `mopac_step-2023.4.24/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/_static/molssi_main_logo.png` & `mopac_step-2023.4.24/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/_static/molssi_main_logo_inverted_white.png` & `mopac_step-2023.4.24/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/_static/molssi_square.png` & `mopac_step-2023.4.24/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/_static/nsf.png` & `mopac_step-2023.4.24/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/conf.py` & `mopac_step-2023.4.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/developer_guide/installation.rst` & `mopac_step-2023.4.24/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/getting_started/index.rst` & `mopac_step-2023.4.24/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/index.rst` & `mopac_step-2023.4.24/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/docs/make.bat` & `mopac_step-2023.4.24/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/__init__.py` & `mopac_step-2023.4.24/mopac_step/__init__.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/data/configuration.txt` & `mopac_step-2023.4.24/mopac_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/data/properties.csv` & `mopac_step-2023.4.24/mopac_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/data/references.bib` & `mopac_step-2023.4.24/mopac_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/energy.py` & `mopac_step-2023.4.24/mopac_step/energy.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/energy_parameters.py` & `mopac_step-2023.4.24/mopac_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/energy_step.py` & `mopac_step-2023.4.24/mopac_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/forceconstants.py` & `mopac_step-2023.4.24/mopac_step/forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/forceconstants_parameters.py` & `mopac_step-2023.4.24/mopac_step/forceconstants_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/forceconstants_step.py` & `mopac_step-2023.4.24/mopac_step/forceconstants_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/installer.py` & `mopac_step-2023.4.24/mopac_step/installer.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/ir.py` & `mopac_step-2023.4.24/mopac_step/ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/ir_parameters.py` & `mopac_step-2023.4.24/mopac_step/ir_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/ir_step.py` & `mopac_step-2023.4.24/mopac_step/ir_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/lewis_structure.py` & `mopac_step-2023.4.24/mopac_step/lewis_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
         self._calculation = "Lewis structure"
         self._model = None
         self._metadata = {**mopac_step.metadata}
         # Don't want user to change keywords!
         del self._metadata["keywords"]
         self.parameters = mopac_step.LewisStructureParameters()
+        self._lattice_opt = False
 
     def description_text(self, P=None):
         """Return a short description of this step.
 
         Return a nicely formatted string describing what this step will
         do.
 
@@ -153,15 +154,15 @@
             else:
                 extra_keywords.append(f"MS={(multiplicity - 1) / 2}")
 
         next_node = super().run(printer)
 
         text = ""
         lines = []
-        lines.append(" ".join(["LEWIS", "LET"] + extra_keywords))
+        lines.append(" ".join(["LEWIS", "LET", "GEO-OK"] + extra_keywords))
         lines.append(system.name)
         lines.append(configuration.name)
 
         text += "\n".join(lines)
         text += "\n"
         text += self.mopac_structure()
         text += "\n"
```

### Comparing `mopac_step-2023.3.31.1/mopac_step/lewis_structure_parameters.py` & `mopac_step-2023.4.24/mopac_step/lewis_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/lewis_structure_step.py` & `mopac_step-2023.4.24/mopac_step/lewis_structure_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/metadata.py` & `mopac_step-2023.4.24/mopac_step/metadata.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/mopac.py` & `mopac_step-2023.4.24/mopac_step/mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/mopac_base.py` & `mopac_step-2023.4.24/mopac_step/mopac_base.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/mopac_step.py` & `mopac_step-2023.4.24/mopac_step/mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/optimization.py` & `mopac_step-2023.4.24/mopac_step/optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/optimization_parameters.py` & `mopac_step-2023.4.24/mopac_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/optimization_step.py` & `mopac_step-2023.4.24/mopac_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/thermodynamics.py` & `mopac_step-2023.4.24/mopac_step/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/thermodynamics_parameters.py` & `mopac_step-2023.4.24/mopac_step/thermodynamics_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/thermodynamics_step.py` & `mopac_step-2023.4.24/mopac_step/thermodynamics_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/tk_energy.py` & `mopac_step-2023.4.24/mopac_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/tk_forceconstants.py` & `mopac_step-2023.4.24/mopac_step/tk_forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/tk_ir.py` & `mopac_step-2023.4.24/mopac_step/tk_ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/tk_lewis_structure.py` & `mopac_step-2023.4.24/mopac_step/tk_lewis_structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,24 +51,23 @@
 
     def create_dialog(self, title="Edit Lewis Structure Step"):
         """Create the dialog!"""
         self.logger.debug("Creating the dialog")
         frame = super().create_dialog(title=title)
 
         # Create all the widgets
-        print(type(self.node))
-        print(type(self.node.parameters))
         P = self.node.parameters
         row = 0
         widgets = []
         for key in mopac_step.LewisStructureParameters.parameters:
             if key not in ("results",):
                 w = self[key] = P[key].widget(frame)
                 w.grid(row=row, column=0, sticky=tk.EW)
                 widgets.append(w)
+                row += 1
         sw.align_labels(widgets, sticky=tk.E)
 
         self.setup_results()
 
         self.logger.debug("Finished creating the dialog")
 
         return frame
```

### Comparing `mopac_step-2023.3.31.1/mopac_step/tk_mopac.py` & `mopac_step-2023.4.24/mopac_step/tk_mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/tk_optimization.py` & `mopac_step-2023.4.24/mopac_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step/tk_thermodynamics.py` & `mopac_step-2023.4.24/mopac_step/tk_thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step.egg-info/PKG-INFO` & `mopac_step-2023.4.24/mopac_step.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopac-step
-Version: 2023.3.31.1
+Version: 2023.4.24
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.4.24 -- Bugfixes for Lewis structure
+  * Correctly handle periodic systems in Lewis structure.
+  * Fixed and issue with the Lewis structure GUI not displaying all the widgets.
+    
 2023.3.31 -- Bugfix
   Lewis structure could reference a variable before it was set, and crash.
   
 2023.3.15 -- Bugfix
   A copy of the input and output files for MOPAC was inadvertently written to the main
   job directory. This has been fixed.
```

### Comparing `mopac_step-2023.3.31.1/mopac_step.egg-info/SOURCES.txt` & `mopac_step-2023.4.24/mopac_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/mopac_step.egg-info/entry_points.txt` & `mopac_step-2023.4.24/mopac_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/setup.py` & `mopac_step-2023.4.24/setup.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/tests/test_mopac_step.py` & `mopac_step-2023.4.24/tests/test_mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.3.31.1/versioneer.py` & `mopac_step-2023.4.24/versioneer.py`

 * *Files identical despite different names*

