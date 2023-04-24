# Comparing `tmp/dynareadout-23.4.1.tar.gz` & `tmp/dynareadout-23.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynareadout-23.4.1.tar", last modified: Mon Apr 24 09:54:29 2023, max compression
+gzip compressed data, was "dynareadout-23.4.2.tar", last modified: Mon Apr 24 10:15:43 2023, max compression
```

## Comparing `dynareadout-23.4.1.tar` & `dynareadout-23.4.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.604387 dynareadout-23.4.1/
--rw-rw-rw-   0        0        0      878 2023-02-01 10:01:57.000000 dynareadout-23.4.1/LICENSE
--rw-rw-rw-   0        0        0      251 2023-02-01 10:03:35.000000 dynareadout-23.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5172 2023-04-24 09:54:29.603390 dynareadout-23.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4395 2023-04-24 08:55:05.000000 dynareadout-23.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.257659 dynareadout-23.4.1/lib/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.256660 dynareadout-23.4.1/lib/dynareadout/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.306742 dynareadout-23.4.1/lib/dynareadout/src/
--rw-rw-rw-   0        0        0    15215 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binary_search.c
--rw-rw-rw-   0        0        0     4052 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binary_search.h
--rw-rw-rw-   0        0        0    30340 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout.c
--rw-rw-rw-   0        0        0     5758 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout.h
--rw-rw-rw-   0        0        0     3252 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout_defines.h
--rw-rw-rw-   0        0        0    11391 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout_directory.c
--rw-rw-rw-   0        0        0     5670 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout_directory.h
--rw-rw-rw-   0        0        0     3791 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout_glob.c
--rw-rw-rw-   0        0        0     1784 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout_glob.h
--rw-rw-rw-   0        0        0    12007 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout_read.c
--rw-rw-rw-   0        0        0     4794 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/binout_read.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.322655 dynareadout-23.4.1/lib/dynareadout/src/cpp/
--rw-rw-rw-   0        0        0    10921 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/array.hpp
--rw-rw-rw-   0        0        0     8819 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/binout.cpp
--rw-rw-rw-   0        0        0     3521 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/binout.hpp
--rw-rw-rw-   0        0        0    17892 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot.cpp
--rw-rw-rw-   0        0        0     7664 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot.hpp
--rw-rw-rw-   0        0        0     7685 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot_part.cpp
--rw-rw-rw-   0        0        0     4841 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot_part.hpp
--rw-rw-rw-   0        0        0     6898 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/key.cpp
--rw-rw-rw-   0        0        0    16564 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/key.hpp
--rw-rw-rw-   0        0        0     2005 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/cpp/vec.hpp
--rw-rw-rw-   0        0        0    14051 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3_buffer.c
--rw-rw-rw-   0        0        0     3502 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3_buffer.h
--rw-rw-rw-   0        0        0     6230 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3_defines.h
--rw-rw-rw-   0        0        0    84055 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3plot.c
--rw-rw-rw-   0        0        0    15111 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3plot.h
--rw-rw-rw-   0        0        0    12089 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3plot_data.c
--rw-rw-rw-   0        0        0     4169 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3plot_error_macros.h
--rw-rw-rw-   0        0        0     6690 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3plot_part_nodes.c
--rw-rw-rw-   0        0        0     5034 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3plot_part_nodes.h
--rw-rw-rw-   0        0        0    11849 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/d3plot_state.c
--rw-rw-rw-   0        0        0     4550 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/extra_string.c
--rw-rw-rw-   0        0        0     2236 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/extra_string.h
--rw-rw-rw-   0        0        0    43016 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/key.c
--rw-rw-rw-   0        0        0     9032 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/key.h
--rw-rw-rw-   0        0        0     5323 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/path.c
--rw-rw-rw-   0        0        0     2490 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/path.h
--rw-rw-rw-   0        0        0     4143 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/path_view.c
--rw-rw-rw-   0        0        0     3545 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/path_view.h
--rw-rw-rw-   0        0        0    25367 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/pgni.h
--rw-rw-rw-   0        0        0     9855 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/profiling.c
--rw-rw-rw-   0        0        0     3589 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/profiling.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.330646 dynareadout-23.4.1/lib/dynareadout/src/python/
--rw-rw-rw-   0        0        0    17631 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/python/conversions.hpp
--rw-rw-rw-   0        0        0     3434 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_binout.cpp
--rw-rw-rw-   0        0        0    12216 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_d3plot.cpp
--rw-rw-rw-   0        0        0     4897 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_key.cpp
--rw-rw-rw-   0        0        0     1786 2023-04-24 09:52:26.000000 dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_module.cpp
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.341604 dynareadout-23.4.1/lib/pybind11/
--rw-rw-rw-   0        0        0     1713 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.258655 dynareadout-23.4.1/lib/pybind11/include/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.506398 dynareadout-23.4.1/lib/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    24657 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     7262 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    67301 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     8683 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2170 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.566061 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    28986 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    51557 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     5649 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    18409 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    25640 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0    43276 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-rw-   0        0        0     1690 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    32860 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0    12071 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     4887 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     4825 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     8501 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/gil.h
--rw-rw-rw-   0        0        0     9127 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    81515 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     9305 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2257 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0   128619 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    96315 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/pytypes.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.573470 dynareadout-23.4.1/lib/pybind11/include/pybind11/stl/
--rw-rw-rw-   0        0        0     4301 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-rw-   0        0        0    15783 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    27798 2023-02-01 10:02:01.000000 dynareadout-23.4.1/lib/pybind11/include/pybind11/stl_bind.h
--rw-rw-rw-   0        0        0      860 2023-04-24 09:53:45.000000 dynareadout-23.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 09:54:29.604387 dynareadout-23.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2417 2023-04-24 09:53:38.000000 dynareadout-23.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.260650 dynareadout-23.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.574466 dynareadout-23.4.1/src/dynareadout/
--rw-rw-rw-   0        0        0     1858 2023-04-24 08:55:05.000000 dynareadout-23.4.1/src/dynareadout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:54:29.602398 dynareadout-23.4.1/src/dynareadout.egg-info/
--rw-rw-rw-   0        0        0     5172 2023-04-24 09:54:29.000000 dynareadout-23.4.1/src/dynareadout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3095 2023-04-24 09:54:29.000000 dynareadout-23.4.1/src/dynareadout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:54:29.000000 dynareadout-23.4.1/src/dynareadout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-01 09:15:58.000000 dynareadout-23.4.1/src/dynareadout.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-04-24 09:54:29.000000 dynareadout-23.4.1/src/dynareadout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-24 09:54:29.000000 dynareadout-23.4.1/src/dynareadout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.289532 dynareadout-23.4.2/
+-rw-rw-rw-   0        0        0      878 2023-02-01 10:01:57.000000 dynareadout-23.4.2/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-02-01 10:03:35.000000 dynareadout-23.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5172 2023-04-24 10:15:43.289532 dynareadout-23.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4395 2023-04-24 08:55:05.000000 dynareadout-23.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.167860 dynareadout-23.4.2/lib/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.166863 dynareadout-23.4.2/lib/dynareadout/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.210744 dynareadout-23.4.2/lib/dynareadout/src/
+-rw-rw-rw-   0        0        0    15215 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binary_search.c
+-rw-rw-rw-   0        0        0     4052 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binary_search.h
+-rw-rw-rw-   0        0        0    30340 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout.c
+-rw-rw-rw-   0        0        0     5758 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout.h
+-rw-rw-rw-   0        0        0     3252 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_defines.h
+-rw-rw-rw-   0        0        0    11391 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_directory.c
+-rw-rw-rw-   0        0        0     5670 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_directory.h
+-rw-rw-rw-   0        0        0     3791 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_glob.c
+-rw-rw-rw-   0        0        0     1784 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_glob.h
+-rw-rw-rw-   0        0        0    12007 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_read.c
+-rw-rw-rw-   0        0        0     4794 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/binout_read.h
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.220717 dynareadout-23.4.2/lib/dynareadout/src/cpp/
+-rw-rw-rw-   0        0        0    10941 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/array.hpp
+-rw-rw-rw-   0        0        0     8819 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.cpp
+-rw-rw-rw-   0        0        0     3521 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.hpp
+-rw-rw-rw-   0        0        0    17892 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.cpp
+-rw-rw-rw-   0        0        0     7664 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.hpp
+-rw-rw-rw-   0        0        0     7685 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.cpp
+-rw-rw-rw-   0        0        0     4841 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.hpp
+-rw-rw-rw-   0        0        0     6898 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/key.cpp
+-rw-rw-rw-   0        0        0    16564 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/key.hpp
+-rw-rw-rw-   0        0        0     2005 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/cpp/vec.hpp
+-rw-rw-rw-   0        0        0    14051 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.c
+-rw-rw-rw-   0        0        0     3502 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.h
+-rw-rw-rw-   0        0        0     6230 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3_defines.h
+-rw-rw-rw-   0        0        0    84060 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot.c
+-rw-rw-rw-   0        0        0    15111 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot.h
+-rw-rw-rw-   0        0        0    12089 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_data.c
+-rw-rw-rw-   0        0        0     4169 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_error_macros.h
+-rw-rw-rw-   0        0        0     6690 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.c
+-rw-rw-rw-   0        0        0     5034 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.h
+-rw-rw-rw-   0        0        0    11849 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/d3plot_state.c
+-rw-rw-rw-   0        0        0     4550 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/extra_string.c
+-rw-rw-rw-   0        0        0     2236 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/extra_string.h
+-rw-rw-rw-   0        0        0    43016 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/key.c
+-rw-rw-rw-   0        0        0     9032 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/key.h
+-rw-rw-rw-   0        0        0     5323 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path.c
+-rw-rw-rw-   0        0        0     2490 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path.h
+-rw-rw-rw-   0        0        0     4143 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path_view.c
+-rw-rw-rw-   0        0        0     3545 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/path_view.h
+-rw-rw-rw-   0        0        0    25367 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/pgni.h
+-rw-rw-rw-   0        0        0     9855 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/profiling.c
+-rw-rw-rw-   0        0        0     3589 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/profiling.h
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.225703 dynareadout-23.4.2/lib/dynareadout/src/python/
+-rw-rw-rw-   0        0        0    17631 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/conversions.hpp
+-rw-rw-rw-   0        0        0     3434 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_binout.cpp
+-rw-rw-rw-   0        0        0    12216 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_d3plot.cpp
+-rw-rw-rw-   0        0        0     4897 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_key.cpp
+-rw-rw-rw-   0        0        0     1786 2023-04-24 10:14:43.000000 dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_module.cpp
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.226701 dynareadout-23.4.2/lib/pybind11/
+-rw-rw-rw-   0        0        0     1713 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.167860 dynareadout-23.4.2/lib/pybind11/include/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.250637 dynareadout-23.4.2/lib/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    24657 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     7262 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    67301 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     8683 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2170 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.258614 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    28986 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    51557 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     5649 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    18409 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    25640 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0    43276 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-rw-   0        0        0     1690 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-rw-   0        0        0    32860 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0    12071 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     4887 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     4825 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     8501 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/gil.h
+-rw-rw-rw-   0        0        0     9127 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    81515 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     9305 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2257 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0   128619 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0    96315 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/pytypes.h
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.259613 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl/
+-rw-rw-rw-   0        0        0     4301 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-rw-   0        0        0    15783 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    27798 2023-02-01 10:02:01.000000 dynareadout-23.4.2/lib/pybind11/include/pybind11/stl_bind.h
+-rw-rw-rw-   0        0        0      860 2023-04-24 10:15:15.000000 dynareadout-23.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:15:43.289532 dynareadout-23.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     2417 2023-04-24 10:15:11.000000 dynareadout-23.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.169854 dynareadout-23.4.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.260610 dynareadout-23.4.2/src/dynareadout/
+-rw-rw-rw-   0        0        0     1858 2023-04-24 08:55:05.000000 dynareadout-23.4.2/src/dynareadout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:15:43.288538 dynareadout-23.4.2/src/dynareadout.egg-info/
+-rw-rw-rw-   0        0        0     5172 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3095 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-01 09:15:58.000000 dynareadout-23.4.2/src/dynareadout.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-24 10:15:43.000000 dynareadout-23.4.2/src/dynareadout.egg-info/top_level.txt
```

### Comparing `dynareadout-23.4.1/LICENSE` & `dynareadout-23.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/PKG-INFO` & `dynareadout-23.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.4.1
+Version: 23.4.2
 Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `dynareadout-23.4.1/README.md` & `dynareadout-23.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binary_search.c` & `dynareadout-23.4.2/lib/dynareadout/src/binary_search.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binary_search.h` & `dynareadout-23.4.2/lib/dynareadout/src/binary_search.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout.c` & `dynareadout-23.4.2/lib/dynareadout/src/binout.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout.h` & `dynareadout-23.4.2/lib/dynareadout/src/binout.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout_defines.h` & `dynareadout-23.4.2/lib/dynareadout/src/binout_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout_directory.c` & `dynareadout-23.4.2/lib/dynareadout/src/binout_directory.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout_directory.h` & `dynareadout-23.4.2/lib/dynareadout/src/binout_directory.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout_glob.c` & `dynareadout-23.4.2/lib/dynareadout/src/binout_glob.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout_glob.h` & `dynareadout-23.4.2/lib/dynareadout/src/binout_glob.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout_read.c` & `dynareadout-23.4.2/lib/dynareadout/src/binout_read.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/binout_read.h` & `dynareadout-23.4.2/lib/dynareadout/src/binout_read.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/array.hpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/array.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
  * misrepresented as being the original software.
  *
  * 3. This notice may not be removed or altered from any source distribution.
  ************************************************************************************/
 
 #pragma once
 #include <cerrno>
+#include <cstdint>
 #include <cstdlib>
 #include <cstring>
 #include <iostream>
 #include <limits>
 #include <stdexcept>
 #include <string>
 #include <type_traits>
```

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/binout.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/binout.hpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/binout.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot.hpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot_part.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/d3plot_part.hpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/d3plot_part.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/key.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/key.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/key.hpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/key.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/cpp/vec.hpp` & `dynareadout-23.4.2/lib/dynareadout/src/cpp/vec.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3_buffer.c` & `dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3_buffer.h` & `dynareadout-23.4.2/lib/dynareadout/src/d3_buffer.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3_defines.h` & `dynareadout-23.4.2/lib/dynareadout/src/d3_defines.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3plot.c` & `dynareadout-23.4.2/lib/dynareadout/src/d3plot.c`

 * *Files 0% similar despite different names*

```diff
@@ -2175,15 +2175,15 @@
 
   d3_word run_time = 0;
   d3_buffer_read_words_at(&plot_file->buffer, &run_time, 1,
                           plot_file->data_pointers[D3PLT_PTR_RUN_TIME]);
   if (plot_file->buffer.error_string) {
     ERROR_AND_NO_RETURN_F_PTR("Failed to read words: %s",
                               plot_file->buffer.error_string);
-    return NULL;
+    return (time_t)0;
   }
   const time_t epoch_time = run_time;
 
   END_PROFILE_FUNC();
   return epoch_time;
 }
