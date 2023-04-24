# Comparing `tmp/tshirt-0.1.dev9.tar.gz` & `tmp/tshirt-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tshirt-0.1.dev9.tar", last modified: Tue Jan 25 05:23:15 2022, max compression
+gzip compressed data, was "tshirt-0.2.tar", last modified: Mon Apr 24 16:35:14 2023, max compression
```

## Comparing `tshirt-0.1.dev9.tar` & `tshirt-0.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.166515 tshirt-0.1.dev9/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       40 2017-01-16 05:08:31.000000 tshirt-0.1.dev9/.gitattributes
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1803 2021-07-03 05:50:30.000000 tshirt-0.1.dev9/.gitignore
--rw-r--r--   0 everettschlawin   (501) staff       (20)        0 2020-02-18 20:41:06.000000 tshirt-0.1.dev9/.gitmodules
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1073 2020-07-06 05:04:56.000000 tshirt-0.1.dev9/LICENSE
--rw-r--r--   0 everettschlawin   (501) staff       (20)       30 2020-09-13 03:03:55.000000 tshirt-0.1.dev9/MANIFEST.in
--rw-r--r--   0 everettschlawin   (501) staff       (20)      956 2022-01-25 05:23:15.166335 tshirt-0.1.dev9/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)      758 2020-07-06 05:04:31.000000 tshirt-0.1.dev9/README.md
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.149767 tshirt-0.1.dev9/docs/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      634 2020-06-22 23:17:25.000000 tshirt-0.1.dev9/docs/Makefile
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2134 2020-11-08 04:57:30.000000 tshirt-0.1.dev9/docs/conf.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.149908 tshirt-0.1.dev9/docs/images/
--rw-r--r--   0 everettschlawin   (501) staff       (20)   176987 2020-06-23 17:58:22.000000 tshirt-0.1.dev9/docs/images/t_shirt_logo.jpg
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1013 2022-01-18 07:12:31.000000 tshirt-0.1.dev9/docs/index.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3631 2022-01-18 07:20:02.000000 tshirt-0.1.dev9/docs/installation.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      795 2020-06-22 23:17:25.000000 tshirt-0.1.dev9/docs/make.bat
--rw-r--r--   0 everettschlawin   (501) staff       (20)      896 2020-11-08 04:57:30.000000 tshirt-0.1.dev9/docs/modules.rst
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.152366 tshirt-0.1.dev9/docs/phot_pipeline/
--rw-r--r--   0 everettschlawin   (501) staff       (20)    37697 2020-07-12 04:40:36.000000 tshirt-0.1.dev9/docs/phot_pipeline/box_time_series_cookbook.ipynb
--rw-r--r--   0 everettschlawin   (501) staff       (20)      439 2020-07-12 04:40:36.000000 tshirt-0.1.dev9/docs/phot_pipeline/example_phot_param_file.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      397 2020-07-12 04:40:36.000000 tshirt-0.1.dev9/docs/phot_pipeline/phot_pipeline.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     4789 2021-12-03 07:54:32.000000 tshirt-0.1.dev9/docs/phot_pipeline/phot_pipeline_parameters.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1049 2021-03-29 20:26:21.000000 tshirt-0.1.dev9/docs/phot_pipeline/running_phot_pipeline.rst
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.152617 tshirt-0.1.dev9/docs/reduction/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      915 2021-02-18 21:10:57.000000 tshirt-0.1.dev9/docs/reduction/reduction.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      178 2020-06-23 18:40:40.000000 tshirt-0.1.dev9/docs/reduction/reduction_param.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       78 2020-12-07 06:50:34.000000 tshirt-0.1.dev9/docs/requirements.txt
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.154608 tshirt-0.1.dev9/docs/spec_pipeline/
--rw-r--r--   0 everettschlawin   (501) staff       (20)   921939 2020-07-06 05:04:31.000000 tshirt-0.1.dev9/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2669 2020-07-12 04:40:36.000000 tshirt-0.1.dev9/docs/spec_pipeline/batch_processing.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2721 2021-10-14 21:52:05.000000 tshirt-0.1.dev9/docs/spec_pipeline/parameter_file.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      481 2020-07-12 04:40:36.000000 tshirt-0.1.dev9/docs/spec_pipeline/spec_pipeline.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)    34730 2020-07-13 07:19:44.000000 tshirt-0.1.dev9/docs/spec_pipeline/test_spec_pipeline.ipynb
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.156320 tshirt-0.1.dev9/docs/specific_modules/
--rw-r--r--   0 everettschlawin   (501) staff       (20)    36491 2022-01-18 07:07:34.000000 tshirt-0.1.dev9/docs/specific_modules/ROEBA.ipynb
--rw-r--r--   0 everettschlawin   (501) staff       (20)      182 2022-01-18 07:09:23.000000 tshirt-0.1.dev9/docs/specific_modules/specific_modules.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       38 2022-01-25 05:23:15.166562 tshirt-0.1.dev9/setup.cfg
--rw-r--r--   0 everettschlawin   (501) staff       (20)      850 2022-01-25 05:17:11.000000 tshirt-0.1.dev9/setup.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.158645 tshirt-0.1.dev9/tshirt/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      122 2022-01-25 05:17:57.000000 tshirt-0.1.dev9/tshirt/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      212 2019-02-19 20:21:03.000000 tshirt-0.1.dev9/tshirt/allk1255_centroid.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.159344 tshirt-0.1.dev9/tshirt/chisquare/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.1.dev9/tshirt/chisquare/directory_placeholder.dat
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.159471 tshirt-0.1.dev9/tshirt/cleaned_tser/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.1.dev9/tshirt/cleaned_tser/directory_placeholder.dat
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.159689 tshirt-0.1.dev9/tshirt/directory_info/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2221 2021-12-03 07:54:32.000000 tshirt-0.1.dev9/tshirt/directory_info/directory_list.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1081 2021-12-03 07:54:32.000000 tshirt-0.1.dev9/tshirt/directory_info/example_data_list.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)      767 2019-02-19 20:21:03.000000 tshirt-0.1.dev9/tshirt/example_fits.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.146879 tshirt-0.1.dev9/tshirt/existing_dat/
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.159909 tshirt-0.1.dev9/tshirt/existing_dat/spectra/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      738 2019-02-19 20:21:03.000000 tshirt-0.1.dev9/tshirt/existing_dat/spectra/fratio_yang2016.csv
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2122 2019-02-19 20:21:03.000000 tshirt-0.1.dev9/tshirt/fit_models.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    52675 2020-06-14 23:10:48.000000 tshirt-0.1.dev9/tshirt/fit_tser_emcee.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     6638 2020-10-16 22:10:25.000000 tshirt-0.1.dev9/tshirt/mie_model.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.160178 tshirt-0.1.dev9/tshirt/parameters/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      308 2020-07-12 22:57:27.000000 tshirt-0.1.dev9/tshirt/parameters/fit_params.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.160306 tshirt-0.1.dev9/tshirt/parameters/mie_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      434 2020-07-12 22:57:38.000000 tshirt-0.1.dev9/tshirt/parameters/mie_params/simplePoly.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.160644 tshirt-0.1.dev9/tshirt/parameters/phot_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2385 2020-07-12 22:54:25.000000 tshirt-0.1.dev9/tshirt/parameters/phot_params/example_batch_phot.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3425 2021-08-17 21:22:42.000000 tshirt-0.1.dev9/tshirt/parameters/phot_params/example_phot_parameters.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)      423 2020-07-12 22:53:44.000000 tshirt-0.1.dev9/tshirt/parameters/phot_params/keywords_for_phot_pipeline.csv
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.161088 tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2558 2021-04-13 04:23:56.000000 tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2924 2021-04-13 04:23:56.000000 tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2479 2021-07-03 05:50:30.000000 tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2483 2021-12-03 07:54:32.000000 tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.161196 tshirt-0.1.dev9/tshirt/parameters/reduction_parameters/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      456 2020-07-12 22:55:39.000000 tshirt-0.1.dev9/tshirt/parameters/reduction_parameters/example_reduction_parameters.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.161527 tshirt-0.1.dev9/tshirt/parameters/spec_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     4108 2021-04-30 04:13:31.000000 tshirt-0.1.dev9/tshirt/parameters/spec_params/default_params.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1847 2020-07-12 22:55:24.000000 tshirt-0.1.dev9/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1888 2020-07-13 07:19:44.000000 tshirt-0.1.dev9/tshirt/parameters/spec_params/example_spec_parameters.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.161624 tshirt-0.1.dev9/tshirt/parameters/spec_params/test_params/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2196 2021-03-29 20:26:21.000000 tshirt-0.1.dev9/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml
--rw-r--r--   0 everettschlawin   (501) staff       (20)       50 2020-07-12 22:57:46.000000 tshirt-0.1.dev9/tshirt/parameters/telluric_bands.yaml
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.162859 tshirt-0.1.dev9/tshirt/pipeline/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       56 2020-10-29 18:02:05.000000 tshirt-0.1.dev9/tshirt/pipeline/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    10465 2020-12-19 05:05:58.000000 tshirt-0.1.dev9/tshirt/pipeline/analysis.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3825 2021-09-30 04:43:40.000000 tshirt-0.1.dev9/tshirt/pipeline/fit_2dgauss.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.165500 tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       84 2021-12-17 05:29:57.000000 tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      766 2020-02-22 00:15:21.000000 tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/check_wavecal.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2542 2020-08-04 02:08:51.000000 tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/hst_inst_funcs.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1395 2021-03-28 04:41:20.000000 tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/jwst_inst_funcs.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     7545 2022-01-25 04:40:05.000000 tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/rowamp_sub.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    98652 2021-12-17 06:06:57.000000 tshirt-0.1.dev9/tshirt/pipeline/phot_pipeline.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    15131 2022-01-18 07:02:08.000000 tshirt-0.1.dev9/tshirt/pipeline/prep_images.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2764 2021-12-03 07:54:32.000000 tshirt-0.1.dev9/tshirt/pipeline/sim_data.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    99863 2021-10-13 03:38:12.000000 tshirt-0.1.dev9/tshirt/pipeline/spec_pipeline.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)    13318 2021-12-03 07:54:32.000000 tshirt-0.1.dev9/tshirt/pipeline/utils.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1446 2019-02-19 20:21:03.000000 tshirt-0.1.dev9/tshirt/quick_timeit.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      449 2020-06-14 23:28:01.000000 tshirt-0.1.dev9/tshirt/specific_fits.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.166182 tshirt-0.1.dev9/tshirt/tests/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     5527 2022-01-18 06:52:08.000000 tshirt-0.1.dev9/tshirt/tests/test_phot_algorithms.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2889 2021-10-14 22:43:01.000000 tshirt-0.1.dev9/tshirt/tests/test_pipe_basics.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      244 2021-12-03 07:54:32.000000 tshirt-0.1.dev9/tshirt/tests/test_rowamp_sub.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      957 2021-10-14 23:26:52.000000 tshirt-0.1.dev9/tshirt/tests/test_window_placement.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3232 2020-11-30 06:14:07.000000 tshirt-0.1.dev9/tshirt/tser_tests.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-01-25 05:23:15.159243 tshirt-0.1.dev9/tshirt.egg-info/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      956 2022-01-25 05:23:15.000000 tshirt-0.1.dev9/tshirt.egg-info/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2894 2022-01-25 05:23:15.000000 tshirt-0.1.dev9/tshirt.egg-info/SOURCES.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2022-01-25 05:23:15.000000 tshirt-0.1.dev9/tshirt.egg-info/dependency_links.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)       88 2022-01-25 05:23:15.000000 tshirt-0.1.dev9/tshirt.egg-info/requires.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        7 2022-01-25 05:23:15.000000 tshirt-0.1.dev9/tshirt.egg-info/top_level.txt
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.222730 tshirt-0.2/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       40 2017-01-16 05:08:31.000000 tshirt-0.2/.gitattributes
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1803 2021-07-03 05:50:30.000000 tshirt-0.2/.gitignore
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        0 2020-02-18 20:41:06.000000 tshirt-0.2/.gitmodules
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1073 2020-07-06 05:04:56.000000 tshirt-0.2/LICENSE
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       30 2020-09-13 03:03:55.000000 tshirt-0.2/MANIFEST.in
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      914 2023-04-24 16:35:14.222568 tshirt-0.2/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      758 2020-07-06 05:04:31.000000 tshirt-0.2/README.md
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.204801 tshirt-0.2/docs/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      634 2020-06-22 23:17:25.000000 tshirt-0.2/docs/Makefile
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2262 2022-06-19 02:43:46.000000 tshirt-0.2/docs/conf.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.204938 tshirt-0.2/docs/images/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   176987 2020-06-23 17:58:22.000000 tshirt-0.2/docs/images/t_shirt_logo.jpg
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1013 2022-01-18 07:12:31.000000 tshirt-0.2/docs/index.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3631 2022-01-18 07:20:02.000000 tshirt-0.2/docs/installation.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      795 2020-06-22 23:17:25.000000 tshirt-0.2/docs/make.bat
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      896 2020-11-08 04:57:30.000000 tshirt-0.2/docs/modules.rst
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.206859 tshirt-0.2/docs/phot_pipeline/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    37697 2020-07-12 04:40:36.000000 tshirt-0.2/docs/phot_pipeline/box_time_series_cookbook.ipynb
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      439 2020-07-12 04:40:36.000000 tshirt-0.2/docs/phot_pipeline/example_phot_param_file.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      397 2020-07-12 04:40:36.000000 tshirt-0.2/docs/phot_pipeline/phot_pipeline.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     5443 2022-07-31 20:21:48.000000 tshirt-0.2/docs/phot_pipeline/phot_pipeline_parameters.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1049 2021-03-29 20:26:21.000000 tshirt-0.2/docs/phot_pipeline/running_phot_pipeline.rst
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.207122 tshirt-0.2/docs/reduction/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      915 2021-02-18 21:10:57.000000 tshirt-0.2/docs/reduction/reduction.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      178 2020-06-23 18:40:40.000000 tshirt-0.2/docs/reduction/reduction_param.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       78 2020-12-07 06:50:34.000000 tshirt-0.2/docs/requirements.txt
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.209216 tshirt-0.2/docs/spec_pipeline/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   921939 2020-07-06 05:04:31.000000 tshirt-0.2/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2669 2020-07-12 04:40:36.000000 tshirt-0.2/docs/spec_pipeline/batch_processing.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     4557 2022-08-05 00:10:07.000000 tshirt-0.2/docs/spec_pipeline/parameter_file.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      481 2020-07-12 04:40:36.000000 tshirt-0.2/docs/spec_pipeline/spec_pipeline.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    34730 2020-07-13 07:19:44.000000 tshirt-0.2/docs/spec_pipeline/test_spec_pipeline.ipynb
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.210242 tshirt-0.2/docs/specific_modules/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    36491 2022-01-18 07:07:34.000000 tshirt-0.2/docs/specific_modules/ROEBA.ipynb
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      182 2022-01-18 07:09:23.000000 tshirt-0.2/docs/specific_modules/specific_modules.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       38 2023-04-24 16:35:14.222779 tshirt-0.2/setup.cfg
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      867 2022-12-01 09:32:17.000000 tshirt-0.2/setup.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.212542 tshirt-0.2/tshirt/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      118 2022-12-01 09:32:17.000000 tshirt-0.2/tshirt/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      212 2019-02-19 20:21:03.000000 tshirt-0.2/tshirt/allk1255_centroid.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.213405 tshirt-0.2/tshirt/chisquare/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.2/tshirt/chisquare/directory_placeholder.dat
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.213567 tshirt-0.2/tshirt/cleaned_tser/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      141 2019-02-19 20:21:03.000000 tshirt-0.2/tshirt/cleaned_tser/directory_placeholder.dat
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.214089 tshirt-0.2/tshirt/directory_info/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2261 2022-08-03 23:25:51.000000 tshirt-0.2/tshirt/directory_info/directory_list.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1081 2021-12-03 07:54:32.000000 tshirt-0.2/tshirt/directory_info/example_data_list.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      767 2019-02-19 20:21:03.000000 tshirt-0.2/tshirt/example_fits.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.199577 tshirt-0.2/tshirt/existing_dat/
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.214332 tshirt-0.2/tshirt/existing_dat/spectra/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      738 2019-02-19 20:21:03.000000 tshirt-0.2/tshirt/existing_dat/spectra/fratio_yang2016.csv
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2122 2019-02-19 20:21:03.000000 tshirt-0.2/tshirt/fit_models.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    52675 2020-06-14 23:10:48.000000 tshirt-0.2/tshirt/fit_tser_emcee.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     6638 2020-10-16 22:10:25.000000 tshirt-0.2/tshirt/mie_model.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.214645 tshirt-0.2/tshirt/parameters/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      308 2020-07-12 22:57:27.000000 tshirt-0.2/tshirt/parameters/fit_params.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.214833 tshirt-0.2/tshirt/parameters/mie_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      434 2020-07-12 22:57:38.000000 tshirt-0.2/tshirt/parameters/mie_params/simplePoly.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.215292 tshirt-0.2/tshirt/parameters/phot_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2385 2020-07-12 22:54:25.000000 tshirt-0.2/tshirt/parameters/phot_params/example_batch_phot.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3425 2021-08-17 21:22:42.000000 tshirt-0.2/tshirt/parameters/phot_params/example_phot_parameters.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      423 2020-07-12 22:53:44.000000 tshirt-0.2/tshirt/parameters/phot_params/keywords_for_phot_pipeline.csv
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.215893 tshirt-0.2/tshirt/parameters/phot_params/test_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2558 2021-04-13 04:23:56.000000 tshirt-0.2/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2924 2021-04-13 04:23:56.000000 tshirt-0.2/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2479 2021-07-03 05:50:30.000000 tshirt-0.2/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2483 2021-12-03 07:54:32.000000 tshirt-0.2/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.216115 tshirt-0.2/tshirt/parameters/reduction_parameters/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      456 2020-07-12 22:55:39.000000 tshirt-0.2/tshirt/parameters/reduction_parameters/example_reduction_parameters.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.216725 tshirt-0.2/tshirt/parameters/spec_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     4632 2023-02-10 07:04:53.000000 tshirt-0.2/tshirt/parameters/spec_params/default_params.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1847 2020-07-12 22:55:24.000000 tshirt-0.2/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1888 2020-07-13 07:19:44.000000 tshirt-0.2/tshirt/parameters/spec_params/example_spec_parameters.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.216892 tshirt-0.2/tshirt/parameters/spec_params/test_params/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2196 2021-03-29 20:26:21.000000 tshirt-0.2/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       50 2020-07-12 22:57:46.000000 tshirt-0.2/tshirt/parameters/telluric_bands.yaml
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.219977 tshirt-0.2/tshirt/pipeline/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       56 2020-10-29 18:02:05.000000 tshirt-0.2/tshirt/pipeline/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    10465 2020-12-19 05:05:58.000000 tshirt-0.2/tshirt/pipeline/analysis.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3825 2021-09-30 04:43:40.000000 tshirt-0.2/tshirt/pipeline/fit_2dgauss.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.220751 tshirt-0.2/tshirt/pipeline/instrument_specific/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       84 2021-12-17 05:29:57.000000 tshirt-0.2/tshirt/pipeline/instrument_specific/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      766 2020-02-22 00:15:21.000000 tshirt-0.2/tshirt/pipeline/instrument_specific/check_wavecal.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2542 2020-08-04 02:08:51.000000 tshirt-0.2/tshirt/pipeline/instrument_specific/hst_inst_funcs.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3344 2022-11-05 04:51:59.000000 tshirt-0.2/tshirt/pipeline/instrument_specific/jwst_inst_funcs.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    13115 2022-12-04 05:37:18.000000 tshirt-0.2/tshirt/pipeline/instrument_specific/rowamp_sub.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   102607 2023-03-03 08:13:25.000000 tshirt-0.2/tshirt/pipeline/phot_pipeline.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    15131 2022-01-18 07:02:08.000000 tshirt-0.2/tshirt/pipeline/prep_images.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2878 2022-07-09 15:42:59.000000 tshirt-0.2/tshirt/pipeline/sim_data.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)   112049 2023-03-20 05:37:33.000000 tshirt-0.2/tshirt/pipeline/spec_pipeline.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)    13318 2021-12-03 07:54:32.000000 tshirt-0.2/tshirt/pipeline/utils.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1446 2019-02-19 20:21:03.000000 tshirt-0.2/tshirt/quick_timeit.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      449 2020-06-14 23:28:01.000000 tshirt-0.2/tshirt/specific_fits.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.222252 tshirt-0.2/tshirt/tests/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     5527 2022-01-18 06:52:08.000000 tshirt-0.2/tshirt/tests/test_phot_algorithms.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2889 2021-10-14 22:43:01.000000 tshirt-0.2/tshirt/tests/test_pipe_basics.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      244 2021-12-03 07:54:32.000000 tshirt-0.2/tshirt/tests/test_rowamp_sub.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      957 2021-10-14 23:26:52.000000 tshirt-0.2/tshirt/tests/test_window_placement.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3232 2020-11-30 06:14:07.000000 tshirt-0.2/tshirt/tser_tests.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:35:14.213282 tshirt-0.2/tshirt.egg-info/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      914 2023-04-24 16:35:14.000000 tshirt-0.2/tshirt.egg-info/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2894 2023-04-24 16:35:14.000000 tshirt-0.2/tshirt.egg-info/SOURCES.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2023-04-24 16:35:14.000000 tshirt-0.2/tshirt.egg-info/dependency_links.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       98 2023-04-24 16:35:14.000000 tshirt-0.2/tshirt.egg-info/requires.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        7 2023-04-24 16:35:14.000000 tshirt-0.2/tshirt.egg-info/top_level.txt
```

### Comparing `tshirt-0.1.dev9/.gitignore` & `tshirt-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/LICENSE` & `tshirt-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/PKG-INFO` & `tshirt-0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: tshirt
-Version: 0.1.dev9
+Version: 0.2
 Summary: A package to analyze time series data, especially for exoplanets
 Home-page: https://github.com/eas342/tshirt
 Author: Everett Schlawin, Kayli Glidic
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 `tshirt` README
 ==========================================
 The Time Series Helper & Integration Reduction Tool `tshirt` is a general-purpose tool for time series science.
