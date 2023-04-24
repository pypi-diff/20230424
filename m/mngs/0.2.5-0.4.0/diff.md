# Comparing `tmp/mngs-0.2.5.tar.gz` & `tmp/mngs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mngs-0.2.5.tar", last modified: Thu Mar 24 03:28:27 2022, max compression
+gzip compressed data, was "mngs-0.4.0.tar", last modified: Mon Apr 24 00:11:29 2023, max compression
```

## Comparing `mngs-0.2.5.tar` & `mngs-0.4.0.tar`

### file list

```diff
@@ -1,121 +1,140 @@
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:09.816094 mngs-0.2.5/
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)    35149 2021-09-25 06:22:17.000000 mngs-0.2.5/LICENSE
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)       64 2021-09-25 06:22:17.000000 mngs-0.2.5/MANIFEST.in
--rw-r--r--   0 ywatanabe  (1038) ywatanabe  (1038)     3085 2022-03-24 03:20:09.816094 mngs-0.2.5/PKG-INFO
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)     2572 2021-10-28 14:04:56.000000 mngs-0.2.5/README.md
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      152 2022-03-24 03:20:09.817094 mngs-0.2.5/setup.cfg
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     2448 2021-10-28 14:04:56.000000 mngs-0.2.5/setup.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:30.160096 mngs-0.2.5/src/
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:35.389095 mngs-0.2.5/src/mngs/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      413 2022-03-24 03:15:10.000000 mngs-0.2.5/src/mngs/__init__.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:35.675095 mngs-0.2.5/src/mngs/dsp/
--rwxrwx---   0 ywatanabe  (1038) ywatanabe  (1038)     6633 2021-04-10 08:27:42.000000 mngs-0.2.5/src/mngs/dsp/BandPassFiltering.py
--rwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)     2313 2021-12-21 12:39:44.000000 mngs-0.2.5/src/mngs/dsp/FeatureExtractor.py
--rwxrwx---   0 ywatanabe  (1038) ywatanabe  (1038)     5313 2021-11-30 07:17:53.000000 mngs-0.2.5/src/mngs/dsp/HilbertTransformation.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      148 2021-12-11 00:46:47.000000 mngs-0.2.5/src/mngs/dsp/_BANDS_LIM_HZ_DICT.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      561 2021-12-11 00:45:07.000000 mngs-0.2.5/src/mngs/dsp/__init__.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      558 2021-11-29 04:04:51.000000 mngs-0.2.5/src/mngs/dsp/_bandpassfilter.py
--rwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)     8803 2021-11-30 08:07:47.000000 mngs-0.2.5/src/mngs/dsp/feature_extractions.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      657 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/dsp/fft_powers.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1052 2021-10-28 14:04:56.000000 mngs-0.2.5/src/mngs/dsp/wavelet.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:42.789095 mngs-0.2.5/src/mngs/general/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1065 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/general/TimeStamper.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      930 2021-12-22 03:06:00.000000 mngs-0.2.5/src/mngs/general/__init__.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     2882 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/general/_xml2dict.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)    15227 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/general/cuda_collect_env.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     2144 2021-12-03 08:59:55.000000 mngs-0.2.5/src/mngs/general/debug.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      502 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/general/latex.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     3982 2022-03-24 02:58:31.000000 mngs-0.2.5/src/mngs/general/load.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     2181 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/general/mat2py.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)    12082 2021-12-22 03:06:29.000000 mngs-0.2.5/src/mngs/general/misc.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     4750 2021-12-18 18:53:10.000000 mngs-0.2.5/src/mngs/general/pandas.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1932 2022-03-23 08:24:41.000000 mngs-0.2.5/src/mngs/general/path.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     3145 2021-11-22 03:02:52.000000 mngs-0.2.5/src/mngs/general/repro.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     8919 2022-03-23 08:26:55.000000 mngs-0.2.5/src/mngs/general/save.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      640 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/general/torch.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:46.607095 mngs-0.2.5/src/mngs/io/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      356 2021-12-16 13:30:12.000000 mngs-0.2.5/src/mngs/io/__init__.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     3982 2022-03-24 02:58:31.000000 mngs-0.2.5/src/mngs/io/load.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1932 2022-03-23 08:24:41.000000 mngs-0.2.5/src/mngs/io/path.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     8919 2022-03-23 08:26:55.000000 mngs-0.2.5/src/mngs/io/save.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:52.303095 mngs-0.2.5/src/mngs/ml/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)    15664 2021-12-04 10:04:50.000000 mngs-0.2.5/src/mngs/ml/ClassificationReporter.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     3452 2021-12-12 05:44:12.000000 mngs-0.2.5/src/mngs/ml/ClassifierServer.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     3077 2021-12-18 07:56:20.000000 mngs-0.2.5/src/mngs/ml/EarlyStopping.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)    15339 2021-12-18 17:04:02.000000 mngs-0.2.5/src/mngs/ml/LearningCurveLogger.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     3447 2021-12-12 05:48:53.000000 mngs-0.2.5/src/mngs/ml/__Classifiers.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      381 2021-12-15 00:49:33.000000 mngs-0.2.5/src/mngs/ml/__init__.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:53.720095 mngs-0.2.5/src/mngs/ml/act/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      124 2021-12-15 00:31:43.000000 mngs-0.2.5/src/mngs/ml/act/__init__.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      220 2021-12-15 00:31:02.000000 mngs-0.2.5/src/mngs/ml/act/_define.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:57.635095 mngs-0.2.5/src/mngs/ml/layer/
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      141 2021-12-15 00:32:48.000000 mngs-0.2.5/src/mngs/ml/layer/_Pass.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)       52 2021-12-15 00:34:42.000000 mngs-0.2.5/src/mngs/ml/layer/__init__.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      122 2021-12-15 00:34:16.000000 mngs-0.2.5/src/mngs/ml/layer/_switch.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:01.107094 mngs-0.2.5/src/mngs/ml/loss/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1387 2021-12-10 04:10:07.000000 mngs-0.2.5/src/mngs/ml/loss/MultiTaskLoss.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      623 2021-12-10 04:19:03.000000 mngs-0.2.5/src/mngs/ml/loss/_L1L2Losses.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)        0 2021-12-10 04:07:27.000000 mngs-0.2.5/src/mngs/ml/loss/__init__.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:03.583094 mngs-0.2.5/src/mngs/ml/optim/
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:04.331094 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)        0 2021-12-07 00:44:44.000000 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:07.272094 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)       91 2021-12-07 00:43:01.000000 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)     7915 2021-12-07 00:43:01.000000 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)     9051 2021-12-07 00:43:01.000000 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)     8568 2021-12-07 00:43:01.000000 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)     6934 2021-12-07 00:43:01.000000 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      696 2021-12-07 00:43:01.000000 mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      128 2021-12-15 00:28:17.000000 mngs-0.2.5/src/mngs/ml/optim/__init__.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      713 2021-12-15 00:28:48.000000 mngs-0.2.5/src/mngs/ml/optim/_get_set.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:08.567094 mngs-0.2.5/src/mngs/ml/plt/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      147 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/plt/__init__.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:09.420094 mngs-0.2.5/src/mngs/ml/plt/aucs/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)       71 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/plt/aucs/__init__.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1625 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/plt/aucs/example.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     7036 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/plt/aucs/pre_rec_auc.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     5503 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/plt/aucs/roc_auc.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     5834 2021-11-21 20:54:12.000000 mngs-0.2.5/src/mngs/ml/plt/confusion_matrix.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)    17121 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/silhoute_score_block.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:09.568094 mngs-0.2.5/src/mngs/ml/utils/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1295 2021-12-17 05:40:19.000000 mngs-0.2.5/src/mngs/ml/utils/_DefaultDataset.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      269 2021-12-20 07:05:04.000000 mngs-0.2.5/src/mngs/ml/utils/__init__.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      596 2021-12-20 10:21:14.000000 mngs-0.2.5/src/mngs/ml/utils/_format_samples_for_sktime.py
--rwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)      704 2021-11-30 02:09:26.000000 mngs-0.2.5/src/mngs/ml/utils/_get_params.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      507 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/utils/_merge_labels.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1197 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/ml/utils/_under_sample.py
--rw-rw-r--   0 ywatanabe  (1038) ywatanabe  (1038)      437 2021-12-17 13:19:24.000000 mngs-0.2.5/src/mngs/ml/utils/_verify_n_gpus.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:09.673094 mngs-0.2.5/src/mngs/plt/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      454 2021-11-27 09:40:49.000000 mngs-0.2.5/src/mngs/plt/__init__.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     3511 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/_ax_extend.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1688 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/_ax_scientific_notation.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      328 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/_ax_set_n_ticks.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      949 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/_ax_set_position.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     4801 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/_configure_mpl.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      560 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/_draw_a_cube.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      795 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/_get_RGBA_from_colormap.py
--rwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)      412 2021-11-27 09:43:50.000000 mngs-0.2.5/src/mngs/plt/_mk_patches.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1308 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/annotated_heatmap.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1524 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/colors.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1004 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/plt/get_mpl_color.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:09.715094 mngs-0.2.5/src/mngs/resource/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)       93 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/resource/__init__.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     4702 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/resource/get.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      745 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/resource/limit_RAM.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:09.784094 mngs-0.2.5/src/mngs/stats/
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      388 2021-10-12 14:10:43.000000 mngs-0.2.5/src/mngs/stats/__init__.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     2056 2021-09-25 06:39:13.000000 mngs-0.2.5/src/mngs/stats/_bonferroni_correction.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     2002 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/stats/_brunner_munzel_test.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      495 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/stats/_calc_partial_corr.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     6941 2021-09-25 06:38:59.000000 mngs-0.2.5/src/mngs/stats/_fdr_correction.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)     1153 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/stats/_multicompair.py
--rwxrwxr-x   0 ywatanabe  (1038) ywatanabe  (1038)      814 2021-09-25 06:22:17.000000 mngs-0.2.5/src/mngs/stats/_nocorrelation_test.py
--rw-r--r--   0 ywatanabe  (1038) ywatanabe  (1038)     2604 2021-10-12 20:21:30.000000 mngs-0.2.5/src/mngs/stats/_smirnov_grubbs.py
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:19:35.473095 mngs-0.2.5/src/mngs.egg-info/
--rw-r--r--   0 ywatanabe  (1038) ywatanabe  (1038)     3085 2022-03-24 03:18:30.000000 mngs-0.2.5/src/mngs.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1038) ywatanabe  (1038)     3178 2022-03-24 03:18:55.000000 mngs-0.2.5/src/mngs.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1038) ywatanabe  (1038)        1 2022-03-24 03:18:31.000000 mngs-0.2.5/src/mngs.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1038) ywatanabe  (1038)      131 2022-03-24 03:18:32.000000 mngs-0.2.5/src/mngs.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1038) ywatanabe  (1038)        5 2022-03-24 03:18:32.000000 mngs-0.2.5/src/mngs.egg-info/top_level.txt
-drwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)        0 2022-03-24 03:20:09.799094 mngs-0.2.5/test/
--rwxr-xr-x   0 ywatanabe  (1038) ywatanabe  (1038)      183 2021-10-26 14:04:36.000000 mngs-0.2.5/test/test_import_mngs.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)    35149 2023-04-24 00:10:34.000000 mngs-0.4.0/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2023-04-24 00:10:34.000000 mngs-0.4.0/MANIFEST.in
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3085 2023-04-24 00:11:29.212652 mngs-0.4.0/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2572 2023-04-24 00:10:34.000000 mngs-0.4.0/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2023-04-24 00:11:29.212652 mngs-0.4.0/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2448 2023-04-24 00:10:34.000000 mngs-0.4.0/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.202653 mngs-0.4.0/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.202653 mngs-0.4.0/src/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      632 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.202653 mngs-0.4.0/src/mngs/dsp/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6633 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/BandPassFiltering.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2313 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/FeatureExtractor.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5313 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/HilbertTransformation.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      148 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/_BANDS_LIM_HZ_DICT.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      772 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      558 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/_bandpassfilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      176 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/_common_average.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      316 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/_gaussian_filter1d.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/_normalize_time.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      328 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/_take_random_references.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9045 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/feature_extractions.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      973 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/fft_amps.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1052 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/dsp/wavelet.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/general/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1065 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/TimeStamper.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      988 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/_xml2dict.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/cuda_collect_env.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2144 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/debug.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/latex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4536 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/mat2py.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15159 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4750 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/pandas.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1932 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3145 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/repro.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9025 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/save.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/general/torch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/io/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      356 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/io/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4536 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/io/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1932 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/io/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9025 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/io/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/linalg/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/linalg/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/linalg/_misc.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/ClassificationReporter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/ClassifierServer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3077 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/EarlyStopping.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/LearningCurveLogger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      410 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/act/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/act/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/act/_define.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/layer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/layer/_Pass.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/layer/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/layer/_switch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/loss/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/loss/MultiTaskLoss.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/loss/_L1L2Losses.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/loss/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/optim/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/optim/_get_set.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      147 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/plt/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/plt/aucs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/plt/aucs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/plt/aucs/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/plt/aucs/pre_rec_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/plt/aucs/roc_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6878 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/plt/confusion_matrix.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/silhoute_score_block.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/ml/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/utils/_DefaultDataset.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      269 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/utils/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/utils/_format_samples_for_sktime.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      704 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/utils/_get_params.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      507 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/utils/_merge_labels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/utils/_under_sample.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/ml/utils/_verify_n_gpus.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2147 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2932 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1233 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      406 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/nn/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      654 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_add_hue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2966 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_ax_circular_hist.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3511 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_ax_extend.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_ax_fill_between.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1688 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_ax_scientific_notation.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      328 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_ax_set_n_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      949 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_ax_set_position.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      452 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_ax_set_size.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4801 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_configure_mpl.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_draw_a_cube.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_get_RGBA_from_colormap.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      605 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_mk_colorbar.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/_mk_patches.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/annotated_heatmap.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/colors.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/plt/get_mpl_color.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/resource/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/resource/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/resource/get.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/resource/limit_RAM.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.212652 mngs-0.4.0/src/mngs/stats/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      462 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_bonferroni_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_brunner_munzel_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_calc_partial_corr.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_corr_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_fdr_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_multicompair.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_nocorrelation_test.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_smirnov_grubbs.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2023-04-24 00:10:34.000000 mngs-0.4.0/src/mngs/stats/_to_asterisks.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2023-04-24 00:11:29.202653 mngs-0.4.0/src/mngs.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3085 2023-04-24 00:11:28.000000 mngs-0.4.0/src/mngs.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3725 2023-04-24 00:11:29.000000 mngs-0.4.0/src/mngs.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2023-04-24 00:11:28.000000 mngs-0.4.0/src/mngs.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      195 2023-04-24 00:11:29.000000 mngs-0.4.0/src/mngs.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2023-04-24 00:11:29.000000 mngs-0.4.0/src/mngs.egg-info/top_level.txt
```

### Comparing `mngs-0.2.5/LICENSE` & `mngs-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/PKG-INFO` & `mngs-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 0.2.5
+Version: 0.4.0
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: GPL3.0
 Keywords: utils,utilities,python,machine learning
 Platform: UNKNOWN
