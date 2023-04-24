# Comparing `tmp/fmu_tools-1.8.1.tar.gz` & `tmp/fmu_tools-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fmu_tools-1.8.1.tar", last modified: Tue Oct 12 12:08:10 2021, max compression
+gzip compressed data, was "dist/fmu_tools-1.9.0.tar", last modified: Wed Oct 27 16:43:47 2021, max compression
```

## Comparing `fmu_tools-1.8.1.tar` & `fmu_tools-1.9.0.tar`

### file list

```diff
@@ -1,208 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     4298 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      896 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/docs/fmu_logo/
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/fmu_logo/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    32715 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/fmu_logo/fmu_logo_with_text.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5990 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/fmu_logo/fmu_logo_coviz.svg
--rwxr-xr-x   0 runner    (1001) docker     (121)     4102 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/fmu_logo/fmu_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/create_rft_ertobs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/docs/images/
--rwxr-xr-x   0 runner    (1001) docker     (121)    69206 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput_singlereference.png
--rwxr-xr-x   0 runner    (1001) docker     (121)     6052 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_depend1.png
--rwxr-xr-x   0 runner    (1001) docker     (121)   191613 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_example1.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    17911 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_corr1.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    85413 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput_dependencies.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    99679 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_fullmc_corr.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    69368 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput_singlereference_and_seed.png
--rwxr-xr-x   0 runner    (1001) docker     (121)   211268 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput.png
--rwxr-xr-x   0 runner    (1001) docker     (121)   185422 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput1.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    82564 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_defaultvalues.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    39464 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_general_input.png
--rwxr-xr-x   0 runner    (1001) docker     (121)   304297 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput2.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    57803 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_backgroundvalues.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    64797 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput_example_velocities.png
--rwxr-xr-x   0 runner    (1001) docker     (121)    10214 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_background_geninput.png
--rwxr-xr-x   0 runner    (1001) docker     (121)   172669 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/images/design_designinput_background_noseed.png
--rw-r--r--   0 runner    (1001) docker     (121)     7240 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/qcreset.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8060 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/_static/equinor_logo_only.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     8688 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/_static/equinor-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    19937 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/_static/equinor-logo2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    25380 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/_static/equinor_logo.jpg
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      827 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/rmsvolumetrics2csv.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/qcforward.rst
--rw-r--r--   0 runner    (1001) docker     (121)    23018 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/qcproperties.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     9325 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/docs/qcforward/
--rw-r--r--   0 runner    (1001) docker     (121)     5018 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/qcforward/gridquality.inc
--rw-r--r--   0 runner    (1001) docker     (121)     7353 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/qcforward/grid_statistics.inc
--rw-r--r--   0 runner    (1001) docker     (121)     8266 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/qcforward/wellzon_vs_grid.inc
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21934 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/docs/fmudesign.rst
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3500 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/.github/workflows/fmu-tools.yml
--rw-r--r--   0 runner    (1001) docker     (121)      837 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/.github/workflows/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-12 12:06:29.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     6598 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu_tools.egg-info/entry_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/fipmapper/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/fipmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22656 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/fipmapper/fipmapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/qcproperties/
--rw-r--r--   0 runner    (1001) docker     (121)     7116 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcproperties/_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcproperties/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7058 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcproperties/_aggregate_df.py
--rw-r--r--   0 runner    (1001) docker     (121)     5806 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcproperties/_grid2df.py
--rw-r--r--   0 runner    (1001) docker     (121)     8406 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcproperties/qcproperties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6950 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcproperties/_well2df.py
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/extract_grid_zone_tops.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/qcdata/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11906 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcdata/qcdata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/rms/
--rw-r--r--   0 runner    (1001) docker     (121)     7881 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/rms/volumetrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    22703 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/rms/create_rft_ertobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/rms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16524 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/rms/qcreset.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/_common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/
--rw-r--r--   0 runner    (1001) docker     (121)     9143 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_wellzonation_vs_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     6628 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_grid_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5923 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_qcforward.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asroxapi.json
--rw-r--r--   0 runner    (1001) docker     (121)      938 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/gridquality_asfile.json
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asfile.json
--rw-r--r--   0 runner    (1001) docker     (121)      943 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/gridquality_asroxapi.json
--rw-r--r--   0 runner    (1001) docker     (121)     6938 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/_grid_quality.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/qcforward/qcforward.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/
--rw-r--r--   0 runner    (1001) docker     (121)    37287 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/create_design.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10837 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/_tornado_onebyone.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      687 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21846 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/design_distributions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5323 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/_designsummary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/fmudesignrunner.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7911 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/_add_webviz_tornado_onebyone.py
--rw-r--r--   0 runner    (1001) docker     (121)    25556 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/tools/sensitivities/_excel2dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/src/fmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/fipmapper/
--rw-r--r--   0 runner    (1001) docker     (121)     7557 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/fipmapper/test_fipmapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    12447 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/fipmapper/test_disjointsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/test_qcdata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/qcproperties/
--rw-r--r--   0 runner    (1001) docker     (121)    13849 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/qcproperties/test_qcproperties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/qcproperties/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/qcproperties/data/propstat.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/qcproperties/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/test_extract_zone_tops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/rms/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/rms_eclipse.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A6_1.obs
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A4.txt
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/layer_zone_table.csv
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A2_1.obs
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A5_1.obs
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A5.txt
--rw-r--r--   0 runner    (1001) docker     (121)      508 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/rft_input_table_4modelcase.csv
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A4_1.obs
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A3_1.obs
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/well_date_rft.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A6.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/R_A3.txt
--rw-r--r--   0 runner    (1001) docker     (121)      341 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/expected_files/layer_zone_table.txt
--rw-r--r--   0 runner    (1001) docker     (121)      469 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/input_table_drogon.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/
--rw-r--r--   0 runner    (1001) docker     (121)   197525 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A2.csv
--rw-r--r--   0 runner    (1001) docker     (121)  1130760 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A4.csv
--rw-r--r--   0 runner    (1001) docker     (121)   202390 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A3.csv
--rw-r--r--   0 runner    (1001) docker     (121)   202390 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A5.csv
--rw-r--r--   0 runner    (1001) docker     (121)   202390 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A6.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/rms/volumetricsdata/
--rwxr-xr-x   0 runner    (1001) docker     (121)    40726 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/volumetricsdata/14_geo_gas_1.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1714 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/volumetricsdata/2_simgrid_vol_oil_1.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1644 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/volumetricsdata/1_geogrid_vol_oil_1.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     8600 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/test_rmsvolumetrics.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24011 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/test_create_rft_ertobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/rms/test_qcreset_in_roxenv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/data/zone_tops_from_grid/
--rw-r--r--   0 runner    (1001) docker     (121)   368221 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/data/zone_tops_from_grid/OP_1.w
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/qcforward/
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/qcforward/test_gridquality.py
--rw-r--r--   0 runner    (1001) docker     (121)     8880 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/qcforward/test_qcforward_in_roxenv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/qcforward/test_wellzonation_vs_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     6896 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/qcforward/test_grid_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/sensitivities/
--rw-r--r--   0 runner    (1001) docker     (121)     8312 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/test_design_distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/sensitivities/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/sensitivities/data/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)     5994 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/distributions/design.csv
--rwxr-xr-x   0 runner    (1001) docker     (121)    14391 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/distributions/design.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/distributions/designsummary.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/sensitivities/data/results/
--rwxr-xr-x   0 runner    (1001) docker     (121)   508763 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/results/geovolumes_collected.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/
--rw-r--r--   0 runner    (1001) docker     (121)     5208 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/seeds.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    14950 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_singlereference_and_seed.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (121)    29827 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_background.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    29812 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_background_extseeds.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    16773 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_example1.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    22195 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_onebyone.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)     4985 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/doe1.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)      500 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/seeds.csv
--rw-r--r--   0 runner    (1001) docker     (121)    21878 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_singlereference.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (121)    24954 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_example2.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (121)    33233 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_mc_with_correls.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    21647 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_example_velocities.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)     4723 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/correlations.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    29815 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_background_no_seed.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    21883 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_default_no_seed.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/data/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/test_use_cases.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2481 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/test_create_design.py
--rw-r--r--   0 runner    (1001) docker     (121)     8362 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/test_excel2dict.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2603 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/test_calc_tornado.py
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/tests/sensitivities/test_designmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 12:08:10.000000 fmu_tools-1.8.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1206 2021-10-12 12:05:57.000000 fmu_tools-1.8.1/examples/example_create_design.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     4298 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/docs/fmu_logo/
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/fmu_logo/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    32715 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/fmu_logo/fmu_logo_with_text.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5990 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/fmu_logo/fmu_logo_coviz.svg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4102 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/fmu_logo/fmu_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4597 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/create_rft_ertobs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/docs/images/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    69206 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput_singlereference.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6052 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_depend1.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)   191613 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_example1.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    17911 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_corr1.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    85413 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput_dependencies.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    99679 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_fullmc_corr.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    69368 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput_singlereference_and_seed.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)   211268 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)   185422 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput1.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    82564 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_defaultvalues.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    39464 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_general_input.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)   304297 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput2.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    57803 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_backgroundvalues.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    64797 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput_example_velocities.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10214 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_background_geninput.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)   172669 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/images/design_designinput_background_noseed.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7240 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/qcreset.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     8060 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/_static/equinor_logo_only.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/_static/equinor-logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    19937 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/_static/equinor-logo2.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    25380 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/_static/equinor_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/rmsvolumetrics2csv.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/qcforward.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    23018 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/qcproperties.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9325 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/docs/qcforward/
+-rw-r--r--   0 runner    (1001) docker     (121)     7068 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/qcforward/bw_vs_gridprops.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     5018 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/qcforward/gridquality.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     7353 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/qcforward/grid_statistics.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     8266 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/qcforward/wellzon_vs_grid.inc
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21934 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/docs/fmudesign.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3500 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/.github/workflows/fmu-tools.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/.github/workflows/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 16:42:10.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     6851 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu_tools.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/fipmapper/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/fipmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22656 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/fipmapper/fipmapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/qcproperties/
+-rw-r--r--   0 runner    (1001) docker     (121)     7116 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcproperties/_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcproperties/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7058 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcproperties/_aggregate_df.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5806 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcproperties/_grid2df.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8406 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcproperties/qcproperties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6950 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcproperties/_well2df.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4884 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/extract_grid_zone_tops.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/qcdata/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11868 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcdata/qcdata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/rms/
+-rw-r--r--   0 runner    (1001) docker     (121)     7881 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/rms/volumetrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22703 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/rms/create_rft_ertobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/rms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16524 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/rms/qcreset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/_common.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/
+-rw-r--r--   0 runner    (1001) docker     (121)     9141 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_wellzonation_vs_grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13141 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_blockedwells_vs_gridprops.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6628 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_grid_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8470 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_qcforward.py
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)     1294 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asroxapi.json
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/gridquality_asfile.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/bw_vs_gridprops_asfile.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asfile.json
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/gridquality_asroxapi.json
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/bw_vs_gridprops_asroxapi.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6938 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/_grid_quality.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/qcforward/qcforward.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/
+-rw-r--r--   0 runner    (1001) docker     (121)    37287 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/create_design.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10837 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/_tornado_onebyone.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      687 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21846 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/design_distributions.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5323 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/_designsummary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2889 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/fmudesignrunner.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7911 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/_add_webviz_tornado_onebyone.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25556 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/tools/sensitivities/_excel2dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/src/fmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1263 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/fipmapper/
+-rw-r--r--   0 runner    (1001) docker     (121)     7557 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/fipmapper/test_fipmapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12447 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/fipmapper/test_disjointsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/test_qcdata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/qcproperties/
+-rw-r--r--   0 runner    (1001) docker     (121)    13849 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcproperties/test_qcproperties.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/qcproperties/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcproperties/data/propstat.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcproperties/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/test_extract_zone_tops.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/rms/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/rms_eclipse.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A6_1.obs
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A4.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/layer_zone_table.csv
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A2_1.obs
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A5_1.obs
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A5.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/rft_input_table_4modelcase.csv
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A4_1.obs
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A3_1.obs
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/well_date_rft.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/R_A3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/expected_files/layer_zone_table.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/input_table_drogon.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/
+-rw-r--r--   0 runner    (1001) docker     (121)   197525 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A2.csv
+-rw-r--r--   0 runner    (1001) docker     (121)  1130760 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A4.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   202390 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A3.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   202390 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A5.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   202390 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A6.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/rms/volumetricsdata/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    40726 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/volumetricsdata/14_geo_gas_1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1714 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/volumetricsdata/2_simgrid_vol_oil_1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1644 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/volumetricsdata/1_geogrid_vol_oil_1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8600 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/test_rmsvolumetrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24011 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/test_create_rft_ertobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/rms/test_qcreset_in_roxenv.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/data/zone_tops_from_grid/
+-rw-r--r--   0 runner    (1001) docker     (121)   368221 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/data/zone_tops_from_grid/OP_1.w
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/qcforward/
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcforward/test_gridquality.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8880 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcforward/test_qcforward_in_roxenv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcforward/test_wellzonation_vs_grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6896 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcforward/test_grid_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3096 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/qcforward/test_bw_vs_gridprops.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/sensitivities/
+-rw-r--r--   0 runner    (1001) docker     (121)     8312 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/test_design_distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/sensitivities/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/sensitivities/data/distributions/
+-rw-r--r--   0 runner    (1001) docker     (121)     5994 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/distributions/design.csv
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14391 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/distributions/design.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/distributions/designsummary.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/sensitivities/data/results/
+-rwxr-xr-x   0 runner    (1001) docker     (121)   508763 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/results/geovolumes_collected.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     5208 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/seeds.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)    14950 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_singlereference_and_seed.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (121)    29827 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_background.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)    29812 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_background_extseeds.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)    16773 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_example1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)    22195 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_onebyone.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)     4985 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/doe1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/seeds.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    21878 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_singlereference.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    24954 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_example2.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (121)    33233 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_mc_with_correls.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)    21647 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_example_velocities.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)     4723 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/correlations.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)    29815 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_background_no_seed.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)    21883 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_default_no_seed.xlsx
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3404 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/test_use_cases.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2481 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/test_create_design.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8362 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/test_excel2dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2603 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/test_calc_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/tests/sensitivities/test_designmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 16:43:47.000000 fmu_tools-1.9.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1206 2021-10-27 16:41:38.000000 fmu_tools-1.9.0/examples/example_create_design.py
```

### Comparing `fmu_tools-1.8.1/CONTRIBUTING.rst` & `fmu_tools-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/setup.py` & `fmu_tools-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/setup.cfg` & `fmu_tools-1.9.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 1
 
 [flake8]
 exclude = docs, tests/data
 max-line-length = 88
