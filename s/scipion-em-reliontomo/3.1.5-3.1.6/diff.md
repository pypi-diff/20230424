# Comparing `tmp/scipion-em-reliontomo-3.1.5.tar.gz` & `tmp/scipion-em-reliontomo-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-reliontomo-3.1.5.tar", last modified: Fri Apr 21 08:17:52 2023, max compression
+gzip compressed data, was "scipion-em-reliontomo-3.1.6.tar", last modified: Mon Apr 24 13:54:51 2023, max compression
```

## Comparing `scipion-em-reliontomo-3.1.5.tar` & `scipion-em-reliontomo-3.1.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.372264 scipion-em-reliontomo-3.1.5/reliontomo/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.372264 scipion-em-reliontomo-3.1.5/reliontomo/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/cmd/compareStarFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.372264 scipion-em-reliontomo-3.1.5/reliontomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/convert30_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/convert40_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/convertBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/reliontomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_3d_classify_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_import_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_per_part_per_tilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_relion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_ctf_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_de_novo_initial_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_edit_particles_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_coordinates_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_subtomograms_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_make_pseudo_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_matching_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_tomogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_refine_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_tomo_frame_align.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/relion_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/reliontomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_compare_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_import_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_refine_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/cmd/compareStarFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/convert30_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/convert40_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/convertBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_3d_classify_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_import_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_per_part_per_tilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_relion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_ctf_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_de_novo_initial_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_edit_particles_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_coordinates_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_subtomograms_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_make_pseudo_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_matching_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_tomogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_refine_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_tomo_frame_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/relion_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/reliontomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_compare_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_import_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_refine_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/setup.py
```

### Comparing `scipion-em-reliontomo-3.1.5/LICENSE` & `scipion-em-reliontomo-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/PKG-INFO` & `scipion-em-reliontomo-3.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.5
+Version: 3.1.6
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.5/README.rst` & `scipion-em-reliontomo-3.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/__init__.py` & `scipion-em-reliontomo-3.1.6/reliontomo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import pwem
 import relion
 from reliontomo.constants import RELIONTOMO_HOME, RELIONTOMO_DEFAULT, RELION, RELIONTOMO_CUDA_LIB, V4_0
 
 _logo = "relion_logo.png"
 _references = ['Scheres2012a', 'Scheres2012b', 'Kimanius2016', 'Zivanov2018']