```

### Comparing `mngs-0.2.5/README.md` & `mngs-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/setup.py` & `mngs-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/dsp/BandPassFiltering.py` & `mngs-0.4.0/src/mngs/dsp/BandPassFiltering.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/dsp/FeatureExtractor.py` & `mngs-0.4.0/src/mngs/dsp/FeatureExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Time-stamp: "2021-12-21 21:41:38 (ywatanabe)"
+# Time-stamp: "2022-10-07 12:51:52 (ywatanabe)"
 
 import torch
 import torch.nn as nn
 import mngs
 
 from functools import partial
```

### Comparing `mngs-0.2.5/src/mngs/dsp/HilbertTransformation.py` & `mngs-0.4.0/src/mngs/dsp/HilbertTransformation.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/dsp/__init__.py` & `mngs-0.4.0/src/mngs/dsp/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 from ._bandpassfilter import bandpassfilter
-from .fft_powers import calc_fft_powers
+from .fft_amps import calc_fft_amps, calc_fft_powers
 from .wavelet import wavelet
 from .FeatureExtractor import FeatureExtractor
 from .feature_extractions import (
     rfft_bands,
     rfft,
     bandstop,
     spectrogram,
@@ -26,7 +26,11 @@
     amp,
     amp_band,
     hilbert,
     fft,
     bandpass,
 )
 from ._BANDS_LIM_HZ_DICT import BANDS_LIM_HZ_DICT