-ignore = E203, W503
+ignore = E203, W503, C901, F541
 
 [aliases]
 test = pytest
 
 [tool:pytest]
 markers = 
 	integration: marks a test as an integration test
```

### Comparing `fmu_tools-1.8.1/.gitignore` & `fmu_tools-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/fmu_logo/README.md` & `fmu_tools-1.9.0/docs/fmu_logo/README.md`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/fmu_logo/fmu_logo_with_text.svg` & `fmu_tools-1.9.0/docs/fmu_logo/fmu_logo_with_text.svg`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/fmu_logo/fmu_logo_coviz.svg` & `fmu_tools-1.9.0/docs/fmu_logo/fmu_logo_coviz.svg`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/fmu_logo/fmu_logo.svg` & `fmu_tools-1.9.0/docs/fmu_logo/fmu_logo.svg`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/create_rft_ertobs.rst` & `fmu_tools-1.9.0/docs/create_rft_ertobs.rst`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput_singlereference.png` & `fmu_tools-1.9.0/docs/images/design_designinput_singlereference.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_depend1.png` & `fmu_tools-1.9.0/docs/images/design_depend1.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_example1.png` & `fmu_tools-1.9.0/docs/images/design_example1.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_corr1.png` & `fmu_tools-1.9.0/docs/images/design_corr1.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput_dependencies.png` & `fmu_tools-1.9.0/docs/images/design_designinput_dependencies.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_fullmc_corr.png` & `fmu_tools-1.9.0/docs/images/design_fullmc_corr.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput_singlereference_and_seed.png` & `fmu_tools-1.9.0/docs/images/design_designinput_singlereference_and_seed.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput.png` & `fmu_tools-1.9.0/docs/images/design_designinput.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput1.png` & `fmu_tools-1.9.0/docs/images/design_designinput1.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_defaultvalues.png` & `fmu_tools-1.9.0/docs/images/design_defaultvalues.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_general_input.png` & `fmu_tools-1.9.0/docs/images/design_general_input.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput2.png` & `fmu_tools-1.9.0/docs/images/design_designinput2.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_backgroundvalues.png` & `fmu_tools-1.9.0/docs/images/design_backgroundvalues.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput_example_velocities.png` & `fmu_tools-1.9.0/docs/images/design_designinput_example_velocities.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_background_geninput.png` & `fmu_tools-1.9.0/docs/images/design_background_geninput.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/images/design_designinput_background_noseed.png` & `fmu_tools-1.9.0/docs/images/design_designinput_background_noseed.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/qcreset.rst` & `fmu_tools-1.9.0/docs/qcreset.rst`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/_static/equinor_logo_only.jpg` & `fmu_tools-1.9.0/docs/_static/equinor_logo_only.jpg`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/_static/equinor-logo.png` & `fmu_tools-1.9.0/docs/_static/equinor-logo.png`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/_static/equinor-logo2.jpg` & `fmu_tools-1.9.0/docs/_static/equinor-logo2.jpg`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/_static/equinor_logo.jpg` & `fmu_tools-1.9.0/docs/_static/equinor_logo.jpg`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/rmsvolumetrics2csv.rst` & `fmu_tools-1.9.0/docs/rmsvolumetrics2csv.rst`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/qcforward.rst` & `fmu_tools-1.9.0/docs/qcforward.rst`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 * All methods shall have a similar appearance (... as similar as possible)
 
 Methods:
 
 
 * :ref:`Compare well zonation and grid <qcforward-welzonvsgrid>`
 * :ref:`Grid quality indicators <qcforward-gridqualindicators>`
