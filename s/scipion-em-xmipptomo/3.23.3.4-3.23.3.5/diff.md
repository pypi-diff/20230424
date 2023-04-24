# Comparing `tmp/scipion-em-xmipptomo-3.23.3.4.tar.gz` & `tmp/scipion-em-xmipptomo-3.23.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-xmipptomo-3.23.3.4.tar", last modified: Thu Apr 20 22:01:49 2023, max compression
+gzip compressed data, was "scipion-em-xmipptomo-3.23.3.5.tar", last modified: Mon Apr 24 10:50:57 2023, max compression
```

## Comparing `scipion-em-xmipptomo-3.23.3.4.tar` & `scipion-em-xmipptomo-3.23.3.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.815284 scipion-em-xmipptomo-3.23.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.807284 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:01:49.815284 scipion-em-xmipptomo-3.23.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.807284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_align_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_applyAlignmentTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_coords_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_resize_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_flexalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_half_maps_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_project_top.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resizeTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resize_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_roiIJ.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_splitTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtomo_map_back.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtraction_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_xmipptomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/monotomo_tree_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_phantom_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_score_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/xmipp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.951076 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 10:50:57.000000 scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.955076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.955076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_align_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_applyAlignmentTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_coords_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_resize_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_flexalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_half_maps_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_project_top.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resizeTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resize_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_roiIJ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_splitTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtomo_map_back.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtraction_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.955076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_xmipptomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:50:57.959076 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/monotomo_tree_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_phantom_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_score_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-24 10:48:59.000000 scipion-em-xmipptomo-3.23.3.5/xmipptomo/xmipp_logo.png
```

### Comparing `scipion-em-xmipptomo-3.23.3.4/CHANGES.txt` & `scipion-em-xmipptomo-3.23.3.5/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 V3.23.03.4:
+ - Map back fix: works with 3d classes
+V3.23.03.4:
  - Mapback waits now when scheduled and not the reference is needed (validation added)
 
 V3.23.03.3:
  - Fit vesicles removed (moved to tomo)
 
 V3.23.03.2:
  - Mapback scales any reference to match the tomogram sampling.
```

### Comparing `scipion-em-xmipptomo-3.23.3.4/LICENSE` & `scipion-em-xmipptomo-3.23.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.4
+Version: 3.23.3.5
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.4
+Version: 3.23.3.5
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/SOURCES.txt` & `scipion-em-xmipptomo-3.23.3.5/scipion_em_xmipptomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/setup.py` & `scipion-em-xmipptomo-3.23.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/__init__.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # **************************************************************************
 import xmipp3
 import subprocess, os
 import pyworkflow.utils as pwutils
 
 _logo = "xmipp_logo.png"
 _references = ['delaRosaTrevin2013']
-__version__ = "3.23.03.4" #X.YY.MM.sv
+__version__ = "3.23.03.5" #X.YY.MM.sv
         # X.Y.M = version of the xmipp release associated.
         # sv = Set this to ".0" on each xmipp  release.
         # For not release version (hotfix) increase it --> ".1", ".2", ...
 
 class Plugin(xmipp3.Plugin):
 
     @classmethod
```

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/bibtex.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/__init__.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_align_transform.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_align_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_applyAlignmentTS.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_applyAlignmentTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_apply_alignment_subtomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_apply_alignment_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_cltomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_connected_components.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_connected_components.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_coords_roi.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_coords_roi.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_resize_base.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_resize_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_tomograms.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_crop_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_extract_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_filter_coordinates_by_map.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_filter_coordinates_by_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_flexalign.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_flexalign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_half_maps_subtomos.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_half_maps_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_tomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_phantom_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_project_top.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_project_top.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resizeTS.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resizeTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resize_tomograms.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resize_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_roiIJ.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_roiIJ.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_coordinates.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_transform.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_score_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_splitTS.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_splitTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtomo_map_back.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtomo_map_back.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from pwem.protocols import EMProtocol
 
 from pyworkflow import BETA
 from pyworkflow.protocol import STEPS_PARALLEL
 from pyworkflow.protocol.params import PointerParam, EnumParam, BooleanParam, FloatParam
 from pyworkflow.utils import createLink
 
-from tomo.objects import Tomogram, SetOfCoordinates3D, SetOfSubTomograms, SetOfClassesSubTomograms, SubTomogram, \
+from tomo.objects import Tomogram, SetOfCoordinates3D, SetOfSubTomograms, SetOfClassesSubTomograms, ClassSubTomogram, \
     MATRIX_CONVERSION, SetOfTomograms
 from tomo.protocols import ProtTomoBase
 from xmipp3.convert import alignmentToRow
 import tomo.constants as const
 
 REFERENCE = 'Reference'
 
@@ -134,42 +134,43 @@
 
     # --------------------------- STEPS functions -------------------------------
 
 
     def prepareReference(self, invertContrast):
         """ Prepares the reference for the mapback"""
         fnRef = self.getFinalRefName()
-        sourceRef = self.getSourceReferenceFn()
+        refItem = self.getSourceReference()
+        sourceRefFn = refItem.getFileName()
+        refSampling = refItem.getSamplingRate()
 
         # Do we need this conversion!!
         # img = ImageHandler()
         # img.convert(sourceRef, fnRef)
 
-        refSampling = self.inputRef.get().getSamplingRate()
         tomoSampling = self.getInputSetOfTomograms().getSamplingRate()
         # for xmipp 0.5 means halving, 2 means doubling
         factor = refSampling/tomoSampling
         if invertContrast:
-            self.runJob("xmipp_image_operate", " -i %s  --mult -1 -o %s" % (sourceRef, fnRef))
-            sourceRef = fnRef
+            self.runJob("xmipp_image_operate", " -i %s  --mult -1 -o %s" % (sourceRefFn, fnRef))
+            sourceRefFn = fnRef
 
         if factor != 1:
-            self.runJob("xmipp_image_resize", " -i %s  --factor %0.2f -o %s" % (sourceRef, factor, fnRef))
+            self.runJob("xmipp_image_resize", " -i %s  --factor %0.2f -o %s" % (sourceRefFn, factor, fnRef))
 
 
         if not os.path.exists(fnRef):
-            createLink(sourceRef, fnRef)
+            createLink(sourceRefFn, fnRef)
 
-    def getSourceReferenceFn(self):
+    def getSourceReference(self):
         """ Returns the source reference file name: representative from the first class or the reference param"""
         if self._useClasses():
             firstClass = self.inputClasses.get().getFirstItem()
             return firstClass.getRepresentative()
         else:
-            return self.inputRef.get().getFileName()
+            return self.inputRef.get()
 
     def getFinalRefName(self):
         """ returns the final path of the reference"""
         return self._getExtraPath('reference.mrc')
 
     def getFinalTomoName(self, tomo):
         """ Returns the final tomogram name having a tomogram. Uses the Tilt Series Id"""
```

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtraction_subtomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols/protocol_subtraction_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols.conf` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/__init__.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_extract_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_monotomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_crop.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_crop.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_resize.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_xmipptomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/tests/test_protocols_xmipptomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/utils.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/__init__.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/monotomo_tree_provider.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/monotomo_tree_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_cltomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_phantom_create.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_phantom_create.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_score_subtomos.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/viewers/viewer_score_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/wizards.py` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.4/xmipptomo/xmipp_logo.png` & `scipion-em-xmipptomo-3.23.3.5/xmipptomo/xmipp_logo.png`

 * *Files identical despite different names*

