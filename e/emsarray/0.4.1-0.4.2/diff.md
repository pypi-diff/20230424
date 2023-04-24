# Comparing `tmp/emsarray-0.4.1.tar.gz` & `tmp/emsarray-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emsarray-0.4.1.tar", last modified: Wed Feb  8 06:39:40 2023, max compression
+gzip compressed data, was "emsarray-0.4.2.tar", last modified: Mon Apr 24 05:08:21 2023, max compression
```

## Comparing `emsarray-0.4.1.tar` & `emsarray-0.4.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.490536 emsarray-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-02-08 06:39:31.000000 emsarray-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-02-08 06:39:40.490536 emsarray-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-08 06:39:31.000000 emsarray-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-08 06:39:31.000000 emsarray-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-08 06:39:40.490536 emsarray-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 06:39:31.000000 emsarray-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.474536 emsarray-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.482536 emsarray-0.4.1/src/emsarray/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/accessors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.486536 emsarray-0.4.1/src/emsarray/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.486536 emsarray-0.4.1/src/emsarray/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/commands/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/commands/export_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/commands/extract_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.490536 emsarray-0.4.1/src/emsarray/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/compat/shapely.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.490536 emsarray-0.4.1/src/emsarray/conventions/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45292 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/arakawa_c.py
--rw-r--r--   0 runner    (1001) docker     (123)    19472 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/shoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    52965 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/conventions/ugrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/nco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.490536 emsarray-0.4.1/src/emsarray/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/operations/depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/operations/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/operations/point_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/operations/triangulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    23122 2023-02-08 06:39:31.000000 emsarray-0.4.1/src/emsarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.486536 emsarray-0.4.1/src/emsarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-02-08 06:39:40.000000 emsarray-0.4.1/src/emsarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-02-08 06:39:40.000000 emsarray-0.4.1/src/emsarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 06:39:40.000000 emsarray-0.4.1/src/emsarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-08 06:39:40.000000 emsarray-0.4.1/src/emsarray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-08 06:39:40.000000 emsarray-0.4.1/src/emsarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-08 06:39:40.000000 emsarray-0.4.1/src/emsarray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:39:40.490536 emsarray-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-02-08 06:39:31.000000 emsarray-0.4.1/tests/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-08 06:39:31.000000 emsarray-0.4.1/tests/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-08 06:39:31.000000 emsarray-0.4.1/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-08 06:39:31.000000 emsarray-0.4.1/tests/test_get_dataset_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-02-08 06:39:31.000000 emsarray-0.4.1/tests/test_nco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-08 06:39:31.000000 emsarray-0.4.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-02-08 06:39:31.000000 emsarray-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 05:08:11.000000 emsarray-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-24 05:08:21.395366 emsarray-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-24 05:08:11.000000 emsarray-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-24 05:08:11.000000 emsarray-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-24 05:08:21.395366 emsarray-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:08:11.000000 emsarray-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.387366 emsarray-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/accessors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/export_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/commands/extract_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/compat/shapely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/src/emsarray/conventions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45292 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/arakawa_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19472 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/shoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52965 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/conventions/ugrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/nco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/src/emsarray/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/point_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/operations/triangulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23259 2023-04-24 05:08:11.000000 emsarray-0.4.2/src/emsarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.391366 emsarray-0.4.2/src/emsarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 05:08:21.000000 emsarray-0.4.2/src/emsarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:08:21.395366 emsarray-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_get_dataset_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_nco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-24 05:08:11.000000 emsarray-0.4.2/tests/test_utils.py
```

### Comparing `emsarray-0.4.1/LICENSE` & `emsarray-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/PKG-INFO` & `emsarray-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: emsarray
-Version: 0.4.1
+Version: 0.4.2
 Summary: xarray extension that supports multiple geometry conventions
 Author: "Coastal Environmental Modelling team, Oceans and Atmosphere, CSIRO"
 Author-email: "coasts@csiro.au"
 License: "BSD-3-Clause"
 Project-URL: Documentation, https://emsarray.readthedocs.io/
-Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.1/
+Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.2/
 Project-URL: Source, https://github.com/csiro-coasts/emsarray/
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 Provides-Extra: tutorial
 Provides-Extra: complete
 Provides-Extra: docs
 Provides-Extra: testing
```

### Comparing `emsarray-0.4.1/README.md` & `emsarray-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/pyproject.toml` & `emsarray-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/setup.cfg` & `emsarray-0.4.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = emsarray
 description = xarray extension that supports multiple geometry conventions
-version = 0.4.1
+version = 0.4.2
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "Coastal Environmental Modelling team, Oceans and Atmosphere, CSIRO"
 author_email = "coasts@csiro.au"
 license = "BSD-3-Clause"
 project_urls = 
 	Documentation = https://emsarray.readthedocs.io/
-	Release notes = https://emsarray.readthedocs.io/en/stable/releases/0.4.1/
+	Release notes = https://emsarray.readthedocs.io/en/stable/releases/0.4.2/
 	Source = https://github.com/csiro-coasts/emsarray/
 
 [options]
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
```

### Comparing `emsarray-0.4.1/src/emsarray/__init__.py` & `emsarray-0.4.2/src/emsarray/__init__.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/accessors.py` & `emsarray-0.4.2/src/emsarray/accessors.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/cli/__init__.py` & `emsarray-0.4.2/src/emsarray/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/cli/command.py` & `emsarray-0.4.2/src/emsarray/cli/command.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/cli/commands/clip.py` & `emsarray-0.4.2/src/emsarray/cli/commands/clip.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/cli/commands/export_geometry.py` & `emsarray-0.4.2/src/emsarray/cli/commands/export_geometry.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/cli/commands/extract_points.py` & `emsarray-0.4.2/src/emsarray/cli/commands/extract_points.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/cli/utils.py` & `emsarray-0.4.2/src/emsarray/cli/utils.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/compat/shapely.py` & `emsarray-0.4.2/src/emsarray/compat/shapely.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/__init__.py` & `emsarray-0.4.2/src/emsarray/conventions/__init__.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/_base.py` & `emsarray-0.4.2/src/emsarray/conventions/_base.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/_registry.py` & `emsarray-0.4.2/src/emsarray/conventions/_registry.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/_utils.py` & `emsarray-0.4.2/src/emsarray/conventions/_utils.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/arakawa_c.py` & `emsarray-0.4.2/src/emsarray/conventions/arakawa_c.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/grid.py` & `emsarray-0.4.2/src/emsarray/conventions/grid.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/shoc.py` & `emsarray-0.4.2/src/emsarray/conventions/shoc.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/conventions/ugrid.py` & `emsarray-0.4.2/src/emsarray/conventions/ugrid.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/exceptions.py` & `emsarray-0.4.2/src/emsarray/exceptions.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/formats.py` & `emsarray-0.4.2/src/emsarray/formats.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/masking.py` & `emsarray-0.4.2/src/emsarray/masking.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import logging
 import operator
 import pathlib
 from typing import Any, Dict, Hashable, List, cast
 
 import numpy as np
 import xarray as xr
+from xarray.core.dtypes import maybe_promote
 
 from emsarray import utils
 from emsarray.types import Pathish
 
 logger = logging.getLogger(__name__)
 
 
@@ -67,15 +68,14 @@
 
     logger.info("Applying masks...")
     # This is done variable-by-variable, as trying to do it to the entire
     # dataset is very memory intensive. This allows us to offload data to the
     # file system, at the added expense of having to recombine the dataset
     # afterwards.
     for key, data_array in dataset.data_vars.items():
-        logger.debug("DataArray %s", key)
         masked_data_array = mask_grid_data_array(mask, data_array)
         variable_path = work_path / f"{key}.nc"
         mfdataset_names.append(variable_path)
         utils.to_netcdf_with_fixes(masked_data_array.to_dataset(name=key), variable_path)
         del masked_data_array
 
     # Coordinates are handled differently. They have been trimmed already, but
