# Comparing `tmp/scipion-em-tomo-3.1.7.tar.gz` & `tmp/scipion-em-tomo-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomo-3.1.7.tar", last modified: Fri Apr 21 09:07:25 2023, max compression
+gzip compressed data, was "scipion-em-tomo-3.1.8.tar", last modified: Mon Apr 24 13:02:54 2023, max compression
```

## Comparing `scipion-em-tomo-3.1.7.tar` & `scipion-em-tomo-3.1.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.681352 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.681352 scipion-em-tomo-3.1.7/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.685353 scipion-em-tomo-3.1.7/tomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/convert/mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   100531 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.693353 scipion-em-tomo-3.1.7/tomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_assignTransformationTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2tomoMask.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_consensus_classes_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ctf_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_extract_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_fit_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates_from_scipion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomomasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_misalignTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_particles_to_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_rotate_astigmatism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_split_evenodd_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_tomo_to_mics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_consensus_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_convert_coords3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_correct_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_estimate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.693353 scipion-em-tomo-3.1.7/tomo/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/HIV-Picking-with-Dynamo.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/HIV-Reconstruction.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/HIV-Subtomogram-averaging.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/Membrane picking-with-PySeg.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/tomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_base_centralized_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_fit_vesicles.py
--rw-r--r--   0 runner    (1001) docker     (123)    41397 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    43270 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_tomo_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/tomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/viewer_split_evenodd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    40940 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.024696 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 13:02:53.000000 scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.024696 scipion-em-tomo-3.1.8/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.028696 scipion-em-tomo-3.1.8/tomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/convert/mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   101779 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.032696 scipion-em-tomo-3.1.8/tomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_assignTransformationTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2tomoMask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_consensus_classes_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ctf_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_extract_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_fit_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates_from_scipion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomomasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_misalignTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_particles_to_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_rotate_astigmatism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_split_evenodd_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_tomo_to_mics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_consensus_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_convert_coords3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_correct_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_estimate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.032696 scipion-em-tomo-3.1.8/tomo/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/HIV-Picking-with-Dynamo.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/HIV-Reconstruction.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/HIV-Subtomogram-averaging.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/Membrane picking-with-PySeg.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/tomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_base_centralized_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_fit_vesicles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41397 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43270 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_tomo_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:02:54.036696 scipion-em-tomo-3.1.8/tomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/viewer_split_evenodd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40940 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-24 12:56:49.000000 scipion-em-tomo-3.1.8/tomo/wizards.py
```

### Comparing `scipion-em-tomo-3.1.7/LICENSE` & `scipion-em-tomo-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/PKG-INFO` & `scipion-em-tomo-3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.7
+Version: 3.1.8
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.7/README.rst` & `scipion-em-tomo-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/PKG-INFO` & `scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.7
+Version: 3.1.8
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/SOURCES.txt` & `scipion-em-tomo-3.1.8/scipion_em_tomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/setup.py` & `scipion-em-tomo-3.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/__init__.py` & `scipion-em-tomo-3.1.8/tomo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pwem
 
-__version__ = '3.1.7'
+__version__ = '3.1.8'
 _logo = "icon.png"
 _references = []
 
 
 class Plugin(pwem.Plugin):
     @classmethod
     def _defineVariables(cls):
```

### Comparing `scipion-em-tomo-3.1.7/tomo/constants.py` & `scipion-em-tomo-3.1.8/tomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/convert/__init__.py` & `scipion-em-tomo-3.1.8/tomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/convert/convert.py` & `scipion-em-tomo-3.1.8/tomo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/convert/mdoc.py` & `scipion-em-tomo-3.1.8/tomo/convert/mdoc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/icon.png` & `scipion-em-tomo-3.1.8/tomo/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/objects.py` & `scipion-em-tomo-3.1.8/tomo/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1688,21 +1688,22 @@
         super().copyInfo(other)
         if hasattr(other, '_coordsPointer'):  # Like the vesicles in pyseg
             self.copyAttributes(other, '_coordsPointer')
 
     def hasCoordinates3D(self):
         return self._coordsPointer.hasValue()
 
-    def getCoordinates3D(self):
+    def getCoordinates3D(self, asPointer = False):
         """ Returns the SetOfCoordinates associated with
         this SetOfSubTomograms"""
-        return self._coordsPointer.get()
+
+        return self._coordsPointer if asPointer else self._coordsPointer.get()
 
     def setCoordinates3D(self, coordinates):