+from ._normalize_time import normalize_time
+from ._common_average import common_average
+from ._take_random_references import take_random_references
+from ._gaussian_filter1d import gaussian_filter1d
```

### Comparing `mngs-0.2.5/src/mngs/dsp/_bandpassfilter.py` & `mngs-0.4.0/src/mngs/dsp/_bandpassfilter.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/dsp/feature_extractions.py` & `mngs-0.4.0/src/mngs/dsp/feature_extractions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Time-stamp: "2021-11-30 17:09:22 (ylab)"
+# Time-stamp: "2022-10-07 13:35:38 (ywatanabe)"
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pyro
 import torch
 import torch.nn.functional as F
 import torchaudio
@@ -123,39 +123,45 @@
     if return_freq:
         return fft_coef, freq
     else:
         return fft_coef
 
 
 def rfft_bands(
-    x, samp_rate, bands_str=["delta", "theta", "lalpha", "halpha", "beta", "gamma"]
+        x, samp_rate, bands_str=["delta", "theta", "lalpha", "halpha", "beta", "gamma"], normalize=False,
 ):
     """
     Returns mean absolute rfft coefficients of bands.
     Bands' definitions are as follows.
 
     BANDS_LIM_HZ_DICT = {
         "delta": [0.5, 4],
         "theta": [4, 8],
         "lalpha": [8, 10],
         "halpha": [10, 13],
         "beta": [13, 32],
         "gamma": [32, 75],
     }
+    
+    rfft_bands_p = partial(mngs.dsp.rfft_bands, samp_rate=samp_rate)
     """
     coef, freq = rfft(x, samp_rate)
+    amp = coef.abs()
+    
+    if normalize:
+        amp /= amp.sum(axis=-1, keepdims=True)
 
-    coef_bands_abs_mean = []
+    amp_bands_abs_mean = []
     for band_str in bands_str:
         low, high = BANDS_LIM_HZ_DICT[band_str]
         indi_band = (low <= freq) & (freq <= high)
-        coef_band_abs_mean = coef[..., indi_band].abs().mean(dim=-1)
-        coef_bands_abs_mean.append(coef_band_abs_mean)
+        amp_band_abs_mean = amp[..., indi_band].mean(dim=-1)
+        amp_bands_abs_mean.append(amp_band_abs_mean)
 
-    return torch.stack(coef_bands_abs_mean, dim=-1)
+    return torch.stack(amp_bands_abs_mean, dim=-1)
 
 
 def rfft(x, samp_rate):
     fn = partial(_rfft_1d, samp_rate=samp_rate, return_freq=False)
     fft_coef = _apply_to_the_time_dim(fn, x)
     freq = torch.fft.rfftfreq(x.shape[-1], d=1 / samp_rate)
     return fft_coef, freq
@@ -324,7 +330,10 @@
     fig.show()
 
 
 if __name__ == "__main__":
     SAMP_RATE = 1000
     x = demo_sig(freqs_hz=[2, 3, 5, 10], samp_rate=SAMP_RATE, len_sec=2)
     # x = torch.tensor(chirp(time, 3, 500, 100))
+    coef, freq = rfft(x, SAMP_RATE)
+    amp = coef.abs()
+
```

### Comparing `mngs-0.2.5/src/mngs/dsp/wavelet.py` & `mngs-0.4.0/src/mngs/dsp/wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/TimeStamper.py` & `mngs-0.4.0/src/mngs/general/TimeStamper.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/__init__.py` & `mngs-0.4.0/src/mngs/general/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 from .debug import *
 from .latex import add_hat_in_the_latex_style, to_the_latex_style
 from .mat2py import *
 from .misc import (connect_nums, connect_strs, copy_files, copy_the_file,
                    decapitalize, fmt_size, grep, is_defined_global,
                    is_defined_local, is_later_or_equal, isclose, listed_dict,
                    merge_dicts_wo_overlaps, pop_keys, search, squeeze_spaces,
-                   take_the_closest, is_nan)
+                   take_the_closest, is_nan, partial_at, describe, wait_key, _return_counting_process)
 from .pandas import col_to_last, col_to_top, force_dataframe, merge_columns
 from .repro import *
 from .TimeStamper import *
 from .torch import *
```

### Comparing `mngs-0.2.5/src/mngs/general/_xml2dict.py` & `mngs-0.4.0/src/mngs/general/_xml2dict.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/cuda_collect_env.py` & `mngs-0.4.0/src/mngs/general/cuda_collect_env.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/debug.py` & `mngs-0.4.0/src/mngs/general/debug.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/load.py` & `mngs-0.4.0/src/mngs/general/load.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,27 @@
     import pickle
 
     import h5py
     import numpy as np
     import pandas as pd
     import torch
     import yaml
+    import mne
 
     # csv
     if lpath.endswith(".csv"):
         obj = pd.read_csv(lpath, **kwargs)
+    # excel
+    if (
+        lpath.endswith(".xls")
+        or lpath.endswith(".xlsx")
+        or lpath.endswith(".xlsm")
+        or lpath.endswith(".xlsb")
+    ):
+        obj = pd.read_excel(lpath, **kwargs)
     # numpy
     if lpath.endswith(".npy"):
         obj = np.load(lpath)
     # pkl
     if lpath.endswith(".pkl"):
         with open(lpath, "rb") as l:
             obj = pickle.load(l)
@@ -58,35 +67,48 @@
             obj.update(obj_tmp)
     # txt
     if lpath.endswith(".txt"):
         f = open(lpath, "r")
         obj = [l.strip("\n\r") for l in f]
         f.close()
     # pth
-    if lpath.endswith(".pth"):
+    if lpath.endswith(".pth") or lpath.endswith(".pt"):
         # return model.load_state_dict(torch.load(lpath))
         obj = torch.load(lpath)
 
+    # mat
     if lpath.endswith(".mat"):
         import pymatreader
 
         obj = pymatreader.read_mat(lpath)
     # xml
     if lpath.endswith("xml"):
         from ._xml2dict import xml2dict
 
         obj = xml2dict(lpath)
+    # edf
+    if lpath.endswith("edf"):
+        obj = mne.io.read_raw_edf(lpath)
+    # con    
+    if lpath.endswith("con"):
+        _obj = mne.io.read_raw(lpath)
+        obj = _obj.to_data_frame()
+        obj["samp_rate"] = _obj.info.get("sfreq")
+    # mrk
+    if lpath.endswith("mrk"):
+        obj = mne.io.kit.read_mrk(lpath)
 
     # catboost model
     if lpath.endswith(".cbm"):
         obj = obj.load_model(lpath)
