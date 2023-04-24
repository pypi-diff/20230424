# Comparing `tmp/gdstk-0.9.37.tar.gz` & `tmp/gdstk-0.9.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdstk-0.9.37.tar", last modified: Sun Feb 12 15:59:08 2023, max compression
+gzip compressed data, was "gdstk-0.9.38.tar", last modified: Mon Apr 24 00:09:53 2023, max compression
```

## Comparing `gdstk-0.9.37.tar` & `gdstk-0.9.38.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:59:08.675735 gdstk-0.9.37/
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-12 15:58:57.000000 gdstk-0.9.37/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-12 15:58:57.000000 gdstk-0.9.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-12 15:58:57.000000 gdstk-0.9.37/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-02-12 15:59:08.675735 gdstk-0.9.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-02-12 15:58:57.000000 gdstk-0.9.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:59:08.631734 gdstk-0.9.37/gdstk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-02-12 15:59:08.000000 gdstk-0.9.37/gdstk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-02-12 15:59:08.000000 gdstk-0.9.37/gdstk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 15:59:08.000000 gdstk-0.9.37/gdstk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 15:59:08.000000 gdstk-0.9.37/gdstk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-12 15:59:08.000000 gdstk-0.9.37/gdstk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-12 15:59:08.000000 gdstk-0.9.37/gdstk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-12 15:58:57.000000 gdstk-0.9.37/gdstk.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-12 15:58:57.000000 gdstk-0.9.37/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:59:08.639734 gdstk-0.9.37/python/
--rw-r--r--   0 runner    (1001) docker     (123)    44164 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/cell_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/curve_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   128218 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/docstrings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    95122 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/flexpath_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    87046 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/gdstk_module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/gdswriter_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/label_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/library_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24531 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/parsing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/polygon_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/rawcell_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/reference_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/repetition_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    90116 2023-02-12 15:58:57.000000 gdstk-0.9.37/python/robustpath_object.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 15:59:08.675735 gdstk-0.9.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-02-12 15:58:57.000000 gdstk-0.9.37/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:59:08.659734 gdstk-0.9.37/src/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/allocator.h
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/array.h
--rw-r--r--   0 runner    (1001) docker     (123)    39430 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/cell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/cell.h
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/clipper_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/clipper_tools.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:59:08.659734 gdstk-0.9.37/src/clipperlib/
--rw-r--r--   0 runner    (1001) docker     (123)   153647 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/clipperlib/clipper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/clipperlib/clipper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/curve.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/curve.h
--rw-r--r--   0 runner    (1001) docker     (123)    49359 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/flexpath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/flexpath.h
--rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/font.h
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/gdsii.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/gdsii.h
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/gdstk.h
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/gdswriter.h
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/label.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/label.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:59:08.675735 gdstk-0.9.37/src/libqhull_r/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83123 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/geom2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    51296 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/geom_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/geom_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   108561 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/global_r.c
--rw-r--r--   0 runner    (1001) docker     (123)   156212 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/io_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/io_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    80295 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/libqhull_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    62510 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/libqhull_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    23930 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/mem_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/mem_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   242779 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/merge_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/merge_r.h
--rw-r--r--   0 runner    (1001) docker     (123)   180894 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/poly2_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    58558 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/poly_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/poly_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/qhull_ra.h
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/qset_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/qset_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/random_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/random_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/rboxlib_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    34822 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/stat_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/stat_r.h
--rw-r--r--   0 runner    (1001) docker     (123)    25503 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/user_r.c
--rw-r--r--   0 runner    (1001) docker     (123)    36663 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/user_r.h
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/usermem_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/userprintf_r.c
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/libqhull_r/userprintf_rbox_r.c
--rw-r--r--   0 runner    (1001) docker     (123)   124427 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/library.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/map.h
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/oasis.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/oasis.h
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/pathcommon.h
--rw-r--r--   0 runner    (1001) docker     (123)    64639 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/polygon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/polygon.h
--rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/property.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/property.h
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/rawcell.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/rawcell.h
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/reference.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/reference.h
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/repetition.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/repetition.h
--rw-r--r--   0 runner    (1001) docker     (123)    67153 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/robustpath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/robustpath.h
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/set.h
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/sort.h
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/style.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/style.h
--rw-r--r--   0 runner    (1001) docker     (123)    24232 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-02-12 15:58:57.000000 gdstk-0.9.37/src/vec.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:09:53.498544 gdstk-0.9.38/
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-24 00:09:33.000000 gdstk-0.9.38/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-24 00:09:33.000000 gdstk-0.9.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 00:09:33.000000 gdstk-0.9.38/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-24 00:09:53.498544 gdstk-0.9.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-24 00:09:33.000000 gdstk-0.9.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:09:53.454542 gdstk-0.9.38/gdstk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-24 00:09:53.000000 gdstk-0.9.38/gdstk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-24 00:09:53.000000 gdstk-0.9.38/gdstk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:09:53.000000 gdstk-0.9.38/gdstk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:09:53.000000 gdstk-0.9.38/gdstk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 00:09:53.000000 gdstk-0.9.38/gdstk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 00:09:53.000000 gdstk-0.9.38/gdstk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-24 00:09:33.000000 gdstk-0.9.38/gdstk.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 00:09:33.000000 gdstk-0.9.38/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:09:53.462542 gdstk-0.9.38/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    44164 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/cell_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/curve_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   128218 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/docstrings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    95122 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/flexpath_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    87046 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/gdstk_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/gdswriter_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/label_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/library_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24531 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/parsing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/polygon_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/rawcell_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/reference_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/repetition_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    90116 2023-04-24 00:09:33.000000 gdstk-0.9.38/python/robustpath_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:09:53.498544 gdstk-0.9.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-24 00:09:33.000000 gdstk-0.9.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:09:53.478543 gdstk-0.9.38/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/allocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39454 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/cell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/cell.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/clipper_tools.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/clipper_tools.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:09:53.482543 gdstk-0.9.38/src/clipperlib/
+-rw-r--r--   0 runner    (1001) docker     (123)   153647 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/clipperlib/clipper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/clipperlib/clipper.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/curve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/curve.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49359 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/flexpath.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/flexpath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/font.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/gdsii.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/gdsii.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/gdstk.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/gdswriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/label.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/label.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:09:53.498544 gdstk-0.9.38/src/libqhull_r/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83123 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/geom2_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    51296 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/geom_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/geom_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   108561 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/global_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)   156212 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/io_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/io_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80295 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/libqhull_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    62510 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/libqhull_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23930 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/mem_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/mem_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   242779 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/merge_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/merge_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)   180894 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/poly2_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58558 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/poly_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/poly_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/qhull_ra.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/qset_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/qset_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/random_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/random_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/rboxlib_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34822 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/stat_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/stat_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25503 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/user_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36663 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/user_r.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/usermem_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/userprintf_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/libqhull_r/userprintf_rbox_r.c
+-rw-r--r--   0 runner    (1001) docker     (123)   126051 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/library.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37490 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/oasis.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/oasis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/pathcommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64723 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/polygon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/polygon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15710 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/property.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/property.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/rawcell.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/rawcell.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/reference.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/reference.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/repetition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/repetition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67329 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/robustpath.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/robustpath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/sort.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/style.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/style.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-24 00:09:33.000000 gdstk-0.9.38/src/vec.h
```

### Comparing `gdstk-0.9.37/CMakeLists.txt` & `gdstk-0.9.38/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/LICENSE` & `gdstk-0.9.38/LICENSE`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/PKG-INFO` & `gdstk-0.9.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdstk
-Version: 0.9.37
+Version: 0.9.38
 Summary: Python module for creation and manipulation of GDSII files.
 Home-page: https://github.com/heitzmann/gdstk
 Author: Lucas H. Gabrielli
 Author-email: heitzmann@gmail.com
 License: Boost Software License v1.0
 Keywords: GDSII CAD layout
 Platform: OS Independent
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Provides: gdstk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GDSTK 0.9.37
+# GDSTK 0.9.38
 
 [![Boost Software License - Version 1.0](https://img.shields.io/github/license/heitzmann/gdstk.svg)](https://www.boost.org/LICENSE_1_0.txt)
 [![Tests Runner](https://github.com/heitzmann/gdstk/workflows/Tests%20Runner/badge.svg)](https://github.com/heitzmann/gdstk/actions)
 [![Publish Docs](https://github.com/heitzmann/gdstk/workflows/Publish%20Docs/badge.svg)](http://heitzmann.github.io/gdstk)
 [![Downloads](https://img.shields.io/github/downloads/heitzmann/gdstk/total.svg)](https://github.com/heitzmann/gdstk/releases)
 
 Gdstk (GDSII Tool Kit) is a C++ library for creation and manipulation of GDSII and OASIS files.
```