-__version__ = '3.1.5'
+__version__ = '3.1.6'
 
 
 class Plugin(relion.Plugin):
     _supportedVersions = [V4_0]
     _homeVar = RELIONTOMO_HOME
     _pathVars = [RELIONTOMO_HOME]
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/bibtex.py` & `scipion-em-reliontomo-3.1.6/reliontomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/cmd/compareStarFiles.py` & `scipion-em-reliontomo-3.1.6/reliontomo/cmd/compareStarFiles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/constants.py` & `scipion-em-reliontomo-3.1.6/reliontomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/convert/__init__.py` & `scipion-em-reliontomo-3.1.6/reliontomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/convert/convert30_tomo.py` & `scipion-em-reliontomo-3.1.6/reliontomo/convert/convert30_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/convert/convert40_tomo.py` & `scipion-em-reliontomo-3.1.6/reliontomo/convert/convert40_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/convert/convertBase.py` & `scipion-em-reliontomo-3.1.6/reliontomo/convert/convertBase.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/objects.py` & `scipion-em-reliontomo-3.1.6/reliontomo/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         represents it will be copied and, after that, this method will be used to update the corresponding
         attributes with the generated files."""
         for p in EnumRe4GenFilesProps:
             currentFile = join(extraPath, p.value)
             if exists(currentFile):
                 setattr(self, p.name, String(currentFile))
 
-    def getTomograms(self):
+    def getTomogramsStar(self):
         return self._tomograms.get()
 
     def getParticles(self):
         return self._particles.get()
 
     def getTrajectories(self):
         return self._trajectories.get()
@@ -262,15 +262,17 @@
 
     def copyInfo(self, other):
         self.copyAttributes(other,'_filesMaster', '_tomograms', '_particles', '_trajectories', '_manifolds', '_referenceFsc',
                             '_relionBinning', '_tsSamplingRate', '_samplingRate', '_boxSize', '_nReParticles',
                             '_coordsPointer')
         self._acquisition.copyInfo(other._acquisition)
         # self._relionMd = relionMd if relionMd else relionTomoMetadata
-
+    def _samplingRateStr(self):
+        return "%0.2f Å/px" % self.getCurrentSamplingRate()
+        
     # def iterPSubtomos(self, ts=None, orderBy='id'):
     #     if ts is None:
     #         tsId = None
     #     elif isinstance(ts, str):
     #         tsId = ts
     #     elif isinstance(ts, TiltSeries):
     #         tsId = ts.getTsId()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/__init__.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_3d_classify_subtomograms.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_3d_classify_subtomograms.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from reliontomo.constants import OUT_PARTICLES_STAR
 from reliontomo.objects import RelionSetOfPseudoSubtomograms
 from reliontomo.protocols import ProtRelionRefineSubtomograms
 from reliontomo.protocols.protocol_base_refine import ProtRelionRefineBase
 from reliontomo import Plugin
 from pyworkflow.protocol import FloatParam, BooleanParam, GE, LE, IntParam, StringParam
 from reliontomo.utils import getProgram
-from tomo.objects import SetOfClassesSubTomograms, SetOfAverageSubTomograms
+from tomo.objects import SetOfClassesSubTomograms, SetOfSubTomograms
 
 
 class outputObjects(Enum):
     relionParticles = RelionSetOfPseudoSubtomograms
     classes = SetOfClassesSubTomograms
 
 
@@ -176,22 +176,23 @@
         # Output RelionParticles
         relionParticles = self.genRelionParticles()
 
         # Output classes
         classes3D = self._createSetOfClassesSubTomograms(relionParticles)
         classes3D.setImages(relionParticles)
         self._fillClassesFromIter(classes3D, self.nIterations.get())
-        averages = SetOfAverageSubTomograms.create(self._getPath(),
-                                                   template='avgPSubtomograms%s.sqlite',
-                                                   suffix='')
-        averages.setSamplingRate(relionParticles.getCurrentSamplingRate())
-        for class3D in classes3D:
-            vol = class3D.getRepresentative()
-            vol.setObjId(class3D.getObjId())
-            averages.append(vol)
+
+        # averages = SetOfAverageSubTomograms.create(self._getPath(),
+        #                                            template='avgPSubtomograms%s.sqlite',
+        #                                            suffix='')
+        # averages.setSamplingRate(relionParticles.getCurrentSamplingRate())
+        # for class3D in classes3D:
+        #     vol = class3D.getRepresentative()
+        #     vol.setObjId(class3D.getObjId())
+        #     averages.append(vol)
 
         outputDict = {outputObjects.relionParticles.name: relionParticles,
                       outputObjects.classes.name: classes3D}
         self._defineOutputs(**outputDict)
         self._defineSourceRelation(inParticles, relionParticles)
         self._defineSourceRelation(inParticles, classes3D)
 
@@ -258,19 +259,20 @@
         cmd += '--pad %i ' % (1 if self.skipPadding.get() else 2)
 
         # Additional args
         cmd += self._genAddiotionalBaseCmd()
 
         return cmd
 
-    def _createSetOfClassesSubTomograms(self, subTomograms, suffix=''):
+    def _createSetOfClassesSubTomograms(self, subTomograms:SetOfSubTomograms, suffix=''):
         classes = SetOfClassesSubTomograms.create(self._getPath(),
                                                   template='subtomogramClasses%s.sqlite',
                                                   suffix=suffix)
         classes.setImages(subTomograms)
+        classes.setCoordinates3D(subTomograms.getCoordinates3D(asPointer=True))
         return classes
 
     def _fillClassesFromIter(self, clsSet, iteration):
         """ Create the SetOfClasses3D from a given iteration. """
         self._loadClassifyInfo(iteration)
         clsSet.classifyItems(updateItemCallback=self._updateParticle,
                              updateClassCallback=self._updateClass,
@@ -302,17 +304,24 @@
         item._rlnLogLikeliContribution = Float(row.rlnLogLikeliContribution)
         item._rlnMaxValueProbDistribution = Float(row.rlnMaxValueProbDistribution)
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesInfo:
             _, row = self._classesInfo[classId]
-            fn = row.rlnReferenceImage + ":mrc"
+            fn = row.rlnReferenceImage
             item.setAlignment3D()
-            item.getRepresentative().setLocation(fn)
+
+            # Representative stuff
+            representative =item.getRepresentative()
+            representative.setLocation(fn)
+            representative.setSamplingRate(self.inReParticles.get().getCurrentSamplingRate())
+            # relion mrc are technically stacks. Fix this
+            representative.fixMRCVolume()
+
             item._rlnclassDistribution = Float(row.rlnClassDistribution)
             item._rlnAccuracyRotations = Float(row.rlnAccuracyRotations)
             item._rlnAccuracyTranslations = Float(row.rlnAccuracyTranslationsAngst)
 
     def _cleanUndesiredFiles(self):
         """Remove all files generated by relion_classify 3d excepting the ones which
         correspond to the last iteration. Example for iteration 25:
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_import_from_star.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_import_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def createOutputStep(self):
         return self.genRelionParticles(binningFactor=self.binningFactor.get(), boxSize=self.croppedBoxSize.get())
 
     # -------------------------- INFO functions -------------------------------
 
     # --------------------------- UTILS functions -----------------------------
     def _genCommonCmd(self):