+* :ref:`Blocked wells vs grid properties <qcforward-bwvsprops>`
 * :ref:`Run grid statistics <qcforward-gridstatistics>`
 
 .. include:: qcforward/wellzon_vs_grid.inc
 
 .. include:: qcforward/gridquality.inc
 
+.. include:: qcforward/bw_vs_gridprops.inc
+
 .. include:: qcforward/grid_statistics.inc
```

### Comparing `fmu_tools-1.8.1/docs/qcproperties.rst` & `fmu_tools-1.9.0/docs/qcproperties.rst`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/conf.py` & `fmu_tools-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/qcforward/gridquality.inc` & `fmu_tools-1.9.0/docs/qcforward/gridquality.inc`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/qcforward/grid_statistics.inc` & `fmu_tools-1.9.0/docs/qcforward/grid_statistics.inc`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/qcforward/wellzon_vs_grid.inc` & `fmu_tools-1.9.0/docs/qcforward/wellzon_vs_grid.inc`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/docs/fmudesign.rst` & `fmu_tools-1.9.0/docs/fmudesign.rst`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/LICENSE` & `fmu_tools-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/.github/workflows/fmu-tools.yml` & `fmu_tools-1.9.0/.github/workflows/fmu-tools.yml`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/.github/workflows/codecov.yml` & `fmu_tools-1.9.0/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/PKG-INFO` & `fmu_tools-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu_tools
-Version: 1.8.1
+Version: 1.9.0
 Summary: Library for various tools scripts in FMU scope
 Home-page: https://github.com/equinor/fmu-tools
 Author: Equinor R&T
 Author-email: jriv@equinor.com
 License: UNKNOWN
 Keywords: fmu,tools
 Platform: UNKNOWN