-        
+
     # if mngs.general.is_defined_local("obj"):
     if "obj" in locals():
-        print("\nLoaded from: {}\n".format(lpath))
+        if show:
+            print("\nLoaded from: {}\n".format(lpath))
         return obj
     else:
         return None
 
 
 def check_encoding(file_path):
     from chardet.universaldetector import UniversalDetector
@@ -108,43 +130,44 @@
     import sys
 
     spec = importlib.util.find_spec(package_str)
     data_dir = os.path.join(spec.origin.split("src")[0], "data")
     resource_path = os.path.join(data_dir, resource)
     return resource_path
 
+
 def load_yaml_as_an_optuna_dict(fpath_yaml, trial):
-    _d = load(fpath_yaml)    
-    
+    _d = load(fpath_yaml)
+
     for k, v in _d.items():
-        
+
         dist = v["distribution"]
 
         if dist == "categorical":
             _d[k] = trial.suggest_categorical(k, v["values"])
 
         elif dist == "uniform":
             _d[k] = trial.suggest_int(k, float(v["min"]), float(v["max"]))
-            
+
         elif dist == "loguniform":
             _d[k] = trial.suggest_loguniform(k, float(v["min"]), float(v["max"]))
 
         elif dist == "intloguniform":
             _d[k] = trial.suggest_int(k, float(v["min"]), float(v["max"]), log=True)
-            
+
     return _d
 
+
 def load_study_rdb(study_name, rdb_raw_bytes_url):
     """
     study = load_study_rdb(
         study_name="YOUR_STUDY_NAME",
         rdb_raw_bytes_url="sqlite:///*.db"
     )
     """
     import optuna
+
     # rdb_raw_bytes_url = "sqlite:////tmp/fake/ywatanabe/_MicroNN_WindowSize-1.0-sec_MaxEpochs_100_2021-1216-1844/optuna_study_test_file#0.db"
     storage = optuna.storages.RDBStorage(url=rdb_raw_bytes_url)
     study = optuna.load_study(study_name=study_name, storage=storage)
     print(f"\nLoaded: {rdb_raw_bytes_url}\n")
     return study
-    
-
```

### Comparing `mngs-0.2.5/src/mngs/general/mat2py.py` & `mngs-0.4.0/src/mngs/general/mat2py.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/misc.py` & `mngs-0.4.0/src/mngs/general/misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 from collections import defaultdict
 
 import mngs
 import numpy as np
 import pandas as pd
 import torch
 from natsort import natsorted
-
+from functools import partial, wraps
+import warnings
+import readchar
+import threading
 
 ################################################################################
 ## strings
 ################################################################################
 def decapitalize(s):
     if not s:  # check that s is not empty string
         return s
@@ -63,15 +66,15 @@
     a callable, it's passed the Match object and must return
     a replacement string to be used.
     """
     # return re.sub(" +", " ", string)
     return re.sub(pattern, repl, string)
 
 
-def search(patterns, strings, only_perfect_match=False):
+def search(patterns, strings, only_perfect_match=False, as_bool=False):
     """
     regular expression is acceptable for patterns.
 
     Example:
         patterns = ['orange', 'banana']
         strings = ['apple', 'orange', 'apple', 'apple_juice', 'banana', 'orange_juice']
         print(search(patterns, strings))
@@ -84,15 +87,17 @@
     """
 
     ## For single string objects
     def to_list(s_or_p):
         if isinstance(s_or_p, collections.abc.KeysView):
             s_or_p = list(s_or_p)
 
-        elif not isinstance(s_or_p, (list, tuple, pd.core.indexes.base.Index)):
+        elif not isinstance(
+            s_or_p, (list, tuple, pd.core.indexes.base.Index, pd.core.series.Series)
+        ):
             s_or_p = [s_or_p]
 
         return s_or_p
 
     patterns = to_list(patterns)
     strings = to_list(strings)
 
@@ -110,15 +115,23 @@
             for i_str, string in enumerate(strings):
                 if pattern == string:
                     indi_matched.append(i_str)
 
     ## Sorts the indices according to the original strings
     indi_matched = natsorted(indi_matched)
     keys_matched = list(np.array(strings)[indi_matched])
-    return indi_matched, keys_matched
+
+    if as_bool:
+        bool_matched = np.zeros(len(strings), dtype=bool)
+        if np.unique(indi_matched).size != 0:
+            bool_matched[np.unique(indi_matched)] = True
+        return bool_matched, keys_matched
+
+    else:
+        return indi_matched, keys_matched
 
 
 def grep(str_list, search_key):
     """
     Example:
         str_list = ['apple', 'orange', 'apple', 'apple_juice', 'banana', 'orange_juice']
         search_key = 'orange'
@@ -216,17 +229,19 @@
     return [math.isclose(a, b) for a, b in zip(mutable_a, mutable_b)]
 
 
 ################################################################################
 ## dictionary
 ################################################################################
 def merge_dicts_wo_overlaps(*dicts):
-    merged_dict = {} # init
+    merged_dict = {}  # init
     for dict in dicts:
-        assert mngs.general.search(merged_dict.keys(), dict.keys(), only_perfect_match=True) == ([], [])
+        assert mngs.general.search(
+            merged_dict.keys(), dict.keys(), only_perfect_match=True
+        ) == ([], [])
         merged_dict.update(dict)
     return merged_dict
 
 
 def listed_dict(keys=None):  # Is there a better name?
     """
     Example 1:
@@ -387,21 +402,121 @@
     dst = sdir + fname + ext
 
     if "ipython" not in __file__:  # for ipython
         # shutil.copyfile(__file__, dst)
         # print(f"Saved to: {dst}")
         _copy_a_file(__file__, dst)
 
+
 def is_nan(X):
     if isinstance(X, pd.DataFrame):
         if X.isna().any().any():
             raise ValueError("NaN was found in X")
     elif isinstance(X, np.ndarray):
-        if np.isnan(X).any():        
+        if np.isnan(X).any():
             raise ValueError("NaN was found in X")
     elif torch.is_tensor(X):
-        if X.isnan().any():        
+        if X.isnan().any():
             raise ValueError("NaN was found in X")
     elif isinstance(X, (float, int)):
         if math.isnan(X):
             raise ValueError("X was NaN")
 
+
+def partial_at(func, index, value):
+    @wraps(func)
+    def result(*rest, **kwargs):
+        args = []
+        args.extend(rest[:index])
+        args.append(value)
+        args.extend(rest[index:])
+        return func(*args, **kwargs)
+
+    return result
+
+
+def describe(df, method="mean", factor=1):
+    df = pd.DataFrame(df)
+    # df = df[~df[0].isna()]
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", RuntimeWarning)
+        if method == "mean":
+            return round(np.nanmean(df), 3), round(np.nanstd(df) / factor, 3)
+        if method == "median":
+            med = df.describe().T["50%"].iloc[0]
+            IQR = df.describe().T["75%"].iloc[0] - df.describe().T["25%"].iloc[0]
+            return round(med, 3), round(IQR / factor, 3)
+
+
+# def describe(arr, method="mean", factor=1):
+#     arr = pd.DataFrame(arr)
+#     arr = np.hstack(arr[~np.isnan(arr)])
+
+#     with warnings.catch_warnings():
+#         warnings.simplefilter("ignore", RuntimeWarning)
+#         if method == "mean":
+#             return np.nanmean(df), np.nanstd(df) / factor
+#         if method == "median":
+#             med = df.describe().T["50%"].iloc[0]
+#             IQR = df.describe().T["75%"].iloc[0] - df.describe().T["25%"].iloc[0]
+#             return med, IQR / factor
+
+# def count():
+#     counter = 0
+#     while True:
+#         print(counter)
+#         time.sleep(1)
+#         counter += 1
+def _return_counting_process():
+    import multiprocessing
+
+    def _count():
+        counter = 0
+        while True:
+            print(counter)
+            time.sleep(1)
+            counter += 1
+
+    p1 = multiprocessing.Process(target=_count)
+    p1.start()
+    return p1
+
+
+def wait_key(process, tgt_key="q"):
+    """
+    Example:
+        import mngs
+        p1 = mngs.general._return_counting_process()
+        mngs.gen.wait_key(p1)
+        # press q
+    """
+    pressed_key = None
+    while pressed_key != tgt_key:  # "q"
+        pressed_key = readchar.readchar()
+        print(pressed_key)
+    process.terminate()
+
+
+class ThreadWithReturnValue(threading.Thread):
+    """
+    Example:
+        t = ThreadWithReturnValue(
+            target=func, args=(,), kwargs={key: val}
+        )
+        t.start()
+        out = t.join()
+    
+    """
+    def __init__(
+        self, group=None, target=None, name=None, args=(), kwargs={}, Verbose=None
+    ):
+        Thread.__init__(self, group, target, name, args, kwargs)
+        self._return = None
+
+    def run(self):
+        if self._target is not None:
+            self._return = self._target(*self._args, **self._kwargs)
+
+    def join(self, *args):
+        ### fixme
+        Thread.join(self, *args)
+        return self._return
```

### Comparing `mngs-0.2.5/src/mngs/general/pandas.py` & `mngs-0.4.0/src/mngs/general/pandas.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/path.py` & `mngs-0.4.0/src/mngs/general/path.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/repro.py` & `mngs-0.4.0/src/mngs/general/repro.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/general/save.py` & `mngs-0.4.0/src/mngs/general/save.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import csv
 
 import pandas as pd
 import mngs
 import numpy as np
+import scipy
 
 import warnings
 
 
 if "general" in __file__:
     with warnings.catch_warnings():
         warnings.simplefilter("always")
@@ -129,14 +130,18 @@
             with h5py.File(spath, "w") as hf:
                 for (name, obj) in zip(name_list, obj_list):
                     hf.create_dataset(name, data=obj)
         # pth
         elif spath.endswith(".pth"):
             torch.save(obj, spath)
 
+        # mat
+        elif spath.endswith(".mat"):
+            scipy.io.savemat(spath, obj)
+
         # catboost model
         elif spath.endswith(".cbm"):
             obj.save_model(spath)
 
         else:
             raise ValueError("obj was not saved.")
```

### Comparing `mngs-0.2.5/src/mngs/general/torch.py` & `mngs-0.4.0/src/mngs/general/torch.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/io/load.py` & `mngs-0.4.0/src/mngs/io/load.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,27 @@
     import pickle
 
     import h5py
     import numpy as np
     import pandas as pd
     import torch
     import yaml
+    import mne
 
     # csv
     if lpath.endswith(".csv"):
         obj = pd.read_csv(lpath, **kwargs)
+    # excel
+    if (
+        lpath.endswith(".xls")
+        or lpath.endswith(".xlsx")
+        or lpath.endswith(".xlsm")
+        or lpath.endswith(".xlsb")
+    ):
+        obj = pd.read_excel(lpath, **kwargs)
     # numpy
     if lpath.endswith(".npy"):
         obj = np.load(lpath)
     # pkl
     if lpath.endswith(".pkl"):
         with open(lpath, "rb") as l:
             obj = pickle.load(l)
@@ -58,35 +67,48 @@
             obj.update(obj_tmp)
     # txt
     if lpath.endswith(".txt"):
         f = open(lpath, "r")
         obj = [l.strip("\n\r") for l in f]
         f.close()
     # pth
-    if lpath.endswith(".pth"):
+    if lpath.endswith(".pth") or lpath.endswith(".pt"):
         # return model.load_state_dict(torch.load(lpath))
         obj = torch.load(lpath)
 
+    # mat
     if lpath.endswith(".mat"):
         import pymatreader
 
         obj = pymatreader.read_mat(lpath)
     # xml
     if lpath.endswith("xml"):
         from ._xml2dict import xml2dict
 
         obj = xml2dict(lpath)
+    # edf
+    if lpath.endswith("edf"):
+        obj = mne.io.read_raw_edf(lpath)
+    # con    
+    if lpath.endswith("con"):
+        _obj = mne.io.read_raw(lpath)
+        obj = _obj.to_data_frame()
+        obj["samp_rate"] = _obj.info.get("sfreq")
+    # mrk
+    if lpath.endswith("mrk"):
+        obj = mne.io.kit.read_mrk(lpath)
 
     # catboost model
     if lpath.endswith(".cbm"):
         obj = obj.load_model(lpath)
-        
+
     # if mngs.general.is_defined_local("obj"):
     if "obj" in locals():
-        print("\nLoaded from: {}\n".format(lpath))
+        if show:
+            print("\nLoaded from: {}\n".format(lpath))
         return obj
     else:
         return None
 
 
 def check_encoding(file_path):
     from chardet.universaldetector import UniversalDetector
@@ -108,43 +130,44 @@
     import sys
 
     spec = importlib.util.find_spec(package_str)
     data_dir = os.path.join(spec.origin.split("src")[0], "data")
     resource_path = os.path.join(data_dir, resource)
     return resource_path
 
+
 def load_yaml_as_an_optuna_dict(fpath_yaml, trial):
-    _d = load(fpath_yaml)    
-    
+    _d = load(fpath_yaml)
+
     for k, v in _d.items():
-        
+
         dist = v["distribution"]
 
         if dist == "categorical":
             _d[k] = trial.suggest_categorical(k, v["values"])
 
         elif dist == "uniform":
             _d[k] = trial.suggest_int(k, float(v["min"]), float(v["max"]))
-            
+
         elif dist == "loguniform":
             _d[k] = trial.suggest_loguniform(k, float(v["min"]), float(v["max"]))
 
         elif dist == "intloguniform":
             _d[k] = trial.suggest_int(k, float(v["min"]), float(v["max"]), log=True)
-            
+
     return _d
 
+
 def load_study_rdb(study_name, rdb_raw_bytes_url):
     """
     study = load_study_rdb(
         study_name="YOUR_STUDY_NAME",
         rdb_raw_bytes_url="sqlite:///*.db"
     )
     """
     import optuna
+
     # rdb_raw_bytes_url = "sqlite:////tmp/fake/ywatanabe/_MicroNN_WindowSize-1.0-sec_MaxEpochs_100_2021-1216-1844/optuna_study_test_file#0.db"
     storage = optuna.storages.RDBStorage(url=rdb_raw_bytes_url)
     study = optuna.load_study(study_name=study_name, storage=storage)
     print(f"\nLoaded: {rdb_raw_bytes_url}\n")
     return study
-    
-
```

### Comparing `mngs-0.2.5/src/mngs/io/path.py` & `mngs-0.4.0/src/mngs/io/path.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/io/save.py` & `mngs-0.4.0/src/mngs/io/save.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import csv
 
 import pandas as pd
 import mngs
 import numpy as np
+import scipy
 
 import warnings
 
 
 if "general" in __file__:
     with warnings.catch_warnings():
         warnings.simplefilter("always")
@@ -129,14 +130,18 @@
             with h5py.File(spath, "w") as hf:
                 for (name, obj) in zip(name_list, obj_list):
                     hf.create_dataset(name, data=obj)
         # pth
         elif spath.endswith(".pth"):
             torch.save(obj, spath)
 
+        # mat
+        elif spath.endswith(".mat"):
+            scipy.io.savemat(spath, obj)
+
         # catboost model
         elif spath.endswith(".cbm"):
             obj.save_model(spath)
 
         else:
             raise ValueError("obj was not saved.")
```

### Comparing `mngs-0.2.5/src/mngs/ml/ClassifierServer.py` & `mngs-0.4.0/src/mngs/ml/ClassifierServer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2021-12-12 14:45:57 (ywatanabe)"
+# Time-stamp: "2022-11-01 18:46:25 (ywatanabe)"
 
 
-from catboost import CatBoostClassifier
+# from catboost import CatBoostClassifier
 from sklearn.discriminant_analysis import QuadraticDiscriminantAnalysis
 from sklearn.ensemble import AdaBoostClassifier
 from sklearn.gaussian_process import GaussianProcessClassifier
 from sklearn.linear_model import (
     LogisticRegression,
     PassiveAggressiveClassifier,
     Perceptron,
```

### Comparing `mngs-0.2.5/src/mngs/ml/EarlyStopping.py` & `mngs-0.4.0/src/mngs/ml/EarlyStopping.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/LearningCurveLogger.py` & `mngs-0.4.0/src/mngs/ml/LearningCurveLogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         ## delete here in the future
         ## rename "gt_label" to "true_class"
         if "gt_label" in dict_to_log.keys():
             dict_to_log["true_class"] = dict_to_log.pop("gt_label")
             # del dict_to_log["gt_label"]
         ########################################
 
-        assert step in ["Training", "Validation", "Test"]
+        # assert step in ["Training", "Validation", "Test"]
 
         ## Initialize self.logged_dict
         for k_to_log in dict_to_log.keys():
             try:
                 self.logged_dict[step][k_to_log].append(dict_to_log[k_to_log])
             except:
                 self.logged_dict[step].update({k_to_log: []})
@@ -64,21 +64,20 @@
             pivot_column=None,
         )
 
     def get_x_of_i_epoch(self, x, step, i_epoch):
         """
         lc_logger.get_x_of_i_epoch("true_label_diag", "Validation", 3)
         """
-        assert step in ['Training', "Validation", "Test"]
-        indi = np.array(self.logged_dict[step]['i_epoch']) == i_epoch
+        # assert step in ['Training', "Validation", "Test"]
+        indi = np.array(self.logged_dict[step]["i_epoch"]) == i_epoch
         x_all_arr = np.array(self.logged_dict[step][x])
         assert len(indi) == len(x_all_arr)
         return x_all_arr[indi]
 
-
     def plot_learning_curves(
         self,
         plt,
         plt_config_dict=None,
         title=None,
         max_n_ticks=4,
         linewidth=1,
@@ -120,15 +119,16 @@
 
             if re.search("[aA][cC][cC]", plt_k):  # acc, ylim, yticks
                 ax.set_ylim(0, 1)
                 ax.set_yticks([0, 0.5, 1.0])
 
             for step_k in self.dfs_pivot_i_global.keys():
 
-                if step_k == "Training":  # line
+                if step_k == re.search("^[Tt]rain", step_k):  # line
+                    # if step_k == "Training":  # line
                     ax.plot(
                         self.dfs_pivot_i_global[step_k].index,
                         self.dfs_pivot_i_global[step_k][plt_k],
                         label=step_k,
                         color=mngs.plt.colors.to_RGBA(COLOR_DICT[step_k], alpha=0.9),
                         linewidth=linewidth,
                     )
@@ -151,19 +151,19 @@
                         ax.axvline(
                             x=i_global_epoch_start,
                             ymin=-1e4,  # ax.get_ylim()[0],
                             ymax=1e4,  # ax.get_ylim()[1],
                             linestyle="--",
                             color=mngs.plt.colors.to_RGBA("gray", alpha=0.5),
                         )
-                        ax.text(
-                            i_global_epoch_start,
-                            ax.get_ylim()[1] * 1.0,
-                            f"epoch#{i_epoch}",
-                        )
+                        # ax.text(
+                        #     i_global_epoch_start,
+                        #     ax.get_ylim()[1] * 1.0,
+                        #     f"epoch#{i_epoch}",
+                        # )
                     ########################################
 
                 if (step_k == "Validation") or (step_k == "Test"):  # scatter
                     ax.scatter(
                         self.dfs_pivot_i_global[step_k].index,
                         self.dfs_pivot_i_global[step_k][plt_k],
                         label=step_k,
@@ -182,29 +182,29 @@
             df_pivot_i_epoch_step.columns
         )
         print("\n----------------------------------------\n")
         print(f"\n{step}: (mean of batches)\n")
         pprint(df_pivot_i_epoch_step)
         print("\n----------------------------------------\n")
 
-
     @staticmethod
     def _find_keys_to_plot(logged_dict):
         _steps_str = list(logged_dict.keys())
         _, keys_to_plot = mngs.general.search(
             "_plot",
             list(logged_dict[_steps_str[0]].keys()),
         )
         return keys_to_plot
 
     @staticmethod
     def _rename_if_key_to_plot(keys):
         def _rename_key_to_plot(key_to_plot):
-            renamed = key_to_plot[:-5]
-            renamed = renamed.replace("_", " ")
+            # renamed = key_to_plot[:-5]
+            renamed = re.sub("_plot", "", key_to_plot).replace("_", " ")
+            # renamed = renamed.replace("_", " ")
             capitalized = []
             for s in renamed.split(" "):
                 if not re.search("^[A-Z]", s):
                     capitalized.append(s.capitalize())
                 else:
                     capitalized.append(s)
             renamed = mngs.general.connect_strs(capitalized, filler=" ")
```

### Comparing `mngs-0.2.5/src/mngs/ml/loss/MultiTaskLoss.py` & `mngs-0.4.0/src/mngs/ml/loss/MultiTaskLoss.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/loss/_L1L2Losses.py` & `mngs-0.4.0/src/mngs/ml/loss/_L1L2Losses.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py` & `mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py` & `mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py` & `mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py` & `mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py` & `mngs-0.4.0/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/optim/_get_set.py` & `mngs-0.4.0/src/mngs/ml/optim/_get_set.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/plt/aucs/example.py` & `mngs-0.4.0/src/mngs/ml/plt/aucs/example.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/plt/aucs/pre_rec_auc.py` & `mngs-0.4.0/src/mngs/ml/plt/aucs/pre_rec_auc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 
+import warnings
 from itertools import cycle
 
 import numpy as np
 from sklearn.metrics import average_precision_score, precision_recall_curve
 
 
 def solve_the_intersection_of_a_line_and_iso_f1_curve(f1, a, b):
@@ -13,73 +14,89 @@
         2) the iso-f1 curve: y = f1 * x / (2 * x - f1)
     , where a, b, and f1 are the constant values.
     """
     _a = 2 * a
     _b = -a * f1 + 2 * b - f1
     _c = -b * f1
 