-        inRelionParticles = self.inReParticles.get()
+        inRelionParticles = self.getInputParticles()
         cmd = ''
 
         # Cancel this for now
         self.info("Using optimization_set: %s" % inRelionParticles.filesMaster)
         cmd += '--i %s ' % inRelionParticles.filesMaster
 
         # This would be either the particles start file in the set or a new generated one from the subtomo set.
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_per_part_per_tilt.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_per_part_per_tilt.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     # -------------------------- UTILS functions -----------------------------
     def _genIOCommand(self):
         inPSubtomos = self.inReParticles.get()
         trajectories = inPSubtomos.getTrajectories()
         postProcess = inPSubtomos.getReferenceFsc()
         half1, half2 = self.recVolume.get().getHalfMaps().split(',')
         cmd = '--p %s ' % inPSubtomos.getParticles()
-        cmd += '--t %s ' % inPSubtomos.getTomograms()
+        cmd += '--t %s ' % inPSubtomos.getTomogramsStar()
         cmd += '--o %s ' % self._getExtraPath()
         if trajectories:
             cmd += '--mot %s ' % trajectories
         cmd += '--ref1 %s ' % half1
         cmd += '--ref2 %s ' % half2
         cmd += '--mask %s ' % self.inRefMask.get().getFileName()
         if postProcess:
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_refine.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,22 @@
         cmd += self._genCTFBaseCmd()  # CTF args
         cmd += self._genOptimisationBaseCmd()  # Optimisation args
         cmd += self._genComputeBaseCmd()  # Compute args
         cmd += self._genAddiotionalBaseCmd()  # Additional args
         return cmd
 
     def _genIOBaseCmd(self):
-        cmd = '--i %s ' % self.getOutStarFileName()
+
+        inRelionParticles = self.getInputParticles()
+
+        # Use optimization set file
+        self.info("Using optimization_set: %s" % inRelionParticles.filesMaster)
+        cmd = '--ios %s ' % inRelionParticles.filesMaster
+
+        cmd += '--i %s ' % self.getOutStarFileName()
         cmd += '--o %s ' % (self._getExtraPath() + '/')  # If not, Relion will concatenate it directly as a prefix
         cmd += '--j %i ' % self.numberOfThreads
         return cmd
 
     def _genCTFBaseCmd(self):
         cmd = ''
         if self.doCTF.get():
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_relion.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_relion.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
     def _defineCommonInputParams(self, form):
         form.addSection(label=Message.LABEL_INPUT)
         form.addParam('inReParticles', PointerParam,
                       pointerClass='RelionSetOfPseudoSubtomograms',
                       label='Relion particles')
 
+    def getInputParticles(self):
+        return self.inReParticles.get()
+
     def getOutStarFileName(self):
         return self._getExtraPath(IN_PARTICLES_STAR)
 
     def genInStarFile(self, withPriors=False):
         """It will check if the set size and the stored particles star file are of the same size or not. In
         the first case, a link will be made to the previous particles star file to avoid generating it and in the
         second case, a new file will be generated containing only the ones present in the input set."""
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_ctf_refine.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_ctf_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_de_novo_initial_model.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_de_novo_initial_model.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_edit_particles_star.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_edit_particles_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_coordinates_from_star.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_coordinates_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_subtomograms_from_star.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_subtomograms_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_make_pseudo_subtomos.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_make_pseudo_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_matching_coordinates.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_matching_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_post_process.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_post_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     relionParticles = RelionSetOfPseudoSubtomograms
     postProcessVolume = VolumeMask
 
 
 class ProtRelionPostProcess(ProtRelionTomoBase):
     """Sharpen a 3D reference map and estimate the gold-standard FSC curves for subtomogram averaging"""
 
-    _label = 'Sharpen a 3D reference maps'
+    _label = 'postprocessing'
     _devStatus = BETA
     _possibleOutputs = outputObjects
 
     def __init__(self, **kargs):
         super().__init__(**kargs)
 
     # -------------------------- DEFINE param functions -----------------------
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_prepare_data.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_prepare_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_tomogram.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_tomogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             if self.recTomoMode.get() == SINGLE_TOMO:
                 summary.append('The selected tomogram was *%s*.' % self.tomoId.get())
         return summary
 
     # --------------------------- UTILS functions -----------------------------
 
     def _genTomoRecCommand(self, tomoId):
