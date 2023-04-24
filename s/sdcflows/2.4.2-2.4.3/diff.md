# Comparing `tmp/sdcflows-2.4.2.tar.gz` & `tmp/sdcflows-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdcflows-2.4.2.tar", last modified: Thu Apr 20 13:07:47 2023, max compression
+gzip compressed data, was "sdcflows-2.4.3.tar", last modified: Mon Apr 24 13:11:49 2023, max compression
```

## Comparing `sdcflows-2.4.2.tar` & `sdcflows-2.4.3.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.787796 sdcflows-2.4.2/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.739796 sdcflows-2.4.2/.maint/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1594 2023-04-20 13:07:26.000000 sdcflows-2.4.2/.maint/CONTRIBUTORS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-04-20 13:07:26.000000 sdcflows-2.4.2/.maint/FORMER.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-20 13:07:26.000000 sdcflows-2.4.2/.maint/MAINTAINERS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-04-20 13:07:26.000000 sdcflows-2.4.2/.maint/PIs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-04-20 13:07:26.000000 sdcflows-2.4.2/.maint/ROADMAP.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9457 2023-04-20 13:07:26.000000 sdcflows-2.4.2/.maint/update_authors.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1174 2023-04-20 13:07:26.000000 sdcflows-2.4.2/.maint/update_requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21864 2023-04-20 13:07:26.000000 sdcflows-2.4.2/CHANGES.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-04-20 13:07:26.000000 sdcflows-2.4.2/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-20 13:07:26.000000 sdcflows-2.4.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-04-20 13:07:26.000000 sdcflows-2.4.2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-04-20 13:07:26.000000 sdcflows-2.4.2/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-20 13:07:47.787796 sdcflows-2.4.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2023-04-20 13:07:26.000000 sdcflows-2.4.2/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      218 2023-04-20 13:07:26.000000 sdcflows-2.4.2/min-requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-20 13:07:26.000000 sdcflows-2.4.2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-20 13:07:26.000000 sdcflows-2.4.2/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.739796 sdcflows-2.4.2/sdcflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      502 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.739796 sdcflows-2.4.2/sdcflows/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3266 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/cli/find_estimators.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.739796 sdcflows-2.4.2/sdcflows/cli/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/cli/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/cli/tests/test_find_estimators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3011 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.747796 sdcflows-2.4.2/sdcflows/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/affine.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.747796 sdcflows-2.4.2/sdcflows/data/flirtsch/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_1.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_2.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_4.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_quick.cnf
--rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/fmap-any_registration.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/fmap-any_registration_testing.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)  5801500 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/fmap_atlas.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/fmap_atlas_2_MNI152NLin2009cAsym_affine.mat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      960 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/sd_syn.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/sd_syn_sloppy.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/data/translation_rigid.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17569 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/fieldmaps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.747796 sdcflows-2.4.2/sdcflows/interfaces/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/brainmask.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23457 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/bspline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4440 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/epi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/fmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5483 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/reportlets.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.747796 sdcflows-2.4.2/sdcflows/interfaces/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4506 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/tests/test_bspline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/tests/test_epi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/tests/test_fmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1770 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/tests/test_reportlets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4243 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18032 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/interfaces/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.751796 sdcflows-2.4.2/sdcflows/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.751796 sdcflows-2.4.2/sdcflows/tests/data/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.755796 sdcflows-2.4.2/sdcflows/tests/data/dsA/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.735796 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.755796 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/anat/sub-01_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.755796 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.759796 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.759796 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.759796 sdcflows-2.4.2/sdcflows/tests/data/dsB/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      270 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.735796 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.735796 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.763796 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.763796 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.767796 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.767796 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.771796 sdcflows-2.4.2/sdcflows/tests/data/dsC/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/dataset_description.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.735796 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.771796 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/anat/sub-01_FLAIR.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T1w.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T2w.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.771796 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.779796 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.nii.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.779796 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_bold.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_sbref.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/dsC/task-rest_bold.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1954195 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/epi.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/field-coeff-tests.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29820 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/topup-coeff-fixed.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29726 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/topup-coeff.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)  2210404 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/data/topup-field.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11243 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/test_fieldmaps.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6003 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2110 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/tests/test_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16934 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/transform.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.779796 sdcflows-2.4.2/sdcflows/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6762 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/bimap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10294 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/epimanip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5069 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/phasemanip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.779796 sdcflows-2.4.2/sdcflows/utils/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1460 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/tests/test_misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/tests/test_phasemanip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1214 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/tests/test_tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7232 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/tests/test_wrangler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7852 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21284 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/utils/wrangler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.779796 sdcflows-2.4.2/sdcflows/viz/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/viz/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4092 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/viz/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.783796 sdcflows-2.4.2/sdcflows/workflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3747 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/ancillary.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.783796 sdcflows-2.4.2/sdcflows/workflows/apply/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/apply/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6544 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/apply/correction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/apply/registration.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.783796 sdcflows-2.4.2/sdcflows/workflows/apply/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/apply/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30980 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5277 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/apply/tests/test_correction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4362 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/apply/tests/test_registration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6275 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.783796 sdcflows-2.4.2/sdcflows/workflows/fit/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13253 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/fieldmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16449 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/pepolar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24995 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/syn.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.787796 sdcflows-2.4.2/sdcflows/workflows/fit/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1727 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_fit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_pepolar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3946 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_phdiff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6807 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_syn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9632 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/outputs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.787796 sdcflows-2.4.2/sdcflows/workflows/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/tests/test_ancillary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2023-04-20 13:07:26.000000 sdcflows-2.4.2/sdcflows/workflows/tests/test_base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.739796 sdcflows-2.4.2/sdcflows.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10864 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-20 13:07:47.000000 sdcflows-2.4.2/sdcflows.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2336 2023-04-20 13:07:47.787796 sdcflows-2.4.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-04-20 13:07:26.000000 sdcflows-2.4.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-20 13:07:47.787796 sdcflows-2.4.2/tools/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-04-20 13:07:26.000000 sdcflows-2.4.2/tools/cache_templateflow.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/.maint/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1594 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/CONTRIBUTORS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/FORMER.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/MAINTAINERS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/PIs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/ROADMAP.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9457 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/update_authors.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1174 2023-04-24 13:11:30.000000 sdcflows-2.4.3/.maint/update_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22205 2023-04-24 13:11:30.000000 sdcflows-2.4.3/CHANGES.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-04-24 13:11:30.000000 sdcflows-2.4.3/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-24 13:11:30.000000 sdcflows-2.4.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-04-24 13:11:30.000000 sdcflows-2.4.3/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      411 2023-04-24 13:11:30.000000 sdcflows-2.4.3/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-24 13:11:49.588117 sdcflows-2.4.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2023-04-24 13:11:30.000000 sdcflows-2.4.3/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      218 2023-04-24 13:11:30.000000 sdcflows-2.4.3/min-requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-04-24 13:11:30.000000 sdcflows-2.4.3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-24 13:11:30.000000 sdcflows-2.4.3/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      502 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3266 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/find_estimators.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows/cli/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3464 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/cli/tests/test_find_estimators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3011 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.536116 sdcflows-2.4.3/sdcflows/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/affine.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.536116 sdcflows-2.4.3/sdcflows/data/flirtsch/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_1.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_2.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_4.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_quick.cnf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap-any_registration.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap-any_registration_testing.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  5801500 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap_atlas.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/fmap_atlas_2_MNI152NLin2009cAsym_affine.mat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      960 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/sd_syn.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      978 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/sd_syn_sloppy.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/data/translation_rigid.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17569 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/fieldmaps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.540116 sdcflows-2.4.3/sdcflows/interfaces/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4729 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/brainmask.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23807 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/bspline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4440 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/epi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/fmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5483 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/reportlets.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.540116 sdcflows-2.4.3/sdcflows/interfaces/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4506 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_bspline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1482 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_epi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_fmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1770 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_reportlets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4243 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18032 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/interfaces/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.544116 sdcflows-2.4.3/sdcflows/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.544116 sdcflows-2.4.3/sdcflows/tests/data/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.548116 sdcflows-2.4.3/sdcflows/tests/data/dsA/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.520116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.548116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/sub-01_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/anat/sub-01_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.552116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.556116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/fmap/sub-01_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.560116 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsA/sub-01/func/sub-01_task-rest_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.560116 sdcflows-2.4.3/sdcflows/tests/data/dsB/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      270 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.520116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.520116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.560116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/anat/sub-01_ses-1_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.564116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/dwi/sub-01_ses-1_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/fmap/sub-01_ses-1_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsB/sub-01/ses-1/func/sub-01_ses-1_task-rest_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsC/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      256 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/dataset_description.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.524116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.568116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/sub-01_FLAIR.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T1w.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/anat/sub-01_T2w.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.572116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-AP_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-LR_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-PA_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_dwi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/dwi/sub-01_dir-RL_sbref.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_acq-single_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-AP_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-LR_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-PA_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_dir-RL_epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_fieldmap.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_magnitude2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase1.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phase2.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/fmap/sub-01_phasediff.nii.gz
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_bold.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/sub-01/func/sub-01_task-rest_sbref.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/dsC/task-rest_bold.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1954195 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/epi.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2302 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/field-coeff-tests.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29820 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/topup-coeff-fixed.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29726 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/topup-coeff.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  2210404 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/data/topup-field.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11243 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/test_fieldmaps.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6003 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2110 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/tests/test_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16934 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/transform.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6762 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/bimap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10294 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/epimanip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5069 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/phasemanip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.580116 sdcflows-2.4.3/sdcflows/utils/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1460 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_phasemanip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1214 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7232 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tests/test_wrangler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7852 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21284 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/utils/wrangler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/viz/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/viz/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4092 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/viz/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/workflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3747 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/ancillary.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/workflows/apply/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6544 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/correction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5286 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/registration.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.584117 sdcflows-2.4.3/sdcflows/workflows/apply/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30980 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5277 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_correction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4362 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_registration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6275 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/sdcflows/workflows/fit/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13253 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/fieldmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16449 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/pepolar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24995 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/syn.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/sdcflows/workflows/fit/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1727 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_fit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3179 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_pepolar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3946 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_phdiff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6807 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_syn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9632 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/outputs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/sdcflows/workflows/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/tests/test_ancillary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2710 2023-04-24 13:11:30.000000 sdcflows-2.4.3/sdcflows/workflows/tests/test_base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.528116 sdcflows-2.4.3/sdcflows.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10864 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-24 13:11:49.000000 sdcflows-2.4.3/sdcflows.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2336 2023-04-24 13:11:49.592116 sdcflows-2.4.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-04-24 13:11:30.000000 sdcflows-2.4.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-24 13:11:49.588117 sdcflows-2.4.3/tools/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-04-24 13:11:30.000000 sdcflows-2.4.3/tools/cache_templateflow.py
```

### Comparing `sdcflows-2.4.2/.maint/CONTRIBUTORS.md` & `sdcflows-2.4.3/.maint/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/.maint/FORMER.md` & `sdcflows-2.4.3/.maint/FORMER.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/.maint/MAINTAINERS.md` & `sdcflows-2.4.3/.maint/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/.maint/PIs.md` & `sdcflows-2.4.3/.maint/PIs.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/.maint/ROADMAP.md` & `sdcflows-2.4.3/.maint/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/.maint/update_authors.py` & `sdcflows-2.4.3/.maint/update_authors.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/.maint/update_requirements.py` & `sdcflows-2.4.3/.maint/update_requirements.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/CHANGES.rst` & `sdcflows-2.4.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+2.4.3 (April 24, 2023)
+======================
+Bug-fix release in the 2.4.x series.
+
+This fix resolves an inconsistency of treatment of phase-difference and
+scanner-calculated fieldmaps, relative to PEPolar and SyN. Fieldmaps in
+orientations other than RAS were impacted.
+
+* FIX: Reorient fieldmaps to RAS before estimating B-splines (#354)
+
 2.4.2 (April 20, 2023)
 ======================
 Bug-fix release in the 2.4.x series.
 
 Same fixes as 2.4.1, but this time for phase-difference and direct fieldmaps
 we missed last time.
```

### Comparing `sdcflows-2.4.2/LICENSE` & `sdcflows-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/PKG-INFO` & `sdcflows-2.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdcflows
-Version: 2.4.2
+Version: 2.4.3
 Summary: Susceptibility Distortion Correction (SDC) workflows for EPI MR schemes.
 Home-page: https://www.nipreps.org/sdcflows
 Author: The SDCflows developers
 Author-email: nipreps@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.nipreps.org/sdcflows
 Project-URL: GitHub, https://github.com/nipreps/sdcflows
```

### Comparing `sdcflows-2.4.2/README.rst` & `sdcflows-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/cli/find_estimators.py` & `sdcflows-2.4.3/sdcflows/cli/find_estimators.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/cli/tests/test_find_estimators.py` & `sdcflows-2.4.3/sdcflows/cli/tests/test_find_estimators.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/conftest.py` & `sdcflows-2.4.3/sdcflows/conftest.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/affine.json` & `sdcflows-2.4.3/sdcflows/data/affine.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0.cnf` & `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_1.cnf` & `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_1.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_2.cnf` & `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_2.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_4.cnf` & `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_4.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/flirtsch/b02b0_quick.cnf` & `sdcflows-2.4.3/sdcflows/data/flirtsch/b02b0_quick.cnf`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/fmap-any_registration.json` & `sdcflows-2.4.3/sdcflows/data/fmap-any_registration.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/fmap-any_registration_testing.json` & `sdcflows-2.4.3/sdcflows/data/fmap-any_registration_testing.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/fmap_atlas.nii.gz` & `sdcflows-2.4.3/sdcflows/data/fmap_atlas.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/sd_syn.json` & `sdcflows-2.4.3/sdcflows/data/sd_syn.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/sd_syn_sloppy.json` & `sdcflows-2.4.3/sdcflows/data/sd_syn_sloppy.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/data/translation_rigid.json` & `sdcflows-2.4.3/sdcflows/data/translation_rigid.json`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/fieldmaps.py` & `sdcflows-2.4.3/sdcflows/fieldmaps.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/brainmask.py` & `sdcflows-2.4.3/sdcflows/interfaces/brainmask.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/bspline.py` & `sdcflows-2.4.3/sdcflows/interfaces/bspline.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,22 +136,25 @@
         # Output name baseline
         out_name = fname_presuffix(
             self.inputs.in_data, suffix="_field", newpath=runtime.cwd
         )
 
         # Load in the fieldmap
         fmapnii = nb.load(self.inputs.in_data)
+        fmapnii = nb.as_closest_canonical(fmapnii)
         zooms = fmapnii.header.get_zooms()
 
         # Get a mask (or define on the spot to cover the full extent)
         masknii = (
             nb.load(self.inputs.in_mask)
             if isdefined(self.inputs.in_mask)
             else None
         )
+        if masknii is not None:
+            masknii = nb.as_closest_canonical(masknii)
 
         # Determine the shape of bspline coefficients
         # This should not change with resizing, so do it first
         bs_grids = [bspline_grid(fmapnii, control_zooms_mm=sp) for sp in self.inputs.bs_spacing]
 
         need_resize = np.any(np.array(zooms) < self.inputs.zooms_min)
         if need_resize:
@@ -174,25 +177,28 @@
         # Generate a numpy array with the mask
         mask = (
             np.ones(fmapnii.shape, dtype=bool) if masknii is None
             else np.asanyarray(masknii.dataobj) > 1e-4
         )
 
         # Recenter the fieldmap
+        center = 0
         if self.inputs.recenter == "mode":
             from scipy.stats import mode
 
             # Handle pre- and post-1.9 mode behavior.
             # squeeze can be dropped when the minimum version reaches 1.9
             # Will become: data -= mode(data[mask], keepdims=False).mode
-            data -= np.squeeze(mode(data[mask]).mode)
+            center = np.squeeze(mode(data[mask]).mode)
         elif self.inputs.recenter == "median":
-            data -= np.median(data[mask])
+            center = np.median(data[mask])
         elif self.inputs.recenter == "mean":
-            data -= np.mean(data[mask])
+            center = np.mean(data[mask])
+
+        data -= center
 
         # Calculate collocation matrix from (possibly resized) image and knot grids
         colmat = sparse_vstack(grid_bspline_weights(fmapnii, grid) for grid in bs_grids).T.tocsr()
 
         bs_grids_str = ['x'.join(str(s) for s in grid.shape) for grid in bs_grids]
         bs_grids_str[-1] = f"and {bs_grids_str[-1]}"
         LOGGER.info(
@@ -220,19 +226,22 @@
             ).to_filename(out_level)
             index += n
             self._results["out_coeff"].append(out_level)
 
         # Interpolating in the original grid will require a new collocation matrix
         if need_resize:
             fmapnii = nb.load(self.inputs.in_data)
-            data = fmapnii.get_fdata(dtype="float32")
-            mask = (
-                np.ones_like(fmapnii.dataobj, dtype=bool) if masknii is None
-                else np.asanyarray(nb.load(self.inputs.in_mask).dataobj) > 1e-4
-            )
+            fmapnii = nb.as_closest_canonical(fmapnii)
+            data = fmapnii.get_fdata(dtype="float32") - center
+            if masknii is not None:
+                masknii = nb.load(self.inputs.in_mask)
+                masknii = nb.as_closest_canonical(masknii)
+                mask = np.asanyarray(masknii.dataobj) > 1e-4
+            else:
+                mask = np.ones_like(fmapnii.dataobj, dtype=bool)
             colmat = sparse_vstack(
                 grid_bspline_weights(fmapnii, grid) for grid in bs_grids
             ).T.tocsr()
 
         regressors = colmat[mask.reshape(-1), :]
         interp_data = np.zeros_like(data)
         # Interpolate the field from the coefficients just calculated
```

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/epi.py` & `sdcflows-2.4.3/sdcflows/interfaces/epi.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/fmap.py` & `sdcflows-2.4.3/sdcflows/interfaces/fmap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/reportlets.py` & `sdcflows-2.4.3/sdcflows/interfaces/reportlets.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/tests/test_bspline.py` & `sdcflows-2.4.3/sdcflows/interfaces/tests/test_bspline.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/tests/test_epi.py` & `sdcflows-2.4.3/sdcflows/interfaces/tests/test_epi.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/tests/test_fmap.py` & `sdcflows-2.4.3/sdcflows/interfaces/tests/test_fmap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/tests/test_reportlets.py` & `sdcflows-2.4.3/sdcflows/interfaces/tests/test_reportlets.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/tests/test_utils.py` & `sdcflows-2.4.3/sdcflows/interfaces/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/interfaces/utils.py` & `sdcflows-2.4.3/sdcflows/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/data/epi.nii.gz` & `sdcflows-2.4.3/sdcflows/tests/data/epi.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/data/field-coeff-tests.nii.gz` & `sdcflows-2.4.3/sdcflows/tests/data/field-coeff-tests.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/data/topup-coeff-fixed.nii.gz` & `sdcflows-2.4.3/sdcflows/tests/data/topup-coeff-fixed.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/data/topup-coeff.nii.gz` & `sdcflows-2.4.3/sdcflows/tests/data/topup-coeff.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/data/topup-field.nii.gz` & `sdcflows-2.4.3/sdcflows/tests/data/topup-field.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/test_fieldmaps.py` & `sdcflows-2.4.3/sdcflows/tests/test_fieldmaps.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/test_transform.py` & `sdcflows-2.4.3/sdcflows/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/tests/test_version.py` & `sdcflows-2.4.3/sdcflows/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/transform.py` & `sdcflows-2.4.3/sdcflows/transform.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/bimap.py` & `sdcflows-2.4.3/sdcflows/utils/bimap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/epimanip.py` & `sdcflows-2.4.3/sdcflows/utils/epimanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/misc.py` & `sdcflows-2.4.3/sdcflows/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/phasemanip.py` & `sdcflows-2.4.3/sdcflows/utils/phasemanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/tests/test_misc.py` & `sdcflows-2.4.3/sdcflows/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/tests/test_phasemanip.py` & `sdcflows-2.4.3/sdcflows/utils/tests/test_phasemanip.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/tests/test_tools.py` & `sdcflows-2.4.3/sdcflows/utils/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/tests/test_wrangler.py` & `sdcflows-2.4.3/sdcflows/utils/tests/test_wrangler.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/tools.py` & `sdcflows-2.4.3/sdcflows/utils/tools.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/utils/wrangler.py` & `sdcflows-2.4.3/sdcflows/utils/wrangler.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/viz/utils.py` & `sdcflows-2.4.3/sdcflows/viz/utils.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/ancillary.py` & `sdcflows-2.4.3/sdcflows/workflows/ancillary.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/apply/correction.py` & `sdcflows-2.4.3/sdcflows/workflows/apply/correction.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/apply/registration.py` & `sdcflows-2.4.3/sdcflows/workflows/apply/registration.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz` & `sdcflows-2.4.3/sdcflows/workflows/apply/tests/fieldcoeff.nii.gz`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/apply/tests/test_correction.py` & `sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_correction.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/apply/tests/test_registration.py` & `sdcflows-2.4.3/sdcflows/workflows/apply/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/base.py` & `sdcflows-2.4.3/sdcflows/workflows/base.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/fit/fieldmap.py` & `sdcflows-2.4.3/sdcflows/workflows/fit/fieldmap.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/fit/pepolar.py` & `sdcflows-2.4.3/sdcflows/workflows/fit/pepolar.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/fit/syn.py` & `sdcflows-2.4.3/sdcflows/workflows/fit/syn.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_fit.py` & `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_pepolar.py` & `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_pepolar.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_phdiff.py` & `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_phdiff.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/fit/tests/test_syn.py` & `sdcflows-2.4.3/sdcflows/workflows/fit/tests/test_syn.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/outputs.py` & `sdcflows-2.4.3/sdcflows/workflows/outputs.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/tests/test_ancillary.py` & `sdcflows-2.4.3/sdcflows/workflows/tests/test_ancillary.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows/workflows/tests/test_base.py` & `sdcflows-2.4.3/sdcflows/workflows/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows.egg-info/PKG-INFO` & `sdcflows-2.4.3/sdcflows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdcflows
-Version: 2.4.2
+Version: 2.4.3
 Summary: Susceptibility Distortion Correction (SDC) workflows for EPI MR schemes.
 Home-page: https://www.nipreps.org/sdcflows
 Author: The SDCflows developers
 Author-email: nipreps@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://www.nipreps.org/sdcflows
 Project-URL: GitHub, https://github.com/nipreps/sdcflows
```

### Comparing `sdcflows-2.4.2/sdcflows.egg-info/SOURCES.txt` & `sdcflows-2.4.3/sdcflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/sdcflows.egg-info/requires.txt` & `sdcflows-2.4.3/sdcflows.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdcflows-2.4.2/setup.cfg` & `sdcflows-2.4.3/setup.cfg`

 * *Files identical despite different names*