-    x_f = (-_b + np.sqrt(_b ** 2 - 4 * _a * _c)) / (2 * _a)
+    x_f = (-_b + np.sqrt(_b**2 - 4 * _a * _c)) / (2 * _a)
     y_f = a * x_f + b
 
     return (x_f, y_f)
 
 
+def to_onehot(labels, n_classes):
+    eye = np.eye(n_classes, dtype=int)
+    return eye[labels]
+
+
 def pre_rec_auc(plt, true_class, pred_proba, labels):
     """
     Calculates the precision recall curve.
     """
-    ## One-hot encoding
-    def to_onehot(labels, n_classes):
-        eye = np.eye(n_classes, dtype=int)
-        return eye[labels]
 
     # Use label_binarize to be multi-label like settings
     n_classes = len(labels)
-    true_class = to_onehot(true_class, n_classes)
+    true_class_onehot = to_onehot(true_class, n_classes)
 
     # For each class
     precision = dict()
     recall = dict()
     threshold = dict()
     pre_rec_auc = dict()
     for i in range(n_classes):
-        precision[i], recall[i], threshold[i] = precision_recall_curve(
-            true_class[:, i], pred_proba[:, i]
-        )
-        pre_rec_auc[i] = average_precision_score(true_class[:, i], pred_proba[:, i])
+        true_class_i_onehot = true_class_onehot[:, i]
+        pred_proba_i = pred_proba[:, i]
+
+        try:
+            precision[i], recall[i], threshold[i] = precision_recall_curve(
+                true_class_i_onehot,
+                pred_proba_i,
+            )
+            pre_rec_auc[i] = average_precision_score(true_class_i_onehot, pred_proba_i)
+        except Exception as e:
+            print(e)
+            precision[i], recall[i], threshold[i], pre_rec_auc[i] = (
+                np.nan,
+                np.nan,
+                np.nan,
+                np.nan,
+            )
 