```

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3plot.h` & `dynareadout-23.4.2/lib/dynareadout/src/d3plot.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3plot_data.c` & `dynareadout-23.4.2/lib/dynareadout/src/d3plot_data.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3plot_error_macros.h` & `dynareadout-23.4.2/lib/dynareadout/src/d3plot_error_macros.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3plot_part_nodes.c` & `dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3plot_part_nodes.h` & `dynareadout-23.4.2/lib/dynareadout/src/d3plot_part_nodes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/d3plot_state.c` & `dynareadout-23.4.2/lib/dynareadout/src/d3plot_state.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/extra_string.c` & `dynareadout-23.4.2/lib/dynareadout/src/extra_string.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/extra_string.h` & `dynareadout-23.4.2/lib/dynareadout/src/extra_string.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/key.c` & `dynareadout-23.4.2/lib/dynareadout/src/key.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/key.h` & `dynareadout-23.4.2/lib/dynareadout/src/key.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/path.c` & `dynareadout-23.4.2/lib/dynareadout/src/path.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/path.h` & `dynareadout-23.4.2/lib/dynareadout/src/path.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/path_view.c` & `dynareadout-23.4.2/lib/dynareadout/src/path_view.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/path_view.h` & `dynareadout-23.4.2/lib/dynareadout/src/path_view.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/pgni.h` & `dynareadout-23.4.2/lib/dynareadout/src/pgni.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/profiling.c` & `dynareadout-23.4.2/lib/dynareadout/src/profiling.c`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/profiling.h` & `dynareadout-23.4.2/lib/dynareadout/src/profiling.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/python/conversions.hpp` & `dynareadout-23.4.2/lib/dynareadout/src/python/conversions.hpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_binout.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_binout.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_d3plot.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_d3plot.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_key.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_key.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/dynareadout/src/python/pybind11_module.cpp` & `dynareadout-23.4.2/lib/dynareadout/src/python/pybind11_module.cpp`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/LICENSE` & `dynareadout-23.4.2/lib/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/attr.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/buffer_info.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/cast.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/chrono.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/complex.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/class.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/common.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/descr.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/init.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/internals.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/detail/typeid.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/eigen.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/embed.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/eval.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/functional.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/gil.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/iostream.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/numpy.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/operators.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/options.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/pybind11.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/pytypes.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/stl/filesystem.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/stl.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/lib/pybind11/include/pybind11/stl_bind.h` & `dynareadout-23.4.2/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/pyproject.toml` & `dynareadout-23.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynareadout"
-version = "23.04.1"
+version = "23.04.2"
 authors = [
   { name = "PucklaJ", email = "jonaas.pucher000000@gmail.com"},
 ]
 description = "Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `dynareadout-23.4.1/setup.py` & `dynareadout-23.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,11 +46,11 @@
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_binout.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_d3plot.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_key.cpp'),
         os.path.join(dynareadout_dir, 'src', 'python', 'pybind11_module.cpp'),
     ])
 
 setup(name='dynareadout',
-      version='23.04.1',
+      version='23.04.2',
       ext_modules=[dynareadout_c],
       zip_safe=False,
       include_package_data=True)
```

### Comparing `dynareadout-23.4.1/src/dynareadout/__init__.py` & `dynareadout-23.4.2/src/dynareadout/__init__.py`

 * *Files identical despite different names*

### Comparing `dynareadout-23.4.1/src/dynareadout.egg-info/PKG-INFO` & `dynareadout-23.4.2/src/dynareadout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynareadout
-Version: 23.4.1
+Version: 23.4.2
 Summary: Ansi C library for parsing binary output files of LS Dyna (d3plot, binout) with bindings for python
 Author-email: PucklaJ <jonaas.pucher000000@gmail.com>
 Project-URL: Homepage, https://github.com/PucklaJ/dynareadout
 Project-URL: Bug Trackers, https://github.com/PucklaJ/dynareadout/issues
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: zlib/libpng License
```

### Comparing `dynareadout-23.4.1/src/dynareadout.egg-info/SOURCES.txt` & `dynareadout-23.4.2/src/dynareadout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