-        """ Set the SetOfCoordinates associates with
+        """ Set the SetOfCoordinates associated with
         this set of particles.
          """
         if isinstance(coordinates, Pointer):
             self._coordsPointer = coordinates
         else:
             self._coordsPointer.set(coordinates)
 
@@ -1849,14 +1850,40 @@
 
 class SetOfClassesSubTomograms(data.SetOfClasses):
     """ Store results from a subtomogram averaging method. """
     ITEM_TYPE = ClassSubTomogram
     REP_TYPE = AverageSubTomogram
     REP_SET_TYPE =SetOfAverageSubTomograms
 
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self._coordsPointer = Pointer()
+
+    def copyInfo(self, other):
+        """ Copy properties from other set of images to current one"""
+        super().copyInfo(other)
+        if other._coordsPointer.hasValue():
+            self.copyAttributes(other, '_coordsPointer')
+        else:
+            logger.warning("The source %s seems an old execution and does not have coordinates associated."
+                           " This may set may fail with some protocols treating contained classes "
+                           "as SetOfSubtomograms with coordinates.")
+    def setCoordinates3D(self, coordinates):
+        """ Set the SetOfCoordinates associated with
+        this set.
+         """
+        if isinstance(coordinates, Pointer):
+            self._coordsPointer = coordinates
+        else:
+            self._coordsPointer.set(coordinates)
+
+    def _setItemMapperPath(self, item:ClassSubTomogram):
+        """ This will happen when retrieving any item from this set. We take this chance to 'inject' the coordinates."""
+        super()._setItemMapperPath(item)
+        item.setCoordinates3D(self._coordsPointer)
 
 class LandmarkModel(data.EMObject):
     """Represents the set of landmarks belonging to a specific tilt-series."""
 
     def __init__(self, tsId=None, fileName=None, modelName=None, size=5, applyTSTransformation=True, **kwargs):
         data.EMObject.__init__(self, **kwargs)
         self._tsId = String(tsId)
```

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/__init__.py` & `scipion-em-tomo-3.1.8/tomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_alignment_assign.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_assignTransformationTS.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_assignTransformationTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2subtomo.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2tomoMask.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_assign_tomo2tomoMask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_base.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_compose_TS.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_compose_TS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_consensus_classes_subtomo.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_consensus_classes_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ctf_validate.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ctf_validate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_extract_coordinates.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_fit_ellipsoid.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_fit_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates_from_scipion.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_coordinates_from_scipion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_subtomograms.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomograms.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomomasks.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_import_tomomasks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_misalignTS.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_misalignTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_particles_to_subtomograms.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_particles_to_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_rotate_astigmatism.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_rotate_astigmatism.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_split_evenodd_subtomos.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_split_evenodd_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_tomo_to_mics.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_tomo_to_mics.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_base.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_consensus_alignment.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_consensus_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_convert_coords3d.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_convert_coords3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_correct_motion.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_correct_motion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_estimate_ctf.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_estimate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_import.py` & `scipion-em-tomo-3.1.8/tomo/protocols/protocol_ts_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/protocols.conf` & `scipion-em-tomo-3.1.8/tomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/templates/HIV-Picking-with-Dynamo.json.template` & `scipion-em-tomo-3.1.8/tomo/templates/HIV-Picking-with-Dynamo.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/templates/HIV-Reconstruction.json.template` & `scipion-em-tomo-3.1.8/tomo/templates/HIV-Reconstruction.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/templates/HIV-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.8/tomo/templates/HIV-Subtomogram-averaging.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/templates/Membrane picking-with-PySeg.json.template` & `scipion-em-tomo-3.1.8/tomo/templates/Membrane picking-with-PySeg.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/templates/Ribosomes-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.8/tomo/templates/Ribosomes-Subtomogram-averaging.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/__init__.py` & `scipion-em-tomo-3.1.8/tomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/test_base_centralized_layer.py` & `scipion-em-tomo-3.1.8/tomo/tests/test_base_centralized_layer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/test_compose_TS.py` & `scipion-em-tomo-3.1.8/tomo/tests/test_compose_TS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/test_fit_vesicles.py` & `scipion-em-tomo-3.1.8/tomo/tests/test_fit_vesicles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/test_import.py` & `scipion-em-tomo-3.1.8/tomo/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/test_objects.py` & `scipion-em-tomo-3.1.8/tomo/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/test_tomo_base.py` & `scipion-em-tomo-3.1.8/tomo/tests/test_tomo_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/tests/test_transformations.py` & `scipion-em-tomo-3.1.8/tomo/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/utils.py` & `scipion-em-tomo-3.1.8/tomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/viewers/__init__.py` & `scipion-em-tomo-3.1.8/tomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/viewers/viewer_split_evenodd.py` & `scipion-em-tomo-3.1.8/tomo/viewers/viewer_split_evenodd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/viewers/viewers_data.py` & `scipion-em-tomo-3.1.8/tomo/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/viewers/views.py` & `scipion-em-tomo-3.1.8/tomo/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/viewers/views_tkinter_tree.py` & `scipion-em-tomo-3.1.8/tomo/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.7/tomo/wizards.py` & `scipion-em-tomo-3.1.8/tomo/wizards.py`

 * *Files identical despite different names*