-    ################################################################################
     ## Average precision: micro and macro
-    ################################################################################
+
     # A "micro-average": quantifying score on all classes jointly
     precision["micro"], recall["micro"], threshold["micro"] = precision_recall_curve(
-        true_class.ravel(), pred_proba.ravel()
+        true_class_onehot.ravel(), pred_proba.ravel()
     )
     pre_rec_auc["micro"] = average_precision_score(
-        true_class, pred_proba, average="micro"
+        true_class_onehot, pred_proba, average="micro"
     )
-    # print(
-    #     "Average precision score, micro-averaged over all classes: {0:0.2f}".format(
-    #         pre_rec_auc["micro"]
-    #     )
-    # )
 
     # macro
-    pre_rec_auc["macro"] = average_precision_score(
-        true_class, pred_proba, average="macro"
-    )
-    # print(
-    #     "Average precision score, macro-averaged over all classes: {0:0.2f}".format(
-    #         pre_rec_auc["macro"]
-    #     )
+    _pre_rec_aucs = []
+    for i in range(n_classes):
+        try:
+            _pre_rec_aucs.append(
+                average_precision_score(
+                    true_class_onehot[:, i], pred_proba[:, i], average="macro"
+                )
+            )
+        except Exception as e:
+            print(
+                f'\nPRE-REC-AUC for "{labels[i]}" was not defined and NaN-filled '
+                "for a calculation purpose (for the macro avg.)\n"
+            )
+            _pre_rec_aucs.append(np.nan)
+    pre_rec_auc["macro"] = np.nanmean(_pre_rec_aucs)
+
+    # pre_rec_auc["macro"] = average_precision_score(
+    #     true_class_onehot, pred_proba, average="macro"
     # )
 
-    ################################################################################
-    ## Plot
-    ################################################################################
     # Plot Precision-Recall curve for each class and iso-f1 curves
     colors = cycle(["navy", "turquoise", "darkorange", "cornflowerblue", "teal"])
     fig, ax = plt.subplots()
     ax.set_box_aspect(1)
     lines = []
     legends = []
```

### Comparing `mngs-0.2.5/src/mngs/ml/plt/confusion_matrix.py` & `mngs-0.4.0/src/mngs/ml/plt/confusion_matrix.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,41 +8,58 @@
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 
 def confusion_matrix(
     plt,
     cm,
     labels=None,
+    pred_labels=None,
+    true_labels=None,
     label_rotation_xy=(0, 0),
     title=None,
     colorbar=True,
-    extend_ratio=1.0,
+    x_extend_ratio=1.0,
+    y_extend_ratio=1.0,        
 ):
     """
     Inverse the y-axis and plot the confusion matrix as a heatmap.
     The predicted labels (in x-axis) is symboled with hat (^).
     The plt object is passed to adjust the figure size
 
+    cm = np.random.randint(low=0, high=10, size=[3,4])
+    x: predicted labels
+    y: true_labels
+    
     kwargs:
 
         "extend_ratio":
             Determines how much the axes objects (not the fig object) are extended
             in the vertical direction.
 
     """
-    df = pd.DataFrame(data=cm).copy()
+    df = pd.DataFrame(data=cm).copy().T
     vmax = np.array(df).max().astype(int)
 
