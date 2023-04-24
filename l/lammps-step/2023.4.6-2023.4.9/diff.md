# Comparing `tmp/lammps_step-2023.4.6.tar.gz` & `tmp/lammps_step-2023.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammps_step-2023.4.6.tar", last modified: Tue Mar  7 03:50:21 2023, max compression
+gzip compressed data, was "lammps_step-2023.4.9.tar", last modified: Thu Mar  9 15:50:18 2023, max compression
```

## Comparing `lammps_step-2023.4.6.tar` & `lammps_step-2023.4.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.788042 lammps_step-2023.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.792043 lammps_step-2023.4.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.792043 lammps_step-2023.4.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.792043 lammps_step-2023.4.6/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.796043 lammps_step-2023.4.6/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/density.png
--rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/edit_forcefield.png
--rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/edit_initialization.png
--rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/edit_npt.png
--rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/edit_packmol.png
--rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/lammps_flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/getting_started/nist.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.796043 lammps_step-2023.4.6/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/lammps_step/
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/lammps_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/custom_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/lammps_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/data/seamm-lammps.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21595 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/initialization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/initialization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    80548 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/minimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/npt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/npt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/npt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/nve_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/nve_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/nvt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/nvt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    30803 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_npt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/tk_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/velocities_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/lammps_step/velocities_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/lammps_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-03-07 03:50:21.000000 lammps_step-2023.4.6/lammps_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-07 03:50:21.000000 lammps_step-2023.4.6/lammps_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 03:50:21.000000 lammps_step-2023.4.6/lammps_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-07 03:50:21.000000 lammps_step-2023.4.6/lammps_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-07 03:50:21.000000 lammps_step-2023.4.6/lammps_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-07 03:50:21.000000 lammps_step-2023.4.6/lammps_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 03:50:06.000000 lammps_step-2023.4.6/lammps_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:50:21.804042 lammps_step-2023.4.6/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/tests/data/Ar_xtal_energy.flow
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/tests/test_lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/tests/test_lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-07 03:50:05.000000 lammps_step-2023.4.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.378035 lammps_step-2023.4.9/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.386036 lammps_step-2023.4.9/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/density.png
+-rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_forcefield.png
+-rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_initialization.png
+-rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_npt.png
+-rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/edit_packmol.png
+-rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/lammps_flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/getting_started/nist.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.386036 lammps_step-2023.4.9/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/custom_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/data/seamm-lammps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21595 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/initialization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/initialization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81558 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/minimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/npt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/npt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nve_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nve_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nvt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/nvt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30803 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/tk_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/velocities_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/lammps_step/velocities_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/lammps_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 15:50:18.000000 lammps_step-2023.4.9/lammps_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:50:05.000000 lammps_step-2023.4.9/lammps_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:50:18.394036 lammps_step-2023.4.9/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/data/Ar_xtal_energy.flow
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/test_lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/tests/test_lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-09 15:50:02.000000 lammps_step-2023.4.9/versioneer.py
```

### Comparing `lammps_step-2023.4.6/CONTRIBUTING.rst` & `lammps_step-2023.4.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/HISTORY.rst` & `lammps_step-2023.4.9/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 =======
 History
 =======
+2023.4.9 -- Hid the warning from pymbar
+   * Importing pymbar timeseries writes a warning to the terminal about its proper
+     usage. SEAMM already handles the warned case, so the message is simply confusing to
+     users and hence this release hides it.
+     
 2023.4.6 -- Better forcefield handling.
    * Added correct molecule numbers for valence forcefields.
    * Correctly handle ReaxFF from OpenKim
    * Updated for some minor changes in OpenKim
 
 2023.2.6 -- Added handling of OPLS-AA forcefield
    * Added handling of the OPLS-AA forcefield
```

### Comparing `lammps_step-2023.4.6/LICENSE` & `lammps_step-2023.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/PKG-INFO` & `lammps_step-2023.4.9/lammps_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lammps_step
-Version: 2023.4.6
+Name: lammps-step
+Version: 2023.4.9
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,19 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.4.9 -- Hid the warning from pymbar
+   * Importing pymbar timeseries writes a warning to the terminal about its proper
+     usage. SEAMM already handles the warned case, so the message is simply confusing to
+     users and hence this release hides it.
+     
 2023.4.6 -- Better forcefield handling.
    * Added correct molecule numbers for valence forcefields.
    * Correctly handle ReaxFF from OpenKim
    * Updated for some minor changes in OpenKim
 
 2023.2.6 -- Added handling of OPLS-AA forcefield
    * Added handling of the OPLS-AA forcefield