```

### Comparing `fmu_tools-1.8.1/src/fmu_tools.egg-info/SOURCES.txt` & `fmu_tools-1.9.0/src/fmu_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,33 +47,37 @@
 docs/images/design_designinput_dependencies.png
 docs/images/design_designinput_example_velocities.png
 docs/images/design_designinput_singlereference.png
 docs/images/design_designinput_singlereference_and_seed.png
 docs/images/design_example1.png
 docs/images/design_fullmc_corr.png
 docs/images/design_general_input.png
+docs/qcforward/bw_vs_gridprops.inc
 docs/qcforward/grid_statistics.inc
 docs/qcforward/gridquality.inc
 docs/qcforward/wellzon_vs_grid.inc
 examples/example_create_design.py
 src/fmu/__init__.py
 src/fmu/tools/__init__.py
 src/fmu/tools/_common.py
 src/fmu/tools/extract_grid_zone_tops.py
 src/fmu/tools/version.py
 src/fmu/tools/fipmapper/__init__.py
 src/fmu/tools/fipmapper/fipmapper.py
 src/fmu/tools/qcdata/__init__.py
 src/fmu/tools/qcdata/qcdata.py
 src/fmu/tools/qcforward/__init__.py
+src/fmu/tools/qcforward/_blockedwells_vs_gridprops.py
 src/fmu/tools/qcforward/_grid_quality.py
 src/fmu/tools/qcforward/_grid_statistics.py
 src/fmu/tools/qcforward/_qcforward.py
 src/fmu/tools/qcforward/_wellzonation_vs_grid.py
 src/fmu/tools/qcforward/qcforward.py