@@ -19,9 +17,7 @@
 - Reduce raw data: flat field, bias subtract, gain correct, etc. This has been demonstrated to work with merged CCD images from Mont4K imager on the Kuiper-61 inch on Mt Bigelow, AZ.
 - Extract Photometry
 - Extract Spectroscopy
 
 
 See the read-the-docs page for information on how to install and use `tshirt`:
 [https://tshirt.readthedocs.io/en/latest/](https://tshirt.readthedocs.io/en/latest/)
-
-
```

### Comparing `tshirt-0.1.dev9/README.md` & `tshirt-0.2/README.md`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/Makefile` & `tshirt-0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/conf.py` & `tshirt-0.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,8 +54,13 @@
 # a list of builtin themes.
 #
 html_theme = 'sphinx_rtd_theme'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ['_static']
+
+# Explicitly set the version of Python and its requirements
+# python:
+#   install:
+#     - requirements: docs/requirements.txt
```

### Comparing `tshirt-0.1.dev9/docs/images/t_shirt_logo.jpg` & `tshirt-0.2/docs/images/t_shirt_logo.jpg`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/index.rst` & `tshirt-0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/installation.rst` & `tshirt-0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/make.bat` & `tshirt-0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/modules.rst` & `tshirt-0.2/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/phot_pipeline/box_time_series_cookbook.ipynb` & `tshirt-0.2/docs/phot_pipeline/box_time_series_cookbook.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/phot_pipeline/phot_pipeline_parameters.rst` & `tshirt-0.2/docs/phot_pipeline/phot_pipeline_parameters.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 You will need to specify a list of files, source name and a list of source coordinates in pixels [x,y].
 The first source should be the target and the rest will be reference stars.
 The ``jdRef`` parameter specifies a reference epoch for time series plots.
 
 Source Aperture Photometry Geometry
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Specify the aperture geometry, sizes as well as the box finding size for locating sources. The options for geometry `srcGeometry` are "Circular" and "Rectangular".
+Specify the aperture geometry, aperture sizes, and the box finding size for locating sources. The options for geometry `srcGeometry` are "Circular", "Rectangular", and "CircularAnnulus". If using ``CircularAnnulus``, the inner and outer radii are set by the ``srcStart`` and the ``srcEnd`` keywords while ignoring ``apRadius``,  ``apHeight`` and ``apWidth``. If using ``Rectangular``, the ``apHeight`` and ``apWidth`` keywords are used to define the source aperture size while ignoring ``apRadius``,  ``srcStart`` and ``srcEnd``. 
 
 Background Aperture Photometry Geometry
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Specify the background aperture geometry (:code:`bkgGeometry`). You can use either ``CircularAnnulus`` or ``Rectangle``. If using ``CircularAnnulus``, the inner and outer radii are set by the ``backStart`` and the ``backEnd`` keywords, while ignoring ``backHeight`` and ``backWidth``. If using ``Rectangular``, the ``backHeight`` and ``backWidth`` keywords are used to define the background aperture size. Regardless of the geometry, the background aperture is always centered relative to the source aperture. The offset between background aperture and the source aperture is set by ``backOffset``, which is a 2 element list in the form of [DX, DY], where DX and DY are the offset in number of pixels.
 
 
-Background Aperture Photometry Geometry
+Background Subtraction Methods
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Specify the background method (:code:`bkgMethod`). The options are
    - "mean" (default). This calculates the mean background value per pixel and subtracts this from all source pixels
    - "median". This calculates the median background value value per pixel and subtracts this from all source pixels
    - "robust mean". This calculates the robust mean background value value per pixel and subtracts this from all source pixels.
-   - "colrow". This calculates a column-by-colum and/or row-by-row fit to the background. The parameters are similar to the :doc:`Spec Background Parameters </spec_pipeline/parameter_file>`. Specify the :code:`bkgOrderX`, :code:`bkgOrderY` for the polynomial orders of the fits. For example :code:`bkgOrderX: 1` for a linear fit. The order and which directions to be specified are in the :code:`bkgSubDirections` parameter. To do :code:`bkgSubDirections: ['Y','X']` would do the Y direction (column-by-column) first and then the X direction (row-by-row). :code:`bkgSubDirections: ['X']` would only do row-by-row subtraction.
+   - "colrow". This calculates a column-by-colum and/or row-by-row fit to the background. The parameters are similar to the :doc:`Spec Background Parameters </spec_pipeline/parameter_file>`. Specify the :code:`bkgOrderX`, :code:`bkgOrderY` for the polynomial orders of the fits. For example :code:`bkgOrderX: 1` for a linear fit. The order and which directions to be specified are in the :code:`backsub_directions` parameter. To do :code:`backsub_directions: ['Y','X']` would do the Y direction (column-by-column) first and then the X direction (row-by-row). :code:`backsub_directions: ['X']` would only do row-by-row subtraction.
    - "rowAmp". This is a somewhat JWST-specific code that will do row-by-row subtraction of the whole array (masking out sources) but treats each column individually. The sources are masked by making all pixels with a circle with radius :code:`backStart` from the source Nan and then using :code:`numpy.nanmedian()` to calculate the median of each row within a given amplifier. Mileage may vary if sources extend over an entire amplifier (512 pixels for JWST Stripe mode, also called 4 output amplifier mode).
 
 
 Fixed Aperture Sizes
 ~~~~~~~~~~~~~~~~~~~~~~~
-For the circular aperture ``apRadius``, ``apHeight`` and ``apWidth`` give the source radius, and the inner and outer radii of the background annulus. For a rectangular aperture, the ``apHeight`` and ``apWidth`` describe the height and width. These units are in pixels.
-
+For the circular aperture, ``apRadius`` gives the source radius, and ``backStart`` and ``backEnd`` give the inner and outer radii of the background annulus. For a rectangular aperture, the ``apHeight`` and ``apWidth`` describe the height and width of the source, and ``backHeight`` and ``backWidth`` describe the height and width of the background. These units are in pixels.
 
 Scaled Aperture Sizes
 ~~~~~~~~~~~~~~~~~~~~~~
 The apertures can be fixed for all images or be scaled with the FWHM using either ``scaleAperture: True`` or ``scaleAperture: False``. If true, specify the scaling factor. The source aperture will be the FWHM multiplied by the scaling factor 
 
 .. math::
 
@@ -54,9 +53,8 @@
 You can also specify an ``apRange`` parameter which sets the minimum and maximum allowed FWHM. This adds some robustness in the case the FWHM found is wacky - for example if clouds go over.
 
 
 Timing Method
 ~~~~~~~~~~~~~~~~~~~~~~
 The ``phot_pipeline`` will automatically find the JD time from the ``DATE-OBS`` and ``TIME-OBS`` keywords. However, if using JWST data, all the integrations are packed into a singel fits file with one ``DATE-OBS`` and ``TIME-OBS``. In this case, the data must be split into individual integrations, which are assigned an ``ON_INT`` keyword. If ``timineMethod`` is set to ``JWSTint``, then ``phot_pipeline`` will use the calculate integration times using ``TFRAME`` and ``INTTIME`` in the header.
 
-
-
+The parameter :code:`dateKeyword` will tell :code:`tshirt` to look for a specific FITS keyword for the date. Otherwise it searches common ones like :code:`DATE-OBS` or :code:`DATE_OBS`.
```

### Comparing `tshirt-0.1.dev9/docs/phot_pipeline/running_phot_pipeline.rst` & `tshirt-0.2/docs/phot_pipeline/running_phot_pipeline.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/reduction/reduction.rst` & `tshirt-0.2/docs/reduction/reduction.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb` & `tshirt-0.2/docs/spec_pipeline/CoRoT-1b_Example_Annotated_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/spec_pipeline/batch_processing.rst` & `tshirt-0.2/docs/spec_pipeline/batch_processing.rst`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/spec_pipeline/parameter_file.rst` & `tshirt-0.2/docs/spec_pipeline/parameter_file.rst`

 * *Files 23% similar despite different names*

```diff
@@ -54,7 +54,33 @@
     img, head = spec.get_default_im()
     imgSub, bkgModel, subHead = spec.do_backsub(img,head,directions=spec.param['bkgSubDirections'])
     profileList, smooth_img_list = spec.find_profile(imgSub,subHead,showEach=True)
     
 This will show you one profile fit at a time with the spline knots shown. You can step through each cross-dispersion pixel by pressing "c". When you are done, press "q" to quick the python debugger (pdb).
  
 
+waveCalMethod
+~~~~~~~~~~~~~~
+The method to turn the dispersion pixels into wavelengths.
+
+* :code:`None` When it is :code:`None` (:code:`null` in the YAML file), the wavelengths are equal to the pixel in microns (just as a placeholder)
+
+* :code:`NIRCamTSquickPoly` Quick polynomial fit to NIRCam grism time series from before flight measurement (use with caution)
+
+* :code:`wfc3Dispersion` Hubble Space Telescope Wide Field Camera 3 quick wavecal (use with caution)
+
+* :code:`quick_nrs_prism` Simple Polynomial fit to the NIRSpec prism using the jwst pipeline evaluated at Y=16 on 2022-07-15 (use with caution)
+
+* :code:`grismr_poly_dms` A polynomial fit to flight data from program 1076. Should be accurate to within a few angstroms for F322W2. F444W depends on where the target position lands after position adjustments.
+
+saveSpatialProfileStats
+~~~~~~~~~~~~~~~~~~~~~~~
+If True, save the spatial profile centroid and FWHM for de-trending from the median profile. If False, those are populated with NaN.
+
+profilePix
+~~~~~~~~~~
+If None, all dispersion pixels (along the wavelength direction) are used in calculating spatial profile statistics. If a 2 element list like :code:`[50,100]`, pixels 50 through 100 in the dispersion/wavelength direction will be used to measure the spatial profile statistics. Note that this only has an effect if :code:`saveSpatialProfileStats` is :code:`True` and this will not affect the extraction in current versions of tshirt. It will ony affect the saved profile statistics.
+
+useSmoothProfileForStats
+~~~~~~~~~~~~~~~~~~~~~~~~
+Use the smoothed profile for the profile statistics? If True, the statistics will be on the man profile along the dispersion direction. Otherwise, a median of the data is calculated. Note that if :code:`fixedProfile` is True, this will give constant statistics for all images
+
```

### Comparing `tshirt-0.1.dev9/docs/spec_pipeline/test_spec_pipeline.ipynb` & `tshirt-0.2/docs/spec_pipeline/test_spec_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/docs/specific_modules/ROEBA.ipynb` & `tshirt-0.2/docs/specific_modules/ROEBA.ipynb`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/setup.py` & `tshirt-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 with open("README.md", "r") as fh:
     ## skip the HTML, which doesn't work on PyPI
     long_description = "".join(fh.readlines()[4:])
 
 setup(
     name='tshirt',
-    version='0.1dev9',
+    version='0.2',
     author='Everett Schlawin, Kayli Glidic',
     packages=['tshirt','tshirt.pipeline',
               'tshirt.pipeline.instrument_specific'],
     url="https://github.com/eas342/tshirt",
     description="A package to analyze time series data, especially for exoplanets",
     include_package_data=True,
     install_requires=[
         "numpy>=1.15",
         "scipy>=1.1.0",
         "astropy>=2.0",
         "tqdm>=4.46.0",
         "photutils>=0.4.1",
         "bokeh>=1.4.0",
-        "pytest"
+        "pytest",
+        "celerite2"
     ],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `tshirt-0.1.dev9/tshirt/directory_info/directory_list.yaml` & `tshirt-0.2/tshirt/directory_info/directory_list.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 - diagnostics/variance_img/README.md
 - diagnostics/profile_fit/README.md
 - diagnostics/phot_poly_backsub/README.md
 - diagnostics/trimmed_flat/README.md
 - diagnostics/spec_backsub/README.md
 - diagnostics/rowamp_sub/README.md
+- diagnostics/spatial_profile/README.md
 - plots/directory_placeholder.dat
 - plots/individual_fits/directory_placeholder.dat
 - plots/model_parameter_explorations/directory_placeholder.dat
 - plots/photometry/postage_stamps/directory_placeholder.dat
 - plots/photometry/star_labels/directory_placeholder.dat
 - plots/photometry/tser_allstar/directory_placeholder.dat
 - plots/photometry/tser_refcor/directory_placeholder.dat
```

### Comparing `tshirt-0.1.dev9/tshirt/directory_info/example_data_list.txt` & `tshirt-0.2/tshirt/directory_info/example_data_list.txt`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/example_fits.py` & `tshirt-0.2/tshirt/example_fits.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/existing_dat/spectra/fratio_yang2016.csv` & `tshirt-0.2/tshirt/existing_dat/spectra/fratio_yang2016.csv`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/fit_models.py` & `tshirt-0.2/tshirt/fit_models.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/fit_tser_emcee.py` & `tshirt-0.2/tshirt/fit_tser_emcee.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/mie_model.py` & `tshirt-0.2/tshirt/mie_model.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/phot_params/example_batch_phot.yaml` & `tshirt-0.2/tshirt/parameters/phot_params/example_batch_phot.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/phot_params/example_phot_parameters.yaml` & `tshirt-0.2/tshirt/parameters/phot_params/example_phot_parameters.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml` & `tshirt-0.2/tshirt/parameters/phot_params/test_params/phot_param_k2_22_annulus.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml` & `tshirt-0.2/tshirt/parameters/phot_params/test_params/phot_param_k2_22_colrow.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml` & `tshirt-0.2/tshirt/parameters/phot_params/test_params/test_drifting_psf.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml` & `tshirt-0.2/tshirt/parameters/phot_params/test_params/test_rowamp_sub.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/spec_params/default_params.yaml` & `tshirt-0.2/tshirt/parameters/spec_params/default_params.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 backPreScreen: False ## Pre-screen the background for outliers before trying to fit?
 splineSpecFitOrder: 3 ## order of the Spline to fit along the dispersion direction (for profile & badpix)
 splineSigRej: 2 ## number of sigma to reject when fitting the Splines along dispersion direction
 splinePreScreen: False ## pre-screen the points going into spline fitting?
 splineFloor: null ## set a floor for spline fitting in logarithmic space or None to use 2X the read noise.
 sigForBadPx: 300 ## number of sigma difference from smoothed profile where to mark bad pixels
 numSplineKnots: 20 ## number of spline Knots when fitting the Splines along the dispersion direction
+nImgForProfile: 1 ## number of images to used to calculate a profile when the profile is fixed
 nanTreatment: 'leave' ## How to treat NaNs in image? 'zero' will set to 0, 'leave' will leave at NaN
 lowPassFreqCC: 0.99 ## Below this frequency, all information is included for cross-corr alignment analysis
 hiPassFreqCC: 0.015 ## Above this frequency, all information is included for cross-corr alignment analysis
 nOffsetCC: 20 ## maximum number of pixels for cross-correlation during alignment stage
 specShiftMultiplier: 1.0 ## this is a multiplier to shift the spectra an extra fraction
 waveCalMethod: null ## the wavelength calibration method (None/null, NIRCamTS, simGRISMC, wfc3Dispersion)
 waveCalOffset: 0.0 ## offset to the wavelength calibration, subtracted afterwards
@@ -50,7 +51,12 @@
 dispNoiseCorrelation: False ## Treat the read noise as correlated across spectral pixels?
 readNoiseCorrDispVal: 0.01 ## The value of read noise correlation in disp direction (if used)
 ignorePhotNoiseInCovariance: False ## a diagnostic parameter to see covariance weights w/ out photon noise
 superWeights: False ## Use (S/N)^2 to weight instead of optimal extraction
 fixedProfile: False ## Use a fixed profile for all images?
 readFromTshirtExamples: False ## read the data from T-shirt examples within the package? Use only for examples.
 saveRefRow: False ## save rows of reference pixels?
+dateKeyword: DATE-OBS ## default FITS keyword to find date/time information from
+DATE-OBS: None ## manually supply a DATE-OBS if nothing is available in the header
+saveSpatialProfileStats: False ## save the spatial profile stats
+profilePix: null ## the pixels to use in calculating the spatial profile statistics (not used in extraction)
+useSmoothProfileForStats: False ## use the spline-smoothed profile for profile statistics?
```

### Comparing `tshirt-0.1.dev9/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml` & `tshirt-0.2/tshirt/parameters/spec_params/example_batch_spec_parameters.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/spec_params/example_spec_parameters.yaml` & `tshirt-0.2/tshirt/parameters/spec_params/example_spec_parameters.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml` & `tshirt-0.2/tshirt/parameters/spec_params/test_params/basic_hst_spec.yaml`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/analysis.py` & `tshirt-0.2/tshirt/pipeline/analysis.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/fit_2dgauss.py` & `tshirt-0.2/tshirt/pipeline/fit_2dgauss.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/check_wavecal.py` & `tshirt-0.2/tshirt/pipeline/instrument_specific/check_wavecal.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/instrument_specific/hst_inst_funcs.py` & `tshirt-0.2/tshirt/pipeline/instrument_specific/hst_inst_funcs.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/phot_pipeline.py` & `tshirt-0.2/tshirt/pipeline/phot_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,16 @@
                          'subpixelMethod': 'exact','excludeList': None,
                          'dateFormat': 'Two Part','copyCentroidFile': None,
                          'bkgMethod': 'mean','diagnosticMode': False,
                          'bkgOrderX': 1, 'bkgOrderY': 1,'backsub_directions': ['Y','X'],
                          'readFromTshirtExamples': False,
                          'saturationVal': None, 'satNPix': 5, 'nanReplaceValue': 0.0,
                          'DATE-OBS': None,
-                         'driftFile': None
+                         'dateKeyword': 'DATE-OBS',
+                         'driftFile': None,
                          }
         
         
         for oneKey in defaultParams.keys():
             if oneKey not in self.param:
                 self.param[oneKey] = defaultParams[oneKey]
         
@@ -239,14 +240,18 @@
     def check_parameters(self):
         assert type(self.param['backOffset']) == list,"Background offset is not a list"
         assert len(self.param['backOffset']) == 2,'Background offset must by a 2 element list'
     
     def set_up_apertures(self,positions):
         if self.param['srcGeometry'] == 'Circular':
             self.srcApertures = CircularAperture(positions,r=self.param['apRadius'])
+            
+        elif self.param['srcGeometry'] == 'CircularAnnulus':
+            self.srcApertures = CircularAnnulus(positions,r_in=self.param['srcStart'],
+                                                    r_out=self.param['srcEnd'])
         elif self.param['srcGeometry'] == 'Square':
             self.srcApertures = RectangularAperture(positions,w=self.param['apRadius'],
                                                     h=self.param['apRadius'],theta=0)
         elif self.param['srcGeometry'] == 'Rectangular':
             self.srcApertures = RectangularAperture(positions,w=self.param['apWidth'],
                                                     h=self.param['apHeight'],theta=0)
         else:
@@ -360,19 +365,20 @@
         drift_dat.meta['Zero File'] = str(drift_dat['File'][refIndex])
         print("Saving Drift file to {}".format(outPath))
         drift_dat.write(outPath,overwrite=True,format='ascii.ecsv')
     
     
     def showStarChoices(self,img=None,head=None,custPos=None,showAps=False,
                         srcLabel=None,figSize=None,showPlot=False,
+                        allLabels=None,
                         apColor='black',backColor='black',
                         vmin=None,vmax=None,index=None,
                         labelColor='white',
                         xLim=None,yLim=None,
-                        txtOffset=20):
+                        txtOffset=20,diffImgIndex=None):
         """
         Show the star choices for photometry
         
         Parameters
         ------------------
         img : numpy 2D array, optional
             An image to plot
@@ -380,15 +386,17 @@
             header for image
         custPos : numpy 2D array or list of tuple coordinates, optional
             Custom positions
         showAps : bool, optional
             Show apertures rather than circle stars
         srcLabel : str or None, optional
             What should the source label be? The default is "src"
-        srcLabel : list or None, optional
+        allLabels : list of str
+            Names for all aperture labels. Must be the same length as the number of sources
+        figSize : list or None, optional
             Specify the size of the plot.
             This is useful for looking at high/lower resolution
         showPlot : bool
             Show the plot? If True, it will show, otherwise it is saved as a file
         apColor: str
             The color for the source apertures
         backColor: str
@@ -403,25 +411,31 @@
             Color for the text label for sources
         xLim: None or two element list
             Specify the minimum and maximum X for the plot. For example xLim=[40,60]
         yLim: None or two element list
             Specify the minimum and maximum Y for the plot. For example yLim=[40,60]
         txtOffset: float
             The X and Y offset to place the text label for a source
+        diffImgIndex: int
+            Choose a file index from which to subtract a reference image
         """
         fig, ax = plt.subplots(figsize=figSize)
         
         if index is None:
             index = self.get_default_index()
         
         if img is None:
             img, head = self.getImg(self.fileL[index])
         else:
             img_other, head = self.get_default_im(img=img,head=None)
         
+        if diffImgIndex is not None:
+            img2, head2 = self.getImg(self.fileL[diffImgIndex])
+            img = img - img2
+        
         if vmin is None:
             useVmin = np.nanpercentile(img,1)
         else:
             useVmin = vmin
         
         if vmax is None:
             useVmax = np.nanpercentile(img,99)
@@ -461,21 +475,24 @@
             ax.scatter(showApPos[:,0],showApPos[:,1], s=rad, facecolors='none', edgecolors='r')
             outName = 'st_labels_{}.pdf'.format(self.dataFileDescrip)
         
         for ind, onePos in enumerate(showApPos):
             
             #circ = plt.Circle((onePos[0], onePos[1]), rad, color='r')
             #ax.add_patch(circ)
-            if ind == 0:
-                if srcLabel is None:
-                    name='src'
+            if allLabels is None:
+                if ind == 0:
+                    if srcLabel is None:
+                        name='src'
+                    else:
+                        name=srcLabel
                 else:
-                    name=srcLabel
+                    name=str(ind)
             else:
-                name=str(ind)
+                name=allLabels[ind]
             ax.text(onePos[0]+txtOffset,onePos[1]+txtOffset,name,color=labelColor)
         
         ax.set_xlabel('X (px)')
         ax.set_ylabel('Y (px)')
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.05)
         fig.colorbar(imData,label='Counts',cax=cax)
@@ -483,14 +500,15 @@
         ax.set_xlim(xLim)
         ax.set_ylim(yLim)
         
         if showPlot == True:
             fig.show()
         else:
             outF = os.path.join(self.baseDir,'plots','photometry','star_labels',outName)
+            print("Saving plot to {}".format(outF))
             fig.savefig(outF,
                         bbox_inches='tight')
             plt.close(fig)
 
     def showStamps(self,img=None,head=None,custPos=None,custFWHM=None,
                    vmin=None,vmax=None,showPlot=False,boxsize=None,index=None):
         """
@@ -954,48 +972,52 @@
         
         A reminder to myself to write a script to clear the positions.
         Sometimes, if you get bad positions from a previous file, they 
         will wind up being used again. Need to reset the srcAperture.positions!
         """
     
     def get_date(self,head):
-        if 'DATE-OBS' in head:
-            useDate = head['DATE-OBS']
+        if self.param['dateKeyword'] in head:
+            useDate = head[self.param['dateKeyword']]
         elif 'DATE_OBS' in head:
             useDate = head['DATE_OBS']
         elif 'DATE' in head:
-            warnings.warn('DATE-OBS not found in header. Using DATE instead')
+            warnings.warn('{} not found in header. Using DATE instead'.format(self.param['dateKeyword']))
             month1, day1, year1 = head['DATE'].split("/")
             useDate = "-".join([year1,month1,day1])
         elif 'DATE-OBS' in self.param:
             warnings.warn('Using DATE-OBS from parameter file.')
             useDate = self.param['DATE-OBS']
         else:
             warnings.warn('Date headers not found in header. Making it nan')
             useDate = np.nan
         
         if self.param['dateFormat'] == 'Two Part':
             t0 = Time(useDate+'T'+head['TIME-OBS'])
         elif self.param['dateFormat'] == 'One Part':
             t0 = Time(useDate)
+        elif self.param['dateFormat'] == 'MJD':
+            t0 = Time(useDate,format='mjd')
+        elif self.param['dateFormat'] == 'JD':
+            t0 = Time(useDate,format='jd')
         else:
             raise Exception("Date format {} not understdood".format(self.param['dateFormat']))
         
         
         if 'timingMethod' in self.param:
             if self.param['timingMethod'] == 'JWSTint':
                 if 'INTTIME' in head:
                     int_time = head['INTTIME']
                 elif 'EFFINTTM' in head:
                     int_time = head['EFFINTTM']
                 else:
                     warnings.warn("Couldn't find inttime in header. Setting to 0")
                     int_time = 0
                 
-                t0 = t0 + (head['TFRAME'] + int_time) * (head['ON_NINT']) * u.second
+                t0 = t0 + (head['TFRAME'] + int_time) * (head['ON_NINT'] - 0.5) * u.second
             elif self.param['timingMethod'] == 'intCounter':
                 t0 = t0 + (head['ON_NINT']) * 1.0 * u.min ## placeholder to spread out time
         
         return t0
     
     def get_read_noise(self,head):
         if self.param['readNoise'] != None:
@@ -1392,15 +1414,15 @@
         fig : matplotlib figure object
             If the figure was created separately, use the input axis object
         showLegend : bool
             Show a legend?
         normReg: list with two items or None
             Relative region over which to fit a baseline and re-normalize. This only works on reference-corrected photometry for now
         doBin : float or None
-            The bin size if showing binned data. This only works on reference-corrected photometry for now
+            The bin size if showing binned data.
         doNorm : bool
             Normalize the individual time series?
         yLim:  List
             List of Y limit to show
         errBar : string or None
             Describes how error bars will be displayed. None=none, 'all'=every point,'one'=representative
         excludeSrc : List or None
@@ -1482,15 +1504,21 @@
                     yplot = yNorm - offset * oneSrc
                 else:
                     yplot = yFlux - offset * oneSrc
                 
                 ## To avoid repeat colors, switch to dashed lins
                 if oneSrc >= 10: linestyle='dashed'
                 else: linestyle= 'solid'
-                ax.plot(jdArr - jdRef,yplot,label=pLabel,linestyle=linestyle)
+
+                if doBin is not None:
+                    xplot, yplot2, yplot_err = do_binning(jdArr - jdRef,yplot,nBin=doBin)
+                else:
+                    xplot = jdArr - jdRef
+                    yplot2 = yplot
+                ax.plot(xplot,yplot2,label=pLabel,linestyle=linestyle)
         
             if head['SRCGEOM'] == 'Circular':
                 ax.set_title('Src Ap='+str(head['APRADIUS'])+',Back=['+str(head['BKGSTART'])+','+
                              str(head['BKGEND'])+']')
         ax.set_xlabel('JD - '+str(jdRef))
         ax.set_ylim(yLim[0],yLim[1])
         if doNorm == True:
@@ -1506,23 +1534,24 @@
         else:
             if refCorrect == True:
                 outName = 'tser_refcor/refcor_{}.pdf'.format(self.dataFileDescrip)
                 outPath = os.path.join(self.baseDir,'plots','photometry',outName)
             else:
                 outName = 'raw_tser_{}.pdf'.format(self.dataFileDescrip)
                 outPath = os.path.join(self.baseDir,'plots','photometry','tser_allstar',outName)
-            fig.savefig(outPath)
+            fig.savefig(outPath,bbox_inches='tight')
             plt.close(fig)
         
         HDUList.close()
         
         
     
     def print_phot_statistics(self,refCorrect=True,excludeSrc=None,shorten=False,
-                              returnOnly=False,removeLinear=True):
+                              returnOnly=False,removeLinear=True,
+                              startInd=0,endInd=15):
         """
         Print the calculated and theoretical noise as a table
                               
         Parameters
         ----------
         refCorrect: bool
             Use reference stars to correct target?
@@ -1536,50 +1565,69 @@
             Useful if analyzing the baseline befor transit, for example.
         returnOnly: bool
             If True, a table is returned.
             If False, a table is printed and another is returned
         
         removeLinear: bool
             Remove a linear trend from the data first?
+                              
+        startInd: int
+            If shorten is True, only uses a subset of the data starting with StartInd
+        
+        endInd: int
+            If shorten is True, only uses a subset of the data ending with endInd
+        
+        
         """
         HDUList = fits.open(self.photFile)
         photHDU = HDUList['PHOTOMETRY']
         photArr = photHDU.data
         head = photHDU.header
         timeArr = HDUList['TIME'].data
         errArr = HDUList['PHOT ERR'].data
         
         t = Table()
         if (head['NSOURCE'] == 1) & (refCorrect == True):
             warnings.warn('Only once source, so defaulting to refCorrect=False')
             refCorrect = False
         
         if shorten == True:
-            photArr = photArr[0:15,:]
-            nImg = 15
+            photArr = photArr[startInd:endInd,:]
+            errArr = errArr[startInd:endInd,:]
+            nImg = endInd - startInd
+            timeArr = timeArr[startInd:endInd]
         else:
             nImg = self.nImg
         
         if refCorrect == True:
             yCorrected, yCorrected_err = self.refSeries(photArr,errArr,
                                                         excludeSrc=excludeSrc)
             
             if removeLinear == True:
                 xNorm = (timeArr - np.min(timeArr))/(np.max(timeArr) - np.min(timeArr))
                 poly_fit = robust_poly(xNorm,yCorrected,1)
                 yCorrected = yCorrected / np.polyval(poly_fit,xNorm)
             
             if shorten == True:
-                yCorrected = yCorrected[0:15]
+                yCorrected = yCorrected[startInd:endInd]
             
             t['Stdev (%)'] = np.round([np.nanstd(yCorrected) * 100.],4)
             t['Theo Err (%)'] = np.round(np.nanmedian(yCorrected_err) * 100.,4)
             mad = np.nanmedian(np.abs(yCorrected - np.nanmedian(yCorrected)))
             t['MAD (%)'] = np.round(mad * 100.,4)
         else:
+            if removeLinear == True:
+                xNorm = (timeArr - np.min(timeArr))/(np.max(timeArr) - np.min(timeArr))
+                for oneSrc in np.arange(self.nsrc):
+                    y1 = photArr[:,oneSrc]
+                    poly_fit = robust_poly(xNorm,y1,1)
+                    yDetrended= y1 / np.polyval(poly_fit,xNorm)
+                    photArr[:,oneSrc] = yDetrended
+                    errArr[:,oneSrc] = errArr[:,oneSrc] / np.polyval(poly_fit,xNorm)
+            
             t['Source #'] = np.arange(self.nsrc)
             medFlux = np.nanmedian(photArr,axis=0)
             t['Stdev (%)'] = np.round(np.nanstd(photArr,axis=0) / medFlux * 100.,4)
             t['Theo Err (%)'] = np.round(np.nanmedian(errArr,axis=0) / medFlux * 100.,4)
             tiledFlux = np.tile(medFlux,[nImg,1])
             mad = np.nanmedian(np.abs(photArr - tiledFlux),axis=0) / medFlux
             t['MAD (%)'] = np.round(mad * 100.,4)
@@ -1601,15 +1649,18 @@
         
         jdHDU = HDUList['TIME']
         jdArr = jdHDU.data
         t = jdArr - np.round(np.min(jdArr))
         timeHead = jdHDU.header
         
         cenData = HDUList['CENTROIDS'].data
-        fwhmData = HDUList['FWHM'].data
+        if 'FWHM' in HDUList:
+            fwhmData = HDUList['FWHM'].data
+        else:
+            fwhmData = np.zeros_like(cenData) * np.nan
         
         backData = HDUList['BACKG PHOT'].data
         
         fig, axArr = plt.subplots(7,sharex=True)
         yCorr, yCorr_err = self.refSeries(photArr,errArr,excludeSrc=excludeSrc)
         axArr[0].plot(t,yCorr)
         axArr[0].set_ylabel('Ref Cor F')
@@ -2261,58 +2312,86 @@
     xmax = img.shape[1] - 1
     ymax = img.shape[0] - 1
     out_x = np.minimum(np.maximum(xCoord,0),xmax)
     out_y = np.minimum(np.maximum(yCoord,0),ymax)
 
     return out_x,out_y
 
-def do_binning(x,y,nBin=20):
+def do_binning(x,y,nBin=20,yerr=None,returnXwidth=False):
     """
     A function that uses scipy binned_statistic to bin data
     
     It also calculates the standard error in each bin,
     which can be used as an error estimate
     
     Parameters
     --------------
     x: numpy array
         Independent variable for use in assigning data to bins
     y: numpy array
         Dependent variable to be binned
-    
+    yerr: numpy array (optional)
+        The error on the y points
+    nBin: int or numpy array
+        The number of bins or else the bin array
+    returnXwidth: bool
+        Return the X widths?
+        
     Returns
     -------------
     3 item tuple:
     xBin, yBin, yStd
     
     xBin: numpy array
         Middles of the bins
     yBin: numpy array
         mean value in bin
     yStd: numpy array
-        standard error of each bin
+        If yerr supplied,standard error of each bin
+        If yerr not supplied, the standard deviation of each bin
+    xWidth: numpy array
+        The x widths? If returnXwidth is True
     """
     yBins = Table()
     for oneStatistic in ['mean','std','count']:
         yBin, xEdges, binNum = binned_statistic(x,y,
                                                 statistic=oneStatistic,bins=nBin)
         yBins[oneStatistic] = yBin
 
-    ## Standard error in the mean
-    stdErrM = yBins['std'] / np.sqrt(yBins['count'])
+    if yerr is not None:
+        weights = 1./yerr**2
+        wSum, xEdges, binNum = binned_statistic(x,weights * y,
+                                                statistic='sum',bins=nBin)
+        sumW, xEdges, binNum = binned_statistic(x,weights,
+                                                statistic='sum',bins=nBin)
+        yWAvg = wSum/sumW
+        yWAvg_err = 1./np.sqrt(sumW)
+
+
     xShow = (xEdges[:-1] + xEdges[1:])/2.
-    yShow = yBins['mean']
-    yErrShow = stdErrM
+    xWidth = xEdges[1:] - xEdges[:-1]
+    if yerr is None:
+        stdErrM = yBins['std'] / np.sqrt(yBins['count'])
+        ## Standard error in the mean
+        yErrShow = stdErrM
+        yShow = yBins['mean']
+    else:
+        yShow = yWAvg
+        yErrShow = yWAvg_err
 
-    return xShow, yShow, yErrShow
+    if returnXwidth == True:
+        return xShow, yShow, yErrShow, xWidth
+    else:
+        return xShow, yShow, yErrShow
 
 def allan_variance(x,y,yerr=None,removeLinear=False,yLim=[None,None],
                    binMin=50,binMax=2000,customShortName=None,
                    logPlot=True,clip=False,xUnit='min',
-                   yUnit='ppm',showPlot=False):
+                   yUnit='ppm',showPlot=False,custTitle=None,
+                   nBinSequence=20):
     """
     Make an Allan Variance plot for a time series
     to see if it bins as sqrt(N) statistics
     
     Parameters
     ------------
     x: numpy array
@@ -2326,22 +2405,26 @@
         Name for file
     yLim: 2 element list
         Specify custom Y values for the plot
     binMin: int
         Bin size for the smallest # of bins
     binMax: int
         Bin size for the largest # of bins
+    nBinSequence: int
+        Number of bins to cycle through in sequence
     removeLinear: bool
         Remove a linear trend from the time series first?
     clip: bool
         Clip the first few points?
     xUnit: str
         Name of units for X axis of input series
     yUnit: str
         Name of units for Y axis to be binned
+    custTitle: str or None
+        Custom title name. If None, will generate one automatically
     showPlot: bool
         Render the plot with matplotlib? If False, it is saved instead.
     """
 
     if clip == True:
         x = x[2:]
         y = y[2:]
@@ -2355,15 +2438,20 @@
         y = y / ymod
     
     if yUnit == 'ppm':
         y = y * 1e6
         yerr = yerr * 1e6
     nPt = len(y)
     
-    logBinNums = np.linspace(np.log10(binMin),np.log10(binMax),20)
+    maxAllowedBinNumber = len(x) // 2
+    if (binMax > maxAllowedBinNumber):
+        warnings.warn("Maximum number of bins is greater than the number of points. Setting binMax to {}".format(maxAllowedBinNumber))
+        binMax = maxAllowedBinNumber
+    
+    logBinNums = np.linspace(np.log10(binMin),np.log10(binMax),nBinSequence)
     binNums = np.array(10**logBinNums,dtype=np.int)
     
     binSizes, stds, theoNoise, wNoise = [], [], [], []
     
     if yerr is not None:
         theoNoiseNoBin = np.median(yerr)
     else:
@@ -2387,27 +2475,32 @@
     binSizes.append(cadence)
     theoNoise.append(theoNoiseNoBin)
     wNoise.append(whiteNoiseStart)
 
 
     ## only Use finite values (ignore NaNs where binning isn't possible)
     usePts = np.isfinite(stds)
-
+    #pdb.set_trace()
     fig, ax = plt.subplots(figsize=(5,4))
     if logPlot == True:
         ax.loglog(np.array(binSizes)[usePts],np.array(stds)[usePts],label='Measured')
     else:
         ax.semilogx(np.array(binSizes)[usePts],np.array(stds)[usePts],label='Measured')
     ax.plot(binSizes,theoNoise,label='Read + Photon Noise')
     ax.plot(binSizes,wNoise,label='White noise scaling')
     ax.set_xlabel('Bin Size ({})'.format(xUnit))
     ax.set_ylabel(r'$\sigma$ ({})'.format(yUnit))
     ax.set_ylim(yLim)
     ax.legend()
-    ax.set_title("Allan Variance (Linear De-trend = {})".format(removeLinear))
+    if custTitle is None:
+        thisTitle = "Allan Variance (Linear De-trend = {})".format(removeLinear)
+    else:
+        thisTitle = custTitle
+    
+    ax.set_title(thisTitle)
     outName = 'all_var_{}_removelinear_{}.pdf'.format(customShortName,removeLinear)
     
     baseDir = get_baseDir()
     outPath = os.path.join(baseDir,'plots','allan_variance',outName)
     if showPlot == True:
         fig.show()
     else:
```

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/prep_images.py` & `tshirt-0.2/tshirt/pipeline/prep_images.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/sim_data.py` & `tshirt-0.2/tshirt/pipeline/sim_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import sys
 import os
 from pkg_resources import resource_filename
 import matplotlib.pyplot as plt
 import glob
 from photutils import CircularAperture, CircularAnnulus
 from photutils import RectangularAperture
-from photutils import centroid_2dg, aperture_photometry
+from photutils import aperture_photometry
+if photutils.__version__ > "1.0":
+    from photutils.centroids import centroid_2dg
+else:
+    from photutils import centroid_2dg
 import photutils
 import numpy as np
 from astropy.time import Time
 import astropy.units as u
 import pdb
 from copy import deepcopy
 import yaml
```

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/spec_pipeline.py` & `tshirt-0.2/tshirt/pipeline/spec_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     from bokeh.models import WheelZoomTool
     from bokeh.palettes import Dark2_5 as palette
     # itertools handles the cycling
     import itertools
 except ImportError as err2:
     print("Could not import bokeh plotting. Interactive plotting may not work")
 
+try:
+    from astropy.modeling import models, fitting
+except ImportError as err3:
+    print("Could not import astropy modeling for spatial profiles")
+
 from . import phot_pipeline
 from . import utils
 from . import instrument_specific
 
 path_to_example = "parameters/spec_params/example_spec_parameters.yaml"
 exampleParamPath = pkg_resources.resource_filename('tshirt',path_to_example)
 
@@ -222,22 +227,49 @@
                 #     for oneDepth in np.arange(depth):
                 #         value = value[0]
                 # if type(value) == list:
                 #     self.paramLists.append(oneKey)
                 #     self.counts.append(len(self.batchParam[oneKey]))
         return header
     
+    def get_median_img(self,nImg):
+        """
+        Calculate the median image fron n images
+
+        Parameters
+        ----------
+        nImg: int
+            Number of images to use for the profile
+        """
+        nSpacing = self.nImg // nImg
+        indToUse = np.arange(0,self.nImg,nSpacing)
+        nUsed = len(indToUse)
+        img, head = self.get_default_im()
+        all_img = np.zeros([nUsed,img.shape[0],img.shape[1]])
+        
+        for count,oneInd in enumerate(indToUse):
+            oneImgName = self.fileL[oneInd]
+            img2, head2 = self.getImg(oneImgName)
+            all_img[count,:,:] = img2
+        medImg = np.median(all_img,axis=0)
+        return medImg, head
+
+
     def do_extraction(self,useMultiprocessing=False):
         """
         Extract all spectroscopy
         """
         fileCountArray = np.arange(self.nImg)
         
         if self.param['fixedProfile'] == True:
-            img, head = self.get_default_im()
+            if (self.nImg > self.param['nImgForProfile']) & (self.param['nImgForProfile'] > 1):
+                img, head = self.get_median_img(self.param['nImgForProfile'])
+            else:
+                img, head = self.get_default_im()
+            
             imgSub, bkgModel, subHead = self.do_backsub(img,head,saveFits=False,
                                                         directions=self.param['bkgSubDirections'])
             profileList, smooth_img_list = self.find_profile(imgSub,subHead,saveFits=True,masterProfile=True)
             
             if (self.param['readNoiseCorrelation'] == True):
                 ## Only run the read noise inverse covariance matrix scheme once for fixed profile
                 
@@ -275,25 +307,33 @@
         optSpec_err = np.zeros_like(optSpec)
         sumSpec = np.zeros_like(optSpec)
         sumSpec_err = np.zeros_like(optSpec)
         backSpec = np.zeros_like(optSpec)
         
         refRows = np.zeros([self.nImg,nDisp]) * np.nan
         
+        cenArr = np.zeros([self.nsrc,self.nImg]) * np.nan
+        fwhmArr = np.zeros([self.nsrc,self.nImg]) * np.nan
+        
         for ind in fileCountArray:
             specDict = outputSpec[ind]
             timeArr.append(specDict['t0'].jd)
             optSpec[:,ind,:] = specDict['opt spec']
             optSpec_err[:,ind,:] = specDict['opt spec err']
             sumSpec[:,ind,:] = specDict['sum spec']
             sumSpec_err[:,ind,:] = specDict['sum spec err']
             backSpec[:,ind,:] = specDict['back spec']
             if 'ref row' in specDict:
                 refRows[ind,:] = specDict['ref row']
             airmass.append(specDict['airmass'])
+            
+            if 'cen' in specDict:
+                cenArr[:,ind] = specDict['cen']
+            if 'fwhm' in specDict:
+                fwhmArr[:,ind] = specDict['fwhm']
                 
         
         hdu = fits.PrimaryHDU(optSpec)
         hdu.header['NSOURCE'] = (self.nsrc,'Number of sources with spectroscopy')
         hdu.header['NIMG'] = (self.nImg,'Number of images')
         hdu.header['AXIS1'] = ('disp','dispersion axis')
         hdu.header['AXIS2'] = ('image','image axis')
@@ -335,19 +375,38 @@
         ## Save the mean refence pixel rows
         hduRef = fits.ImageHDU(refRows)
         hduRef.header['AXIS1'] = ('X','Image X axis')
         hduRef.header['AXIS2'] = ('image', 'image axis, ie. which integration')
         hduRef.header['BUNIT'] = ('counts', 'should be e- if gain has been applied')
         hduRef.header['VAL'] = ('Mean','Each pixel is the mean of the 4 bottom reference pixels')
         hduRef.name = 'REFPIX'
-         
+        
+        ## Save the wavelength array
+        hduWave = fits.ImageHDU(self.wavecal(dispPixelArr,head=exHeader))
+        hduWave.header['AXIS1'] = ('wavelength','wavelength (microns)')
+        hduWave.header['BUNIT'] = ('microns','wavelength unit')
+        hduWave.name = 'WAVELENGTH'
+        
+        ## Save the spatial centroid
+        hduCen = fits.ImageHDU(cenArr)
+        hduCen.header['AXIS1'] = ('image','spatial / time axis')
+        hduCen.header['AXIS2'] = ('src','source axis for multiple sources')
+        hduCen.header['BUNITS'] = ('px', 'pixels in spatial direction')
+        hduCen.name = 'CENTROID'
+        
+        hduFWHM = fits.ImageHDU(fwhmArr)
+        hduFWHM.header['AXIS1'] = ('image','spatial / time axis')
+        hduFWHM.header['AXIS2'] = ('src','source axis for multiple sources')
+        hduFWHM.header['BUNITS'] = ('px', 'pixels in spatial direction')
+        hduFWHM.name = 'FWHM'
+        
         HDUList = fits.HDUList([hdu,hduOptErr,hduSum,hduSumErr,
                                 hduBack,hduDispIndices,
                                 hduTime,hduFileNames,hduOrigHeader,
-                                hduRef])
+                                hduRef,hduWave,hduCen,hduFWHM])
         HDUList.writeto(self.specFile,overwrite=True)
         
     
     def backsub_oneDir(self,img,head,oneDirection,saveFits=False,
                        showEach=False,ind=None,custPrefix=None):
         """
         Do the background subtraction in a specified direction
@@ -913,14 +972,16 @@
         
         optSpectra = np.zeros([self.nsrc,nDisp])
         optSpectra_err = np.zeros_like(optSpectra)
         sumSpectra = np.zeros_like(optSpectra)
         sumSpectra_err = np.zeros_like(optSpectra)
         backSpectra = np.zeros_like(optSpectra)
         
+        cenInfo = np.zeros([self.nsrc])
+        fwhmInfo = np.zeros([self.nsrc])
         
         for oneSrc in np.arange(self.nsrc):
             profile_img = profile_img_list[oneSrc]
             smooth_img = smooth_img_list[oneSrc]
             
             ## Find the bad pixels and their missing weights
             finitep = (np.isfinite(img) & np.isfinite(varImg) & np.isfinite(smooth_img))
@@ -1027,25 +1088,80 @@
                     weightName = ''
                 
                 weightName = '{}_weights{}.fits'.format(prefixName,weightName)
                 weightPath = os.path.join(self.baseDir,'diagnostics','variance_img',weightName)
                 primHDU = fits.PrimaryHDU(weight2D)
                 primHDU.writeto(weightPath,overwrite=True)
             
+            if self.param['saveSpatialProfileStats'] == True:
+                ## get the centroid and FWHM info
+                if self.param['profilePix'] == None:
+                    profDispStart_0 = self.param['dispPixels'][0]
+                    profDispEnd_0 = self.param['dispPixels'][1]
+                else:
+                    profDispStart_0 = self.param['profilePix'][0]
+                    profDispEnd_0 = self.param['profilePix'][1]
+                
+                profDispStart = profDispStart_0 + self.dispOffsets[oneSrc]
+                profDispEnd = profDispEnd_0 + self.dispOffsets[oneSrc]
+                
+                profilePix = ((dispIndices > profDispStart) &
+                             (dispIndices <= profDispEnd))
+                
+                oneSourcePos = self.param['starPositions'][oneSrc]
+                startSpatial = int(oneSourcePos - self.param['apWidth'] / 2.)
+                endSpatial = int(oneSourcePos + self.param['apWidth'] / 2.)
+                spatial_var = np.arange(startSpatial,endSpatial) ## independent variable
+                
+                if self.param['useSmoothProfileForStats'] == True:
+                    if self.param['dispDirection'] == 'x':
+                        spatial_profile = np.nanmean(profile_img[startSpatial:endSpatial,profilePix],axis=1)
+                    else:
+                        spatial_profile = np.nanmean(profile_img[profilePix,startSpatial:endSpatial],axis=0)
+                else:
+                    if self.param['dispDirection'] == 'x':
+                        spatial_profile = np.nanmedian(imgSub[startSpatial:endSpatial,profilePix],axis=1)
+                    else:
+                        spatial_profile = np.nanmedian(imgSub[profilePix,startSpatial:endSpatial],axis=0)
+                
+                fitter = fitting.LevMarLSQFitter()
+                ampGuess = np.max(spatial_profile) - np.min(spatial_profile)
+                meanGuess = np.median(spatial_var)
+                gauss1d = models.Gaussian1D(amplitude=ampGuess, mean=meanGuess, stddev=3)
+                line_orig = models.Linear1D(slope=0.0, intercept=np.min(spatial_profile))
+                comb_gauss = line_orig + gauss1d
+                fitted_model = fitter(comb_gauss, spatial_var,spatial_profile, maxiter=111)
+                cenInfo[oneSrc] = fitted_model.mean_1.value
+                fwhmInfo[oneSrc] = fitted_model.stddev_1.value * 2.35
+                if saveFits == True:
+                    fig, ax = plt.subplots()
+                    ax.plot(spatial_var,spatial_profile,label='data')
+                    ax.plot(spatial_var,fitted_model(spatial_var),label='Model')
+                    spat_profile_name = 'spatial_prof_{}_src_{}.pdf'.format(prefixName,oneSrc)
+                    spatial_prof_path = os.path.join(self.baseDir,'diagnostics','spatial_profile',spat_profile_name)
+                    ax.legend()
+                    ax.set_title('Cen={}, FWHM={}'.format(cenInfo[oneSrc],fwhmInfo[oneSrc]))
+                    print("Saving spatial profile to {}".format(spatial_prof_path))
+                    fig.savefig(spatial_prof_path)
+                    plt.close(fig)
         
         extractDict = {} ## spectral extraction dictionary
         extractDict['t0'] = t0
         extractDict['disp indices'] = dispIndices
         extractDict['opt spec'] = optSpectra
         extractDict['opt spec err'] = optSpectra_err
         extractDict['sum spec'] = sumSpectra
         extractDict['sum spec err'] = sumSpectra_err
         extractDict['back spec'] = backSpectra
         extractDict['airmass'] = airmass
         
+        if self.param['saveSpatialProfileStats'] == True:
+            extractDict['cen'] = cenInfo
+            extractDict['fwhm'] = fwhmInfo
+        
         if self.param['saveRefRow'] == True:
             refRow = np.mean(img[0:4,:],axis=0)
             extractDict['ref row'] = refRow
         
         return extractDict
     
     def norm_spec(self,x,y,numSplineKnots=None,srcInd=0):
@@ -1311,15 +1427,16 @@
     
     def dyn_specFile(self,src=0):
         return "{}_src_{}.fits".format(self.dyn_specFile_prefix,src)
         
     def plot_dynamic_spec(self,src=0,saveFits=True,specAtTop=True,align=False,
                           alignDiagnostics=False,extraFF=False,
                           specType='Optimal',showPlot=False,
-                          vmin=None,vmax=None):
+                          vmin=None,vmax=None,flipX=False,
+                          waveCal=False):
         """
         Plots a dynamic spectrum of the data
         
         Parameters
         -----------
         showPlot: bool, optional
             Show the plot in addition to saving?
@@ -1337,14 +1454,18 @@
             Spectrum type - 'Optimal' or 'Sum'
         showPlot: bool
             Show a plot with the spectrum?
         vmin: float or None
             Value minimum for dynamic spectrum image
         vmax: float or None
             Value maximum for dynamic spectrum image
+        flipX: bool
+            Flip the X axis?
+        waveCal: bool
+            Calibrate the dispersion to wavelength?
         """
         if os.path.exists(self.specFile) == False:
             raise Exception("No spectrum file found. Run extraction first...")
         
         HDUList = fits.open(self.specFile)
         if specType == 'Optimal':
             extSpec = HDUList['OPTIMAL SPEC'].data[src]
@@ -1418,50 +1539,77 @@
             
             avgHDU = fits.ImageHDU(avgSpec)
             avgHDU.name = 'AVG SPEC'
             
             avgErrHDU = fits.ImageHDU(avgSpec_err)
             avgErrHDU.name = 'AVG SPEC ERR'
             
-
-                
+            ## Save the wavelength array
+            hduWave = fits.ImageHDU(self.wavecal(waveIndices))
+            hduWave.header['AXIS1'] = ('wavelength','wavelength (microns)')
+            hduWave.header['BUNIT'] = ('microns','wavelength unit')
+            hduWave.name = 'WAVELENGTH'
             
             ## Expect a card-too-long warning
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", message= "Card is too long, comment will be truncated")
-                outHDUList = fits.HDUList([dynHDU,dynHDUerr,dispHDU,timeHDU,offsetHDU,avgHDU, avgErrHDU])
+                outHDUList = fits.HDUList([dynHDU,dynHDUerr,dispHDU,timeHDU,offsetHDU,avgHDU, avgErrHDU, hduWave])
                 if align == True:
                     if specType == 'Optimal':
                         alignedHDU = fits.ImageHDU(useSpec,HDUList['OPTIMAL SPEC'].header)
                     else:
                         alignedHDU = fits.ImageHDU(useSpec,HDUList['SUM SPEC'].header)
                     ## Save the aligned spectra
                     outHDUList.append(alignedHDU)
                 outHDUList.writeto(self.dyn_specFile(src),overwrite=True)
         
         if specAtTop == True:
             fig, axArr = plt.subplots(2, sharex=True,gridspec_kw={'height_ratios': [1, 3]})
             axTop = axArr[0]
-            axTop.plot(waveIndices,avgSpec)
+            if waveCal == True:
+                x_spec = self.wavecal(waveIndices)
+            else:
+                x_spec = waveIndices
+            
+            axTop.plot(x_spec,avgSpec)
             ax = axArr[1]
         else:
             fig, ax = plt.subplots()
         
         if vmin is None:
             vmin=0.95
         if vmax is None:
             vmax=1.05
         
-        imShowData = ax.imshow(dynamicSpec,vmin=vmin,vmax=vmax)
-        ax.invert_yaxis()
+        if waveCal == True:
+            all_waves = self.wavecal(waveIndices)
+            extent = [all_waves[0],all_waves[-1],0,dynamicSpec.shape[0]]
+        else:
+            extent = None
+        
+        imShowData = ax.imshow(dynamicSpec,vmin=vmin,vmax=vmax,origin='lower',
+                               extent=extent)
         ax.set_aspect('auto')
-        ax.set_xlabel('Disp (pixels)')
+        if waveCal == True:
+            ax.set_xlabel('Wavelength ($\mu$m)')
+        else:
+            ax.set_xlabel('Disp (pixels)')
+        
         ax.set_ylabel('Time (Image #)')
         dispPix = np.array(self.param['dispPixels']) + self.dispOffsets[src]
-        ax.set_xlim(dispPix[0],dispPix[1])
+        if waveCal == True:
+            disp_X = self.wavecal(dispPix)
+        else:
+            disp_X = dispPix
+        
+        if flipX == True:
+            ax.set_xlim(disp_X[1],disp_X[0])
+        else:
+            ax.set_xlim(disp_X[0],disp_X[1])
+        
         fig.colorbar(imShowData,label='Normalized Flux')
         if specAtTop == True:
             ## Fix the axes to be the same
             pos = ax.get_position()
             pos2 = axTop.get_position()
             axTop.set_position([pos.x0,pos2.y0,pos.width,pos2.height])
             
@@ -1473,47 +1621,96 @@
         if showPlot == True:
             fig.show()
         else:
             plt.close(fig)
         
         HDUList.close()
     
-    def plot_noise_spectrum(self,src=0,showPlot=True,yLim=None):
+    def plot_noise_spectrum(self,src=0,showPlot=True,yLim=None,
+                            startInd=0,endInd=None,waveCal=False,
+                            waveBin=False,nbins=10,
+                            returnNoiseSpec=False):
         """
         Plot the Noise Spectrum from the Dynamic Spectrum
         
         Parameters
         ----------
         src: int
             Index number for the source
         showPlot: bool
             Show a plot in backend?
         yLim: list or None
             Specify the y limits
+        startInd: int
+            Starting time index to use
+        endInd: int or None
+            Ending index to use. None will use all
+        
+        waveCal: bool
+            Wavelength calibrate the dispersion pixel
+                            
+        waveBin: bool
+            Bin the wavelengths ?
+        nbins: int
+            How many wavelength bins should be used?
+        
+        returnNoiseSpec: bool
+            Return the noise spectrum? If True, an astropy table is returned
         """
         fig, ax = plt.subplots()
-        HDUList = fits.open(self.dyn_specFile(src))
-        x = HDUList['DISP INDICES'].data
-        y = np.nanstd(HDUList['DYNAMIC SPEC'].data,axis=0)
-        theo_y = np.nanmedian(HDUList['DYN SPEC ERR'].data,axis=0)
-        ax.plot(x,y * 100.,label='Measured noise')
-        ax.plot(x,theo_y * 100.,label='Theoretical noise')
-        ax.set_xlabel("Disp Pixel")
+        
+        if waveBin == True:
+            res = self.print_noise_wavebin(nbins=nbins,startInd=startInd,endInd=endInd)
+            if waveCal == True:
+                x_plot = res['Wave (mid)']
+            else:
+                x_plot = res['Disp Mid']
+            y = res['Stdev (%)'] / 100.
+            theo_y = res['Theo Err (%)'] / 100.
+        else:
+            HDUList = fits.open(self.dyn_specFile(src))
+            x = HDUList['DISP INDICES'].data
+            if waveCal == True:
+                x_plot = self.wavecal(x)
+            else:
+                x_plot = x
+            
+            y = np.nanstd(HDUList['DYNAMIC SPEC'].data[startInd:endInd,:],axis=0)
+            
+            theo_y = np.nanmedian(HDUList['DYN SPEC ERR'].data[startInd:endInd,:],axis=0)
+        
+        if waveCal == True:
+            xLabel = 'Wavelength ($\mu$m)'
+        else:
+            xLabel = "Disp Pixel"
+        
+        ax.plot(x_plot,y * 100.,label='Measured noise')
+        ax.plot(x_plot,theo_y * 100.,label='Theoretical noise')
+        ax.set_xlabel(xLabel)
         ax.set_ylabel("Noise (%)")
         if yLim is not None:
             ax.set_ylim(yLim[0],yLim[1])
         ax.legend()
         
         if showPlot == True:
             fig.show()
         else:
             outName = 'noise_spec_{}.pdf'.format(self.dataFileDescrip)
             outPath = os.path.join(self.baseDir,'plots','spectra','noise_spectrum',outName)
             print("Writing noise spectrum to {}".format(outPath))
             fig.savefig(outPath,overwrite=True)
+        if waveBin == False:
+            HDUList.close()
+        
+        if returnNoiseSpec == True:
+            t = Table()
+            t['x'] = x_plot
+            t['y'] = y
+            t['theo_y'] = theo_y
+            return t
     
     def plot_spec_offsets(self,src=0):
         if os.path.exists(self.dyn_specFile(src)) == False:
             self.plot_dynamic_spec(src=src,saveFits=True)
         HDUList = fits.open(self.dyn_specFile(src))
         time = HDUList['TIME'].data
         specOffset = HDUList['SPEC OFFSETS'].data
@@ -1636,15 +1833,16 @@
         
         outHDU[0].data = dyn_specRatio
         outHDU[0].name = 'DYNAMIC SPECTRATIO'
         print("writing output to {}".format(self.dyn_specFile('ratio')))
         outHDU.writeto(self.dyn_specFile('ratio'),overwrite=True)
     
     def make_wavebin_series(self,specType='Optimal',src=0,nbins=10,dispIndices=None,
-                            recalculate=False,align=False,refCorrect=False):
+                            recalculate=False,align=False,refCorrect=False,
+                            binStarts=None,binEnds=None):
         """
         Bin wavelengths together and generate a time series from the dynamic spectrum
         
         Parameters
         ----------
         specType: str
             Type of extraction 'Optimal' vs 'Sum'
@@ -1656,14 +1854,19 @@
             The detector pixel indices over which to create the wavelength bins
         recalculate: bool
             Re-caalculate the dynamic spectrum?
         align: bool
             Automatically align all the spectra? This is passed to plot_dynamic_spec
         refCorrect: bool
             Use the reference corrected photometry?
+        binStarts: numpy array or None
+            Specify starting points for the bins. If None, binStarts are calculated automatically
+        binEnds: numpy array or None
+            Specify starting points for the bins w/ Python, so the last point is binEnds - 1.
+            If None, binEnds are calculated automatically.
         """
         
         ## Check if there is a previous dynamic spec file with same parameters
         
         if (os.path.exists(self.dyn_specFile(src)) == True):
             head_dyn = fits.getheader(self.dyn_specFile(src),ext=0)
             if phot_pipeline.exists_and_equal(head_dyn,'ALIGNED',align):
@@ -1705,24 +1908,25 @@
         
         if dispIndices == None:
             dispSt, dispEnd = np.array(np.array(self.param['dispPixels']) + self.dispOffsets[src],dtype=np.int)
         else:
             dispSt, dispEnd = dispIndices
         
         binEdges = np.array(np.linspace(dispSt,dispEnd,nbins+1),dtype=np.int)
-        binStarts = binEdges[0:-1]
-        binEnds = binEdges[1:]
+        if binStarts is None:
+            binStarts = binEdges[0:-1]
+        if binEnds is None:
+            binEnds = binEdges[1:]
         binIndices = np.arange(len(binStarts))
         
         binGrid = np.zeros([nTime,nbins])
         binGrid_err = np.zeros_like(binGrid)
         
         binned_disp = np.zeros(nbins)
         
-        #db.set_trace()
         
         for ind, binStart, binEnd in zip(binIndices,binStarts,binEnds):
             theseWeights = weights[:,binStart:binEnd]
             binGrid[:,ind] = np.nansum(dynSpec[:,binStart:binEnd] * theseWeights ,1)
             normFactor = np.nanmedian(binGrid[:,ind])
             binGrid[:,ind] = binGrid[:,ind] / normFactor
             binGrid_err[:,ind] = np.sqrt(np.nansum((dynSpec_err[:,binStart:binEnd] * theseWeights)**2,1))
@@ -1744,26 +1948,34 @@
         dispTable = Table()
         dispTable['Bin Start'] = binStarts
         dispTable['Bin Middle'] = binned_disp
         dispTable['Bin End'] = binEnds
         
         dispHDU = fits.BinTableHDU(dispTable)
         dispHDU.name = "DISP INDICES"
-        outHDUList = fits.HDUList([outHDU,errHDU,timeHDU,offsetHDU,dispHDU])
+        
+        waveTable = Table()
+        for oneColumn in dispTable.colnames:
+            waveTable[oneColumn] = self.wavecal(dispTable[oneColumn])
+        waveHDU = fits.BinTableHDU(waveTable)
+        waveHDU.name = 'WAVELENGTHS'
+        
+        outHDUList = fits.HDUList([outHDU,errHDU,timeHDU,offsetHDU,dispHDU,waveHDU])
         outHDUList.writeto(self.wavebin_specFile(nbins,src),overwrite=True)
         
         HDUList.close()
     
     def get_offset_time(self,time):
         return np.floor(np.min(time))
     
     def plot_wavebin_series(self,nbins=10,offset=0.005,showPlot=False,yLim=None,xLim=None,
                             recalculate=False,dispIndices=None,differential=False,
                             interactive=False,unit='fraction',align=False,specType='Optimal',
-                            src=0,refCorrect=False):
+                            src=0,refCorrect=False,binStarts=None,binEnds=None,
+                            timeBin=False,nTimeBin=150,waveLabels=False):
         """
         Plot a normalized lightcurve for wavelength-binned data one wavelength at a time with
         an offset between the lightcurves.
         
         Parameters
         ----------
         nbins: int
@@ -1807,27 +2019,37 @@
             Type of extraction 'Optimal' vs 'Sum'
         align: bool
             Automatically align all the spectra? This is passed to plot_dynamic_spec
         src: int
             Index number for which spectrum to look at (used for Multi-object spectroscopy)
         refCorrect: bool
             Correct by reference stars for MOS?
+        timeBin: bool
+            Bin the points in time?
+        nTimeBin
+            Number of points to bin in time
         """
         if (os.path.exists(self.wavebin_specFile(nbins=nbins,srcInd=src)) == False) | (recalculate == True):
             self.make_wavebin_series(nbins=nbins,dispIndices=dispIndices,recalculate=recalculate,
-                                     specType=specType,align=align,src=src,refCorrect=refCorrect)
+                                     specType=specType,align=align,src=src,refCorrect=refCorrect,
+                                     binStarts=binStarts,binEnds=binEnds)
         
         HDUList = fits.open(self.wavebin_specFile(nbins=nbins,srcInd=src))
         time = HDUList['TIME'].data
         offset_time = self.get_offset_time(time)
         
         disp = HDUList['DISP INDICES'].data
         
         binGrid = HDUList['BINNED F'].data
         binGrid_err = HDUList['BINNED ERR'].data
+        
+        if waveLabels == True:
+            waves_table = Table(HDUList['WAVELENGTHS'].data)
+            waves = np.array(waves_table['Bin Middle'])
+        
         if differential == True:
             weights = 1./(np.nanmean(binGrid_err,0))**2
             weights2D = np.tile(weights,[binGrid.shape[0],1])
             
             avgSeries = (np.nansum(binGrid * weights2D,1)) / np.nansum(weights2D,1)
             
             avgSeries2D = np.tile(avgSeries,[len(disp),1]).transpose()
@@ -1864,19 +2086,31 @@
             p.add_tools(HoverTool(tooltips=[('name', '@name'),('index','@ind')]))
             bokeh.plotting.show(p)
             
         else:
             fig, ax = plt.subplots()
             for ind,oneDisp in enumerate(disp):
                 if unit == 'fraction':
-                    y_plot = binGrid[:,ind] - offset * ind
+                    y_plot_full_tres = binGrid[:,ind] - offset * ind
+                else:
+                    y_plot_full_tres = (binGrid[:,ind] - 1.0) * 1e6 - offset * ind * 1e6
+                
+                if timeBin == True:
+                    goodP = np.ones_like(time,dtype=bool)
+                    y_plot, xEdges, binNum = binned_statistic(time[goodP],y_plot_full_tres[goodP],
+                                                              bins=nTimeBin)
+                    time_plot = (xEdges[:-1] + xEdges[1:])/2.
                 else:
-                    y_plot = (binGrid[:,ind] - 1.0) * 1e6 - offset * ind * 1e6
+                    y_plot = y_plot_full_tres
+                    time_plot = time
                 
-                ax.errorbar(time - offset_time,y_plot,fmt='o')
+                ax.errorbar(time_plot - offset_time,y_plot,fmt='o')
+                
+                if waveLabels == True:
+                    ax.text(time_plot[-1] - offset_time,y_plot[-1],'{:.2f} $\mu$m'.format(waves[ind]))
             
             if yLim is not None:
                 ax.set_ylim(yLim[0],yLim[1])
             
             if xLim is not None:
                 ax.set_xlim(xLim[0],xLim[1])
             
@@ -1887,22 +2121,23 @@
                 ax.set_ylabel('(Normalized Flux - 1.0) (ppm)')
             
             if showPlot == True:
                 fig.show()
             else:
                 outName = 'wavebin_tser_{}_src_{}.pdf'.format(self.dataFileDescrip,src)
                 outPath = os.path.join(self.baseDir,'plots','spectra','wavebin_tseries',outName)
-                fig.savefig(outPath)
+                fig.savefig(outPath,bbox_inches='tight')
                 plt.close(fig)
 
             
             HDUList.close()
     
     
-    def get_wavebin_series(self,nbins=10,recalculate=False,specType='Optimal',srcInd=0):
+    def get_wavebin_series(self,nbins=10,recalculate=False,specType='Optimal',srcInd=0,
+                           binStarts=None,binEnds=None):
         """
         Get a table of the the wavelength-binned time series
         
         
         Parameters
         -----------
         nbins: int
@@ -1917,14 +2152,20 @@
             The type of spectral extraction routine
             Eg. "Sum" for sum extraction, "Optimal" for optimal extraction
             This will be skipped over if recalculate=False and a file already exists
         
         srcInd: int, optional
             The index of the source. For single objects it is 0.
         
+        binStarts: int, optional or None
+            Pixel starting positions (or None). If None, it will be calculated as a linear spacing
+        
+        binEnds: int, optional
+            Pixel ending positions (or None). If None, it will be calculated as a linear spacing
+        
         Returns
         --------
         t1: astropy table
             A table of wavelength-binned flux values
         t2: astropy table
             A table of wavelength-binned error values
         
@@ -1933,15 +2174,16 @@
         
         >>> from tshirt.pipeline import spec_pipeline
         >>> spec = spec_pipeline.spec()
         >>> t1, t2 = spec.get_wavebin_series()
         """
         sFile = self.wavebin_specFile(nbins=nbins,srcInd=srcInd)
         if (os.path.exists(sFile) == False) | (recalculate == True):
-            self.plot_wavebin_series(nbins=nbins,recalculate=recalculate,specType=specType)
+            self.plot_wavebin_series(nbins=nbins,recalculate=recalculate,specType=specType,
+                                     binStarts=binStarts,binEnds=binEnds)
         HDUList = fits.open(sFile)
         disp = HDUList['DISP INDICES'].data
         binGrid = HDUList['BINNED F'].data
         binGrid_err = HDUList['BINNED ERR'].data
         time = HDUList['TIME'].data
         t1, t2 = Table(), Table()
         t1['Time'] = time
@@ -1952,27 +2194,37 @@
             t1['{:.3f}um Flux'.format(wave)] = binGrid[:,ind]
             t2['{:.3f}um Error'.format(wave)] = binGrid_err[:,ind]
         
         HDUList.close()
         return t1, t2
     
     def print_noise_wavebin(self,nbins=10,shorten=False,recalculate=False,align=False,
-                            specType='Optimal',npoints=15,srcInd=0):
+                            specType='Optimal',npoints=15,srcInd=0,
+                            startInd=0,endInd=None):
         """ 
         Get a table of noise measurements for all wavelength bins
         
         Parameters
         ----------
         nbins: int
             The number of wavelength bins
         shorten: bool
             Use a short segment of the full time series?
-            This could be useful for avoiding bad data or a deep transit
+            This could be useful for avoiding bad data or a deep transit.
+            This overrides startInd and endInd so choose either shorten or specify
+            the start and end indices
         npoints: int
-            Number of points to include in the calculation (if shorten is True)
+            Number of points to include in the calculation (only if shorten is True)
+            This will only use the first npoints.
+        startInd: int
+            Starting time index to use (for specifying a time interval via indices)
+            Shorten will supercede this so keep it False to use startInd.
+        endInd: int
+            Ending time index to use (for specifying a time interval via indices).
+            Shorten will supercede this so keep it False to use endInd.
         recalculate: bool
             Recalculate the wavebin series and dynamic spectrum?
         specType: str
             Type of extraction 'Optimal' vs 'Sum'
         align: bool
             Automatically align all the spectra? This is passed to plot_dynamic_spec
         srcInd: int
@@ -1998,14 +2250,16 @@
         t['Disp Mid'] = disp['Bin Middle']
         t['Disp End'] = disp['Bin End']
         t['Wave (st)'] = np.round(self.wavecal(disp['Bin Start']),3)
         t['Wave (mid)'] = np.round(self.wavecal(t['Disp Mid']),3)
         t['Wave (end)'] = np.round(self.wavecal(disp['Bin End']),3)
         if shorten == True:
             binGrid = binGrid[0:npoints,:]
+        else:
+            binGrid = binGrid[startInd:endInd,:]
         t['Stdev (%)'] = np.round(np.std(binGrid,axis=0) * 100.,4)
         t['Theo Err (%)'] = np.round(np.median(binGrid_err,axis=0) * 100.,4)
         
         medianV = np.median(binGrid,axis=0)
         absDeviation = np.abs(binGrid - medianV)
         t['MAD (%)'] = np.round(np.median(absDeviation,axis=0) * 100.,4)
         
@@ -2247,20 +2501,33 @@
         if waveCalMethod == None:
             wavelengths = dispIndices
         elif waveCalMethod == 'NIRCamTS':
             if head == None:
                 head = fits.getheader(self.specFile,extname='ORIG HEADER')
             wavelengths = instrument_specific.jwst_inst_funcs.ts_wavecal(dispIndices,obsFilter=head['FILTER'],
                                                                          **kwargs)
+        elif waveCalMethod == 'NIRCamTSquickPoly':
+            if head == None:
+                head = fits.getheader(self.specFile,extname='ORIG HEADER')
+            wavelengths = instrument_specific.jwst_inst_funcs.ts_wavecal_quick_nonlin(dispIndices,obsFilter=head['FILTER'],
+                                                                         **kwargs)
         elif waveCalMethod == 'simGRISMC':
             wavelengths = instrument_specific.jwst_inst_funcs.ts_grismc_sim(dispIndices,**kwargs)
         
         elif waveCalMethod == 'wfc3Dispersion':
             wavelengths = instrument_specific.hst_inst_funcs.hstwfc3_wavecal(dispIndices,**kwargs)
-            
+        elif waveCalMethod == 'quick_nrs_prism':
+            wavelengths = instrument_specific.jwst_inst_funcs.quick_nirspec_prism(dispIndices)
+        elif waveCalMethod == 'grismr_poly_dms':
+            if head == None:
+                head = fits.getheader(self.specFile,extname='ORIG HEADER')
+                obsFilter = head['FILTER']
+            else:
+                obsFilter = 'F322W2'
+            wavelengths = instrument_specific.jwst_inst_funcs.flight_poly_grismr_nc(dispIndices,obsFilter=obsFilter)
         else:
             raise Exception("Unrecognized wavelength calibration method {}".format(waveCalMethod))
             
         wavelengths = wavelengths - self.param['waveCalOffset']
         return wavelengths
```

### Comparing `tshirt-0.1.dev9/tshirt/pipeline/utils.py` & `tshirt-0.2/tshirt/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/quick_timeit.py` & `tshirt-0.2/tshirt/quick_timeit.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/tests/test_phot_algorithms.py` & `tshirt-0.2/tshirt/tests/test_phot_algorithms.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/tests/test_pipe_basics.py` & `tshirt-0.2/tshirt/tests/test_pipe_basics.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/tests/test_window_placement.py` & `tshirt-0.2/tshirt/tests/test_window_placement.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt/tser_tests.py` & `tshirt-0.2/tshirt/tser_tests.py`

 * *Files identical despite different names*

### Comparing `tshirt-0.1.dev9/tshirt.egg-info/PKG-INFO` & `tshirt-0.2/tshirt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: tshirt
-Version: 0.1.dev9
+Version: 0.2
 Summary: A package to analyze time series data, especially for exoplanets
 Home-page: https://github.com/eas342/tshirt
 Author: Everett Schlawin, Kayli Glidic
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 `tshirt` README
 ==========================================
 The Time Series Helper & Integration Reduction Tool `tshirt` is a general-purpose tool for time series science.
@@ -19,9 +17,7 @@
 - Reduce raw data: flat field, bias subtract, gain correct, etc. This has been demonstrated to work with merged CCD images from Mont4K imager on the Kuiper-61 inch on Mt Bigelow, AZ.
 - Extract Photometry
 - Extract Spectroscopy
 
 
 See the read-the-docs page for information on how to install and use `tshirt`:
 [https://tshirt.readthedocs.io/en/latest/](https://tshirt.readthedocs.io/en/latest/)
-
-
```

### Comparing `tshirt-0.1.dev9/tshirt.egg-info/SOURCES.txt` & `tshirt-0.2/tshirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