### Comparing `gdstk-0.9.37/README.md` & `gdstk-0.9.38/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# GDSTK 0.9.37
+# GDSTK 0.9.38
 
 [![Boost Software License - Version 1.0](https://img.shields.io/github/license/heitzmann/gdstk.svg)](https://www.boost.org/LICENSE_1_0.txt)
 [![Tests Runner](https://github.com/heitzmann/gdstk/workflows/Tests%20Runner/badge.svg)](https://github.com/heitzmann/gdstk/actions)
 [![Publish Docs](https://github.com/heitzmann/gdstk/workflows/Publish%20Docs/badge.svg)](http://heitzmann.github.io/gdstk)
 [![Downloads](https://img.shields.io/github/downloads/heitzmann/gdstk/total.svg)](https://github.com/heitzmann/gdstk/releases)
 
 Gdstk (GDSII Tool Kit) is a C++ library for creation and manipulation of GDSII and OASIS files.
```

### Comparing `gdstk-0.9.37/gdstk.egg-info/PKG-INFO` & `gdstk-0.9.38/gdstk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdstk
-Version: 0.9.37
+Version: 0.9.38
 Summary: Python module for creation and manipulation of GDSII files.
 Home-page: https://github.com/heitzmann/gdstk
 Author: Lucas H. Gabrielli
 Author-email: heitzmann@gmail.com
 License: Boost Software License v1.0
 Keywords: GDSII CAD layout
 Platform: OS Independent
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Provides: gdstk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GDSTK 0.9.37
+# GDSTK 0.9.38
 
 [![Boost Software License - Version 1.0](https://img.shields.io/github/license/heitzmann/gdstk.svg)](https://www.boost.org/LICENSE_1_0.txt)
 [![Tests Runner](https://github.com/heitzmann/gdstk/workflows/Tests%20Runner/badge.svg)](https://github.com/heitzmann/gdstk/actions)
 [![Publish Docs](https://github.com/heitzmann/gdstk/workflows/Publish%20Docs/badge.svg)](http://heitzmann.github.io/gdstk)
 [![Downloads](https://img.shields.io/github/downloads/heitzmann/gdstk/total.svg)](https://github.com/heitzmann/gdstk/releases)
 
 Gdstk (GDSII Tool Kit) is a C++ library for creation and manipulation of GDSII and OASIS files.
```

### Comparing `gdstk-0.9.37/gdstk.egg-info/SOURCES.txt` & `gdstk-0.9.38/gdstk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/cell_object.cpp` & `gdstk-0.9.38/python/cell_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/curve_object.cpp` & `gdstk-0.9.38/python/curve_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/docstrings.cpp` & `gdstk-0.9.38/python/docstrings.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -3432,15 +3432,15 @@
       shapes.  If zero or negative, the library rounding size is used
       (`precision / unit`).
 
 Returns:
     The imported library.
 
 Examples:
-    >>> library = gdstk.read_gds("layout.oas")
+    >>> library = gdstk.read_oas("layout.oas")
     >>> top_cells = library.top_level())!");
 
 PyDoc_STRVAR(read_rawcells_function_doc, R"!(read_rawcells(infile) -> dict
 
 Load cells form a GDSII file without decoding them.
 
 Args:
```

### Comparing `gdstk-0.9.37/python/flexpath_object.cpp` & `gdstk-0.9.38/python/flexpath_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/gdstk_module.cpp` & `gdstk-0.9.38/python/gdstk_module.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/gdswriter_object.cpp` & `gdstk-0.9.38/python/gdswriter_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/label_object.cpp` & `gdstk-0.9.38/python/label_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/library_object.cpp` & `gdstk-0.9.38/python/library_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/parsing.cpp` & `gdstk-0.9.38/python/parsing.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/polygon_object.cpp` & `gdstk-0.9.38/python/polygon_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/rawcell_object.cpp` & `gdstk-0.9.38/python/rawcell_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/reference_object.cpp` & `gdstk-0.9.38/python/reference_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/repetition_object.cpp` & `gdstk-0.9.38/python/repetition_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/python/robustpath_object.cpp` & `gdstk-0.9.38/python/robustpath_object.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/setup.py` & `gdstk-0.9.38/setup.py`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/allocator.h` & `gdstk-0.9.38/src/allocator.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/array.h` & `gdstk-0.9.38/src/array.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/cell.cpp` & `gdstk-0.9.38/src/cell.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -876,15 +876,15 @@
     x -= pad;
     y -= pad;
     w += 2 * pad;
     h += 2 * pad;
 
     FILE* out = fopen(filename, "w");
     if (out == NULL) {
-        fputs("[GDSTK] Unable to open file for SVG output.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open file for SVG output.\n", error_logger);
         return ErrorCode::OutputFileOpenError;
     }
 
     fputs(
         "<?xml version=\"1.0\" encoding=\"UTF-8\"?>\n"
         "<svg xmlns=\"http://www.w3.org/2000/svg\" "
         "xmlns:xlink=\"http://www.w3.org/1999/xlink\" width=\"",
```

### Comparing `gdstk-0.9.37/src/cell.h` & `gdstk-0.9.38/src/cell.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/clipper_tools.cpp` & `gdstk-0.9.38/src/clipper_tools.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,16 @@
                 xnew = hole_min->X;
                 p_closest = p_next;
                 break;
             }
         }
 
         if (p_closest == p_end) {
-            fprintf(stderr, "[GDSTK] Unable to link hole in boolean operation.\n");
+            if (error_logger)
+                fprintf(error_logger, "[GDSTK] Unable to link hole in boolean operation.\n");
             error_code = ErrorCode::BooleanError;
         } else {
             ClipperLib::IntPoint p_new(xnew, hole_min->Y);
             if (p_new.X != p_closest->X || p_new.Y != p_closest->Y)
                 p_closest = contour->insert(p_closest, p_new);
             p_closest = contour->insert(p_closest, holes[i].path->begin(), hole_min + 1);
             p_closest = contour->insert(p_closest, hole_min, holes[i].path->end());
```

### Comparing `gdstk-0.9.37/src/clipper_tools.h` & `gdstk-0.9.38/src/clipper_tools.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/clipperlib/clipper.cpp` & `gdstk-0.9.38/src/clipperlib/clipper.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/clipperlib/clipper.hpp` & `gdstk-0.9.38/src/clipperlib/clipper.hpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/curve.cpp` & `gdstk-0.9.38/src/curve.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/curve.h` & `gdstk-0.9.38/src/curve.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/flexpath.cpp` & `gdstk-0.9.38/src/flexpath.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/flexpath.h` & `gdstk-0.9.38/src/flexpath.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/font.h` & `gdstk-0.9.38/src/font.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/gdsii.cpp` & `gdstk-0.9.38/src/gdsii.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -36,53 +36,61 @@
     const double mantissa = ((double)(real & 0x00FFFFFFFFFFFFFF)) / 72057594037927936.0;
     const double result = mantissa * exp2((double)exponent);
     return (real & 0x8000000000000000) ? -result : result;
 }
 
 ErrorCode gdsii_read_record(FILE* in, uint8_t* buffer, uint64_t& buffer_count) {
     if (buffer_count < 4) {
-        fputs("[GDSTK] Insufficient memory in buffer.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Insufficient memory in buffer.\n", error_logger);
         return ErrorCode::InsufficientMemory;
     }
     uint64_t read_length = fread(buffer, 1, 4, in);
     if (read_length < 4) {
         DEBUG_PRINT("Read bytes (expected 4): %" PRIu64 "\n", read_length);
         if (feof(in) != 0) {
-            fputs("[GDSTK] Unable to read input file. End of file reached unexpectedly.\n", stderr);
+            if (error_logger)
+                fputs("[GDSTK] Unable to read input file. End of file reached unexpectedly.\n",
+                      error_logger);
         } else {
-            fprintf(stderr, "[GDSTK] Unable to read input file. Error number %d\n.", ferror(in));
+            if (error_logger)
+                fprintf(error_logger, "[GDSTK] Unable to read input file. Error number %d\n.",
+                        ferror(in));
         }
         buffer_count = read_length;
         return ErrorCode::InputFileError;
     }
     big_endian_swap16((uint16_t*)buffer, 1);  // second word is interpreted byte-wise (no swaping);
     const uint32_t record_length = *((uint16_t*)buffer);
     if (record_length < 4) {
         DEBUG_PRINT("Record length should be at least 4. Found %" PRIu32 "\n", record_length);
-        fputs("[GDSTK] Invalid or corrupted GDSII file.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Invalid or corrupted GDSII file.\n", error_logger);
         buffer_count = read_length;
         return ErrorCode::InvalidFile;
     } else if (record_length == 4) {
         buffer_count = read_length;
         return ErrorCode::NoError;
     }
     if (buffer_count < 4 + record_length) {
-        fputs("[GDSTK] Insufficient memory in buffer.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Insufficient memory in buffer.\n", error_logger);
         buffer_count = read_length;
         return ErrorCode::InsufficientMemory;
     }
     read_length = fread(buffer + 4, 1, record_length - 4, in);
     buffer_count = 4 + read_length;
     if (read_length < record_length - 4) {
         DEBUG_PRINT("Read bytes (expected %" PRIu32 "): %" PRIu64 "\n", record_length - 4,
                     read_length);
         if (feof(in) != 0) {
-            fputs("[GDSTK] Unable to read input file. End of file reached unexpectedly.\n", stderr);
+            if (error_logger)
+                fputs("[GDSTK] Unable to read input file. End of file reached unexpectedly.\n",
+                      error_logger);
         } else {
-            fprintf(stderr, "[GDSTK] Unable to read input file. Error number %d\n.", ferror(in));
+            if (error_logger)
+                fprintf(error_logger, "[GDSTK] Unable to read input file. Error number %d\n.",
+                        ferror(in));
         }
         return ErrorCode::InputFileError;
     }
     return ErrorCode::NoError;
 }
 
 }  // namespace gdstk
```

### Comparing `gdstk-0.9.37/src/gdsii.h` & `gdstk-0.9.38/src/gdsii.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/gdstk.h` & `gdstk-0.9.38/src/gdstk.h`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #ifndef GDSTK_HEADER_GDSTK
 #define GDSTK_HEADER_GDSTK
 
 #define __STDC_FORMAT_MACROS
 #define _USE_MATH_DEFINES
 
-#define GDSTK_VERSION "0.9.37"
+#define GDSTK_VERSION "0.9.38"
 
 // If GDSTK_CUSTOM_ALLOCATOR is defined, the user must supply implementations
 // for the following dynamic memory management functions:
 // void* allocate(uint64_t size);
 // void* reallocate(void* ptr, uint64_t size);
 // void* allocate_clear(uint64_t size);
 // void free_allocation(void* ptr);
```

### Comparing `gdstk-0.9.37/src/gdswriter.h` & `gdstk-0.9.38/src/gdswriter.h`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         result.timestamp = *timestamp;
     } else {
         get_now(result.timestamp);
     }
 
     result.out = fopen(filename, "wb");
     if (result.out == NULL) {
-        fputs("[GDSTK] Unable to open GDSII file for output.\n", stderr);
+        fputs("[GDSTK] Unable to open GDSII file for output.\n", error_logger);
         if (error_code) *error_code = ErrorCode::OutputFileOpenError;
         return result;
     }
 
     uint64_t len = strlen(library_name);
     if (len % 2) len++;
     uint16_t buffer_start[] = {6,
```

### Comparing `gdstk-0.9.37/src/label.cpp` & `gdstk-0.9.38/src/label.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/label.h` & `gdstk-0.9.38/src/label.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/COPYING.txt` & `gdstk-0.9.38/src/libqhull_r/COPYING.txt`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/geom2_r.c` & `gdstk-0.9.38/src/libqhull_r/geom2_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/geom_r.c` & `gdstk-0.9.38/src/libqhull_r/geom_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/geom_r.h` & `gdstk-0.9.38/src/libqhull_r/geom_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/global_r.c` & `gdstk-0.9.38/src/libqhull_r/global_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/io_r.c` & `gdstk-0.9.38/src/libqhull_r/io_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/io_r.h` & `gdstk-0.9.38/src/libqhull_r/io_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/libqhull_r.c` & `gdstk-0.9.38/src/libqhull_r/libqhull_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/libqhull_r.h` & `gdstk-0.9.38/src/libqhull_r/libqhull_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/mem_r.c` & `gdstk-0.9.38/src/libqhull_r/mem_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/mem_r.h` & `gdstk-0.9.38/src/libqhull_r/mem_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/merge_r.c` & `gdstk-0.9.38/src/libqhull_r/merge_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/merge_r.h` & `gdstk-0.9.38/src/libqhull_r/merge_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/poly2_r.c` & `gdstk-0.9.38/src/libqhull_r/poly2_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/poly_r.c` & `gdstk-0.9.38/src/libqhull_r/poly_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/poly_r.h` & `gdstk-0.9.38/src/libqhull_r/poly_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/qhull_ra.h` & `gdstk-0.9.38/src/libqhull_r/qhull_ra.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/qset_r.c` & `gdstk-0.9.38/src/libqhull_r/qset_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/qset_r.h` & `gdstk-0.9.38/src/libqhull_r/qset_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/random_r.c` & `gdstk-0.9.38/src/libqhull_r/random_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/random_r.h` & `gdstk-0.9.38/src/libqhull_r/random_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/rboxlib_r.c` & `gdstk-0.9.38/src/libqhull_r/rboxlib_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/stat_r.c` & `gdstk-0.9.38/src/libqhull_r/stat_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/stat_r.h` & `gdstk-0.9.38/src/libqhull_r/stat_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/user_r.c` & `gdstk-0.9.38/src/libqhull_r/user_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/user_r.h` & `gdstk-0.9.38/src/libqhull_r/user_r.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/usermem_r.c` & `gdstk-0.9.38/src/libqhull_r/usermem_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/userprintf_r.c` & `gdstk-0.9.38/src/libqhull_r/userprintf_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/libqhull_r/userprintf_rbox_r.c` & `gdstk-0.9.38/src/libqhull_r/userprintf_rbox_r.c`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/library.cpp` & `gdstk-0.9.38/src/library.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -316,15 +316,15 @@
     }
 }
 
 ErrorCode Library::write_gds(const char* filename, uint64_t max_points, tm* timestamp) const {
     ErrorCode error_code = ErrorCode::NoError;
     FILE* out = fopen(filename, "wb");
     if (out == NULL) {
-        fputs("[GDSTK] Unable to open GDSII file for output.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open GDSII file for output.\n", error_logger);
         return ErrorCode::OutputFileOpenError;
     }
 
     tm now = {};
     if (!timestamp) timestamp = get_now(now);
 
     uint64_t len = strlen(name);
@@ -414,15 +414,15 @@
     state.config_flags = config_flags;
 
     if (compression_level > 9) compression_level = 9;
 
     OasisStream out;
     out.file = fopen(filename, "wb");
     if (out.file == NULL) {
-        fputs("[GDSTK] Unable to open OASIS file for output.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open OASIS file for output.\n", error_logger);
         return ErrorCode::OutputFileOpenError;
     }
     out.data_size = 1024 * 1024;
     out.data = (uint8_t*)allocate(out.data_size);
     out.cursor = NULL;
     out.crc32 = state.config_flags & OASIS_CONFIG_INCLUDE_CRC32;
     out.checksum32 = state.config_flags & OASIS_CONFIG_INCLUDE_CHECKSUM32;
@@ -669,15 +669,17 @@
             }
         }
 
         Reference** ref_p = cell->reference_array.items;
         for (uint64_t j = cell->reference_array.count; j > 0; j--) {
             Reference* ref = *ref_p++;
             if (ref->type == ReferenceType::RawCell) {
-                fputs("[GDSTK] Reference to a RawCell cannot be used in an OASIS file.\n", stderr);
+                if (error_logger)
+                    fputs("[GDSTK] Reference to a RawCell cannot be used in an OASIS file.\n",
+                          error_logger);
                 error_code = ErrorCode::MissingReference;
                 continue;
             }
             const char* name_ = (ref->type == ReferenceType::Cell) ? ref->cell->name : ref->name;
             bool reference_exists = cell_name_map.has_key(name_);
             uint8_t info = reference_exists ? 0xF0 : 0xB0;
             bool has_repetition = ref->repetition.get_count() > 1;
@@ -759,25 +761,25 @@
             // Skip empty cells
             if (uncompressed_size > 0) {
                 z_stream s = {};
                 s.zalloc = zalloc;
                 s.zfree = zfree;
                 if (deflateInit2(&s, compression_level, Z_DEFLATED, -15, 8, Z_DEFAULT_STRATEGY) !=
                     Z_OK) {
-                    fputs("[GDSTK] Unable to initialize zlib.\n", stderr);
+                    if (error_logger) fputs("[GDSTK] Unable to initialize zlib.\n", error_logger);
                     error_code = ErrorCode::ZlibError;
                 }
                 s.avail_out = deflateBound(&s, (uLong)uncompressed_size);
                 uint8_t* buffer = (uint8_t*)allocate(s.avail_out);
                 s.next_out = buffer;
                 s.avail_in = (uInt)uncompressed_size;
                 s.next_in = out.data;
                 int ret = deflate(&s, Z_FINISH);
                 if (ret != Z_STREAM_END) {
-                    fputs("[GDSTK] Unable to compress CBLOCK.\n", stderr);
+                    if (error_logger) fputs("[GDSTK] Unable to compress CBLOCK.\n", error_logger);
                     error_code = ErrorCode::ZlibError;
                 }
 
                 oasis_putc((int)OasisRecord::CBLOCK, out);
                 oasis_putc(0, out);
                 oasis_write_unsigned_integer(out, uncompressed_size);
                 oasis_write_unsigned_integer(out, s.total_out);
@@ -1028,16 +1030,17 @@
                         Cell* cp = map.get(reference->name);
                         if (cp) {
                             free_allocation(reference->name);
                             reference->type = ReferenceType::Cell;
                             reference->cell = cp;
                         } else {
                             if (error_code) *error_code = ErrorCode::MissingReference;
-                            fprintf(stderr, "[GDSTK] Missing referenced cell %s\n",
-                                    reference->name);
+                            if (error_logger)
+                                fprintf(error_logger, "[GDSTK] Missing referenced cell %s\n",
+                                        reference->name);
                         }
                     }
                 }
                 map.clear();
                 fclose(in);
                 return library;
             } break;
@@ -1219,17 +1222,18 @@
                 break;
             case GdsiiRecord::STRANS:
                 if (reference)
                     reference->x_reflection = (data16[0] & 0x8000) != 0;
                 else if (label)
                     label->x_reflection = (data16[0] & 0x8000) != 0;
                 if (data16[0] & 0x0006) {
-                    fputs(
-                        "[GDSTK] Absolute magnification and rotation of references is not supported.\n",
-                        stderr);
+                    if (error_logger)
+                        fputs(
+                            "[GDSTK] Absolute magnification and rotation of references is not supported.\n",
+                            error_logger);
                     if (error_code) *error_code = ErrorCode::UnsupportedRecord;
                 }
                 break;
             case GdsiiRecord::MAG:
                 if (reference)
                     reference->magnification = gdsii_real_to_double(data64[0]);
                 else if (label)
@@ -1305,18 +1309,20 @@
             // case GdsiiRecord::MASK:
             // case GdsiiRecord::ENDMASKS:
             // case GdsiiRecord::LIBDIRSIZE:
             // case GdsiiRecord::SRFNAME:
             // case GdsiiRecord::LIBSECUR:
             default:
                 if (buffer[2] < COUNT(gdsii_record_names)) {
-                    fprintf(stderr, "[GDSTK] Record type %s (0x%02X) is not supported.\n",
-                            gdsii_record_names[buffer[2]], buffer[2]);
+                    if (error_logger)
+                        fprintf(error_logger, "[GDSTK] Record type %s (0x%02X) is not supported.\n",
+                                gdsii_record_names[buffer[2]], buffer[2]);
                 } else {
-                    fprintf(stderr, "[GDSTK] Unknown record type 0x%02X.\n", buffer[2]);
+                    if (error_logger)
+                        fprintf(error_logger, "[GDSTK] Unknown record type 0x%02X.\n", buffer[2]);
                 }
                 if (error_code) *error_code = ErrorCode::UnsupportedRecord;
         }
     }
 
     library.free_all();
     fclose(in);
@@ -1326,38 +1332,38 @@
 // TODO: verify modal variables are correctly updated
 Library read_oas(const char* filename, double unit, double tolerance, ErrorCode* error_code) {
     Library library = {};
 
     OasisStream in = {};
     in.file = fopen(filename, "rb");
     if (in.file == NULL) {
-        fputs("[GDSTK] Unable to open OASIS file for input.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open OASIS file for input.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InputFileOpenError;
         return library;
     }
 
     // Check header bytes and START record
     char header[14];
     if (fread(header, 1, 14, in.file) < 14 || memcmp(header, "%SEMI-OASIS\r\n\x01", 14) != 0) {
-        fputs("[GDSTK] Invalid OASIS header found.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Invalid OASIS header found.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InvalidFile;
         fclose(in.file);
         return library;
     }
 
     // Process START record
     uint64_t len;
     uint8_t* version = oasis_read_string(in, false, len);
     if (in.error_code != ErrorCode::NoError) {
         if (error_code) *error_code = in.error_code;
         fclose(in.file);
         return library;
     }
     if (len != 3 || memcmp(version, "1.0", 3) != 0) {
-        fputs("[GDSTK] Unsupported OASIS file version.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unsupported OASIS file version.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InvalidFile;
     }
     free_allocation(version);
 
     double factor = 1 / oasis_read_real(in);
     library.precision = 1e-6 * factor;
     if (unit > 0) {
@@ -1461,15 +1467,17 @@
         //                 ? oasis_record_names[(uint8_t)record]
         //                 : "---");
         switch (record) {
             case OasisRecord::PAD:
                 break;
             case OasisRecord::START:
                 // START is parsed before this loop
-                fputs("[GDSTK] Unexpected START record out of position in file.\n", stderr);
+                if (error_logger)
+                    fputs("[GDSTK] Unexpected START record out of position in file.\n",
+                          error_logger);
                 if (error_code) *error_code = ErrorCode::InvalidFile;
                 break;
             case OasisRecord::END: {
                 FSEEK64(in.file, 0, SEEK_END);
                 library.name = (char*)allocate(4);
                 library.name[0] = 'L';
                 library.name[1] = 'I';
@@ -1525,26 +1533,30 @@
                             ByteArray* cell_name = cell_name_table.items + (uint64_t)ref->cell;
                             ref->cell = map.get((char*)cell_name->bytes);
                             if (!ref->cell) {
                                 ref->type = ReferenceType::Name;
                                 ref->name = (char*)allocate(cell_name->count);
                                 memcpy(ref->name, cell_name->bytes, cell_name->count);
                                 if (error_code) *error_code = ErrorCode::MissingReference;
-                                fprintf(stderr, "[GDSTK] Missing referenced cell %s\n", ref->name);
+                                if (error_logger)
+                                    fprintf(error_logger, "[GDSTK] Missing referenced cell %s\n",
+                                            ref->name);
                             }
                         } else {
                             // Using name
                             cell = map.get(ref->name);
                             if (cell) {
                                 free_allocation(ref->name);
                                 ref->cell = cell;
                                 ref->type = ReferenceType::Cell;
                             } else {
                                 if (error_code) *error_code = ErrorCode::MissingReference;
-                                fprintf(stderr, "[GDSTK] Missing referenced cell %s\n", ref->name);
+                                if (error_logger)
+                                    fprintf(error_logger, "[GDSTK] Missing referenced cell %s\n",
+                                            ref->name);
                             }
                         }
                     }
                 }
                 map.clear();
 
                 Property** prop_p = unfinished_property_name.items;
@@ -2365,28 +2377,28 @@
                     }
                     modal_property_value_list = property->value;
                 }
             } break;
             case OasisRecord::XNAME_IMPLICIT: {
                 oasis_read_unsigned_integer(in);
                 free_allocation(oasis_read_string(in, false, len));
-                fputs("[GDSTK] Record type XNAME ignored.\n", stderr);
+                if (error_logger) fputs("[GDSTK] Record type XNAME ignored.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::UnsupportedRecord;
             } break;
             case OasisRecord::XNAME: {
                 oasis_read_unsigned_integer(in);
                 free_allocation(oasis_read_string(in, false, len));
                 oasis_read_unsigned_integer(in);
-                fputs("[GDSTK] Record type XNAME ignored.\n", stderr);
+                if (error_logger) fputs("[GDSTK] Record type XNAME ignored.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::UnsupportedRecord;
             } break;
             case OasisRecord::XELEMENT: {
                 oasis_read_unsigned_integer(in);
                 free_allocation(oasis_read_string(in, false, len));
-                fputs("[GDSTK] Record type XELEMENT ignored.\n", stderr);
+                if (error_logger) fputs("[GDSTK] Record type XELEMENT ignored.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::UnsupportedRecord;
             } break;
             case OasisRecord::XGEOMETRY: {
                 uint8_t info;
                 oasis_read(&info, 1, 1, in);
                 oasis_read_unsigned_integer(in);
                 if (info & 0x01) {
@@ -2411,20 +2423,21 @@
                     } else {
                         modal_geom_pos.y += y;
                     }
                 }
                 if (info & 0x04) {
                     oasis_read_repetition(in, factor, modal_repetition);
                 }
-                fputs("[GDSTK] Record type XGEOMETRY ignored.\n", stderr);
+                if (error_logger) fputs("[GDSTK] Record type XGEOMETRY ignored.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::UnsupportedRecord;
             } break;
             case OasisRecord::CBLOCK: {
                 if (oasis_read_unsigned_integer(in) != 0) {
-                    fputs("[GDSTK] CBLOCK compression method not supported.\n", stderr);
+                    if (error_logger)
+                        fputs("[GDSTK] CBLOCK compression method not supported.\n", error_logger);
                     if (error_code) *error_code = ErrorCode::InvalidFile;
                     oasis_read_unsigned_integer(in);
                     len = oasis_read_unsigned_integer(in);
                     assert(len <= INT64_MAX);
                     FSEEK64(in.file, (int64_t)len, SEEK_SET);
                 } else {
                     z_stream s = {};
@@ -2435,37 +2448,42 @@
                     s.avail_in = (uInt)oasis_read_unsigned_integer(in);
                     in.data = (uint8_t*)allocate(in.data_size);
                     in.cursor = in.data;
                     s.next_out = in.data;
                     uint8_t* data = (uint8_t*)allocate(s.avail_in);
                     s.next_in = (Bytef*)data;
                     if (fread(s.next_in, 1, s.avail_in, in.file) != s.avail_in) {
-                        fputs("[GDSTK] Unable to read full CBLOCK.\n", stderr);
+                        if (error_logger)
+                            fputs("[GDSTK] Unable to read full CBLOCK.\n", error_logger);
                         if (error_code) *error_code = ErrorCode::InvalidFile;
                     }
                     if (inflateInit2(&s, -15) != Z_OK) {
-                        fputs("[GDSTK] Unable to initialize zlib.\n", stderr);
+                        if (error_logger)
+                            fputs("[GDSTK] Unable to initialize zlib.\n", error_logger);
                         if (error_code) *error_code = ErrorCode::ZlibError;
                     }
                     int ret = inflate(&s, Z_FINISH);
                     if (ret != Z_STREAM_END) {
-                        fputs("[GDSTK] Unable to decompress CBLOCK.\n", stderr);
+                        if (error_logger)
+                            fputs("[GDSTK] Unable to decompress CBLOCK.\n", error_logger);
                         if (error_code) *error_code = ErrorCode::ZlibError;
                     }
                     free_allocation(data);
                     inflateEnd(&s);
                     // Empty CBLOCK
                     if (in.data_size == 0) {
                         free_allocation(in.data);
                         in.data = NULL;
                     }
                 }
             } break;
             default:
-                fprintf(stderr, "[GDSTK] Unknown record type <0x%02X>.\n", (uint8_t)record);
+                if (error_logger)
+                    fprintf(error_logger, "[GDSTK] Unknown record type <0x%02X>.\n",
+                            (uint8_t)record);
                 if (error_code) *error_code = ErrorCode::UnsupportedRecord;
         }
     }
     if (in.error_code != ErrorCode::NoError && error_code) *error_code = in.error_code;
 
 CLEANUP:
     fclose(in.file);
@@ -2554,15 +2572,15 @@
         big_endian_swap16(new_tm_buffer, 6);
         memcpy(new_tm_buffer + 6, new_tm_buffer, 6 * sizeof(uint16_t));
         inout = fopen(filename, "r+b");
     } else {
         inout = fopen(filename, "rb");
     }
     if (inout == NULL) {
-        fputs("[GDSTK] Unable to open GDSII file.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open GDSII file.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InputFileOpenError;
         return result;
     }
 
     while (true) {
         uint64_t record_length = COUNT(buffer);
         ErrorCode err = gdsii_read_record(inout, buffer, record_length);
@@ -2572,15 +2590,15 @@
             return result;
         }
 
         GdsiiRecord record = (GdsiiRecord)buffer[2];
         if (record == GdsiiRecord::BGNLIB) {
             if (record_length != 28) {
                 fclose(inout);
-                fputs("[GDSTK] Invalid or corrupted GDSII file.\n", stderr);
+                if (error_logger) fputs("[GDSTK] Invalid or corrupted GDSII file.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::InvalidFile;
                 return result;
             }
             big_endian_swap16(data16, 6);
             result.tm_year = data16[0] - 1900;
             result.tm_mon = data16[1] - 1;
             result.tm_mday = data16[2];
@@ -2589,29 +2607,31 @@
             result.tm_sec = data16[5];
             if (!new_timestamp) {
                 fclose(inout);
                 return result;
             }
             if (FSEEK64(inout, -24, SEEK_CUR) != 0) {
                 fclose(inout);
-                fputs("[GDSTK] Unable to rewrite library timestamp.\n", stderr);
+                if (error_logger)
+                    fputs("[GDSTK] Unable to rewrite library timestamp.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::FileError;
                 return result;
             }
             fwrite(new_tm_buffer, sizeof(uint16_t), 12, inout);
         } else if (record == GdsiiRecord::BGNSTR && new_timestamp) {
             if (record_length != 28) {
                 fclose(inout);
-                fputs("[GDSTK] Invalid or corrupted GDSII file.\n", stderr);
+                if (error_logger) fputs("[GDSTK] Invalid or corrupted GDSII file.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::InvalidFile;
                 return result;
             }
             if (FSEEK64(inout, -24, SEEK_CUR) != 0) {
                 fclose(inout);
-                fputs("[GDSTK] Unable to rewrite cell timestamp.\n", stderr);
+                if (error_logger)
+                    fputs("[GDSTK] Unable to rewrite cell timestamp.\n", error_logger);
                 if (error_code) *error_code = ErrorCode::FileError;
                 return result;
             }
             fwrite(new_tm_buffer, sizeof(uint16_t), 12, inout);
         } else if (record == GdsiiRecord::ENDLIB) {
             break;
         }
@@ -2626,15 +2646,15 @@
     uint8_t buffer[65537];
     int16_t* data16 = (int16_t*)(buffer + 4);
     uint64_t* data64 = (uint64_t*)(buffer + 4);
     char* str = (char*)(buffer + 4);
 
     FILE* in = fopen(filename, "rb");
     if (in == NULL) {
-        fputs("[GDSTK] Unable to open GDSII file for input.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open GDSII file for input.\n", error_logger);
         return ErrorCode::InputFileOpenError;
     }
 
     ErrorCode error = ErrorCode::NoError;
     uint32_t layer = 0;
     Set<Tag>* next_set = NULL;
     while (true) {
@@ -2691,15 +2711,16 @@
             case GdsiiRecord::BOXTYPE:
             case GdsiiRecord::TEXTTYPE:
                 big_endian_swap16((uint16_t*)data16, 1);
                 if (next_set) {
                     next_set->add(make_tag(layer, data16[0]));
                     next_set = NULL;
                 } else {
-                    fputs("[GDSTK] Inconsistency detected in GDSII file.\n", stderr);
+                    if (error_logger)
+                        fputs("[GDSTK] Inconsistency detected in GDSII file.\n", error_logger);
                     error = ErrorCode::InvalidFile;
                 }
                 break;
             // case GdsiiRecord::HEADER:
             // case GdsiiRecord::BGNLIB:
             // case GdsiiRecord::ENDSTR:
             // case GdsiiRecord::LIBNAME:
@@ -2752,111 +2773,113 @@
     }
     return ErrorCode::InvalidFile;
 }
 
 ErrorCode oas_precision(const char* filename, double& precision) {
     FILE* in = fopen(filename, "rb");
     if (in == NULL) {
-        fputs("[GDSTK] Unable to open OASIS file for input.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open OASIS file for input.\n", error_logger);
         return ErrorCode::InputFileOpenError;
     }
 
     // Check header bytes and START record
     char header[14];
     if (fread(header, 1, 14, in) < 14 || memcmp(header, "%SEMI-OASIS\r\n\x01", 14) != 0) {
-        fputs("[GDSTK] Invalid OASIS header found.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Invalid OASIS header found.\n", error_logger);
         fclose(in);
         return ErrorCode::InvalidFile;
     }
 
     // Process START record
     OasisStream s = {in};
     uint64_t len;
     uint8_t* version = oasis_read_string(s, false, len);
     if (memcmp(version, "1.0", 3) != 0) {
-        fputs("[GDSTK] Unsupported OASIS file version.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unsupported OASIS file version.\n", error_logger);
         free_allocation(version);
         return ErrorCode::InvalidFile;
     }
     free_allocation(version);
 
     precision = 1e-6 / oasis_read_real(s);
     fclose(in);
     return ErrorCode::NoError;
 }
 
 bool oas_validate(const char* filename, uint32_t* signature, ErrorCode* error_code) {
     uint8_t buffer[32 * 1024];
     FILE* in = fopen(filename, "rb");
     if (in == NULL) {
-        fputs("[GDSTK] Unable to open OASIS file for input.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open OASIS file for input.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InputFileOpenError;
         return false;
     }
 
     // Check header bytes and START record
     char header[14];
     if (fread(header, 1, 14, in) < 14 || memcmp(header, "%SEMI-OASIS\r\n\x01", 14) != 0) {
-        fputs("[GDSTK] Invalid OASIS header found.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Invalid OASIS header found.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InvalidFile;
         fclose(in);
         return false;
     }
 
     if (FSEEK64(in, -5, SEEK_END) != 0) {
-        fputs("[GDSTK] Unable to find the END record of the file.\n", stderr);
+        if (error_logger)
+            fputs("[GDSTK] Unable to find the END record of the file.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InvalidFile;
         fclose(in);
         return false;
     }
 
     uint64_t size = ftell(in) + 1;
     uint8_t file_sum[5];
     if (fread(file_sum, 1, COUNT(file_sum), in) < 5) {
-        fputs("[GDSTK] Unable to read the END record of the file.\n", stderr);
+        if (error_logger)
+            fputs("[GDSTK] Unable to read the END record of the file.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InvalidFile;
         fclose(in);
         return false;
     }
 
     if (file_sum[0] == 1) {
         // CRC32
         uint32_t sig = crc32(0, NULL, 0);
         FSEEK64(in, 0, SEEK_SET);
         while (size >= COUNT(buffer)) {
             if (fread(buffer, 1, COUNT(buffer), in) < COUNT(buffer)) {
-                fprintf(stderr, "[GDSTK] Error reading file %s", filename);
+                if (error_logger) fprintf(error_logger, "[GDSTK] Error reading file %s", filename);
                 if (error_code) *error_code = ErrorCode::InvalidFile;
             }
             sig = crc32(sig, buffer, COUNT(buffer));
             size -= COUNT(buffer);
         }
         if (fread(buffer, 1, size, in) < size) {
-            fprintf(stderr, "[GDSTK] Error reading file %s", filename);
+            if (error_logger) fprintf(error_logger, "[GDSTK] Error reading file %s", filename);
             if (error_code) *error_code = ErrorCode::InvalidFile;
         }
         sig = crc32(sig, buffer, (unsigned int)size);
         little_endian_swap32(&sig, 1);
         if (signature) *signature = sig;
         // printf("CRC32: 0x%08X == 0x%08X\n", sig, *(uint32_t*)(file_sum + 1));
         if (sig != *(uint32_t*)(file_sum + 1)) return false;
     } else if (file_sum[0] == 2) {
         // Checksum32
         uint32_t sig = 0;
         FSEEK64(in, 0, SEEK_SET);
         while (size >= COUNT(buffer)) {
             if (fread(buffer, 1, COUNT(buffer), in) < COUNT(buffer)) {
-                fprintf(stderr, "[GDSTK] Error reading file %s", filename);
+                if (error_logger) fprintf(error_logger, "[GDSTK] Error reading file %s", filename);
                 if (error_code) *error_code = ErrorCode::InvalidFile;
             }
             sig = checksum32(sig, buffer, COUNT(buffer));
             size -= COUNT(buffer);
         }
         if (fread(buffer, 1, size, in) < size) {
-            fprintf(stderr, "[GDSTK] Error reading file %s", filename);
+            if (error_logger) fprintf(error_logger, "[GDSTK] Error reading file %s", filename);
             if (error_code) *error_code = ErrorCode::InvalidFile;
         }
         sig = checksum32(sig, buffer, size);
         little_endian_swap32(&sig, 1);
         if (signature) *signature = sig;
         // printf("Checksum32: 0x%08X == 0x%08X\n", sig, *(uint32_t*)(file_sum + 1));
         if (sig != *(uint32_t*)(file_sum + 1)) return false;
```

### Comparing `gdstk-0.9.37/src/library.h` & `gdstk-0.9.38/src/library.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/map.h` & `gdstk-0.9.38/src/map.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/oasis.cpp` & `gdstk-0.9.38/src/oasis.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -22,34 +22,35 @@
 ErrorCode oasis_read(void* buffer, size_t size, size_t count, OasisStream& in) {
     if (in.data) {
         uint64_t total = size * count;
         memcpy(buffer, in.cursor, total);
         in.cursor += total;
         if (in.cursor >= in.data + in.data_size) {
             if (in.cursor > in.data + in.data_size) {
-                fputs("[GDSTK] Error reading compressed data in file.\n", stderr);
+                if (error_logger)
+                    fputs("[GDSTK] Error reading compressed data in file.\n", error_logger);
                 in.error_code = ErrorCode::InputFileError;
             }
             free_allocation(in.data);
             in.data = NULL;
         }
     } else if (fread(buffer, size, count, in.file) < count) {
-        fputs("[GDSTK] Error reading OASIS file.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Error reading OASIS file.\n", error_logger);
         in.error_code = ErrorCode::InputFileError;
     }
     return in.error_code;
 }
 
 static uint8_t oasis_peek(OasisStream& in) {
     uint8_t byte;
     if (in.data) {
         byte = *in.cursor;
     } else {
         if (fread(&byte, 1, 1, in.file) < 1) {
-            fputs("[GDSTK] Error reading OASIS file.\n", stderr);
+            if (error_logger) fputs("[GDSTK] Error reading OASIS file.\n", error_logger);
             if (in.error_code == ErrorCode::NoError) in.error_code = ErrorCode::InputFileError;
         }
         FSEEK64(in.file, -1, SEEK_CUR);
     }
     return byte;
 }
 
@@ -112,15 +113,16 @@
     if (oasis_read(&byte, 1, 1, in) != ErrorCode::NoError) return 0;
 
     uint64_t result = (uint64_t)(byte & 0x7F);
     uint8_t num_bits = 7;
     while (byte & 0x80) {
         if (oasis_read(&byte, 1, 1, in) != ErrorCode::NoError) return result;
         if (num_bits == 63 && byte > 1) {
-            fputs("[GDSTK] Integer above maximal limit found. Clipping.\n", stderr);
+            if (error_logger)
+                fputs("[GDSTK] Integer above maximal limit found. Clipping.\n", error_logger);
             if (in.error_code == ErrorCode::NoError) in.error_code = ErrorCode::Overflow;
             return 0xFFFFFFFFFFFFFFFF;
         }
         result |= ((uint64_t)(byte & 0x7F)) << num_bits;
         num_bits += 7;
     }
     return result;
@@ -162,15 +164,16 @@
 
     result = ((uint64_t)(byte & 0x7F)) >> skip_bits;
     uint8_t bits = byte & ((1 << skip_bits) - 1);
     uint8_t num_bits = 7 - skip_bits;
     while (byte & 0x80) {
         if (oasis_read(&byte, 1, 1, in) != ErrorCode::NoError) return bits;
         if (num_bits > 56 && (byte >> (63 - num_bits)) > 0) {
-            fputs("[GDSTK] Integer above maximal limit found. Clipping.\n", stderr);
+            if (error_logger)
+                fputs("[GDSTK] Integer above maximal limit found. Clipping.\n", error_logger);
             if (in.error_code == ErrorCode::NoError) in.error_code = ErrorCode::Overflow;
             result = 0x7FFFFFFFFFFFFFFF;
             return bits;
         }
         result |= ((uint64_t)(byte & 0x7F)) << num_bits;
         num_bits += 7;
     }
@@ -318,15 +321,15 @@
         case OasisDataType::RealDouble: {
             double value;
             if (oasis_read(&value, sizeof(double), 1, in) != ErrorCode::NoError) return 0;
             little_endian_swap64((uint64_t*)&value, 1);
             return value;
         }
         default:
-            fputs("[GDSTK] Unable to determine real value.\n", stderr);
+            if (error_logger) fputs("[GDSTK] Unable to determine real value.\n", error_logger);
             if (in.error_code == ErrorCode::NoError) in.error_code = ErrorCode::InvalidFile;
     }
     return 0;
 }
 
 uint64_t oasis_read_point_list(OasisStream& in, double scaling, bool closed, Array<Vec2>& result) {
     assert(result.count > 0);
@@ -414,15 +417,15 @@
                 delta.x += scaling * x;
                 delta.y += scaling * y;
                 *cur++ = delta + *ref++;
             }
             result.count += num;
         } break;
         default:
-            fputs("[GDSTK] Point list type not supported.\n", stderr);
+            if (error_logger) fputs("[GDSTK] Point list type not supported.\n", error_logger);
             if (in.error_code == ErrorCode::NoError) in.error_code = ErrorCode::InvalidFile;
             return 0;
     }
     return num;
 }
 
 void oasis_read_repetition(OasisStream& in, double scaling, Repetition& repetition) {
@@ -574,15 +577,15 @@
     } else if (y == 0) {
         if (x < 0) {
             oasis_write_int_internal(out, -x, 2, (uint8_t)OasisDirection::W);
         } else {
             oasis_write_int_internal(out, x, 2, (uint8_t)OasisDirection::E);
         }
     } else {
-        fputs("[GDSTK] Error writing 2-delta.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Error writing 2-delta.\n", error_logger);
     }
 }
 
 void oasis_write_3delta(OasisStream& out, int64_t x, int64_t y) {
     assert(x == 0 || y == 0 || x == y || x == -y);
     if (x == 0) {
         if (y < 0) {
@@ -605,15 +608,15 @@
     } else if (x == -y) {
         if (x < 0) {
             oasis_write_int_internal(out, -x, 3, (uint8_t)OasisDirection::NW);
         } else {
             oasis_write_int_internal(out, x, 3, (uint8_t)OasisDirection::SE);
         }
     } else {
-        fputs("[GDSTK] Error writing 3-delta.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Error writing 3-delta.\n", error_logger);
     }
 }
 
 void oasis_write_gdelta(OasisStream& out, int64_t x, int64_t y) {
     if (x == 0) {
         if (y < 0) {
             oasis_write_int_internal(out, -y, 4, (uint8_t)OasisDirection::S << 1);
@@ -786,62 +789,74 @@
                 }
                 break;
             default:
                 break;
         }
     }
 
+    uint64_t count = points.count - 1;
+    if (list_type == OasisPointList::ManhattanHorizontalFirst ||
+        list_type == OasisPointList::ManhattanVerticalFirst) {
+        if (closed) {
+            --count;
+            if (count < 2 || count % 2 == 1) {
+                // There is probably a duplicate vertex in the polygon,
+                // otherwise the point count should be even.
+                count = points.count - 1;
+                list_type = OasisPointList::Manhattan;
+            }
+        }
+    }
+
     switch (list_type) {
         case OasisPointList::ManhattanHorizontalFirst: {
             oasis_putc((uint8_t)OasisPointList::ManhattanHorizontalFirst, out);
-            uint64_t count = closed ? points.count - 2 : points.count - 1;
             oasis_write_unsigned_integer(out, count);
             prev_delta_is_horizontal = false;
             IntVec2* delta = points.items + 1;
             for (uint64_t i = count; i > 0; i--) {
                 oasis_write_1delta(out, prev_delta_is_horizontal ? delta->y : delta->x);
                 prev_delta_is_horizontal = !prev_delta_is_horizontal;
                 delta++;
             }
         } break;
         case OasisPointList::ManhattanVerticalFirst: {
             oasis_putc((uint8_t)OasisPointList::ManhattanVerticalFirst, out);
-            uint64_t count = closed ? points.count - 2 : points.count - 1;
             oasis_write_unsigned_integer(out, count);
             prev_delta_is_horizontal = true;
             IntVec2* delta = points.items + 1;
             for (uint64_t i = count; i > 0; i--) {
                 oasis_write_1delta(out, prev_delta_is_horizontal ? delta->y : delta->x);
                 prev_delta_is_horizontal = !prev_delta_is_horizontal;
                 delta++;
             }
         } break;
         case OasisPointList::Manhattan: {
             oasis_putc((uint8_t)OasisPointList::Manhattan, out);
-            oasis_write_unsigned_integer(out, points.count - 1);
+            oasis_write_unsigned_integer(out, count);
             IntVec2* delta = points.items + 1;
-            for (uint64_t i = points.count - 1; i > 0; i--) {
+            for (uint64_t i = count; i > 0; i--) {
                 oasis_write_2delta(out, delta->x, delta->y);
                 delta++;
             }
         } break;
         case OasisPointList::Octangular: {
             oasis_putc((uint8_t)OasisPointList::Octangular, out);
-            oasis_write_unsigned_integer(out, points.count - 1);
+            oasis_write_unsigned_integer(out, count);
             IntVec2* delta = points.items + 1;
-            for (uint64_t i = points.count - 1; i > 0; i--) {
+            for (uint64_t i = count; i > 0; i--) {
                 oasis_write_3delta(out, delta->x, delta->y);
                 delta++;
             }
         } break;
         default: {
             oasis_putc((uint8_t)OasisPointList::General, out);
-            oasis_write_unsigned_integer(out, points.count - 1);
+            oasis_write_unsigned_integer(out, count);
             IntVec2* delta = points.items + 1;
-            for (uint64_t i = points.count - 1; i > 0; i--) {
+            for (uint64_t i = count; i > 0; i--) {
                 oasis_write_gdelta(out, delta->x, delta->y);
                 delta++;
             }
         }
     }
 }
```

### Comparing `gdstk-0.9.37/src/oasis.h` & `gdstk-0.9.38/src/oasis.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/pathcommon.h` & `gdstk-0.9.38/src/pathcommon.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/polygon.cpp` & `gdstk-0.9.38/src/polygon.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -417,17 +417,18 @@
         4, 0x0800, 6, 0x0D02, (uint16_t)get_layer(tag), 6, 0x0E02, (uint16_t)get_type(tag)};
     uint16_t buffer_end[] = {4, 0x1100};
     big_endian_swap16(buffer_start, COUNT(buffer_start));
     big_endian_swap16(buffer_end, COUNT(buffer_end));
 
     uint64_t total = point_array.count + 1;
     if (total > 8190) {
-        fputs(
-            "[GDSTK] Polygons with more than 8190 are not supported by the official GDSII specification. This GDSII file might not be compatible with all readers.\n",
-            stderr);
+        if (error_logger)
+            fputs(
+                "[GDSTK] Polygons with more than 8190 are not supported by the official GDSII specification. This GDSII file might not be compatible with all readers.\n",
+                error_logger);
         error_code = ErrorCode::UnofficialSpecification;
     }
     Array<int32_t> coords = {};
     coords.ensure_slots(2 * total);
     coords.count = 2 * total;
 
     Vec2 zero = {0, 0};
@@ -1594,15 +1595,16 @@
         for (uint64_t i = 0; i < islands.count && !found; i++) {
             if (hole_area < island_areas[i] && islands[i]->contain_all(hole->point_array)) {
                 islands_holes[i].append(hole);
                 found = true;
             }
         }
         if (!found) {
-            fprintf(stderr, "[GDSTK] Unable to process polygon hole in contour.\n");
+            if (error_logger)
+                fprintf(error_logger, "[GDSTK] Unable to process polygon hole in contour.\n");
             error_code = ErrorCode::BooleanError;
             hole->clear();
             free_allocation(hole);
         }
     }
 
     holes.clear();
```

### Comparing `gdstk-0.9.37/src/polygon.h` & `gdstk-0.9.38/src/polygon.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/property.cpp` & `gdstk-0.9.38/src/property.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -328,17 +328,18 @@
         big_endian_swap16(buffer_prop, COUNT(buffer_prop));
         fwrite(buffer_prop, sizeof(uint16_t), COUNT(buffer_prop), out);
         fwrite(bytes, 1, len, out);
 
         if (free_bytes) free_allocation(bytes);
     }
     if (count > 128) {
-        fputs(
-            "[GDSTK] Properties with count larger than 128 bytes are not officially supported by the GDSII specification.  This file might not be compatible with all readers.\n",
-            stderr);
+        if (error_logger)
+            fputs(
+                "[GDSTK] Properties with count larger than 128 bytes are not officially supported by the GDSII specification.  This file might not be compatible with all readers.\n",
+                error_logger);
         return ErrorCode::UnofficialSpecification;
     }
     return ErrorCode::NoError;
 }
 
 ErrorCode properties_to_oas(const Property* properties, OasisStream& out, OasisState& state) {
     while (properties) {
```

### Comparing `gdstk-0.9.37/src/property.h` & `gdstk-0.9.38/src/property.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/rawcell.cpp` & `gdstk-0.9.38/src/rawcell.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,16 @@
 ErrorCode RawCell::to_gds(FILE* out) {
     ErrorCode error_code = ErrorCode::NoError;
     if (source) {
         uint64_t off = offset;
         data = (uint8_t*)allocate(size);
         int64_t result = source->offset_read(data, size, off);
         if (result < 0 || (uint64_t)result != size) {
-            fputs("[GDSTK] Unable to read RawCell data form input file.\n", stderr);
+            if (error_logger)
+                fputs("[GDSTK] Unable to read RawCell data form input file.\n", error_logger);
             error_code = ErrorCode::InputFileError;
             size = 0;
         }
         source->uses--;
         if (source->uses == 0) {
             fclose(source->file);
             free_allocation(source);
@@ -94,15 +95,15 @@
     uint8_t buffer[65537];
     char* str = (char*)(buffer + 4);
 
     RawSource* source = (RawSource*)allocate(sizeof(RawSource));
     source->uses = 0;
     source->file = fopen(filename, "rb");
     if (source->file == NULL) {
-        fputs("[GDSTK] Unable to open input GDSII file.\n", stderr);
+        if (error_logger) fputs("[GDSTK] Unable to open input GDSII file.\n", error_logger);
         if (error_code) *error_code = ErrorCode::InputFileOpenError;
         return result;
     }
 
     RawCell* rawcell = NULL;
 
     while (true) {
@@ -125,15 +126,17 @@
                                 dependencies->remove_unordered(i);
                             } else {
                                 (*dependencies)[i] = rawcell;
                                 i++;
                             }
                         } else {
                             dependencies->remove_unordered(i);
-                            fprintf(stderr, "[GDSTK] Referenced cell %s not found.\n", name);
+                            if (error_logger)
+                                fprintf(error_logger, "[GDSTK] Referenced cell %s not found.\n",
+                                        name);
                             if (error_code) *error_code = ErrorCode::MissingReference;
                         }
                         free_allocation(name);
                     }
                 }
                 if (source->uses == 0) {
                     fclose(source->file);
@@ -190,13 +193,13 @@
             free_allocation(name);
         }
         rawcell->clear();
     }
     fclose(source->file);
     free_allocation(source);
     result.clear();
-    fprintf(stderr, "[GDSTK] Invalid GDSII file %s.\n", filename);
+    if (error_logger) fprintf(error_logger, "[GDSTK] Invalid GDSII file %s.\n", filename);
     if (error_code) *error_code = ErrorCode::InvalidFile;
     return result;
 }
 
 }  // namespace gdstk
```

### Comparing `gdstk-0.9.37/src/rawcell.h` & `gdstk-0.9.38/src/rawcell.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/reference.cpp` & `gdstk-0.9.38/src/reference.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -422,17 +422,18 @@
                 x3 = origin.x + rows * v1.x;
                 y3 = origin.y + rows * v1.y;
             }
         }
 
         if (array) {
             if (repetition.columns > UINT16_MAX || repetition.rows > UINT16_MAX) {
-                fputs(
-                    "[GDSTK] Repetition with more than 65535 columns or rows cannot be saved to a GDSII file.\n",
-                    stderr);
+                if (error_logger)
+                    fputs(
+                        "[GDSTK] Repetition with more than 65535 columns or rows cannot be saved to a GDSII file.\n",
+                        error_logger);
                 error_code = ErrorCode::InvalidRepetition;
                 buffer_array[2] = UINT16_MAX;
                 buffer_array[3] = UINT16_MAX;
             } else {
                 buffer_array[2] = (uint16_t)columns;
                 buffer_array[3] = (uint16_t)rows;
             }
```

### Comparing `gdstk-0.9.37/src/reference.h` & `gdstk-0.9.38/src/reference.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/repetition.cpp` & `gdstk-0.9.38/src/repetition.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/repetition.h` & `gdstk-0.9.38/src/repetition.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/robustpath.cpp` & `gdstk-0.9.38/src/robustpath.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1065,18 +1065,19 @@
             norm_v0 = v0.normalize();
             norm_v1 = v1.normalize();
             segments_intersection(p0, v0, p1, v1, du0, du1);
             du0 /= norm_v0;
             du1 /= norm_v1;
         }
     }
-    fprintf(
-        stderr,
-        "[GDSTK] No intersection found in RobustPath spine construction around (%lg, %lg) and (%lg, %lg).\n",
-        p0.x, p0.y, p1.x, p1.y);
+    if (error_logger)
+        fprintf(
+            error_logger,
+            "[GDSTK] No intersection found in RobustPath spine construction around (%lg, %lg) and (%lg, %lg).\n",
+            p0.x, p0.y, p1.x, p1.y);
     return ErrorCode::IntersectionNotFound;
 }
 
 ErrorCode RobustPath::center_intersection(const SubPath &sub0, const Interpolation &offset0,
                                           const SubPath &sub1, const Interpolation &offset1,
                                           double &u0, double &u1) const {
     const double tolerance_sq = tolerance * tolerance;
@@ -1119,18 +1120,19 @@
             norm_v0 = v0.normalize();
             norm_v1 = v1.normalize();
             segments_intersection(p0, v0, p1, v1, du0, du1);
             du0 /= norm_v0;
             du1 /= norm_v1;
         }
     }
-    fprintf(
-        stderr,
-        "[GDSTK] No intersection found in RobustPath center construction around (%lg, %lg) and (%lg, %lg).\n",
-        p0.x, p0.y, p1.x, p1.y);
+    if (error_logger)
+        fprintf(
+            error_logger,
+            "[GDSTK] No intersection found in RobustPath center construction around (%lg, %lg) and (%lg, %lg).\n",
+            p0.x, p0.y, p1.x, p1.y);
     return ErrorCode::IntersectionNotFound;
 }
 
 ErrorCode RobustPath::left_intersection(const SubPath &sub0, const Interpolation &offset0,
                                         const Interpolation &width0, const SubPath &sub1,
                                         const Interpolation &offset1, const Interpolation &width1,
                                         double &u0, double &u1) const {
@@ -1174,18 +1176,19 @@
             norm_v0 = v0.normalize();
             norm_v1 = v1.normalize();
             segments_intersection(p0, v0, p1, v1, du0, du1);
             du0 /= norm_v0;
             du1 /= norm_v1;
         }
     }
-    fprintf(
-        stderr,
-        "[GDSTK] No intersection found in RobustPath left side construction around (%lg, %lg) and (%lg, %lg).\n",
-        p0.x, p0.y, p1.x, p1.y);
+    if (error_logger)
+        fprintf(
+            error_logger,
+            "[GDSTK] No intersection found in RobustPath left side construction around (%lg, %lg) and (%lg, %lg).\n",
+            p0.x, p0.y, p1.x, p1.y);
     return ErrorCode::IntersectionNotFound;
 }
 
 ErrorCode RobustPath::right_intersection(const SubPath &sub0, const Interpolation &offset0,
                                          const Interpolation &width0, const SubPath &sub1,
                                          const Interpolation &offset1, const Interpolation &width1,
                                          double &u0, double &u1) const {
@@ -1229,18 +1232,19 @@
             norm_v0 = v0.normalize();
             norm_v1 = v1.normalize();
             segments_intersection(p0, v0, p1, v1, du0, du1);
             du0 /= norm_v0;
             du1 /= norm_v1;
         }
     }