-        cmd = '--t %s ' % self.inReParticles.getTomograms()
+        cmd = '--t %s ' % self.inReParticles.getTomogramsStar()
         cmd += '--tn %s ' % tomoId
         cmd += '--o %s ' % self._getOutTomoFileName(tomoId)
         cmd += '--bin %.1f ' % self.binFactor.get()
         cmd += '--w %i ' % self.width.get()
         cmd += '--h %i ' % self.height.get()
         cmd += '--d %i ' % self.thickness.get()
         cmd += '--j %i ' % self.numberOfThreads.get()
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,14 @@
         if self.snrWiener.get() > 0:
             cmd += '--SNR %.2f ' % self.snrWiener.get()
         return cmd
 
     def _genTomoMaskRefCmd(self):
         inParticles = self.inReParticles.get()
         cmd = ''
-        cmd += '--t %s ' % inParticles.getTomograms()
+        cmd += '--t %s ' % inParticles.getTomogramsStar()
         cmd += '--p %s ' % self.getOutStarFileName()
         cmd += '--rec %s ' % self._getExtraPath()
         cmd += '--o %s ' % self._getExtraPath()
         cmd += '--mask %s ' % self.solventMask.get().getFileName()
         cmd += '--angpix %.2f ' % (inParticles.getTsSamplingRate() * self.binningFactor.get())
         return cmd
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_refine_subtomograms.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_refine_subtomograms.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         nMpi = self.numberOfMpi.get()
         Plugin.runRelionTomo(self, getProgram('relion_refine', nMpi), self._genAutoRefineCommand(), numberOfMpi=nMpi)
 
     def createOutputStep(self):
         inParticles = self.inReParticles.get()
 
         # Output Relion particles
-        relionParticles = self.genRelionParticles(optimisationFileName='run_optimization_set.star',
+        relionParticles = self.genRelionParticles(optimisationFileName='_optimisation_set.star',
                                                   particles='_data.star')
 
         # Output volume
         vol = AverageSubTomogram()
         volName = self._getExtraPath('_class001.mrc')
         fixVolume(volName)  # Fix header for xmipp to consider it a volume instead of a stack
         vol.setFileName(volName)
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_tomo_frame_align.py` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_tomo_frame_align.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/protocols.conf` & `scipion-em-reliontomo-3.1.6/reliontomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/relion_logo.png` & `scipion-em-reliontomo-3.1.6/reliontomo/relion_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/tests/__init__.py` & `scipion-em-reliontomo-3.1.6/reliontomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_compare_star_files.py` & `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_compare_star_files.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_conversion.py` & `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_import_star_files.py` & `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_import_star_files.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_refine_cycle.py` & `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_refine_cycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
         cls.launchProtocol(protRecPartFromTS)
         return protRecPartFromTS
 
     def _checkRe4Metadata(self, pSubtomoSet, tomogramsFile=None, particlesFile=None, trajectoriesFile=None,
                           manifoldsFile=None, referenceFscFile=None, relionBinning=None):
         self.assertEqual(self.nParticles, pSubtomoSet.getNReParticles())
         self.assertEqual(self.samplingRateOrig, pSubtomoSet.getTsSamplingRate())
-        self.assertEqual(tomogramsFile, pSubtomoSet.getTomograms())
+        self.assertEqual(tomogramsFile, pSubtomoSet.getTomogramsStar())
         self.assertEqual(particlesFile, pSubtomoSet.getParticles())
         self.assertEqual(trajectoriesFile, pSubtomoSet.getTrajectories())
         self.assertEqual(manifoldsFile, pSubtomoSet.getManifolds())
         self.assertEqual(referenceFscFile, pSubtomoSet.getReferenceFsc())
         self.assertEqual(relionBinning, pSubtomoSet.getRelionBinning())
         self.assertEqual(self.samplingRateOrig * relionBinning, pSubtomoSet.getCurrentSamplingRate())
```

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/utils.py` & `scipion-em-reliontomo-3.1.6/reliontomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/reliontomo/wizards.py` & `scipion-em-reliontomo-3.1.6/reliontomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/PKG-INFO` & `scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.5
+Version: 3.1.6
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/SOURCES.txt` & `scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.5/setup.py` & `scipion-em-reliontomo-3.1.6/setup.py`

 * *Files identical despite different names*