+src/fmu/tools/qcforward/_schemas/bw_vs_gridprops_asfile.json
+src/fmu/tools/qcforward/_schemas/bw_vs_gridprops_asroxapi.json
 src/fmu/tools/qcforward/_schemas/gridquality_asfile.json
 src/fmu/tools/qcforward/_schemas/gridquality_asroxapi.json
 src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asfile.json
 src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asroxapi.json
 src/fmu/tools/qcproperties/_aggregate_df.py
 src/fmu/tools/qcproperties/_config_parser.py
 src/fmu/tools/qcproperties/_grid2df.py
@@ -101,14 +105,15 @@
 src/fmu_tools.egg-info/top_level.txt
 tests/conftest.py
 tests/test_extract_zone_tops.py
 tests/test_qcdata.py
 tests/data/zone_tops_from_grid/OP_1.w
 tests/fipmapper/test_disjointsets.py
 tests/fipmapper/test_fipmapper.py
+tests/qcforward/test_bw_vs_gridprops.py
 tests/qcforward/test_grid_statistics.py
 tests/qcforward/test_gridquality.py
 tests/qcforward/test_qcforward_in_roxenv.py
 tests/qcforward/test_wellzonation_vs_grid.py
 tests/qcproperties/conftest.py
 tests/qcproperties/test_qcproperties.py
 tests/qcproperties/data/propstat.yml