```

### Comparing `lammps_step-2023.4.6/README.rst` & `lammps_step-2023.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/Makefile` & `lammps_step-2023.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/_static/SEAMM inverted.png` & `lammps_step-2023.4.9/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/_static/SEAMM logo.png` & `lammps_step-2023.4.9/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/_static/molssi_main_logo.png` & `lammps_step-2023.4.9/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/_static/molssi_main_logo_inverted_white.png` & `lammps_step-2023.4.9/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/_static/molssi_square.png` & `lammps_step-2023.4.9/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/_static/nsf.png` & `lammps_step-2023.4.9/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/conf.py` & `lammps_step-2023.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/developer_guide/installation.rst` & `lammps_step-2023.4.9/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/density.png` & `lammps_step-2023.4.9/docs/getting_started/density.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/edit_forcefield.png` & `lammps_step-2023.4.9/docs/getting_started/edit_forcefield.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/edit_initialization.png` & `lammps_step-2023.4.9/docs/getting_started/edit_initialization.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/edit_npt.png` & `lammps_step-2023.4.9/docs/getting_started/edit_npt.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/edit_packmol.png` & `lammps_step-2023.4.9/docs/getting_started/edit_packmol.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/flowchart.png` & `lammps_step-2023.4.9/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/index.rst` & `lammps_step-2023.4.9/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/lammps_flowchart.png` & `lammps_step-2023.4.9/docs/getting_started/lammps_flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/getting_started/nist.png` & `lammps_step-2023.4.9/docs/getting_started/nist.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/index.rst` & `lammps_step-2023.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/docs/make.bat` & `lammps_step-2023.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/__init__.py` & `lammps_step-2023.4.9/lammps_step/__init__.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/custom.py` & `lammps_step-2023.4.9/lammps_step/custom.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/custom_parameters.py` & `lammps_step-2023.4.9/lammps_step/custom_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/custom_step.py` & `lammps_step-2023.4.9/lammps_step/custom_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/data/configuration.txt` & `lammps_step-2023.4.9/lammps_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/data/properties.csv` & `lammps_step-2023.4.9/lammps_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/data/references.bib` & `lammps_step-2023.4.9/lammps_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/energy.py` & `lammps_step-2023.4.9/lammps_step/energy.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/energy_parameters.py` & `lammps_step-2023.4.9/lammps_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/energy_step.py` & `lammps_step-2023.4.9/lammps_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/initialization.py` & `lammps_step-2023.4.9/lammps_step/initialization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/initialization_parameters.py` & `lammps_step-2023.4.9/lammps_step/initialization_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/initialization_step.py` & `lammps_step-2023.4.9/lammps_step/initialization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/installer.py` & `lammps_step-2023.4.9/lammps_step/installer.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/lammps.py` & `lammps_step-2023.4.9/lammps_step/lammps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 """A node or step for LAMMPS in a flowchart"""
 
+from contextlib import contextmanager
 import copy
 import glob
 import logging
 from math import sqrt, exp, degrees, radians, cos, acos
 from pathlib import Path
 import os
 import os.path
@@ -27,20 +28,52 @@
 import lammps_step
 import molsystem
 import seamm
 import seamm_util
 import seamm_util.printing as printing
 from seamm_util.printing import FormattedText as __
 
-from pymbar import timeseries
+# from pymbar import timeseries
 
 logger = logging.getLogger("lammps")
 job = printing.getPrinter()
 printer = printing.getPrinter("lammps")
 