@@ -126,27 +126,36 @@
         the original data array is returned unmodified.
     """
     dimensions = set(data_array.dims)
 
     try:
         fill_value = find_fill_value(data_array)
     except ValueError:
+        logger.debug(
+            "Data array %r has no valid fill value, leaving as is",
+            data_array.name)
         return data_array
 
     # Loop through each possible mask
     for mask_name, mask_data_array in mask.data_vars.items():
         # If every dimension of this mask exists in the data array, apply it
         if dimensions >= set(mask_data_array.dims):
+            logger.debug(
+                "Masking data array %r with mask %r",
+                data_array.name, mask_name)
             new_data_array = cast(xr.DataArray, data_array.where(mask_data_array, other=fill_value))
             new_data_array.attrs = data_array.attrs
             new_data_array.encoding = data_array.encoding
             return new_data_array
 
     # Fallback, no appropriate mask was found, so don't apply any.
     # This generally happens for data arrays such as time, record, x_grid, etc.
+    logger.debug(
+        "Data array %r had no relevant mask, leaving as is",
+        data_array.name)
     return data_array
 
 
 def find_fill_value(data_array: xr.DataArray) -> Any:
     """
     Float-typed variables can easily be masked. If they don't already have
     a fill value, they can be masked using `NaN` without issue.
@@ -178,32 +187,24 @@
 
     """
     if np.ma.is_masked(data_array.values):
         # xarray does not use masked arrays, but just in case someone has
         # constructed a dataset using one...
         return np.ma.masked
 
-    if '_FillValue' in data_array.encoding:
-        # The dataset was opened with mask_and_scale=True and a mask has been
-        # applied. Masked values are now represented as np.nan, not _FillValue.
-        return np.nan
-
-    if '_FillValue' in data_array.attrs:
-        # The dataset was opened with mask_and_scale=False and a mask has not
-        # been applied. Masked values should be represented using _FillValue.
-        return data_array.attrs['_FillValue']
-
-    if issubclass(data_array.dtype.type, np.floating):
-        # NaN is a useful fallback for a _FillValue, but only if the dtype
-        # is some sort of float. We won't actually _set_ a _FillValue
-        # attribute though, as that can play havok when trying to save
-        # existing datasets. xarray gets real grumpy when you have
-        # a _FillValue and a missing_value, and some existing datasets play
-        # fast and loose with mixing the two.
-        return np.nan
+    attrs = ['_FillValue', 'missing_value']
+    for attr in attrs:
+        if attr in data_array.attrs:
+            # The dataset was opened with mask_and_scale=False and a mask has not
+            # been applied. Masked values should be represented using _FillValue/missing_value.
+            return data_array.attrs[attr]
+
+    promoted_dtype, fill_value = maybe_promote(data_array.dtype)
+    if promoted_dtype == data_array.dtype:
+        return fill_value
 
     raise ValueError("No appropriate fill value found")
 
 
 def calculate_grid_mask_bounds(mask: xr.Dataset) -> Dict[Hashable, slice]:
     """
     Calculate the included bounds of a mask dataset for each dimension.
```

### Comparing `emsarray-0.4.1/src/emsarray/nco.py` & `emsarray-0.4.2/src/emsarray/nco.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/operations/depth.py` & `emsarray-0.4.2/src/emsarray/operations/depth.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/operations/geometry.py` & `emsarray-0.4.2/src/emsarray/operations/geometry.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/operations/point_extraction.py` & `emsarray-0.4.2/src/emsarray/operations/point_extraction.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/operations/triangulate.py` & `emsarray-0.4.2/src/emsarray/operations/triangulate.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/plot.py` & `emsarray-0.4.2/src/emsarray/plot.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/state.py` & `emsarray-0.4.2/src/emsarray/state.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/tutorial.py` & `emsarray-0.4.2/src/emsarray/tutorial.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray/utils.py` & `emsarray-0.4.2/src/emsarray/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import pandas as pd
 import pytz
 import shapely
 import xarray as xr
 from packaging.version import Version
 from xarray.coding import times
 from xarray.core.common import contains_cftime_datetimes