```

### Comparing `fmu_tools-1.8.1/src/fmu_tools.egg-info/PKG-INFO` & `fmu_tools-1.9.0/src/fmu_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmu-tools
-Version: 1.8.1
+Version: 1.9.0
 Summary: Library for various tools scripts in FMU scope
 Home-page: https://github.com/equinor/fmu-tools
 Author: Equinor R&T
 Author-email: jriv@equinor.com
 License: UNKNOWN
 Keywords: fmu,tools
 Platform: UNKNOWN
```

### Comparing `fmu_tools-1.8.1/src/fmu/tools/fipmapper/fipmapper.py` & `fmu_tools-1.9.0/src/fmu/tools/fipmapper/fipmapper.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcproperties/_config_parser.py` & `fmu_tools-1.9.0/src/fmu/tools/qcproperties/_config_parser.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcproperties/_utils.py` & `fmu_tools-1.9.0/src/fmu/tools/qcproperties/_utils.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcproperties/_aggregate_df.py` & `fmu_tools-1.9.0/src/fmu/tools/qcproperties/_aggregate_df.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcproperties/_grid2df.py` & `fmu_tools-1.9.0/src/fmu/tools/qcproperties/_grid2df.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcproperties/qcproperties.py` & `fmu_tools-1.9.0/src/fmu/tools/qcproperties/qcproperties.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcproperties/_well2df.py` & `fmu_tools-1.9.0/src/fmu/tools/qcproperties/_well2df.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/extract_grid_zone_tops.py` & `fmu_tools-1.9.0/src/fmu/tools/extract_grid_zone_tops.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcdata/qcdata.py` & `fmu_tools-1.9.0/src/fmu/tools/qcdata/qcdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 This private module in qcforward is used to parse data on a general level.
 
 The resulting data will be stored as class instance attributes, e.g. self._grid
 
 """
-from os.path import join
-from glob import glob
 import re
+from glob import glob
+from os.path import join
 
 import xtgeo
 from fmu.tools._common import _QCCommon
 
 CMN = _QCCommon()
 
 
@@ -256,15 +256,14 @@
                             bwname=wells.get("bwname", "BW"),
                             wname=well,
                             lognames=settings.get("lognames", "all"),
                         )
                     )
                 xtg_wells.append(mywell)
                 self._xtgdata[welltype][well] = mywell
-                CMN.print_debug(well)
 
             except ValueError as verr:
                 print(f"Could not read well {well}: {verr}")
 
         CMN.print_debug(f"All valid welldata: {xtg_wells}")
 
         for mywell in xtg_wells:
```

### Comparing `fmu_tools-1.8.1/src/fmu/tools/rms/volumetrics.py` & `fmu_tools-1.9.0/src/fmu/tools/rms/volumetrics.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/rms/create_rft_ertobs.py` & `fmu_tools-1.9.0/src/fmu/tools/rms/create_rft_ertobs.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/rms/qcreset.py` & `fmu_tools-1.9.0/src/fmu/tools/rms/qcreset.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/__init__.py` & `fmu_tools-1.9.0/src/fmu/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/_common.py` & `fmu_tools-1.9.0/src/fmu/tools/_common.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/_wellzonation_vs_grid.py` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/_wellzonation_vs_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 This private module in qcforward is used to check wellzonation vs grid zonation
 """
 
 import collections
-from pathlib import Path
-
 import json
-from jsonschema import validate
-import numpy as np
+from pathlib import Path
 
 import fmu.tools
+import numpy as np
 from fmu.tools._common import _QCCommon