-    # x- and y-ticklabels
-    if labels is not None:
-        df.index = [mngs.general.to_the_latex_style(l) for l in labels]  # true labels
-        df.columns = [
-            mngs.general.add_hat_in_the_latex_style(l) for l in labels
-        ]  # predicted labels
-
+    if (labels is not None) and (pred_labels is None):
+        df.columns = [mngs.general.to_the_latex_style(l) for l in labels] # pred_labels
+    if pred_labels is not None:
+        df.columns = [mngs.general.to_the_latex_style(l) for l in pred_labels]
+
+    if (labels is not None) and (true_labels is None):
+        df.index = [mngs.general.to_the_latex_style(l) for l in labels] # true_labels
+    if true_labels is not None:
+        df.index = [mngs.general.to_the_latex_style(l) for l in true_labels]
+        
+    # # x- and y-ticklabels
+    # if labels is not None:
+        
+    #     df.columns = [
+    #         mngs.general.add_hat_in_the_latex_style(l) for l in labels
+    #     ]  # predicted labels
+        
     fig, ax = plt.subplots()
     res = sns.heatmap(
         df,
         annot=True,
         annot_kws={"size": plt.rcParams["font.size"]},
         fmt=".0f",
         cmap="Blues",
@@ -54,23 +71,25 @@
         t.set_text("{:,d}".format(int(t.get_text())))
 
     # Inverts the y-axis
     res.invert_yaxis()
 
     # Makes the frame visible
     for _, spine in res.spines.items():
-        spine.set_visible(True)
+        # spine.set_visible(True)
+        spine.set_visible(False)        
 
     ax.set_xlabel("Predicted label")
     ax.set_ylabel("True label")
     ax.set_title(title)
 
-    ax = mngs.plt.ax_extend(ax, 1, extend_ratio)
+    ax = mngs.plt.ax_extend(ax, x_extend_ratio, y_extend_ratio)
 
-    ax.set_box_aspect(1)
+    if df.shape[0] == df.shape[1]:
+        ax.set_box_aspect(1)
 
     ax.set_xticklabels(
         ax.get_xticklabels(),
         rotation=label_rotation_xy[0],
         fontdict={"verticalalignment": "top"},
     )
 
@@ -83,15 +102,15 @@
     # The size of the confusion matrix
 
     # Calculates the dx
     bbox = ax.get_position()
     left_orig = bbox.x0
     width_orig = bbox.x1 - bbox.x0
     g_x_orig = left_orig + width_orig / 2.0
-    width_tgt = width_orig * extend_ratio  # x_extend_ratio
+    width_tgt = width_orig * x_extend_ratio  # x_extend_ratio
     dx = width_orig - width_tgt
     # print(dx)
 
     """
     The axes objects of the confusion matrix and colorbar are different.
     Here, their sizes are adjusted one by one.
     """
@@ -129,14 +148,16 @@
         cbar = fig.colorbar(
             plt.cm.ScalarMappable(norm=norm, cmap="Blues"),
             cax=cax,
             # shrink=0.68,
         )
         cbar.locator = ticker.MaxNLocator(nbins=4)  # tick_locator
         cbar.update_ticks()
+        # cbar.outline.set_edgecolor("#f9f2d7")
+        cbar.outline.set_edgecolor("white")        
 
     return fig
 
 
 # def AddAxesBBoxRect(fig, ax, ec="k"):
 #     from matplotlib.patches import Rectangle
 
@@ -184,33 +205,39 @@
     classifier = svm.SVC(kernel="linear", C=0.01).fit(X_train, y_train)
 
     ## Checks the confusion_matrix function
     y_pred = classifier.predict(X_test)
     cm = sklearn.metrics.confusion_matrix(y_test, y_pred)
     cm **= 3
 
+    cm = np.random.randint(low=0, high=10, size=[3,4])
+    
     mngs.plt.configure_mpl(
         plt,
         # figsize=(4, 8),
         figsize=(4, 8),
         fontsize=6,
         labelsize=8,
         legendfontsize=7,
         tick_size=0.8,
         tick_width=0.2,
     )
 
-    labels = class_names
+    # labels = class_names
+    pred_labels = ["A", "B", "C"]
+    true_labels = ["a", "b", "c", "d"]    
 
     fig = confusion_matrix(
         plt,
         cm,
-        labels=class_names,
+        # labels=class_names,
+        pred_labels=pred_labels,
+        true_labels=true_labels,
         label_rotation_xy=(60, 60),
-        extend_ratio=0.5,
+        x_extend_ratio=1.,
         colorbar=True,
     )
 
     fig.axes[-1] = mngs.plt.ax_scientific_notation(
         fig.axes[-1],
         3,
         fformat="%3.1f",
```

### Comparing `mngs-0.2.5/src/mngs/ml/silhoute_score_block.py` & `mngs-0.4.0/src/mngs/ml/silhoute_score_block.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/utils/_DefaultDataset.py` & `mngs-0.4.0/src/mngs/ml/utils/_DefaultDataset.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/utils/_format_samples_for_sktime.py` & `mngs-0.4.0/src/mngs/ml/utils/_format_samples_for_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/utils/_get_params.py` & `mngs-0.4.0/src/mngs/ml/utils/_get_params.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/ml/utils/_under_sample.py` & `mngs-0.4.0/src/mngs/ml/utils/_under_sample.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/_ax_extend.py` & `mngs-0.4.0/src/mngs/plt/_ax_extend.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/_ax_scientific_notation.py` & `mngs-0.4.0/src/mngs/plt/_ax_scientific_notation.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/_ax_set_position.py` & `mngs-0.4.0/src/mngs/plt/_ax_set_position.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/_configure_mpl.py` & `mngs-0.4.0/src/mngs/plt/_configure_mpl.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/_draw_a_cube.py` & `mngs-0.4.0/src/mngs/plt/_draw_a_cube.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/_get_RGBA_from_colormap.py` & `mngs-0.4.0/src/mngs/plt/_get_RGBA_from_colormap.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/annotated_heatmap.py` & `mngs-0.4.0/src/mngs/plt/annotated_heatmap.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/plt/get_mpl_color.py` & `mngs-0.4.0/src/mngs/plt/get_mpl_color.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/resource/get.py` & `mngs-0.4.0/src/mngs/resource/get.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/resource/limit_RAM.py` & `mngs-0.4.0/src/mngs/resource/limit_RAM.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/stats/_bonferroni_correction.py` & `mngs-0.4.0/src/mngs/stats/_bonferroni_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/stats/_brunner_munzel_test.py` & `mngs-0.4.0/src/mngs/stats/_brunner_munzel_test.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/stats/_fdr_correction.py` & `mngs-0.4.0/src/mngs/stats/_fdr_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/stats/_multicompair.py` & `mngs-0.4.0/src/mngs/stats/_multicompair.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/stats/_nocorrelation_test.py` & `mngs-0.4.0/src/mngs/stats/_nocorrelation_test.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs/stats/_smirnov_grubbs.py` & `mngs-0.4.0/src/mngs/stats/_smirnov_grubbs.py`

 * *Files identical despite different names*

### Comparing `mngs-0.2.5/src/mngs.egg-info/PKG-INFO` & `mngs-0.4.0/src/mngs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 0.2.5
+Version: 0.4.0
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: GPL3.0
 Keywords: utils,utilities,python,machine learning
 Platform: UNKNOWN
```

### Comparing `mngs-0.2.5/src/mngs.egg-info/SOURCES.txt` & `mngs-0.4.0/src/mngs.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 src/mngs.egg-info/top_level.txt
 src/mngs/dsp/BandPassFiltering.py
 src/mngs/dsp/FeatureExtractor.py
 src/mngs/dsp/HilbertTransformation.py
 src/mngs/dsp/_BANDS_LIM_HZ_DICT.py
 src/mngs/dsp/__init__.py
 src/mngs/dsp/_bandpassfilter.py
+src/mngs/dsp/_common_average.py
+src/mngs/dsp/_gaussian_filter1d.py
+src/mngs/dsp/_normalize_time.py
+src/mngs/dsp/_take_random_references.py
 src/mngs/dsp/feature_extractions.py
-src/mngs/dsp/fft_powers.py
+src/mngs/dsp/fft_amps.py
 src/mngs/dsp/wavelet.py
 src/mngs/general/TimeStamper.py
 src/mngs/general/__init__.py
 src/mngs/general/_xml2dict.py
 src/mngs/general/cuda_collect_env.py
 src/mngs/general/debug.py
 src/mngs/general/latex.py
@@ -32,19 +36,20 @@
 src/mngs/general/repro.py
 src/mngs/general/save.py
 src/mngs/general/torch.py
 src/mngs/io/__init__.py
 src/mngs/io/load.py
 src/mngs/io/path.py
 src/mngs/io/save.py
+src/mngs/linalg/__init__.py
+src/mngs/linalg/_misc.py
 src/mngs/ml/ClassificationReporter.py
 src/mngs/ml/ClassifierServer.py
 src/mngs/ml/EarlyStopping.py
 src/mngs/ml/LearningCurveLogger.py
-src/mngs/ml/__Classifiers.py
 src/mngs/ml/__init__.py
 src/mngs/ml/silhoute_score_block.py
 src/mngs/ml/act/__init__.py
 src/mngs/ml/act/_define.py
 src/mngs/ml/layer/_Pass.py
 src/mngs/ml/layer/__init__.py
 src/mngs/ml/layer/_switch.py
@@ -69,31 +74,44 @@
 src/mngs/ml/utils/_DefaultDataset.py
 src/mngs/ml/utils/__init__.py
 src/mngs/ml/utils/_format_samples_for_sktime.py
 src/mngs/ml/utils/_get_params.py
 src/mngs/ml/utils/_merge_labels.py
 src/mngs/ml/utils/_under_sample.py
 src/mngs/ml/utils/_verify_n_gpus.py
+src/mngs/nn/_BNet.py
+src/mngs/nn/_ChannelGainChanger.py
+src/mngs/nn/_FreqGainChanger.py
+src/mngs/nn/_MNet_1000.py
+src/mngs/nn/_SpatialAttention.py
+src/mngs/nn/_SwapChannels.py
+src/mngs/nn/__init__.py
 src/mngs/plt/__init__.py
+src/mngs/plt/_add_hue.py
+src/mngs/plt/_ax_circular_hist.py
 src/mngs/plt/_ax_extend.py
+src/mngs/plt/_ax_fill_between.py
 src/mngs/plt/_ax_scientific_notation.py
 src/mngs/plt/_ax_set_n_ticks.py
 src/mngs/plt/_ax_set_position.py
+src/mngs/plt/_ax_set_size.py
 src/mngs/plt/_configure_mpl.py
 src/mngs/plt/_draw_a_cube.py
 src/mngs/plt/_get_RGBA_from_colormap.py
+src/mngs/plt/_mk_colorbar.py
 src/mngs/plt/_mk_patches.py
 src/mngs/plt/annotated_heatmap.py
 src/mngs/plt/colors.py
 src/mngs/plt/get_mpl_color.py
 src/mngs/resource/__init__.py
 src/mngs/resource/get.py
 src/mngs/resource/limit_RAM.py
 src/mngs/stats/__init__.py
 src/mngs/stats/_bonferroni_correction.py
 src/mngs/stats/_brunner_munzel_test.py
 src/mngs/stats/_calc_partial_corr.py
+src/mngs/stats/_corr_test.py
 src/mngs/stats/_fdr_correction.py
 src/mngs/stats/_multicompair.py
 src/mngs/stats/_nocorrelation_test.py
 src/mngs/stats/_smirnov_grubbs.py
-test/test_import_mngs.py
+src/mngs/stats/_to_asterisks.py
```