+from xarray.core.dtypes import maybe_promote
 
 from emsarray.types import Pathish
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_CALENDAR = 'proleptic_gregorian'
 
@@ -229,16 +230,18 @@
 
     Parameters
     ----------
     dataset_or_array
         The :class:`xarray.Dataset` or :class:`xarray.DataArray` to update
     """
     for variable in _get_variables(dataset_or_array):
+        current_dtype = variable.dtype
+        promoted_dtype, fill_value = maybe_promote(current_dtype)
         if (
-            issubclass(variable.dtype.type, np.floating)
+            current_dtype == promoted_dtype
             and "_FillValue" not in variable.encoding
             and "_FillValue" not in variable.attrs
         ):
             variable.encoding["_FillValue"] = None
 
 
 def fix_bad_time_units(dataset_or_array: Union[xr.Dataset, xr.DataArray]) -> None:
```

### Comparing `emsarray-0.4.1/src/emsarray.egg-info/PKG-INFO` & `emsarray-0.4.2/src/emsarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: emsarray
-Version: 0.4.1
+Version: 0.4.2
 Summary: xarray extension that supports multiple geometry conventions
 Author: "Coastal Environmental Modelling team, Oceans and Atmosphere, CSIRO"
 Author-email: "coasts@csiro.au"
 License: "BSD-3-Clause"
 Project-URL: Documentation, https://emsarray.readthedocs.io/
-Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.1/
+Project-URL: Release notes, https://emsarray.readthedocs.io/en/stable/releases/0.4.2/
 Project-URL: Source, https://github.com/csiro-coasts/emsarray/
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 Provides-Extra: tutorial
 Provides-Extra: complete
 Provides-Extra: docs
 Provides-Extra: testing
```

### Comparing `emsarray-0.4.1/src/emsarray.egg-info/SOURCES.txt` & `emsarray-0.4.2/src/emsarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/src/emsarray.egg-info/requires.txt` & `emsarray-0.4.2/src/emsarray.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/tests/test_accessors.py` & `emsarray-0.4.2/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/tests/test_binding.py` & `emsarray-0.4.2/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/tests/test_formats.py` & `emsarray-0.4.2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/tests/test_get_dataset_convention.py` & `emsarray-0.4.2/tests/test_get_dataset_convention.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/tests/test_nco.py` & `emsarray-0.4.2/tests/test_nco.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/tests/test_plot.py` & `emsarray-0.4.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `emsarray-0.4.1/tests/test_utils.py` & `emsarray-0.4.2/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,53 +53,74 @@
 
     with netCDF4.Dataset(dataset_path, "r+") as nc_dataset:
         # The time units should now be in an EMS-compatible format
         assert nc_dataset.variables['t'].getncattr('units') == 'hours since 2021-11-01 00:00:00 +10:00'
 
 
 def test_disable_default_fill_value(tmp_path: pathlib.Path):
-    foo = xarray.DataArray(
+    int_var = xarray.DataArray(
         data=np.arange(35, dtype=int).reshape(5, 7),
         dims=['j', 'i'],
         attrs={"Hello": "World"},
     )
-    bar = xarray.DataArray(
-        data=np.arange(35, dtype=np.float64).reshape(5, 7),
-        dims=['j', 'i'],
-    )
-    baz = xarray.DataArray(
+
+    float_var = xarray.DataArray(
         data=np.arange(35, dtype=np.float64).reshape(5, 7),
-        dims=['j', 'i'],
-    )
-    baz.data = np.where(np.tri(5, 7, dtype=bool), baz.data, np.nan)
-    baz.encoding["_FillValue"] = np.nan
+        dims=['j', 'i'])
 
-    dataset = xarray.Dataset(data_vars={"foo": foo, "bar": bar, "baz": baz})
+    f_data = np.where(
+        np.tri(5, 7, dtype=bool),
+        np.arange(35, dtype=np.float64).reshape(5, 7),
+        np.nan)
+    float_with_fill_value_var = xarray.DataArray(data=f_data, dims=['j', 'i'])
+    float_with_fill_value_var.encoding["_FillValue"] = np.nan
+
+    td_data = np.where(
+        np.tri(5, 7, dtype=bool),
+        np.arange(35).reshape(5, 7) * np.timedelta64(1, 'D'),
+        np.timedelta64('nat'))
+    timedelta_with_missing_value_var = xarray.DataArray(
+        data=td_data, dims=['j', 'i'])
+    timedelta_with_missing_value_var.encoding['missing_value'] = np.float64('1e35')
+    timedelta_with_missing_value_var.encoding['units'] = 'days'
+
+    dataset = xarray.Dataset(data_vars={
+        "int_var": int_var,
+        "float_var": float_var,
+        "float_with_fill_value_var": float_with_fill_value_var,
+        "timedelta_with_missing_value_var": timedelta_with_missing_value_var,
+    })
 
     # Save to a netCDF4 and then prove that it is bad
     dataset.to_netcdf(tmp_path / "bad.nc")
     with netCDF4.Dataset(tmp_path / "bad.nc", "r") as nc_dataset:
         # This one shouldn't be here because it is an integer datatype. xarray
         # does the right thing already in this case.
-        assert '_FillValue' not in nc_dataset.variables["foo"].ncattrs()
+        assert '_FillValue' not in nc_dataset.variables["int_var"].ncattrs()
         # This one shouldn't be here as we didnt set it, and the array is full!
         # This is the problem we are trying to solve
-        assert np.isnan(nc_dataset.variables["bar"].getncattr("_FillValue"))
+        assert np.isnan(nc_dataset.variables["float_var"].getncattr("_FillValue"))
         # This one is quite alright, we did explicitly set it after all
-        assert np.isnan(nc_dataset.variables["baz"].getncattr("_FillValue"))
+        assert np.isnan(nc_dataset.variables["float_with_fill_value_var"].getncattr("_FillValue"))
+        # This one is incorrect, a `missing_value` attribute has already been set
+        assert np.isnan(nc_dataset.variables["timedelta_with_missing_value_var"].getncattr("_FillValue"))
 
     utils.disable_default_fill_value(dataset)
     dataset.to_netcdf(tmp_path / "good.nc")
     with netCDF4.Dataset(tmp_path / "good.nc", "r") as nc_dataset:
         # This one should still be unset
-        assert '_FillValue' not in nc_dataset.variables["foo"].ncattrs()
+        assert '_FillValue' not in nc_dataset.variables["int_var"].ncattrs()
         # This one should now be unset
-        assert '_FillValue' not in nc_dataset.variables["bar"].ncattrs()
+        assert '_FillValue' not in nc_dataset.variables["float_var"].ncattrs()
         # Make sure this didn't get clobbered
-        assert np.isnan(nc_dataset.variables["baz"].getncattr("_FillValue"))
+        assert np.isnan(nc_dataset.variables["float_with_fill_value_var"].getncattr("_FillValue"))
+        # This one should now be unset
+        nc_timedelta = nc_dataset.variables["timedelta_with_missing_value_var"]
+        assert '_FillValue' not in nc_timedelta.ncattrs()
+        assert nc_timedelta.getncattr('missing_value') == np.float64('1e35')
 
 
 def test_dataset_like():
     sample_foo = xarray.DataArray(
         data=np.arange(10, dtype=np.int32),
         coords=[np.arange(10) * 2], dims=['x'])
     sample_foo.attrs = {'units': 'meters'}
```