-from fmu.tools.qcforward._qcforward import QCForward, ActionsParser
-
+from fmu.tools.qcforward._qcforward import ActionsParser, QCForward
+from jsonschema import validate
 
 QCC = _QCCommon()
 UNDEF = float("nan")
 
 
 class _LocalData:
     def __init__(self):
```

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/_grid_statistics.py` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/_grid_statistics.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asroxapi.json` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asroxapi.json`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/gridquality_asfile.json` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/gridquality_asfile.json`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asfile.json` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/wellzonation_vs_grid_asfile.json`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/_schemas/gridquality_asroxapi.json` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/_schemas/gridquality_asroxapi.json`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/_grid_quality.py` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/_grid_quality.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/qcforward/qcforward.py` & `fmu_tools-1.9.0/src/fmu/tools/qcforward/qcforward.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,17 +17,18 @@
     # vs
 
     qcjob = qcforward.WellZonationVsGrid()
     qcjob.run(data)
 
 
 """
-from fmu.tools.qcforward._wellzonation_vs_grid import WellZonationVsGrid
-from fmu.tools.qcforward._grid_statistics import GridStatistics
+from fmu.tools.qcforward._blockedwells_vs_gridprops import BlockedWellsVsGridProperties
 from fmu.tools.qcforward._grid_quality import GridQuality
+from fmu.tools.qcforward._grid_statistics import GridStatistics
+from fmu.tools.qcforward._wellzonation_vs_grid import WellZonationVsGrid
 
 
 def wellzonation_vs_grid(data, project=None):
     """Check well zonation or perforations vs 3D grid.
 
     Args:
         data (dict): This is dictonary telling where data comes from
@@ -46,14 +47,26 @@
             a path to a YAML file
     """
 
     gps = GridStatistics()
     gps.run(data, project=project)
 
 
+def blockedwells_vs_gridproperties(data, project=None):
+    """Check blocked wells vs vs grid props.
+
+    Args:
+        data (dict or str): The input data either as a Python dictionary or
+            a path to a YAML file
+    """
+
+    bwgp = BlockedWellsVsGridProperties()
+    bwgp.run(data, project=project)
+
+
 def grid_quality(data, project=None):
     """Check grid quality in 3D grid against user input.
 
     Args:
         data (dict): The input data either as a Python dictionary or
             a path to a YAML file
     """
```

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/create_design.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/create_design.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/_tornado_onebyone.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/_tornado_onebyone.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/__init__.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/__init__.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/design_distributions.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/design_distributions.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/_designsummary.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/_designsummary.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/fmudesignrunner.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/fmudesignrunner.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/_add_webviz_tornado_onebyone.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/_add_webviz_tornado_onebyone.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/src/fmu/tools/sensitivities/_excel2dict.py` & `fmu_tools-1.9.0/src/fmu/tools/sensitivities/_excel2dict.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/README.rst` & `fmu_tools-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/.pre-commit-config.yaml` & `fmu_tools-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/.pylintrc` & `fmu_tools-1.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/fipmapper/test_fipmapper.py` & `fmu_tools-1.9.0/tests/fipmapper/test_fipmapper.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/fipmapper/test_disjointsets.py` & `fmu_tools-1.9.0/tests/fipmapper/test_disjointsets.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/test_qcdata.py` & `fmu_tools-1.9.0/tests/test_qcdata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Testing qcdata loading of XTGeo data"""
 
-from __future__ import absolute_import, division, print_function  # PY2
-
 from os.path import abspath
-import pytest
-
-from fmu.tools.qcdata import QCData
 
+import pytest
 import xtgeo
+from fmu.tools.qcdata import QCData
 
 # filedata
 PATH = abspath(".")  # normally not needed; here due to pytest fixture tmpdir
 GRIDFILE = "../xtgeo-testdata/3dgrids/reek/reek_sim_grid.roff"
 ZONENAME = "Zone"
 ZONEFILE = "../xtgeo-testdata/3dgrids/reek/reek_sim_zone.roff"
 WELLFILES = [
```

### Comparing `fmu_tools-1.8.1/tests/qcproperties/test_qcproperties.py` & `fmu_tools-1.9.0/tests/qcproperties/test_qcproperties.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/qcproperties/data/propstat.yml` & `fmu_tools-1.9.0/tests/qcproperties/data/propstat.yml`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/qcproperties/conftest.py` & `fmu_tools-1.9.0/tests/qcproperties/conftest.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/test_extract_zone_tops.py` & `fmu_tools-1.9.0/tests/test_extract_zone_tops.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A2.csv` & `fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A2.csv`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A4.csv` & `fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A4.csv`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A3.csv` & `fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A3.csv`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A5.csv` & `fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A5.csv`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/rft_ertobs_data/coords/coords-R_A6.csv` & `fmu_tools-1.9.0/tests/rms/rft_ertobs_data/coords/coords-R_A6.csv`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/volumetricsdata/14_geo_gas_1.txt` & `fmu_tools-1.9.0/tests/rms/volumetricsdata/14_geo_gas_1.txt`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/volumetricsdata/2_simgrid_vol_oil_1.txt` & `fmu_tools-1.9.0/tests/rms/volumetricsdata/2_simgrid_vol_oil_1.txt`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/volumetricsdata/1_geogrid_vol_oil_1.txt` & `fmu_tools-1.9.0/tests/rms/volumetricsdata/1_geogrid_vol_oil_1.txt`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/test_rmsvolumetrics.py` & `fmu_tools-1.9.0/tests/rms/test_rmsvolumetrics.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/test_create_rft_ertobs.py` & `fmu_tools-1.9.0/tests/rms/test_create_rft_ertobs.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/rms/test_qcreset_in_roxenv.py` & `fmu_tools-1.9.0/tests/rms/test_qcreset_in_roxenv.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/data/zone_tops_from_grid/OP_1.w` & `fmu_tools-1.9.0/tests/data/zone_tops_from_grid/OP_1.w`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/conftest.py` & `fmu_tools-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/qcforward/test_gridquality.py` & `fmu_tools-1.9.0/tests/qcforward/test_gridquality.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/qcforward/test_qcforward_in_roxenv.py` & `fmu_tools-1.9.0/tests/qcforward/test_qcforward_in_roxenv.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/qcforward/test_wellzonation_vs_grid.py` & `fmu_tools-1.9.0/tests/qcforward/test_wellzonation_vs_grid.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Testing qcforward method wellzonation vs grid"""
 
 import pathlib
 from os.path import abspath