+
+# Temporarily used here to stop pymbar's annoying warning.
+@contextmanager
+def logging_disabled(highest_level=logging.CRITICAL):
+    """
+    A context manager that will prevent any logging messages
+    triggered during the body from being processed.
+
+    :param highest_level: the maximum logging level in use.
+      This would only need to be changed if a custom level greater than CRITICAL
+      is defined.
+
+    From Simon Weber https://gist.github.com/simon-weber/7853144
+    """
+    # two kind-of hacks here:
+    #    * can't get the highest logging level in effect => delegate to the user
+    #    * can't get the current module-level override => use an undocumented
+    #       (but non-private!) interface
+
+    previous_level = logging.root.manager.disable
+
+    logging.disable(highest_level)
+
+    try:
+        yield
+    finally:
+        logging.disable(previous_level)
+
+
+with logging_disabled(highest_level=logging.WARNING):
+    from pymbar import timeseries
+
 # Add LAMMPS's properties to the standard properties
 path = Path(pkg_resources.resource_filename(__name__, "data/"))
 csv_file = path / "properties.csv"
 molsystem.add_properties_from_file(csv_file)
 
 bond_style = {
     "quadratic_bond": "harmonic",
```

### Comparing `lammps_step-2023.4.6/lammps_step/lammps_step.py` & `lammps_step-2023.4.9/lammps_step/lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/lammps_units.py` & `lammps_step-2023.4.9/lammps_step/lammps_units.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/metadata.py` & `lammps_step-2023.4.9/lammps_step/metadata.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/minimization.py` & `lammps_step-2023.4.9/lammps_step/minimization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/minimization_step.py` & `lammps_step-2023.4.9/lammps_step/minimization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/npt.py` & `lammps_step-2023.4.9/lammps_step/npt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/npt_parameters.py` & `lammps_step-2023.4.9/lammps_step/npt_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/npt_step.py` & `lammps_step-2023.4.9/lammps_step/npt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/nve.py` & `lammps_step-2023.4.9/lammps_step/nve.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/nve_parameters.py` & `lammps_step-2023.4.9/lammps_step/nve_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/nve_step.py` & `lammps_step-2023.4.9/lammps_step/nve_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/nvt.py` & `lammps_step-2023.4.9/lammps_step/nvt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/nvt_parameters.py` & `lammps_step-2023.4.9/lammps_step/nvt_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/nvt_step.py` & `lammps_step-2023.4.9/lammps_step/nvt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_custom.py` & `lammps_step-2023.4.9/lammps_step/tk_custom.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_energy.py` & `lammps_step-2023.4.9/lammps_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_initialization.py` & `lammps_step-2023.4.9/lammps_step/tk_initialization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_lammps.py` & `lammps_step-2023.4.9/lammps_step/tk_lammps.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_minimization.py` & `lammps_step-2023.4.9/lammps_step/tk_minimization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_npt.py` & `lammps_step-2023.4.9/lammps_step/tk_npt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_nve.py` & `lammps_step-2023.4.9/lammps_step/tk_nve.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_nvt.py` & `lammps_step-2023.4.9/lammps_step/tk_nvt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/tk_velocities.py` & `lammps_step-2023.4.9/lammps_step/tk_velocities.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/velocities.py` & `lammps_step-2023.4.9/lammps_step/velocities.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/velocities_parameters.py` & `lammps_step-2023.4.9/lammps_step/velocities_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step/velocities_step.py` & `lammps_step-2023.4.9/lammps_step/velocities_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step.egg-info/PKG-INFO` & `lammps_step-2023.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lammps-step
-Version: 2023.4.6
+Name: lammps_step
+Version: 2023.4.9
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,19 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.4.9 -- Hid the warning from pymbar
+   * Importing pymbar timeseries writes a warning to the terminal about its proper
+     usage. SEAMM already handles the warned case, so the message is simply confusing to
+     users and hence this release hides it.
+     
 2023.4.6 -- Better forcefield handling.
    * Added correct molecule numbers for valence forcefields.
    * Correctly handle ReaxFF from OpenKim
    * Updated for some minor changes in OpenKim
 
 2023.2.6 -- Added handling of OPLS-AA forcefield
    * Added handling of the OPLS-AA forcefield
```

### Comparing `lammps_step-2023.4.6/lammps_step.egg-info/SOURCES.txt` & `lammps_step-2023.4.9/lammps_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/lammps_step.egg-info/entry_points.txt` & `lammps_step-2023.4.9/lammps_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/setup.py` & `lammps_step-2023.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/tests/data/Ar_xtal_energy.flow` & `lammps_step-2023.4.9/tests/data/Ar_xtal_energy.flow`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/tests/test_lammps_step.py` & `lammps_step-2023.4.9/tests/test_lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/tests/test_lammps_units.py` & `lammps_step-2023.4.9/tests/test_lammps_units.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.4.6/versioneer.py` & `lammps_step-2023.4.9/versioneer.py`

 * *Files identical despite different names*