-    fprintf(
-        stderr,
-        "[GDSTK] No intersection found in RobustPath right side construction around (%lg, %lg) and (%lg, %lg).\n",
-        p0.x, p0.y, p1.x, p1.y);
+    if (error_logger)
+        fprintf(
+            error_logger,
+            "[GDSTK] No intersection found in RobustPath right side construction around (%lg, %lg) and (%lg, %lg).\n",
+            p0.x, p0.y, p1.x, p1.y);
     return ErrorCode::IntersectionNotFound;
 }
 
 ErrorCode RobustPath::spine(Array<Vec2> &result) const {
     ErrorCode error_code = ErrorCode::NoError;
     if (subpath_array.count == 0) return error_code;
     result.ensure_slots(subpath_array.count + 1);
```

### Comparing `gdstk-0.9.37/src/robustpath.h` & `gdstk-0.9.38/src/robustpath.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/set.h` & `gdstk-0.9.38/src/set.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/sort.h` & `gdstk-0.9.38/src/sort.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/style.cpp` & `gdstk-0.9.38/src/style.cpp`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/style.h` & `gdstk-0.9.38/src/style.h`

 * *Files identical despite different names*

### Comparing `gdstk-0.9.37/src/utils.cpp` & `gdstk-0.9.38/src/utils.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 #include "vec.h"
 
 // Qhull
 #include "libqhull_r/qhull_ra.h"
 
 namespace gdstk {
 
+FILE* error_logger = stderr;
+
+void set_error_logger(FILE* log) { error_logger = log; }
+
 char* copy_string(const char* str, uint64_t* len) {
     uint64_t size = 1 + strlen(str);
     char* result = (char*)allocate(size);
     memcpy(result, str, size);
     if (len) *len = size;
     return result;
 }
@@ -568,18 +572,18 @@
         convex_hull(temp, result);
         temp.clear();
         return;
     }
 
     qhT qh;
     QHULL_LIB_CHECK;
-    qh_zero(&qh, stderr);
+    qh_zero(&qh, error_logger);
     char command[256] = "qhull";
     int exitcode = qh_new_qhull(&qh, 2, (int)points.count, (double*)points.items, false, command,
-                                NULL, stderr);
+                                NULL, error_logger);
 
     if (exitcode == 0) {
         result.ensure_slots(qh.num_facets);
         Vec2* point = result.items + result.count;
         result.count += qh.num_facets;
 
         vertexT* qh_vertex = NULL;
@@ -613,15 +617,15 @@
     qh_freeqhull(&qh, qh_ALL);
 #else
     int curlong, totlong;
     qh_freeqhull(&qh, !qh_ALL);               /* free long memory  */
     qh_memfreeshort(&qh, &curlong, &totlong); /* free short memory and memory allocator */
     if (curlong || totlong) {
         fprintf(
-            stderr,
+            error_logger,
             "[GDSTK] Qhull internal warning: did not free %d bytes of long memory (%d pieces)\n",
             totlong, curlong);
     }
 #endif
 }
 
 char* double_print(double value, uint32_t precision, char* buffer, size_t buffer_size) {
```

### Comparing `gdstk-0.9.37/src/utils.h` & `gdstk-0.9.38/src/utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 // Smooth interpolation (3rd order polynomial with zero derivatives at 0 and 1)
 #define SERP(a, b, u) ((a) + ((b) - (a)) * (3 - 2 * (u)) * (u) * (u))
 
 #ifdef NDEBUG
 #define DEBUG_HERE ((void)0)
 #define DEBUG_PRINT(...) ((void)0)
 #else
-#define DEBUG_HERE                                                   \
-    do {                                                             \
-        fprintf(stderr, "%s:%d:%s\n", __FILE__, __LINE__, __func__); \
-        fflush(stderr);                                              \
+#define DEBUG_HERE                                                         \
+    do {                                                                   \
+        fprintf(error_logger, "%s:%d:%s\n", __FILE__, __LINE__, __func__); \
+        fflush(error_logger);                                              \
     } while (false)
-#define DEBUG_PRINT(...)              \
-    do {                              \
-        fprintf(stderr, __VA_ARGS__); \
-        fflush(stderr);               \
+#define DEBUG_PRINT(...)                    \
+    do {                                    \
+        fprintf(error_logger, __VA_ARGS__); \
+        fflush(error_logger);               \
     } while (false)
 #endif
 
 // From http://esr.ibiblio.org/?p=5095
 #define IS_BIG_ENDIAN (*(uint16_t*)"\0\xFF" < 0x100)
 
 #ifdef _WIN32
@@ -224,10 +224,13 @@
     for (const char* c = key; *c; c++) {
         result ^= (uint64_t)(*c);
         result *= HASH_FNV_PRIME;
     }
     return result;
 }
 
+extern FILE* error_logger;
+void set_error_logger(FILE* log);
+
 }  // namespace gdstk
 
 #endif
```

### Comparing `gdstk-0.9.37/src/vec.h` & `gdstk-0.9.38/src/vec.h`

 * *Files identical despite different names*