-import pytest
-import pandas as pd
 
 import fmu.tools.qcforward as qcf
+import pandas as pd
+import pytest
 
 # filedata
 PATH = abspath(".")  # normally not needed; here due to pytest fixture tmpdir
 GRIDFILE = "../xtgeo-testdata/3dgrids/reek/reek_sim_grid.roff"
 ZONENAME = "Zone"
 ZONEFILE = "../xtgeo-testdata/3dgrids/reek/reek_sim_zone.roff"
 WELLFILES = [
```

### Comparing `fmu_tools-1.8.1/tests/qcforward/test_grid_statistics.py` & `fmu_tools-1.9.0/tests/qcforward/test_grid_statistics.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/test_design_distributions.py` & `fmu_tools-1.9.0/tests/sensitivities/test_design_distributions.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/distributions/design.csv` & `fmu_tools-1.9.0/tests/sensitivities/data/distributions/design.csv`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/distributions/design.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/distributions/design.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/results/geovolumes_collected.csv` & `fmu_tools-1.9.0/tests/sensitivities/data/results/geovolumes_collected.csv`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/seeds.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/seeds.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_singlereference_and_seed.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_singlereference_and_seed.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_background.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_background.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_background_extseeds.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_background_extseeds.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_example1.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_example1.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_onebyone.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_onebyone.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/doe1.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/doe1.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_singlereference.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_singlereference.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_example2.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_example2.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_mc_with_correls.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_mc_with_correls.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_example_velocities.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_example_velocities.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/correlations.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/correlations.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_background_no_seed.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_background_no_seed.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/data/config/design_input_default_no_seed.xlsx` & `fmu_tools-1.9.0/tests/sensitivities/data/config/design_input_default_no_seed.xlsx`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/test_use_cases.py` & `fmu_tools-1.9.0/tests/sensitivities/test_use_cases.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/test_create_design.py` & `fmu_tools-1.9.0/tests/sensitivities/test_create_design.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/test_excel2dict.py` & `fmu_tools-1.9.0/tests/sensitivities/test_excel2dict.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/test_calc_tornado.py` & `fmu_tools-1.9.0/tests/sensitivities/test_calc_tornado.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/tests/sensitivities/test_designmatrix.py` & `fmu_tools-1.9.0/tests/sensitivities/test_designmatrix.py`

 * *Files identical despite different names*

### Comparing `fmu_tools-1.8.1/examples/example_create_design.py` & `fmu_tools-1.9.0/examples/example_create_design.py`

 * *Files identical despite different names*

