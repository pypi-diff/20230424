# Comparing `tmp/dvclive-2.6.4.tar.gz` & `tmp/dvclive-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvclive-2.6.4.tar", last modified: Fri Apr 14 17:58:46 2023, max compression
+gzip compressed data, was "dvclive-2.7.0.tar", last modified: Mon Apr 24 08:54:15 2023, max compression
```

## Comparing `dvclive-2.6.4.tar` & `dvclive-2.7.0.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 17:58:33.000000 dvclive-2.6.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:58:33.000000 dvclive-2.6.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.097698 dvclive-2.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.097698 dvclive-2.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 17:58:33.000000 dvclive-2.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-14 17:58:33.000000 dvclive-2.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-14 17:58:33.000000 dvclive-2.6.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-14 17:58:33.000000 dvclive-2.6.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-14 17:58:33.000000 dvclive-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-14 17:58:46.105698 dvclive-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-14 17:58:33.000000 dvclive-2.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.097698 dvclive-2.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/dvc_plots_diff.png
--rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/studio_compare.png
--rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/vscode_experiments.png
--rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/vscode_plots.png
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-14 17:58:33.000000 dvclive-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 17:58:46.105698 dvclive-2.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 17:58:33.000000 dvclive-2.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.093698 dvclive-2.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.101698 dvclive-2.6.4/src/dvclive/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/optuna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/src/dvclive/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.101698 dvclive-2.6.4/src/dvclive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:58:45.000000 dvclive-2.6.4/src/dvclive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/plots/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/plots/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/plots/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/tests/test_frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_log_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.291425 dvclive-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-24 08:54:03.000000 dvclive-2.7.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 08:54:03.000000 dvclive-2.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.279425 dvclive-2.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.283425 dvclive-2.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 08:54:03.000000 dvclive-2.7.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-24 08:54:03.000000 dvclive-2.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-24 08:54:03.000000 dvclive-2.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-24 08:54:03.000000 dvclive-2.7.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 08:54:03.000000 dvclive-2.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-24 08:54:03.000000 dvclive-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-24 08:54:15.291425 dvclive-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 08:54:03.000000 dvclive-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.283425 dvclive-2.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/dvc_plots_diff.png
+-rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/studio_compare.png
+-rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/vscode_experiments.png
+-rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-04-24 08:54:03.000000 dvclive-2.7.0/docs/vscode_plots.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.283425 dvclive-2.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-24 08:54:03.000000 dvclive-2.7.0/examples/DVCLive-Quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-24 08:54:03.000000 dvclive-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-24 08:54:15.291425 dvclive-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 08:54:03.000000 dvclive-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.279425 dvclive-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/src/dvclive/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19834 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/optuna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/src/dvclive/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/plots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-24 08:54:03.000000 dvclive-2.7.0/src/dvclive/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/src/dvclive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 08:54:15.000000 dvclive-2.7.0/src/dvclive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.287425 dvclive-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.291425 dvclive-2.7.0/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/plots/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/plots/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/plots/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:15.291425 dvclive-2.7.0/tests/test_frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_frameworks/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_log_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 08:54:03.000000 dvclive-2.7.0/tests/test_utils.py
```

### Comparing `dvclive-2.6.4/.cruft.json` & `dvclive-2.7.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/.github/dependabot.yml` & `dvclive-2.7.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/.github/workflows/release.yml` & `dvclive-2.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/.github/workflows/tests.yml` & `dvclive-2.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/.gitignore` & `dvclive-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/.pre-commit-config.yaml` & `dvclive-2.7.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
     rev: 'v0.0.261'
     hooks:
```

### Comparing `dvclive-2.6.4/CODE_OF_CONDUCT.rst` & `dvclive-2.7.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/CONTRIBUTING.rst` & `dvclive-2.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/LICENSE` & `dvclive-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/PKG-INFO` & `dvclive-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6476 636c  : 2.1.Name: dvcl
-00000020: 6976 650a 5665 7273 696f 6e3a 2032 2e36  ive.Version: 2.6
-00000030: 2e34 0a53 756d 6d61 7279 3a20 4d65 7472  .4.Summary: Metr
+00000020: 6976 650a 5665 7273 696f 6e3a 2032 2e37  ive.Version: 2.7
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4d65 7472  .0.Summary: Metr
 00000040: 6963 206c 6f67 6765 7220 666f 7220 4d4c  ic logger for ML
 00000050: 2070 726f 6a65 6374 732e 0a48 6f6d 652d   projects..Home-
 00000060: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000070: 7468 7562 2e63 6f6d 2f69 7465 7261 7469  thub.com/iterati
 00000080: 7665 2f64 7663 6c69 7665 0a4d 6169 6e74  ve/dvclive.Maint
 00000090: 6169 6e65 722d 656d 6169 6c3a 2073 7570  ainer-email: sup
 000000a0: 706f 7274 4064 7663 2e6f 7267 0a4c 6963  port@dvc.org.Lic
@@ -154,323 +154,337 @@
 00000990: 672f 646f 632f 6476 636c 6976 652f 6d6c  g/doc/dvclive/ml
 000009a0: 2d66 7261 6d65 776f 726b 7329 0a0a 5f5f  -frameworks)..__
 000009b0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009c0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009d0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009e0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009f0: 5f5f 5f5f 0a0a 2320 5175 6963 6b73 7461  ____..# Quicksta
-00000a00: 7274 0a0a 2323 2049 6e73 7461 6c6c 202a  rt..## Install *
-00000a10: 6476 636c 6976 652a 0a0a 6060 6063 6f6e  dvclive*..```con
-00000a20: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
-00000a30: 6c6c 2064 7663 6c69 7665 0a60 6060 0a0a  ll dvclive.```..
-00000a40: 2323 2049 6e69 7469 616c 697a 6520 4456  ## Initialize DV
-00000a50: 4320 5265 706f 7369 746f 7279 0a0a 6060  C Repository..``
-00000a60: 6063 6f6e 736f 6c65 0a24 2067 6974 2069  `console.$ git i
-00000a70: 6e69 740a 2420 6476 6320 696e 6974 0a24  nit.$ dvc init.$
-00000a80: 2067 6974 2063 6f6d 6d69 7420 2d6d 2022   git commit -m "
-00000a90: 4456 4320 696e 6974 220a 6060 600a 0a23  DVC init".```..#
-00000aa0: 2320 4578 616d 706c 6520 636f 6465 0a0a  # Example code..
-00000ab0: 436f 7079 2074 6865 2073 6e69 7070 6574  Copy the snippet
-00000ac0: 2062 656c 6f77 2061 7320 6120 6261 7369   below as a basi
-00000ad0: 6320 6578 616d 706c 6520 6f66 2074 6865  c example of the
-00000ae0: 2041 5049 2075 7361 6765 3a0a 0a60 6060   API usage:..```
-00000af0: 7079 7468 6f6e 0a23 2074 7261 696e 2e70  python.# train.p
-00000b00: 790a 696d 706f 7274 2072 616e 646f 6d0a  y.import random.
-00000b10: 696d 706f 7274 2073 7973 0a66 726f 6d20  import sys.from 
-00000b20: 6476 636c 6976 6520 696d 706f 7274 204c  dvclive import L
-00000b30: 6976 650a 0a77 6974 6820 4c69 7665 2873  ive..with Live(s
-00000b40: 6176 655f 6476 635f 6578 703d 5472 7565  ave_dvc_exp=True
-00000b50: 2920 6173 206c 6976 653a 0a20 2020 2065  ) as live:.    e
-00000b60: 706f 6368 7320 3d20 696e 7428 7379 732e  pochs = int(sys.
-00000b70: 6172 6776 5b31 5d29 0a20 2020 206c 6976  argv[1]).    liv
-00000b80: 652e 6c6f 675f 7061 7261 6d28 2265 706f  e.log_param("epo
-00000b90: 6368 7322 2c20 6570 6f63 6873 290a 2020  chs", epochs).  
-00000ba0: 2020 666f 7220 6570 6f63 6820 696e 2072    for epoch in r
-00000bb0: 616e 6765 2865 706f 6368 7329 3a0a 2020  ange(epochs):.  
-00000bc0: 2020 2020 2020 6c69 7665 2e6c 6f67 5f6d        live.log_m
-00000bd0: 6574 7269 6328 2274 7261 696e 2f61 6363  etric("train/acc
-00000be0: 7572 6163 7922 2c20 6570 6f63 6820 2b20  uracy", epoch + 
-00000bf0: 7261 6e64 6f6d 2e72 616e 646f 6d28 2929  random.random())
-00000c00: 0a20 2020 2020 2020 206c 6976 652e 6c6f  .        live.lo
-00000c10: 675f 6d65 7472 6963 2822 7472 6169 6e2f  g_metric("train/
-00000c20: 6c6f 7373 222c 2065 706f 6368 7320 2d20  loss", epochs - 
-00000c30: 6570 6f63 6820 2d20 7261 6e64 6f6d 2e72  epoch - random.r
-00000c40: 616e 646f 6d28 2929 0a20 2020 2020 2020  andom()).       
-00000c50: 206c 6976 652e 6c6f 675f 6d65 7472 6963   live.log_metric
-00000c60: 2822 7661 6c2f 6163 6375 7261 6379 222c  ("val/accuracy",
-00000c70: 6570 6f63 6820 2b20 7261 6e64 6f6d 2e72  epoch + random.r
-00000c80: 616e 646f 6d28 2920 290a 2020 2020 2020  andom() ).      
-00000c90: 2020 6c69 7665 2e6c 6f67 5f6d 6574 7269    live.log_metri
-00000ca0: 6328 2276 616c 2f6c 6f73 7322 2c20 6570  c("val/loss", ep
-00000cb0: 6f63 6873 202d 2065 706f 6368 202d 2072  ochs - epoch - r
-00000cc0: 616e 646f 6d2e 7261 6e64 6f6d 2829 290a  andom.random()).
-00000cd0: 2020 2020 2020 2020 6c69 7665 2e6e 6578          live.nex
-00000ce0: 745f 7374 6570 2829 0a60 6060 0a0a 5365  t_step().```..Se
-00000cf0: 6520 5b49 6e74 6567 7261 7469 6f6e 735d  e [Integrations]
-00000d00: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
-00000d10: 2f64 6f63 2f64 7663 6c69 7665 2f6d 6c2d  /doc/dvclive/ml-
-00000d20: 6672 616d 6577 6f72 6b73 2920 666f 7220  frameworks) for 
-00000d30: 6578 616d 706c 6573 2075 7369 6e67 0a44  examples using.D
-00000d40: 5643 4c69 7665 2061 6c6f 6e67 7369 6465  VCLive alongside
-00000d50: 2064 6966 6665 7265 6e74 204d 4c20 4672   different ML Fr
-00000d60: 616d 6577 6f72 6b73 2e0a 0a23 2320 5275  ameworks...## Ru
-00000d70: 6e6e 696e 670a 0a52 756e 2063 6f75 706c  nning..Run coupl
-00000d80: 6520 6f66 2074 696d 6573 2070 6173 7369  e of times passi
-00000d90: 6e67 2064 6966 6665 7265 6e74 2076 616c  ng different val
-00000da0: 7565 733a 0a0a 6060 6063 6f6e 736f 6c65  ues:..```console
-00000db0: 0a24 2070 7974 686f 6e20 7472 6169 6e2e  .$ python train.
-00000dc0: 7079 2035 0a24 2070 7974 686f 6e20 7472  py 5.$ python tr
-00000dd0: 6169 6e2e 7079 2035 0a24 2070 7974 686f  ain.py 5.$ pytho
-00000de0: 6e20 7472 6169 6e2e 7079 2037 0a60 6060  n train.py 7.```
-00000df0: 0a0a 2323 2043 6f6d 7061 7269 6e67 0a0a  ..## Comparing..
-00000e00: 4456 434c 6976 6520 6f75 7470 7574 7320  DVCLive outputs 
-00000e10: 6361 6e20 6265 2072 656e 6465 7265 6420  can be rendered 
-00000e20: 696e 2064 6966 6665 7265 6e74 2077 6179  in different way
-00000e30: 733a 0a0a 2323 2320 4456 4320 434c 490a  s:..### DVC CLI.
-00000e40: 0a59 6f75 2063 616e 2075 7365 205b 6476  .You can use [dv
-00000e50: 6320 6578 7020 7368 6f77 5d28 6874 7470  c exp show](http
-00000e60: 733a 2f2f 6476 632e 6f72 672f 646f 632f  s://dvc.org/doc/
-00000e70: 636f 6d6d 616e 642d 7265 6665 7265 6e63  command-referenc
-00000e80: 652f 6578 702f 7368 6f77 2920 616e 640a  e/exp/show) and.
-00000e90: 5b64 7663 2070 6c6f 7473 5d28 6874 7470  [dvc plots](http
-00000ea0: 733a 2f2f 6476 632e 6f72 672f 646f 632f  s://dvc.org/doc/
-00000eb0: 636f 6d6d 616e 642d 7265 6665 7265 6e63  command-referenc
-00000ec0: 652f 706c 6f74 7329 2074 6f20 636f 6d70  e/plots) to comp
-00000ed0: 6172 6520 616e 640a 7669 7375 616c 697a  are and.visualiz
-00000ee0: 6520 6d65 7472 6963 732c 2070 6172 616d  e metrics, param
-00000ef0: 6574 6572 7320 616e 6420 706c 6f74 7320  eters and plots 
-00000f00: 6163 726f 7373 2065 7870 6572 696d 656e  across experimen
-00000f10: 7473 3a0a 0a60 6060 636f 6e73 6f6c 650a  ts:..```console.
-00000f20: 2420 6476 6320 6578 7020 7368 6f77 0a60  $ dvc exp show.`
-00000f30: 6060 0a0a 6060 600a e294 80e2 9480 e294  ``..```.........
-00000f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000f50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000f60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000f70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000f80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000f90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000fa0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000fb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000fc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000fd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000fe0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000ff0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001000: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000a00: 7274 0a0a 3c70 2061 6c69 676e 3d27 6365  rt..<p align='ce
+00000a10: 6e74 6572 273e 0a3c 6120 6872 6566 3d22  nter'>.<a href="
+00000a20: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00000a30: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00000a40: 6d2f 6769 7468 7562 2f69 7465 7261 7469  m/github/iterati
+00000a50: 7665 2f64 7663 6c69 7665 2f62 6c6f 622f  ve/dvclive/blob/
+00000a60: 6d61 696e 2f65 7861 6d70 6c65 732f 4456  main/examples/DV
+00000a70: 434c 6976 652d 5175 6963 6b73 7461 7274  CLive-Quickstart
+00000a80: 2e69 7079 6e62 223e 3c69 6d67 2073 7263  .ipynb"><img src
+00000a90: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
+00000aa0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00000ab0: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+00000ac0: 2d62 6164 6765 2e73 7667 2220 2f3e 3c2f  -badge.svg" /></
+00000ad0: 613e 0a3c 2f70 3e0a 0a23 2320 496e 7374  a>.</p>..## Inst
+00000ae0: 616c 6c20 2a64 7663 6c69 7665 2a0a 0a60  all *dvclive*..`
+00000af0: 6060 636f 6e73 6f6c 650a 2420 7069 7020  ``console.$ pip 
+00000b00: 696e 7374 616c 6c20 6476 636c 6976 650a  install dvclive.
+00000b10: 6060 600a 0a23 2320 496e 6974 6961 6c69  ```..## Initiali
+00000b20: 7a65 2044 5643 2052 6570 6f73 6974 6f72  ze DVC Repositor
+00000b30: 790a 0a60 6060 636f 6e73 6f6c 650a 2420  y..```console.$ 
+00000b40: 6769 7420 696e 6974 0a24 2064 7663 2069  git init.$ dvc i
+00000b50: 6e69 740a 2420 6769 7420 636f 6d6d 6974  nit.$ git commit
+00000b60: 202d 6d20 2244 5643 2069 6e69 7422 0a60   -m "DVC init".`
+00000b70: 6060 0a0a 2323 2045 7861 6d70 6c65 2063  ``..## Example c
+00000b80: 6f64 650a 0a43 6f70 7920 7468 6520 736e  ode..Copy the sn
+00000b90: 6970 7065 7420 6265 6c6f 7720 6173 2061  ippet below as a
+00000ba0: 2062 6173 6963 2065 7861 6d70 6c65 206f   basic example o
+00000bb0: 6620 7468 6520 4150 4920 7573 6167 653a  f the API usage:
+00000bc0: 0a0a 6060 6070 7974 686f 6e0a 2320 7472  ..```python.# tr
+00000bd0: 6169 6e2e 7079 0a69 6d70 6f72 7420 7261  ain.py.import ra
+00000be0: 6e64 6f6d 0a69 6d70 6f72 7420 7379 730a  ndom.import sys.
+00000bf0: 6672 6f6d 2064 7663 6c69 7665 2069 6d70  from dvclive imp
+00000c00: 6f72 7420 4c69 7665 0a0a 7769 7468 204c  ort Live..with L
+00000c10: 6976 6528 7361 7665 5f64 7663 5f65 7870  ive(save_dvc_exp
+00000c20: 3d54 7275 6529 2061 7320 6c69 7665 3a0a  =True) as live:.
+00000c30: 2020 2020 6570 6f63 6873 203d 2069 6e74      epochs = int
+00000c40: 2873 7973 2e61 7267 765b 315d 290a 2020  (sys.argv[1]).  
+00000c50: 2020 6c69 7665 2e6c 6f67 5f70 6172 616d    live.log_param
+00000c60: 2822 6570 6f63 6873 222c 2065 706f 6368  ("epochs", epoch
+00000c70: 7329 0a20 2020 2066 6f72 2065 706f 6368  s).    for epoch
+00000c80: 2069 6e20 7261 6e67 6528 6570 6f63 6873   in range(epochs
+00000c90: 293a 0a20 2020 2020 2020 206c 6976 652e  ):.        live.
+00000ca0: 6c6f 675f 6d65 7472 6963 2822 7472 6169  log_metric("trai
+00000cb0: 6e2f 6163 6375 7261 6379 222c 2065 706f  n/accuracy", epo
+00000cc0: 6368 202b 2072 616e 646f 6d2e 7261 6e64  ch + random.rand
+00000cd0: 6f6d 2829 290a 2020 2020 2020 2020 6c69  om()).        li
+00000ce0: 7665 2e6c 6f67 5f6d 6574 7269 6328 2274  ve.log_metric("t
+00000cf0: 7261 696e 2f6c 6f73 7322 2c20 6570 6f63  rain/loss", epoc
+00000d00: 6873 202d 2065 706f 6368 202d 2072 616e  hs - epoch - ran
+00000d10: 646f 6d2e 7261 6e64 6f6d 2829 290a 2020  dom.random()).  
+00000d20: 2020 2020 2020 6c69 7665 2e6c 6f67 5f6d        live.log_m
+00000d30: 6574 7269 6328 2276 616c 2f61 6363 7572  etric("val/accur
+00000d40: 6163 7922 2c65 706f 6368 202b 2072 616e  acy",epoch + ran
+00000d50: 646f 6d2e 7261 6e64 6f6d 2829 2029 0a20  dom.random() ). 
+00000d60: 2020 2020 2020 206c 6976 652e 6c6f 675f         live.log_
+00000d70: 6d65 7472 6963 2822 7661 6c2f 6c6f 7373  metric("val/loss
+00000d80: 222c 2065 706f 6368 7320 2d20 6570 6f63  ", epochs - epoc
+00000d90: 6820 2d20 7261 6e64 6f6d 2e72 616e 646f  h - random.rando
+00000da0: 6d28 2929 0a20 2020 2020 2020 206c 6976  m()).        liv
+00000db0: 652e 6e65 7874 5f73 7465 7028 290a 6060  e.next_step().``
+00000dc0: 600a 0a53 6565 205b 496e 7465 6772 6174  `..See [Integrat
+00000dd0: 696f 6e73 5d28 6874 7470 733a 2f2f 6476  ions](https://dv
+00000de0: 632e 6f72 672f 646f 632f 6476 636c 6976  c.org/doc/dvcliv
+00000df0: 652f 6d6c 2d66 7261 6d65 776f 726b 7329  e/ml-frameworks)
+00000e00: 2066 6f72 2065 7861 6d70 6c65 7320 7573   for examples us
+00000e10: 696e 670a 4456 434c 6976 6520 616c 6f6e  ing.DVCLive alon
+00000e20: 6773 6964 6520 6469 6666 6572 656e 7420  gside different 
+00000e30: 4d4c 2046 7261 6d65 776f 726b 732e 0a0a  ML Frameworks...
+00000e40: 2323 2052 756e 6e69 6e67 0a0a 5275 6e20  ## Running..Run 
+00000e50: 636f 7570 6c65 206f 6620 7469 6d65 7320  couple of times 
+00000e60: 7061 7373 696e 6720 6469 6666 6572 656e  passing differen
+00000e70: 7420 7661 6c75 6573 3a0a 0a60 6060 636f  t values:..```co
+00000e80: 6e73 6f6c 650a 2420 7079 7468 6f6e 2074  nsole.$ python t
+00000e90: 7261 696e 2e70 7920 350a 2420 7079 7468  rain.py 5.$ pyth
+00000ea0: 6f6e 2074 7261 696e 2e70 7920 350a 2420  on train.py 5.$ 
+00000eb0: 7079 7468 6f6e 2074 7261 696e 2e70 7920  python train.py 
+00000ec0: 370a 6060 600a 0a23 2320 436f 6d70 6172  7.```..## Compar
+00000ed0: 696e 670a 0a44 5643 4c69 7665 206f 7574  ing..DVCLive out
+00000ee0: 7075 7473 2063 616e 2062 6520 7265 6e64  puts can be rend
+00000ef0: 6572 6564 2069 6e20 6469 6666 6572 656e  ered in differen
+00000f00: 7420 7761 7973 3a0a 0a23 2323 2044 5643  t ways:..### DVC
+00000f10: 2043 4c49 0a0a 596f 7520 6361 6e20 7573   CLI..You can us
+00000f20: 6520 5b64 7663 2065 7870 2073 686f 775d  e [dvc exp show]
+00000f30: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
+00000f40: 2f64 6f63 2f63 6f6d 6d61 6e64 2d72 6566  /doc/command-ref
+00000f50: 6572 656e 6365 2f65 7870 2f73 686f 7729  erence/exp/show)
+00000f60: 2061 6e64 0a5b 6476 6320 706c 6f74 735d   and.[dvc plots]
+00000f70: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
+00000f80: 2f64 6f63 2f63 6f6d 6d61 6e64 2d72 6566  /doc/command-ref
+00000f90: 6572 656e 6365 2f70 6c6f 7473 2920 746f  erence/plots) to
+00000fa0: 2063 6f6d 7061 7265 2061 6e64 0a76 6973   compare and.vis
+00000fb0: 7561 6c69 7a65 206d 6574 7269 6373 2c20  ualize metrics, 
+00000fc0: 7061 7261 6d65 7465 7273 2061 6e64 2070  parameters and p
+00000fd0: 6c6f 7473 2061 6372 6f73 7320 6578 7065  lots across expe
+00000fe0: 7269 6d65 6e74 733a 0a0a 6060 6063 6f6e  riments:..```con
+00000ff0: 736f 6c65 0a24 2064 7663 2065 7870 2073  sole.$ dvc exp s
+00001000: 686f 770a 6060 600a 0a60 6060 0ae2 9480  how.```..```....
 00001010: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001020: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001030: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001060: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001070: e294 80e2 9480 e294 80e2 9480 e294 800a  ................
-00001080: 4578 7065 7269 6d65 6e74 2020 2020 2020  Experiment      
-00001090: 2020 2020 2020 2020 2020 2043 7265 6174             Creat
-000010a0: 6564 2020 2020 7472 6169 6e2e 6163 6375  ed    train.accu
-000010b0: 7261 6379 2020 2074 7261 696e 2e6c 6f73  racy   train.los
-000010c0: 7320 2020 7661 6c2e 6163 6375 7261 6379  s   val.accuracy
-000010d0: 2020 2076 616c 2e6c 6f73 7320 2020 7374     val.loss   st
-000010e0: 6570 2020 2065 706f 6368 730a e294 80e2  ep   epochs.....
-000010f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001100: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001110: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001120: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001130: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001170: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000011a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000011b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000011c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001080: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000010a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000010b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000010c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000010d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000010e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000010f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001100: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001150: 80e2 9480 0a45 7870 6572 696d 656e 7420  .....Experiment 
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 4372 6561 7465 6420 2020 2074 7261 696e  Created    train
+00001180: 2e61 6363 7572 6163 7920 2020 7472 6169  .accuracy   trai
+00001190: 6e2e 6c6f 7373 2020 2076 616c 2e61 6363  n.loss   val.acc
+000011a0: 7572 6163 7920 2020 7661 6c2e 6c6f 7373  uracy   val.loss
+000011b0: 2020 2073 7465 7020 2020 6570 6f63 6873     step   epochs
+000011c0: 0ae2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000011d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000011e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000011f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001210: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001220: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001230: e294 800a 776f 726b 7370 6163 6520 2020  ....workspace   
-00001240: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 362e 3031 3039 2020 2020 2020 302e    6.0109      0.
-00001270: 3233 3331 3120 2020 2020 2020 2020 2036  23311          6
-00001280: 2e30 3632 2020 2020 302e 3234 3332 3120  .062    0.24321 
-00001290: 2020 2020 2036 2020 2037 0a6d 6173 7465       6   7.maste
-000012a0: 7220 2020 2020 2020 2020 2020 2020 2020  r               
-000012b0: 2020 2020 2020 3038 3a35 3020 504d 2020        08:50 PM  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-000012d0: 2020 2020 2020 2020 2020 202d 2020 2020             -    
-000012e0: 2020 2020 2020 2020 2020 2d20 2020 2020            -     
-000012f0: 2020 2020 202d 2020 2020 2020 2d20 2020       -      -   
-00001300: 2d0a e294 9ce2 9480 e294 8020 3434 3735  -.......... 4475
-00001310: 3834 3520 5b61 756c 6963 2d63 6869 765d  845 [aulic-chiv]
-00001320: 2020 2030 383a 3536 2050 4d20 2020 2020     08:56 PM     
-00001330: 2020 2020 2020 362e 3031 3039 2020 2020        6.0109    
-00001340: 2020 302e 3233 3331 3120 2020 2020 2020    0.23311       
-00001350: 2020 2036 2e30 3632 2020 2020 302e 3234     6.062    0.24
-00001360: 3332 3120 2020 2020 2036 2020 2037 0ae2  321      6   7..
-00001370: 949c e294 80e2 9480 2037 6434 6365 6637  ........ 7d4cef7
-00001380: 205b 7961 7265 722d 746f 6473 5d20 2020   [yarer-tods]   
-00001390: 3038 3a35 3620 504d 2020 2020 2020 2020  08:56 PM        
-000013a0: 2020 2034 2e38 3535 3120 2020 2020 2030     4.8551      0
-000013b0: 2e38 3230 3132 2020 2020 2020 2020 2034  .82012         4
-000013c0: 2e35 3535 3520 2020 302e 3033 3335 3333  .5555   0.033533
-000013d0: 2020 2020 2020 3420 2020 350a e294 94e2        4   5.....
-000013e0: 9480 e294 8020 6435 3033 6638 6520 5b63  ..... d503f8e [c
-000013f0: 7572 7374 2d63 6861 645d 2020 2030 383a  urst-chad]   08:
-00001400: 3536 2050 4d20 2020 2020 2020 2020 2020  56 PM           
-00001410: 342e 3937 3638 2020 2020 2030 2e30 3730  4.9768     0.070
-00001420: 3538 3520 2020 2020 2020 2020 342e 3037  585         4.07
-00001430: 3733 2020 2020 302e 3436 3633 3920 2020  73    0.46639   
-00001440: 2020 2034 2020 2035 0ae2 9480 e294 80e2     4   5........
-00001450: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001460: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001470: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001480: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000014a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000014b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000014c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000014d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000014e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000014f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001500: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001510: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001230: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001240: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001250: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001260: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001280: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000012a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000012b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000012c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000012d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000012e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000012f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001300: 9480 e294 80e2 9480 0a77 6f72 6b73 7061  .........workspa
+00001310: 6365 2020 2020 2020 2020 2020 2020 2020  ce              
+00001320: 2020 2020 2d20 2020 2020 2020 2020 2020      -           
+00001330: 2020 2020 2020 2036 2e30 3130 3920 2020         6.0109   
+00001340: 2020 2030 2e32 3333 3131 2020 2020 2020     0.23311      
+00001350: 2020 2020 362e 3036 3220 2020 2030 2e32      6.062    0.2
+00001360: 3433 3231 2020 2020 2020 3620 2020 370a  4321      6   7.
+00001370: 6d61 7374 6572 2020 2020 2020 2020 2020  master          
+00001380: 2020 2020 2020 2020 2020 2030 383a 3530             08:50
+00001390: 2050 4d20 2020 2020 2020 2020 2020 2020   PM             
+000013a0: 2020 202d 2020 2020 2020 2020 2020 2020     -            
+000013b0: 2d20 2020 2020 2020 2020 2020 2020 202d  -              -
+000013c0: 2020 2020 2020 2020 2020 2d20 2020 2020            -     
+000013d0: 202d 2020 202d 0ae2 949c e294 80e2 9480   -   -..........
+000013e0: 2034 3437 3538 3435 205b 6175 6c69 632d   4475845 [aulic-
+000013f0: 6368 6976 5d20 2020 3038 3a35 3620 504d  chiv]   08:56 PM
+00001400: 2020 2020 2020 2020 2020 2036 2e30 3130             6.010
+00001410: 3920 2020 2020 2030 2e32 3333 3131 2020  9      0.23311  
+00001420: 2020 2020 2020 2020 362e 3036 3220 2020          6.062   
+00001430: 2030 2e32 3433 3231 2020 2020 2020 3620   0.24321      6 
+00001440: 2020 370a e294 9ce2 9480 e294 8020 3764    7.......... 7d
+00001450: 3463 6566 3720 5b79 6172 6572 2d74 6f64  4cef7 [yarer-tod
+00001460: 735d 2020 2030 383a 3536 2050 4d20 2020  s]   08:56 PM   
+00001470: 2020 2020 2020 2020 342e 3835 3531 2020          4.8551  
+00001480: 2020 2020 302e 3832 3031 3220 2020 2020      0.82012     
+00001490: 2020 2020 342e 3535 3535 2020 2030 2e30      4.5555   0.0
+000014a0: 3333 3533 3320 2020 2020 2034 2020 2035  33533      4   5
+000014b0: 0ae2 9494 e294 80e2 9480 2064 3530 3366  .......... d503f
+000014c0: 3865 205b 6375 7273 742d 6368 6164 5d20  8e [curst-chad] 
+000014d0: 2020 3038 3a35 3620 504d 2020 2020 2020    08:56 PM      
+000014e0: 2020 2020 2034 2e39 3736 3820 2020 2020       4.9768     
+000014f0: 302e 3037 3035 3835 2020 2020 2020 2020  0.070585        
+00001500: 2034 2e30 3737 3320 2020 2030 2e34 3636   4.0773    0.466
+00001510: 3339 2020 2020 2020 3420 2020 350a e294  39      4   5...
 00001520: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001530: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001540: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001580: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001590: 0a60 6060 0a0a 6060 6063 6f6e 736f 6c65  .```..```console
-000015a0: 0a24 2064 7663 2070 6c6f 7473 2064 6966  .$ dvc plots dif
-000015b0: 6620 2428 6476 6320 6578 7020 6c69 7374  f $(dvc exp list
-000015c0: 202d 2d6e 616d 6573 2d6f 6e6c 7929 202d   --names-only) -
-000015d0: 2d6f 7065 6e0a 6060 600a 0a21 5b64 7663  -open.```..![dvc
-000015e0: 2070 6c6f 7473 2064 6966 665d 282e 2f64   plots diff](./d
-000015f0: 6f63 732f 6476 635f 706c 6f74 735f 6469  ocs/dvc_plots_di
-00001600: 6666 2e70 6e67 290a 0a23 2323 2044 5643  ff.png)..### DVC
-00001610: 2045 7874 656e 7369 6f6e 2066 6f72 2056   Extension for V
-00001620: 5320 436f 6465 0a0a 496e 7369 6465 2074  S Code..Inside t
-00001630: 6865 0a5b 4456 4320 4578 7465 6e73 696f  he.[DVC Extensio
-00001640: 6e20 666f 7220 5653 2043 6f64 655d 2868  n for VS Code](h
-00001650: 7474 7073 3a2f 2f6d 6172 6b65 7470 6c61  ttps://marketpla
-00001660: 6365 2e76 6973 7561 6c73 7475 6469 6f2e  ce.visualstudio.
-00001670: 636f 6d2f 6974 656d 733f 6974 656d 4e61  com/items?itemNa
-00001680: 6d65 3d49 7465 7261 7469 7665 2e64 7663  me=Iterative.dvc
-00001690: 292c 0a79 6f75 2063 616e 2063 6f6d 7061  ),.you can compa
-000016a0: 7265 2061 6e64 2076 6973 7561 6c69 7a65  re and visualize
-000016b0: 2072 6573 756c 7473 2075 7369 6e67 2074   results using t
-000016c0: 6865 0a5b 4578 7065 7269 6d65 6e74 735d  he.[Experiments]
-000016d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000016e0: 636f 6d2f 6974 6572 6174 6976 652f 7673  com/iterative/vs
-000016f0: 636f 6465 2d64 7663 2f62 6c6f 622f 6d61  code-dvc/blob/ma
-00001700: 696e 2f65 7874 656e 7369 6f6e 2f72 6573  in/extension/res
-00001710: 6f75 7263 6573 2f77 616c 6b74 6872 6f75  ources/walkthrou
-00001720: 6768 2f65 7870 6572 696d 656e 7473 2d74  gh/experiments-t
-00001730: 6162 6c65 2e6d 6429 0a61 6e64 0a5b 506c  able.md).and.[Pl
-00001740: 6f74 735d 2868 7474 7073 3a2f 2f67 6974  ots](https://git
-00001750: 6875 622e 636f 6d2f 6974 6572 6174 6976  hub.com/iterativ
-00001760: 652f 7673 636f 6465 2d64 7663 2f62 6c6f  e/vscode-dvc/blo
-00001770: 622f 6d61 696e 2f65 7874 656e 7369 6f6e  b/main/extension
-00001780: 2f72 6573 6f75 7263 6573 2f77 616c 6b74  /resources/walkt
-00001790: 6872 6f75 6768 2f70 6c6f 7473 2e6d 6429  hrough/plots.md)
-000017a0: 0a76 6965 7773 3a0a 0a21 5b56 5343 6f64  .views:..![VSCod
-000017b0: 6520 4578 7065 7269 6d65 6e74 735d 282e  e Experiments](.
-000017c0: 2f64 6f63 732f 7673 636f 6465 5f65 7870  /docs/vscode_exp
-000017d0: 6572 696d 656e 7473 2e70 6e67 290a 0a21  eriments.png)..!
-000017e0: 5b56 5343 6f64 6520 506c 6f74 735d 282e  [VSCode Plots](.
-000017f0: 2f64 6f63 732f 7673 636f 6465 5f70 6c6f  /docs/vscode_plo
-00001800: 7473 2e70 6e67 290a 0a57 6869 6c65 2065  ts.png)..While e
-00001810: 7870 6572 696d 656e 7473 2061 7265 2072  xperiments are r
-00001820: 756e 6e69 6e67 2c20 6c69 7665 2075 7064  unning, live upd
-00001830: 6174 6573 2077 696c 6c20 6265 2064 6973  ates will be dis
-00001840: 706c 6179 6564 2069 6e20 626f 7468 2076  played in both v
-00001850: 6965 7773 2e0a 0a23 2323 2044 5643 2053  iews...### DVC S
-00001860: 7475 6469 6f0a 0a49 6620 796f 7520 7075  tudio..If you pu
-00001870: 7368 2074 6865 2072 6573 756c 7473 2074  sh the results t
-00001880: 6f20 5b44 5643 2053 7475 6469 6f5d 2868  o [DVC Studio](h
-00001890: 7474 7073 3a2f 2f64 7663 2e6f 7267 2f64  ttps://dvc.org/d
-000018a0: 6f63 2f73 7475 6469 6f29 2c20 796f 7520  oc/studio), you 
-000018b0: 6361 6e0a 636f 6d70 6172 6520 6578 7065  can.compare expe
-000018c0: 7269 6d65 6e74 7320 6167 6169 6e73 7420  riments against 
-000018d0: 7468 6520 656e 7469 7265 2072 6570 6f20  the entire repo 
-000018e0: 6869 7374 6f72 793a 0a0a 215b 5374 7564  history:..![Stud
-000018f0: 696f 2043 6f6d 7061 7265 5d28 2e2f 646f  io Compare](./do
-00001900: 6373 2f73 7475 6469 6f5f 636f 6d70 6172  cs/studio_compar
-00001910: 652e 706e 6729 0a0a 596f 7520 6361 6e20  e.png)..You can 
-00001920: 656e 6162 6c65 0a5b 5374 7564 696f 204c  enable.[Studio L
-00001930: 6976 6520 4578 7065 7269 6d65 6e74 735d  ive Experiments]
-00001940: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
-00001950: 2f64 6f63 2f73 7475 6469 6f2f 7573 6572  /doc/studio/user
-00001960: 2d67 7569 6465 2f70 726f 6a65 6374 732d  -guide/projects-
-00001970: 616e 642d 6578 7065 7269 6d65 6e74 732f  and-experiments/
-00001980: 6c69 7665 2d6d 6574 7269 6373 2d61 6e64  live-metrics-and
-00001990: 2d70 6c6f 7473 290a 746f 2073 6565 206c  -plots).to see l
-000019a0: 6976 6520 7570 6461 7465 7320 7768 696c  ive updates whil
-000019b0: 6520 6578 7065 7269 6d65 6e74 7320 6172  e experiments ar
-000019c0: 6520 7275 6e6e 696e 672e 0a0a 5f5f 5f5f  e running...____
-000019d0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000019e0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000019f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a00: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a10: 5f5f 0a0a 2320 436f 6d70 6172 6973 6f6e  __..# Comparison
-00001a20: 2074 6f20 7265 6c61 7465 6420 7465 6368   to related tech
-00001a30: 6e6f 6c6f 6769 6573 0a0a 2a2a 4456 434c  nologies..**DVCL
-00001a40: 6976 652a 2a20 6973 2061 6e20 2a4d 4c20  ive** is an *ML 
-00001a50: 4c6f 6767 6572 2a2c 2073 696d 696c 6172  Logger*, similar
-00001a60: 2074 6f3a 0a0a 2d20 5b4d 4c46 6c6f 775d   to:..- [MLFlow]
-00001a70: 2868 7474 7073 3a2f 2f6d 6c66 6c6f 772e  (https://mlflow.
-00001a80: 6f72 672f 290a 2d20 5b57 6569 6768 7473  org/).- [Weights
-00001a90: 2026 2042 6961 7365 735d 2868 7474 7073   & Biases](https
-00001aa0: 3a2f 2f77 616e 6462 2e61 692f 7369 7465  ://wandb.ai/site
-00001ab0: 290a 2d20 5b4e 6570 7475 6e65 5d28 6874  ).- [Neptune](ht
-00001ac0: 7470 733a 2f2f 6e65 7074 756e 652e 6169  tps://neptune.ai
-00001ad0: 2f29 0a0a 5468 6520 6d61 696e 2064 6966  /)..The main dif
-00001ae0: 6665 7265 6e63 6520 7769 7468 2074 686f  ference with tho
-00001af0: 7365 202a 4d4c 204c 6f67 6765 7273 2a20  se *ML Loggers* 
-00001b00: 6973 2074 6861 7420 2a2a 4456 434c 6976  is that **DVCLiv
-00001b10: 652a 2a20 646f 6573 206e 6f74 0a2a 2a72  e** does not.**r
-00001b20: 6571 7569 7265 2a2a 2061 6e79 2061 6464  equire** any add
-00001b30: 6974 696f 6e61 6c20 7365 7276 6963 6573  itional services
-00001b40: 206f 7220 7365 7276 6572 7320 746f 2072   or servers to r
-00001b50: 756e 2e0a 0a4c 6f67 6765 6420 6d65 7472  un...Logged metr
-00001b60: 6963 732c 2070 6172 616d 6574 6572 732c  ics, parameters,
-00001b70: 2061 6e64 2070 6c6f 7473 2061 7265 2073   and plots are s
-00001b80: 746f 7265 6420 6173 2070 6c61 696e 2074  tored as plain t
-00001b90: 6578 7420 6669 6c65 7320 7468 6174 2063  ext files that c
-00001ba0: 616e 2062 650a 7665 7273 696f 6e65 6420  an be.versioned 
-00001bb0: 6279 2074 6f6f 6c73 206c 696b 6520 4769  by tools like Gi
-00001bc0: 7420 6f72 2074 7261 636b 6564 2061 7320  t or tracked as 
-00001bd0: 706f 696e 7465 7273 2074 6f20 6669 6c65  pointers to file
-00001be0: 7320 696e 2044 5643 2073 746f 7261 6765  s in DVC storage
-00001bf0: 2e0a 0a59 6f75 2063 616e 2074 6865 6e20  ...You can then 
-00001c00: 7573 6520 6469 6666 6572 656e 7420 5b6f  use different [o
-00001c10: 7074 696f 6e73 5d28 2363 6f6d 7061 7269  ptions](#compari
-00001c20: 6e67 2920 746f 2076 6973 7561 6c69 7a65  ng) to visualize
-00001c30: 2074 6865 206d 6574 7269 6373 2c0a 7061   the metrics,.pa
-00001c40: 7261 6d65 7465 7273 2c20 616e 6420 706c  rameters, and pl
-00001c50: 6f74 7320 6163 726f 7373 2065 7870 6572  ots across exper
-00001c60: 696d 656e 7473 2e0a 0a5f 5f5f 5f5f 5f5f  iments..._______
-00001c70: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001c80: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001c90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001ca0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f0a  _______________.
-00001cb0: 0a23 2043 6f6e 7472 6962 7574 696e 670a  .# Contributing.
-00001cc0: 0a43 6f6e 7472 6962 7574 696f 6e73 2061  .Contributions a
-00001cd0: 7265 2076 6572 7920 7765 6c63 6f6d 652e  re very welcome.
-00001ce0: 2054 6f20 6c65 6172 6e20 6d6f 7265 2c20   To learn more, 
-00001cf0: 7365 6520 7468 650a 5b43 6f6e 7472 6962  see the.[Contrib
-00001d00: 7574 6f72 2047 7569 6465 5d28 434f 4e54  utor Guide](CONT
-00001d10: 5249 4255 5449 4e47 2e72 7374 292e 0a0a  RIBUTING.rst)...
-00001d20: 2320 4c69 6365 6e73 650a 0a44 6973 7472  # License..Distr
-00001d30: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
-00001d40: 2074 6572 6d73 206f 6620 7468 650a 5b41   terms of the.[A
-00001d50: 7061 6368 6520 322e 3020 6c69 6365 6e73  pache 2.0 licens
-00001d60: 655d 2868 7474 7073 3a2f 2f6f 7065 6e73  e](https://opens
-00001d70: 6f75 7263 652e 6f72 672f 6c69 6365 6e73  ource.org/licens
-00001d80: 6573 2f41 7061 6368 652d 322e 3029 2c20  es/Apache-2.0), 
-00001d90: 2a64 7663 6c69 7665 2a20 6973 0a66 7265  *dvclive* is.fre
-00001da0: 6520 616e 6420 6f70 656e 2073 6f75 7263  e and open sourc
-00001db0: 6520 736f 6674 7761 7265 2e0a            e software..
+00001590: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000015a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000015b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000015c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000015d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000015e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000015f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001600: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001610: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001620: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001630: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001640: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001650: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001660: 9480 e294 800a 6060 600a 0a60 6060 636f  ......```..```co
+00001670: 6e73 6f6c 650a 2420 6476 6320 706c 6f74  nsole.$ dvc plot
+00001680: 7320 6469 6666 2024 2864 7663 2065 7870  s diff $(dvc exp
+00001690: 206c 6973 7420 2d2d 6e61 6d65 732d 6f6e   list --names-on
+000016a0: 6c79 2920 2d2d 6f70 656e 0a60 6060 0a0a  ly) --open.```..
+000016b0: 215b 6476 6320 706c 6f74 7320 6469 6666  ![dvc plots diff
+000016c0: 5d28 2e2f 646f 6373 2f64 7663 5f70 6c6f  ](./docs/dvc_plo
+000016d0: 7473 5f64 6966 662e 706e 6729 0a0a 2323  ts_diff.png)..##
+000016e0: 2320 4456 4320 4578 7465 6e73 696f 6e20  # DVC Extension 
+000016f0: 666f 7220 5653 2043 6f64 650a 0a49 6e73  for VS Code..Ins
+00001700: 6964 6520 7468 650a 5b44 5643 2045 7874  ide the.[DVC Ext
+00001710: 656e 7369 6f6e 2066 6f72 2056 5320 436f  ension for VS Co
+00001720: 6465 5d28 6874 7470 733a 2f2f 6d61 726b  de](https://mark
+00001730: 6574 706c 6163 652e 7669 7375 616c 7374  etplace.visualst
+00001740: 7564 696f 2e63 6f6d 2f69 7465 6d73 3f69  udio.com/items?i
+00001750: 7465 6d4e 616d 653d 4974 6572 6174 6976  temName=Iterativ
+00001760: 652e 6476 6329 2c0a 796f 7520 6361 6e20  e.dvc),.you can 
+00001770: 636f 6d70 6172 6520 616e 6420 7669 7375  compare and visu
+00001780: 616c 697a 6520 7265 7375 6c74 7320 7573  alize results us
+00001790: 696e 6720 7468 650a 5b45 7870 6572 696d  ing the.[Experim
+000017a0: 656e 7473 5d28 6874 7470 733a 2f2f 6769  ents](https://gi
+000017b0: 7468 7562 2e63 6f6d 2f69 7465 7261 7469  thub.com/iterati
+000017c0: 7665 2f76 7363 6f64 652d 6476 632f 626c  ve/vscode-dvc/bl
+000017d0: 6f62 2f6d 6169 6e2f 6578 7465 6e73 696f  ob/main/extensio
+000017e0: 6e2f 7265 736f 7572 6365 732f 7761 6c6b  n/resources/walk
+000017f0: 7468 726f 7567 682f 6578 7065 7269 6d65  through/experime
+00001800: 6e74 732d 7461 626c 652e 6d64 290a 616e  nts-table.md).an
+00001810: 640a 5b50 6c6f 7473 5d28 6874 7470 733a  d.[Plots](https:
+00001820: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7465  //github.com/ite
+00001830: 7261 7469 7665 2f76 7363 6f64 652d 6476  rative/vscode-dv
+00001840: 632f 626c 6f62 2f6d 6169 6e2f 6578 7465  c/blob/main/exte
+00001850: 6e73 696f 6e2f 7265 736f 7572 6365 732f  nsion/resources/
+00001860: 7761 6c6b 7468 726f 7567 682f 706c 6f74  walkthrough/plot
+00001870: 732e 6d64 290a 7669 6577 733a 0a0a 215b  s.md).views:..![
+00001880: 5653 436f 6465 2045 7870 6572 696d 656e  VSCode Experimen
+00001890: 7473 5d28 2e2f 646f 6373 2f76 7363 6f64  ts](./docs/vscod
+000018a0: 655f 6578 7065 7269 6d65 6e74 732e 706e  e_experiments.pn
+000018b0: 6729 0a0a 215b 5653 436f 6465 2050 6c6f  g)..![VSCode Plo
+000018c0: 7473 5d28 2e2f 646f 6373 2f76 7363 6f64  ts](./docs/vscod
+000018d0: 655f 706c 6f74 732e 706e 6729 0a0a 5768  e_plots.png)..Wh
+000018e0: 696c 6520 6578 7065 7269 6d65 6e74 7320  ile experiments 
+000018f0: 6172 6520 7275 6e6e 696e 672c 206c 6976  are running, liv
+00001900: 6520 7570 6461 7465 7320 7769 6c6c 2062  e updates will b
+00001910: 6520 6469 7370 6c61 7965 6420 696e 2062  e displayed in b
+00001920: 6f74 6820 7669 6577 732e 0a0a 2323 2320  oth views...### 
+00001930: 4456 4320 5374 7564 696f 0a0a 4966 2079  DVC Studio..If y
+00001940: 6f75 2070 7573 6820 7468 6520 7265 7375  ou push the resu
+00001950: 6c74 7320 746f 205b 4456 4320 5374 7564  lts to [DVC Stud
+00001960: 696f 5d28 6874 7470 733a 2f2f 6476 632e  io](https://dvc.
+00001970: 6f72 672f 646f 632f 7374 7564 696f 292c  org/doc/studio),
+00001980: 2079 6f75 2063 616e 0a63 6f6d 7061 7265   you can.compare
+00001990: 2065 7870 6572 696d 656e 7473 2061 6761   experiments aga
+000019a0: 696e 7374 2074 6865 2065 6e74 6972 6520  inst the entire 
+000019b0: 7265 706f 2068 6973 746f 7279 3a0a 0a21  repo history:..!
+000019c0: 5b53 7475 6469 6f20 436f 6d70 6172 655d  [Studio Compare]
+000019d0: 282e 2f64 6f63 732f 7374 7564 696f 5f63  (./docs/studio_c
+000019e0: 6f6d 7061 7265 2e70 6e67 290a 0a59 6f75  ompare.png)..You
+000019f0: 2063 616e 2065 6e61 626c 650a 5b53 7475   can enable.[Stu
+00001a00: 6469 6f20 4c69 7665 2045 7870 6572 696d  dio Live Experim
+00001a10: 656e 7473 5d28 6874 7470 733a 2f2f 6476  ents](https://dv
+00001a20: 632e 6f72 672f 646f 632f 7374 7564 696f  c.org/doc/studio
+00001a30: 2f75 7365 722d 6775 6964 652f 7072 6f6a  /user-guide/proj
+00001a40: 6563 7473 2d61 6e64 2d65 7870 6572 696d  ects-and-experim
+00001a50: 656e 7473 2f6c 6976 652d 6d65 7472 6963  ents/live-metric
+00001a60: 732d 616e 642d 706c 6f74 7329 0a74 6f20  s-and-plots).to 
+00001a70: 7365 6520 6c69 7665 2075 7064 6174 6573  see live updates
+00001a80: 2077 6869 6c65 2065 7870 6572 696d 656e   while experimen
+00001a90: 7473 2061 7265 2072 756e 6e69 6e67 2e0a  ts are running..
+00001aa0: 0a5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ._______________
+00001ab0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001ac0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001ad0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001ae0: 5f5f 5f5f 5f5f 5f0a 0a23 2043 6f6d 7061  _______..# Compa
+00001af0: 7269 736f 6e20 746f 2072 656c 6174 6564  rison to related
+00001b00: 2074 6563 686e 6f6c 6f67 6965 730a 0a2a   technologies..*
+00001b10: 2a44 5643 4c69 7665 2a2a 2069 7320 616e  *DVCLive** is an
+00001b20: 202a 4d4c 204c 6f67 6765 722a 2c20 7369   *ML Logger*, si
+00001b30: 6d69 6c61 7220 746f 3a0a 0a2d 205b 4d4c  milar to:..- [ML
+00001b40: 466c 6f77 5d28 6874 7470 733a 2f2f 6d6c  Flow](https://ml
+00001b50: 666c 6f77 2e6f 7267 2f29 0a2d 205b 5765  flow.org/).- [We
+00001b60: 6967 6874 7320 2620 4269 6173 6573 5d28  ights & Biases](
+00001b70: 6874 7470 733a 2f2f 7761 6e64 622e 6169  https://wandb.ai
+00001b80: 2f73 6974 6529 0a2d 205b 4e65 7074 756e  /site).- [Neptun
+00001b90: 655d 2868 7474 7073 3a2f 2f6e 6570 7475  e](https://neptu
+00001ba0: 6e65 2e61 692f 290a 0a54 6865 206d 6169  ne.ai/)..The mai
+00001bb0: 6e20 6469 6666 6572 656e 6365 2077 6974  n difference wit
+00001bc0: 6820 7468 6f73 6520 2a4d 4c20 4c6f 6767  h those *ML Logg
+00001bd0: 6572 732a 2069 7320 7468 6174 202a 2a44  ers* is that **D
+00001be0: 5643 4c69 7665 2a2a 2064 6f65 7320 6e6f  VCLive** does no
+00001bf0: 740a 2a2a 7265 7175 6972 652a 2a20 616e  t.**require** an
+00001c00: 7920 6164 6469 7469 6f6e 616c 2073 6572  y additional ser
+00001c10: 7669 6365 7320 6f72 2073 6572 7665 7273  vices or servers
+00001c20: 2074 6f20 7275 6e2e 0a0a 4c6f 6767 6564   to run...Logged
+00001c30: 206d 6574 7269 6373 2c20 7061 7261 6d65   metrics, parame
+00001c40: 7465 7273 2c20 616e 6420 706c 6f74 7320  ters, and plots 
+00001c50: 6172 6520 7374 6f72 6564 2061 7320 706c  are stored as pl
+00001c60: 6169 6e20 7465 7874 2066 696c 6573 2074  ain text files t
+00001c70: 6861 7420 6361 6e20 6265 0a76 6572 7369  hat can be.versi
+00001c80: 6f6e 6564 2062 7920 746f 6f6c 7320 6c69  oned by tools li
+00001c90: 6b65 2047 6974 206f 7220 7472 6163 6b65  ke Git or tracke
+00001ca0: 6420 6173 2070 6f69 6e74 6572 7320 746f  d as pointers to
+00001cb0: 2066 696c 6573 2069 6e20 4456 4320 7374   files in DVC st
+00001cc0: 6f72 6167 652e 0a0a 596f 7520 6361 6e20  orage...You can 
+00001cd0: 7468 656e 2075 7365 2064 6966 6665 7265  then use differe
+00001ce0: 6e74 205b 6f70 7469 6f6e 735d 2823 636f  nt [options](#co
+00001cf0: 6d70 6172 696e 6729 2074 6f20 7669 7375  mparing) to visu
+00001d00: 616c 697a 6520 7468 6520 6d65 7472 6963  alize the metric
+00001d10: 732c 0a70 6172 616d 6574 6572 732c 2061  s,.parameters, a
+00001d20: 6e64 2070 6c6f 7473 2061 6372 6f73 7320  nd plots across 
+00001d30: 6578 7065 7269 6d65 6e74 732e 0a0a 5f5f  experiments...__
+00001d40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d60: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d70: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d80: 5f5f 5f5f 0a0a 2320 436f 6e74 7269 6275  ____..# Contribu
+00001d90: 7469 6e67 0a0a 436f 6e74 7269 6275 7469  ting..Contributi
+00001da0: 6f6e 7320 6172 6520 7665 7279 2077 656c  ons are very wel
+00001db0: 636f 6d65 2e20 546f 206c 6561 726e 206d  come. To learn m
+00001dc0: 6f72 652c 2073 6565 2074 6865 0a5b 436f  ore, see the.[Co
+00001dd0: 6e74 7269 6275 746f 7220 4775 6964 655d  ntributor Guide]
+00001de0: 2843 4f4e 5452 4942 5554 494e 472e 7273  (CONTRIBUTING.rs
+00001df0: 7429 2e0a 0a23 204c 6963 656e 7365 0a0a  t)...# License..
+00001e00: 4469 7374 7269 6275 7465 6420 756e 6465  Distributed unde
+00001e10: 7220 7468 6520 7465 726d 7320 6f66 2074  r the terms of t
+00001e20: 6865 0a5b 4170 6163 6865 2032 2e30 206c  he.[Apache 2.0 l
+00001e30: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+00001e40: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+00001e50: 6963 656e 7365 732f 4170 6163 6865 2d32  icenses/Apache-2
+00001e60: 2e30 292c 202a 6476 636c 6976 652a 2069  .0), *dvclive* i
+00001e70: 730a 6672 6565 2061 6e64 206f 7065 6e20  s.free and open 
+00001e80: 736f 7572 6365 2073 6f66 7477 6172 652e  source software.
+00001e90: 0a                                       .
```

### Comparing `dvclive-2.6.4/README.md` & `dvclive-2.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -83,323 +83,337 @@
 00000520: 672f 646f 632f 6476 636c 6976 652f 6d6c  g/doc/dvclive/ml
 00000530: 2d66 7261 6d65 776f 726b 7329 0a0a 5f5f  -frameworks)..__
 00000540: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000550: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000560: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000570: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000580: 5f5f 5f5f 0a0a 2320 5175 6963 6b73 7461  ____..# Quicksta
-00000590: 7274 0a0a 2323 2049 6e73 7461 6c6c 202a  rt..## Install *
-000005a0: 6476 636c 6976 652a 0a0a 6060 6063 6f6e  dvclive*..```con
-000005b0: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
-000005c0: 6c6c 2064 7663 6c69 7665 0a60 6060 0a0a  ll dvclive.```..
-000005d0: 2323 2049 6e69 7469 616c 697a 6520 4456  ## Initialize DV
-000005e0: 4320 5265 706f 7369 746f 7279 0a0a 6060  C Repository..``
-000005f0: 6063 6f6e 736f 6c65 0a24 2067 6974 2069  `console.$ git i
-00000600: 6e69 740a 2420 6476 6320 696e 6974 0a24  nit.$ dvc init.$
-00000610: 2067 6974 2063 6f6d 6d69 7420 2d6d 2022   git commit -m "
-00000620: 4456 4320 696e 6974 220a 6060 600a 0a23  DVC init".```..#
-00000630: 2320 4578 616d 706c 6520 636f 6465 0a0a  # Example code..
-00000640: 436f 7079 2074 6865 2073 6e69 7070 6574  Copy the snippet
-00000650: 2062 656c 6f77 2061 7320 6120 6261 7369   below as a basi
-00000660: 6320 6578 616d 706c 6520 6f66 2074 6865  c example of the
-00000670: 2041 5049 2075 7361 6765 3a0a 0a60 6060   API usage:..```
-00000680: 7079 7468 6f6e 0a23 2074 7261 696e 2e70  python.# train.p
-00000690: 790a 696d 706f 7274 2072 616e 646f 6d0a  y.import random.
-000006a0: 696d 706f 7274 2073 7973 0a66 726f 6d20  import sys.from 
-000006b0: 6476 636c 6976 6520 696d 706f 7274 204c  dvclive import L
-000006c0: 6976 650a 0a77 6974 6820 4c69 7665 2873  ive..with Live(s
-000006d0: 6176 655f 6476 635f 6578 703d 5472 7565  ave_dvc_exp=True
-000006e0: 2920 6173 206c 6976 653a 0a20 2020 2065  ) as live:.    e
-000006f0: 706f 6368 7320 3d20 696e 7428 7379 732e  pochs = int(sys.
-00000700: 6172 6776 5b31 5d29 0a20 2020 206c 6976  argv[1]).    liv
-00000710: 652e 6c6f 675f 7061 7261 6d28 2265 706f  e.log_param("epo
-00000720: 6368 7322 2c20 6570 6f63 6873 290a 2020  chs", epochs).  
-00000730: 2020 666f 7220 6570 6f63 6820 696e 2072    for epoch in r
-00000740: 616e 6765 2865 706f 6368 7329 3a0a 2020  ange(epochs):.  
-00000750: 2020 2020 2020 6c69 7665 2e6c 6f67 5f6d        live.log_m
-00000760: 6574 7269 6328 2274 7261 696e 2f61 6363  etric("train/acc
-00000770: 7572 6163 7922 2c20 6570 6f63 6820 2b20  uracy", epoch + 
-00000780: 7261 6e64 6f6d 2e72 616e 646f 6d28 2929  random.random())
-00000790: 0a20 2020 2020 2020 206c 6976 652e 6c6f  .        live.lo
-000007a0: 675f 6d65 7472 6963 2822 7472 6169 6e2f  g_metric("train/
-000007b0: 6c6f 7373 222c 2065 706f 6368 7320 2d20  loss", epochs - 
-000007c0: 6570 6f63 6820 2d20 7261 6e64 6f6d 2e72  epoch - random.r
-000007d0: 616e 646f 6d28 2929 0a20 2020 2020 2020  andom()).       
-000007e0: 206c 6976 652e 6c6f 675f 6d65 7472 6963   live.log_metric
-000007f0: 2822 7661 6c2f 6163 6375 7261 6379 222c  ("val/accuracy",
-00000800: 6570 6f63 6820 2b20 7261 6e64 6f6d 2e72  epoch + random.r
-00000810: 616e 646f 6d28 2920 290a 2020 2020 2020  andom() ).      
-00000820: 2020 6c69 7665 2e6c 6f67 5f6d 6574 7269    live.log_metri
-00000830: 6328 2276 616c 2f6c 6f73 7322 2c20 6570  c("val/loss", ep
-00000840: 6f63 6873 202d 2065 706f 6368 202d 2072  ochs - epoch - r
-00000850: 616e 646f 6d2e 7261 6e64 6f6d 2829 290a  andom.random()).
-00000860: 2020 2020 2020 2020 6c69 7665 2e6e 6578          live.nex
-00000870: 745f 7374 6570 2829 0a60 6060 0a0a 5365  t_step().```..Se
-00000880: 6520 5b49 6e74 6567 7261 7469 6f6e 735d  e [Integrations]
-00000890: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
-000008a0: 2f64 6f63 2f64 7663 6c69 7665 2f6d 6c2d  /doc/dvclive/ml-
-000008b0: 6672 616d 6577 6f72 6b73 2920 666f 7220  frameworks) for 
-000008c0: 6578 616d 706c 6573 2075 7369 6e67 0a44  examples using.D
-000008d0: 5643 4c69 7665 2061 6c6f 6e67 7369 6465  VCLive alongside
-000008e0: 2064 6966 6665 7265 6e74 204d 4c20 4672   different ML Fr
-000008f0: 616d 6577 6f72 6b73 2e0a 0a23 2320 5275  ameworks...## Ru
-00000900: 6e6e 696e 670a 0a52 756e 2063 6f75 706c  nning..Run coupl
-00000910: 6520 6f66 2074 696d 6573 2070 6173 7369  e of times passi
-00000920: 6e67 2064 6966 6665 7265 6e74 2076 616c  ng different val
-00000930: 7565 733a 0a0a 6060 6063 6f6e 736f 6c65  ues:..```console
-00000940: 0a24 2070 7974 686f 6e20 7472 6169 6e2e  .$ python train.
-00000950: 7079 2035 0a24 2070 7974 686f 6e20 7472  py 5.$ python tr
-00000960: 6169 6e2e 7079 2035 0a24 2070 7974 686f  ain.py 5.$ pytho
-00000970: 6e20 7472 6169 6e2e 7079 2037 0a60 6060  n train.py 7.```
-00000980: 0a0a 2323 2043 6f6d 7061 7269 6e67 0a0a  ..## Comparing..
-00000990: 4456 434c 6976 6520 6f75 7470 7574 7320  DVCLive outputs 
-000009a0: 6361 6e20 6265 2072 656e 6465 7265 6420  can be rendered 
-000009b0: 696e 2064 6966 6665 7265 6e74 2077 6179  in different way
-000009c0: 733a 0a0a 2323 2320 4456 4320 434c 490a  s:..### DVC CLI.
-000009d0: 0a59 6f75 2063 616e 2075 7365 205b 6476  .You can use [dv
-000009e0: 6320 6578 7020 7368 6f77 5d28 6874 7470  c exp show](http
-000009f0: 733a 2f2f 6476 632e 6f72 672f 646f 632f  s://dvc.org/doc/
-00000a00: 636f 6d6d 616e 642d 7265 6665 7265 6e63  command-referenc
-00000a10: 652f 6578 702f 7368 6f77 2920 616e 640a  e/exp/show) and.
-00000a20: 5b64 7663 2070 6c6f 7473 5d28 6874 7470  [dvc plots](http
-00000a30: 733a 2f2f 6476 632e 6f72 672f 646f 632f  s://dvc.org/doc/
-00000a40: 636f 6d6d 616e 642d 7265 6665 7265 6e63  command-referenc
-00000a50: 652f 706c 6f74 7329 2074 6f20 636f 6d70  e/plots) to comp
-00000a60: 6172 6520 616e 640a 7669 7375 616c 697a  are and.visualiz
-00000a70: 6520 6d65 7472 6963 732c 2070 6172 616d  e metrics, param
-00000a80: 6574 6572 7320 616e 6420 706c 6f74 7320  eters and plots 
-00000a90: 6163 726f 7373 2065 7870 6572 696d 656e  across experimen
-00000aa0: 7473 3a0a 0a60 6060 636f 6e73 6f6c 650a  ts:..```console.
-00000ab0: 2420 6476 6320 6578 7020 7368 6f77 0a60  $ dvc exp show.`
-00000ac0: 6060 0a0a 6060 600a e294 80e2 9480 e294  ``..```.........
-00000ad0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000ae0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000af0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000b00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000b10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000b20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000b30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000b40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000b50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000b60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000b70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000b80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000b90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000590: 7274 0a0a 3c70 2061 6c69 676e 3d27 6365  rt..<p align='ce
+000005a0: 6e74 6572 273e 0a3c 6120 6872 6566 3d22  nter'>.<a href="
+000005b0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+000005c0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+000005d0: 6d2f 6769 7468 7562 2f69 7465 7261 7469  m/github/iterati
+000005e0: 7665 2f64 7663 6c69 7665 2f62 6c6f 622f  ve/dvclive/blob/
+000005f0: 6d61 696e 2f65 7861 6d70 6c65 732f 4456  main/examples/DV
+00000600: 434c 6976 652d 5175 6963 6b73 7461 7274  CLive-Quickstart
+00000610: 2e69 7079 6e62 223e 3c69 6d67 2073 7263  .ipynb"><img src
+00000620: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
+00000630: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00000640: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+00000650: 2d62 6164 6765 2e73 7667 2220 2f3e 3c2f  -badge.svg" /></
+00000660: 613e 0a3c 2f70 3e0a 0a23 2320 496e 7374  a>.</p>..## Inst
+00000670: 616c 6c20 2a64 7663 6c69 7665 2a0a 0a60  all *dvclive*..`
+00000680: 6060 636f 6e73 6f6c 650a 2420 7069 7020  ``console.$ pip 
+00000690: 696e 7374 616c 6c20 6476 636c 6976 650a  install dvclive.
+000006a0: 6060 600a 0a23 2320 496e 6974 6961 6c69  ```..## Initiali
+000006b0: 7a65 2044 5643 2052 6570 6f73 6974 6f72  ze DVC Repositor
+000006c0: 790a 0a60 6060 636f 6e73 6f6c 650a 2420  y..```console.$ 
+000006d0: 6769 7420 696e 6974 0a24 2064 7663 2069  git init.$ dvc i
+000006e0: 6e69 740a 2420 6769 7420 636f 6d6d 6974  nit.$ git commit
+000006f0: 202d 6d20 2244 5643 2069 6e69 7422 0a60   -m "DVC init".`
+00000700: 6060 0a0a 2323 2045 7861 6d70 6c65 2063  ``..## Example c
+00000710: 6f64 650a 0a43 6f70 7920 7468 6520 736e  ode..Copy the sn
+00000720: 6970 7065 7420 6265 6c6f 7720 6173 2061  ippet below as a
+00000730: 2062 6173 6963 2065 7861 6d70 6c65 206f   basic example o
+00000740: 6620 7468 6520 4150 4920 7573 6167 653a  f the API usage:
+00000750: 0a0a 6060 6070 7974 686f 6e0a 2320 7472  ..```python.# tr
+00000760: 6169 6e2e 7079 0a69 6d70 6f72 7420 7261  ain.py.import ra
+00000770: 6e64 6f6d 0a69 6d70 6f72 7420 7379 730a  ndom.import sys.
+00000780: 6672 6f6d 2064 7663 6c69 7665 2069 6d70  from dvclive imp
+00000790: 6f72 7420 4c69 7665 0a0a 7769 7468 204c  ort Live..with L
+000007a0: 6976 6528 7361 7665 5f64 7663 5f65 7870  ive(save_dvc_exp
+000007b0: 3d54 7275 6529 2061 7320 6c69 7665 3a0a  =True) as live:.
+000007c0: 2020 2020 6570 6f63 6873 203d 2069 6e74      epochs = int
+000007d0: 2873 7973 2e61 7267 765b 315d 290a 2020  (sys.argv[1]).  
+000007e0: 2020 6c69 7665 2e6c 6f67 5f70 6172 616d    live.log_param
+000007f0: 2822 6570 6f63 6873 222c 2065 706f 6368  ("epochs", epoch
+00000800: 7329 0a20 2020 2066 6f72 2065 706f 6368  s).    for epoch
+00000810: 2069 6e20 7261 6e67 6528 6570 6f63 6873   in range(epochs
+00000820: 293a 0a20 2020 2020 2020 206c 6976 652e  ):.        live.
+00000830: 6c6f 675f 6d65 7472 6963 2822 7472 6169  log_metric("trai
+00000840: 6e2f 6163 6375 7261 6379 222c 2065 706f  n/accuracy", epo
+00000850: 6368 202b 2072 616e 646f 6d2e 7261 6e64  ch + random.rand
+00000860: 6f6d 2829 290a 2020 2020 2020 2020 6c69  om()).        li
+00000870: 7665 2e6c 6f67 5f6d 6574 7269 6328 2274  ve.log_metric("t
+00000880: 7261 696e 2f6c 6f73 7322 2c20 6570 6f63  rain/loss", epoc
+00000890: 6873 202d 2065 706f 6368 202d 2072 616e  hs - epoch - ran
+000008a0: 646f 6d2e 7261 6e64 6f6d 2829 290a 2020  dom.random()).  
+000008b0: 2020 2020 2020 6c69 7665 2e6c 6f67 5f6d        live.log_m
+000008c0: 6574 7269 6328 2276 616c 2f61 6363 7572  etric("val/accur
+000008d0: 6163 7922 2c65 706f 6368 202b 2072 616e  acy",epoch + ran
+000008e0: 646f 6d2e 7261 6e64 6f6d 2829 2029 0a20  dom.random() ). 
+000008f0: 2020 2020 2020 206c 6976 652e 6c6f 675f         live.log_
+00000900: 6d65 7472 6963 2822 7661 6c2f 6c6f 7373  metric("val/loss
+00000910: 222c 2065 706f 6368 7320 2d20 6570 6f63  ", epochs - epoc
+00000920: 6820 2d20 7261 6e64 6f6d 2e72 616e 646f  h - random.rando
+00000930: 6d28 2929 0a20 2020 2020 2020 206c 6976  m()).        liv
+00000940: 652e 6e65 7874 5f73 7465 7028 290a 6060  e.next_step().``
+00000950: 600a 0a53 6565 205b 496e 7465 6772 6174  `..See [Integrat
+00000960: 696f 6e73 5d28 6874 7470 733a 2f2f 6476  ions](https://dv
+00000970: 632e 6f72 672f 646f 632f 6476 636c 6976  c.org/doc/dvcliv
+00000980: 652f 6d6c 2d66 7261 6d65 776f 726b 7329  e/ml-frameworks)
+00000990: 2066 6f72 2065 7861 6d70 6c65 7320 7573   for examples us
+000009a0: 696e 670a 4456 434c 6976 6520 616c 6f6e  ing.DVCLive alon
+000009b0: 6773 6964 6520 6469 6666 6572 656e 7420  gside different 
+000009c0: 4d4c 2046 7261 6d65 776f 726b 732e 0a0a  ML Frameworks...
+000009d0: 2323 2052 756e 6e69 6e67 0a0a 5275 6e20  ## Running..Run 
+000009e0: 636f 7570 6c65 206f 6620 7469 6d65 7320  couple of times 
+000009f0: 7061 7373 696e 6720 6469 6666 6572 656e  passing differen
+00000a00: 7420 7661 6c75 6573 3a0a 0a60 6060 636f  t values:..```co
+00000a10: 6e73 6f6c 650a 2420 7079 7468 6f6e 2074  nsole.$ python t
+00000a20: 7261 696e 2e70 7920 350a 2420 7079 7468  rain.py 5.$ pyth
+00000a30: 6f6e 2074 7261 696e 2e70 7920 350a 2420  on train.py 5.$ 
+00000a40: 7079 7468 6f6e 2074 7261 696e 2e70 7920  python train.py 
+00000a50: 370a 6060 600a 0a23 2320 436f 6d70 6172  7.```..## Compar
+00000a60: 696e 670a 0a44 5643 4c69 7665 206f 7574  ing..DVCLive out
+00000a70: 7075 7473 2063 616e 2062 6520 7265 6e64  puts can be rend
+00000a80: 6572 6564 2069 6e20 6469 6666 6572 656e  ered in differen
+00000a90: 7420 7761 7973 3a0a 0a23 2323 2044 5643  t ways:..### DVC
+00000aa0: 2043 4c49 0a0a 596f 7520 6361 6e20 7573   CLI..You can us
+00000ab0: 6520 5b64 7663 2065 7870 2073 686f 775d  e [dvc exp show]
+00000ac0: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
+00000ad0: 2f64 6f63 2f63 6f6d 6d61 6e64 2d72 6566  /doc/command-ref
+00000ae0: 6572 656e 6365 2f65 7870 2f73 686f 7729  erence/exp/show)
+00000af0: 2061 6e64 0a5b 6476 6320 706c 6f74 735d   and.[dvc plots]
+00000b00: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
+00000b10: 2f64 6f63 2f63 6f6d 6d61 6e64 2d72 6566  /doc/command-ref
+00000b20: 6572 656e 6365 2f70 6c6f 7473 2920 746f  erence/plots) to
+00000b30: 2063 6f6d 7061 7265 2061 6e64 0a76 6973   compare and.vis
+00000b40: 7561 6c69 7a65 206d 6574 7269 6373 2c20  ualize metrics, 
+00000b50: 7061 7261 6d65 7465 7273 2061 6e64 2070  parameters and p
+00000b60: 6c6f 7473 2061 6372 6f73 7320 6578 7065  lots across expe
+00000b70: 7269 6d65 6e74 733a 0a0a 6060 6063 6f6e  riments:..```con
+00000b80: 736f 6c65 0a24 2064 7663 2065 7870 2073  sole.$ dvc exp s
+00000b90: 686f 770a 6060 600a 0a60 6060 0ae2 9480  how.```..```....
 00000ba0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00000bb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00000bc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00000bd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00000be0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00000bf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000c00: e294 80e2 9480 e294 80e2 9480 e294 800a  ................
-00000c10: 4578 7065 7269 6d65 6e74 2020 2020 2020  Experiment      
-00000c20: 2020 2020 2020 2020 2020 2043 7265 6174             Creat
-00000c30: 6564 2020 2020 7472 6169 6e2e 6163 6375  ed    train.accu
-00000c40: 7261 6379 2020 2074 7261 696e 2e6c 6f73  racy   train.los
-00000c50: 7320 2020 7661 6c2e 6163 6375 7261 6379  s   val.accuracy
-00000c60: 2020 2076 616c 2e6c 6f73 7320 2020 7374     val.loss   st
-00000c70: 6570 2020 2065 706f 6368 730a e294 80e2  ep   epochs.....
-00000c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000c90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000cc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000ce0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000cf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000d00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000d10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000d20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000d30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000d40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000d50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000c00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000c10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000c20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000c30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000c40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000c50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000c60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000c70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000c80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000c90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000ca0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000cb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000cc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000cd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000ce0: 80e2 9480 0a45 7870 6572 696d 656e 7420  .....Experiment 
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d00: 4372 6561 7465 6420 2020 2074 7261 696e  Created    train
+00000d10: 2e61 6363 7572 6163 7920 2020 7472 6169  .accuracy   trai
+00000d20: 6e2e 6c6f 7373 2020 2076 616c 2e61 6363  n.loss   val.acc
+00000d30: 7572 6163 7920 2020 7661 6c2e 6c6f 7373  uracy   val.loss
+00000d40: 2020 2073 7465 7020 2020 6570 6f63 6873     step   epochs
+00000d50: 0ae2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00000d60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00000d70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00000d80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00000d90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00000da0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00000db0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000dc0: e294 800a 776f 726b 7370 6163 6520 2020  ....workspace   
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000df0: 2020 362e 3031 3039 2020 2020 2020 302e    6.0109      0.
-00000e00: 3233 3331 3120 2020 2020 2020 2020 2036  23311          6
-00000e10: 2e30 3632 2020 2020 302e 3234 3332 3120  .062    0.24321 
-00000e20: 2020 2020 2036 2020 2037 0a6d 6173 7465       6   7.maste
-00000e30: 7220 2020 2020 2020 2020 2020 2020 2020  r               
-00000e40: 2020 2020 2020 3038 3a35 3020 504d 2020        08:50 PM  
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00000e60: 2020 2020 2020 2020 2020 202d 2020 2020             -    
-00000e70: 2020 2020 2020 2020 2020 2d20 2020 2020            -     
-00000e80: 2020 2020 202d 2020 2020 2020 2d20 2020       -      -   
-00000e90: 2d0a e294 9ce2 9480 e294 8020 3434 3735  -.......... 4475
-00000ea0: 3834 3520 5b61 756c 6963 2d63 6869 765d  845 [aulic-chiv]
-00000eb0: 2020 2030 383a 3536 2050 4d20 2020 2020     08:56 PM     
-00000ec0: 2020 2020 2020 362e 3031 3039 2020 2020        6.0109    
-00000ed0: 2020 302e 3233 3331 3120 2020 2020 2020    0.23311       
-00000ee0: 2020 2036 2e30 3632 2020 2020 302e 3234     6.062    0.24
-00000ef0: 3332 3120 2020 2020 2036 2020 2037 0ae2  321      6   7..
-00000f00: 949c e294 80e2 9480 2037 6434 6365 6637  ........ 7d4cef7
-00000f10: 205b 7961 7265 722d 746f 6473 5d20 2020   [yarer-tods]   
-00000f20: 3038 3a35 3620 504d 2020 2020 2020 2020  08:56 PM        
-00000f30: 2020 2034 2e38 3535 3120 2020 2020 2030     4.8551      0
-00000f40: 2e38 3230 3132 2020 2020 2020 2020 2034  .82012         4
-00000f50: 2e35 3535 3520 2020 302e 3033 3335 3333  .5555   0.033533
-00000f60: 2020 2020 2020 3420 2020 350a e294 94e2        4   5.....
-00000f70: 9480 e294 8020 6435 3033 6638 6520 5b63  ..... d503f8e [c
-00000f80: 7572 7374 2d63 6861 645d 2020 2030 383a  urst-chad]   08:
-00000f90: 3536 2050 4d20 2020 2020 2020 2020 2020  56 PM           
-00000fa0: 342e 3937 3638 2020 2020 2030 2e30 3730  4.9768     0.070
-00000fb0: 3538 3520 2020 2020 2020 2020 342e 3037  585         4.07
-00000fc0: 3733 2020 2020 302e 3436 3633 3920 2020  73    0.46639   
-00000fd0: 2020 2034 2020 2035 0ae2 9480 e294 80e2     4   5........
-00000fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000010a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000dc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000dd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000de0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000df0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000e00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000e10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000e20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000e30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000e40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000e50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000e60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000e70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000e80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000e90: 9480 e294 80e2 9480 0a77 6f72 6b73 7061  .........workspa
+00000ea0: 6365 2020 2020 2020 2020 2020 2020 2020  ce              
+00000eb0: 2020 2020 2d20 2020 2020 2020 2020 2020      -           
+00000ec0: 2020 2020 2020 2036 2e30 3130 3920 2020         6.0109   
+00000ed0: 2020 2030 2e32 3333 3131 2020 2020 2020     0.23311      
+00000ee0: 2020 2020 362e 3036 3220 2020 2030 2e32      6.062    0.2
+00000ef0: 3433 3231 2020 2020 2020 3620 2020 370a  4321      6   7.
+00000f00: 6d61 7374 6572 2020 2020 2020 2020 2020  master          
+00000f10: 2020 2020 2020 2020 2020 2030 383a 3530             08:50
+00000f20: 2050 4d20 2020 2020 2020 2020 2020 2020   PM             
+00000f30: 2020 202d 2020 2020 2020 2020 2020 2020     -            
+00000f40: 2d20 2020 2020 2020 2020 2020 2020 202d  -              -
+00000f50: 2020 2020 2020 2020 2020 2d20 2020 2020            -     
+00000f60: 202d 2020 202d 0ae2 949c e294 80e2 9480   -   -..........
+00000f70: 2034 3437 3538 3435 205b 6175 6c69 632d   4475845 [aulic-
+00000f80: 6368 6976 5d20 2020 3038 3a35 3620 504d  chiv]   08:56 PM
+00000f90: 2020 2020 2020 2020 2020 2036 2e30 3130             6.010
+00000fa0: 3920 2020 2020 2030 2e32 3333 3131 2020  9      0.23311  
+00000fb0: 2020 2020 2020 2020 362e 3036 3220 2020          6.062   
+00000fc0: 2030 2e32 3433 3231 2020 2020 2020 3620   0.24321      6 
+00000fd0: 2020 370a e294 9ce2 9480 e294 8020 3764    7.......... 7d
+00000fe0: 3463 6566 3720 5b79 6172 6572 2d74 6f64  4cef7 [yarer-tod
+00000ff0: 735d 2020 2030 383a 3536 2050 4d20 2020  s]   08:56 PM   
+00001000: 2020 2020 2020 2020 342e 3835 3531 2020          4.8551  
+00001010: 2020 2020 302e 3832 3031 3220 2020 2020      0.82012     
+00001020: 2020 2020 342e 3535 3535 2020 2030 2e30      4.5555   0.0
+00001030: 3333 3533 3320 2020 2020 2034 2020 2035  33533      4   5
+00001040: 0ae2 9494 e294 80e2 9480 2064 3530 3366  .......... d503f
+00001050: 3865 205b 6375 7273 742d 6368 6164 5d20  8e [curst-chad] 
+00001060: 2020 3038 3a35 3620 504d 2020 2020 2020    08:56 PM      
+00001070: 2020 2020 2034 2e39 3736 3820 2020 2020       4.9768     
+00001080: 302e 3037 3035 3835 2020 2020 2020 2020  0.070585        
+00001090: 2034 2e30 3737 3320 2020 2030 2e34 3636   4.0773    0.466
+000010a0: 3339 2020 2020 2020 3420 2020 350a e294  39      4   5...
 000010b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000010c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000010d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000010e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000010f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001100: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001110: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001120: 0a60 6060 0a0a 6060 6063 6f6e 736f 6c65  .```..```console
-00001130: 0a24 2064 7663 2070 6c6f 7473 2064 6966  .$ dvc plots dif
-00001140: 6620 2428 6476 6320 6578 7020 6c69 7374  f $(dvc exp list
-00001150: 202d 2d6e 616d 6573 2d6f 6e6c 7929 202d   --names-only) -
-00001160: 2d6f 7065 6e0a 6060 600a 0a21 5b64 7663  -open.```..![dvc
-00001170: 2070 6c6f 7473 2064 6966 665d 282e 2f64   plots diff](./d
-00001180: 6f63 732f 6476 635f 706c 6f74 735f 6469  ocs/dvc_plots_di
-00001190: 6666 2e70 6e67 290a 0a23 2323 2044 5643  ff.png)..### DVC
-000011a0: 2045 7874 656e 7369 6f6e 2066 6f72 2056   Extension for V
-000011b0: 5320 436f 6465 0a0a 496e 7369 6465 2074  S Code..Inside t
-000011c0: 6865 0a5b 4456 4320 4578 7465 6e73 696f  he.[DVC Extensio
-000011d0: 6e20 666f 7220 5653 2043 6f64 655d 2868  n for VS Code](h
-000011e0: 7474 7073 3a2f 2f6d 6172 6b65 7470 6c61  ttps://marketpla
-000011f0: 6365 2e76 6973 7561 6c73 7475 6469 6f2e  ce.visualstudio.
-00001200: 636f 6d2f 6974 656d 733f 6974 656d 4e61  com/items?itemNa
-00001210: 6d65 3d49 7465 7261 7469 7665 2e64 7663  me=Iterative.dvc
-00001220: 292c 0a79 6f75 2063 616e 2063 6f6d 7061  ),.you can compa
-00001230: 7265 2061 6e64 2076 6973 7561 6c69 7a65  re and visualize
-00001240: 2072 6573 756c 7473 2075 7369 6e67 2074   results using t
-00001250: 6865 0a5b 4578 7065 7269 6d65 6e74 735d  he.[Experiments]
-00001260: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001270: 636f 6d2f 6974 6572 6174 6976 652f 7673  com/iterative/vs
-00001280: 636f 6465 2d64 7663 2f62 6c6f 622f 6d61  code-dvc/blob/ma
-00001290: 696e 2f65 7874 656e 7369 6f6e 2f72 6573  in/extension/res
-000012a0: 6f75 7263 6573 2f77 616c 6b74 6872 6f75  ources/walkthrou
-000012b0: 6768 2f65 7870 6572 696d 656e 7473 2d74  gh/experiments-t
-000012c0: 6162 6c65 2e6d 6429 0a61 6e64 0a5b 506c  able.md).and.[Pl
-000012d0: 6f74 735d 2868 7474 7073 3a2f 2f67 6974  ots](https://git
-000012e0: 6875 622e 636f 6d2f 6974 6572 6174 6976  hub.com/iterativ
-000012f0: 652f 7673 636f 6465 2d64 7663 2f62 6c6f  e/vscode-dvc/blo
-00001300: 622f 6d61 696e 2f65 7874 656e 7369 6f6e  b/main/extension
-00001310: 2f72 6573 6f75 7263 6573 2f77 616c 6b74  /resources/walkt
-00001320: 6872 6f75 6768 2f70 6c6f 7473 2e6d 6429  hrough/plots.md)
-00001330: 0a76 6965 7773 3a0a 0a21 5b56 5343 6f64  .views:..![VSCod
-00001340: 6520 4578 7065 7269 6d65 6e74 735d 282e  e Experiments](.
-00001350: 2f64 6f63 732f 7673 636f 6465 5f65 7870  /docs/vscode_exp
-00001360: 6572 696d 656e 7473 2e70 6e67 290a 0a21  eriments.png)..!
-00001370: 5b56 5343 6f64 6520 506c 6f74 735d 282e  [VSCode Plots](.
-00001380: 2f64 6f63 732f 7673 636f 6465 5f70 6c6f  /docs/vscode_plo
-00001390: 7473 2e70 6e67 290a 0a57 6869 6c65 2065  ts.png)..While e
-000013a0: 7870 6572 696d 656e 7473 2061 7265 2072  xperiments are r
-000013b0: 756e 6e69 6e67 2c20 6c69 7665 2075 7064  unning, live upd
-000013c0: 6174 6573 2077 696c 6c20 6265 2064 6973  ates will be dis
-000013d0: 706c 6179 6564 2069 6e20 626f 7468 2076  played in both v
-000013e0: 6965 7773 2e0a 0a23 2323 2044 5643 2053  iews...### DVC S
-000013f0: 7475 6469 6f0a 0a49 6620 796f 7520 7075  tudio..If you pu
-00001400: 7368 2074 6865 2072 6573 756c 7473 2074  sh the results t
-00001410: 6f20 5b44 5643 2053 7475 6469 6f5d 2868  o [DVC Studio](h
-00001420: 7474 7073 3a2f 2f64 7663 2e6f 7267 2f64  ttps://dvc.org/d
-00001430: 6f63 2f73 7475 6469 6f29 2c20 796f 7520  oc/studio), you 
-00001440: 6361 6e0a 636f 6d70 6172 6520 6578 7065  can.compare expe
-00001450: 7269 6d65 6e74 7320 6167 6169 6e73 7420  riments against 
-00001460: 7468 6520 656e 7469 7265 2072 6570 6f20  the entire repo 
-00001470: 6869 7374 6f72 793a 0a0a 215b 5374 7564  history:..![Stud
-00001480: 696f 2043 6f6d 7061 7265 5d28 2e2f 646f  io Compare](./do
-00001490: 6373 2f73 7475 6469 6f5f 636f 6d70 6172  cs/studio_compar
-000014a0: 652e 706e 6729 0a0a 596f 7520 6361 6e20  e.png)..You can 
-000014b0: 656e 6162 6c65 0a5b 5374 7564 696f 204c  enable.[Studio L
-000014c0: 6976 6520 4578 7065 7269 6d65 6e74 735d  ive Experiments]
-000014d0: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
-000014e0: 2f64 6f63 2f73 7475 6469 6f2f 7573 6572  /doc/studio/user
-000014f0: 2d67 7569 6465 2f70 726f 6a65 6374 732d  -guide/projects-
-00001500: 616e 642d 6578 7065 7269 6d65 6e74 732f  and-experiments/
-00001510: 6c69 7665 2d6d 6574 7269 6373 2d61 6e64  live-metrics-and
-00001520: 2d70 6c6f 7473 290a 746f 2073 6565 206c  -plots).to see l
-00001530: 6976 6520 7570 6461 7465 7320 7768 696c  ive updates whil
-00001540: 6520 6578 7065 7269 6d65 6e74 7320 6172  e experiments ar
-00001550: 6520 7275 6e6e 696e 672e 0a0a 5f5f 5f5f  e running...____
-00001560: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001570: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001580: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001590: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000015a0: 5f5f 0a0a 2320 436f 6d70 6172 6973 6f6e  __..# Comparison
-000015b0: 2074 6f20 7265 6c61 7465 6420 7465 6368   to related tech
-000015c0: 6e6f 6c6f 6769 6573 0a0a 2a2a 4456 434c  nologies..**DVCL
-000015d0: 6976 652a 2a20 6973 2061 6e20 2a4d 4c20  ive** is an *ML 
-000015e0: 4c6f 6767 6572 2a2c 2073 696d 696c 6172  Logger*, similar
-000015f0: 2074 6f3a 0a0a 2d20 5b4d 4c46 6c6f 775d   to:..- [MLFlow]
-00001600: 2868 7474 7073 3a2f 2f6d 6c66 6c6f 772e  (https://mlflow.
-00001610: 6f72 672f 290a 2d20 5b57 6569 6768 7473  org/).- [Weights
-00001620: 2026 2042 6961 7365 735d 2868 7474 7073   & Biases](https
-00001630: 3a2f 2f77 616e 6462 2e61 692f 7369 7465  ://wandb.ai/site
-00001640: 290a 2d20 5b4e 6570 7475 6e65 5d28 6874  ).- [Neptune](ht
-00001650: 7470 733a 2f2f 6e65 7074 756e 652e 6169  tps://neptune.ai
-00001660: 2f29 0a0a 5468 6520 6d61 696e 2064 6966  /)..The main dif
-00001670: 6665 7265 6e63 6520 7769 7468 2074 686f  ference with tho
-00001680: 7365 202a 4d4c 204c 6f67 6765 7273 2a20  se *ML Loggers* 
-00001690: 6973 2074 6861 7420 2a2a 4456 434c 6976  is that **DVCLiv
-000016a0: 652a 2a20 646f 6573 206e 6f74 0a2a 2a72  e** does not.**r
-000016b0: 6571 7569 7265 2a2a 2061 6e79 2061 6464  equire** any add
-000016c0: 6974 696f 6e61 6c20 7365 7276 6963 6573  itional services
-000016d0: 206f 7220 7365 7276 6572 7320 746f 2072   or servers to r
-000016e0: 756e 2e0a 0a4c 6f67 6765 6420 6d65 7472  un...Logged metr
-000016f0: 6963 732c 2070 6172 616d 6574 6572 732c  ics, parameters,
-00001700: 2061 6e64 2070 6c6f 7473 2061 7265 2073   and plots are s
-00001710: 746f 7265 6420 6173 2070 6c61 696e 2074  tored as plain t
-00001720: 6578 7420 6669 6c65 7320 7468 6174 2063  ext files that c
-00001730: 616e 2062 650a 7665 7273 696f 6e65 6420  an be.versioned 
-00001740: 6279 2074 6f6f 6c73 206c 696b 6520 4769  by tools like Gi
-00001750: 7420 6f72 2074 7261 636b 6564 2061 7320  t or tracked as 
-00001760: 706f 696e 7465 7273 2074 6f20 6669 6c65  pointers to file
-00001770: 7320 696e 2044 5643 2073 746f 7261 6765  s in DVC storage
-00001780: 2e0a 0a59 6f75 2063 616e 2074 6865 6e20  ...You can then 
-00001790: 7573 6520 6469 6666 6572 656e 7420 5b6f  use different [o
-000017a0: 7074 696f 6e73 5d28 2363 6f6d 7061 7269  ptions](#compari
-000017b0: 6e67 2920 746f 2076 6973 7561 6c69 7a65  ng) to visualize
-000017c0: 2074 6865 206d 6574 7269 6373 2c0a 7061   the metrics,.pa
-000017d0: 7261 6d65 7465 7273 2c20 616e 6420 706c  rameters, and pl
-000017e0: 6f74 7320 6163 726f 7373 2065 7870 6572  ots across exper
-000017f0: 696d 656e 7473 2e0a 0a5f 5f5f 5f5f 5f5f  iments..._______
-00001800: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001810: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001820: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001830: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f0a  _______________.
-00001840: 0a23 2043 6f6e 7472 6962 7574 696e 670a  .# Contributing.
-00001850: 0a43 6f6e 7472 6962 7574 696f 6e73 2061  .Contributions a
-00001860: 7265 2076 6572 7920 7765 6c63 6f6d 652e  re very welcome.
-00001870: 2054 6f20 6c65 6172 6e20 6d6f 7265 2c20   To learn more, 
-00001880: 7365 6520 7468 650a 5b43 6f6e 7472 6962  see the.[Contrib
-00001890: 7574 6f72 2047 7569 6465 5d28 434f 4e54  utor Guide](CONT
-000018a0: 5249 4255 5449 4e47 2e72 7374 292e 0a0a  RIBUTING.rst)...
-000018b0: 2320 4c69 6365 6e73 650a 0a44 6973 7472  # License..Distr
-000018c0: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
-000018d0: 2074 6572 6d73 206f 6620 7468 650a 5b41   terms of the.[A
-000018e0: 7061 6368 6520 322e 3020 6c69 6365 6e73  pache 2.0 licens
-000018f0: 655d 2868 7474 7073 3a2f 2f6f 7065 6e73  e](https://opens
-00001900: 6f75 7263 652e 6f72 672f 6c69 6365 6e73  ource.org/licens
-00001910: 6573 2f41 7061 6368 652d 322e 3029 2c20  es/Apache-2.0), 
-00001920: 2a64 7663 6c69 7665 2a20 6973 0a66 7265  *dvclive* is.fre
-00001930: 6520 616e 6420 6f70 656e 2073 6f75 7263  e and open sourc
-00001940: 6520 736f 6674 7761 7265 2e0a            e software..
+00001120: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001130: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001140: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001150: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001160: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001170: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001180: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001190: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000011a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000011b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000011c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000011d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000011e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000011f0: 9480 e294 800a 6060 600a 0a60 6060 636f  ......```..```co
+00001200: 6e73 6f6c 650a 2420 6476 6320 706c 6f74  nsole.$ dvc plot
+00001210: 7320 6469 6666 2024 2864 7663 2065 7870  s diff $(dvc exp
+00001220: 206c 6973 7420 2d2d 6e61 6d65 732d 6f6e   list --names-on
+00001230: 6c79 2920 2d2d 6f70 656e 0a60 6060 0a0a  ly) --open.```..
+00001240: 215b 6476 6320 706c 6f74 7320 6469 6666  ![dvc plots diff
+00001250: 5d28 2e2f 646f 6373 2f64 7663 5f70 6c6f  ](./docs/dvc_plo
+00001260: 7473 5f64 6966 662e 706e 6729 0a0a 2323  ts_diff.png)..##
+00001270: 2320 4456 4320 4578 7465 6e73 696f 6e20  # DVC Extension 
+00001280: 666f 7220 5653 2043 6f64 650a 0a49 6e73  for VS Code..Ins
+00001290: 6964 6520 7468 650a 5b44 5643 2045 7874  ide the.[DVC Ext
+000012a0: 656e 7369 6f6e 2066 6f72 2056 5320 436f  ension for VS Co
+000012b0: 6465 5d28 6874 7470 733a 2f2f 6d61 726b  de](https://mark
+000012c0: 6574 706c 6163 652e 7669 7375 616c 7374  etplace.visualst
+000012d0: 7564 696f 2e63 6f6d 2f69 7465 6d73 3f69  udio.com/items?i
+000012e0: 7465 6d4e 616d 653d 4974 6572 6174 6976  temName=Iterativ
+000012f0: 652e 6476 6329 2c0a 796f 7520 6361 6e20  e.dvc),.you can 
+00001300: 636f 6d70 6172 6520 616e 6420 7669 7375  compare and visu
+00001310: 616c 697a 6520 7265 7375 6c74 7320 7573  alize results us
+00001320: 696e 6720 7468 650a 5b45 7870 6572 696d  ing the.[Experim
+00001330: 656e 7473 5d28 6874 7470 733a 2f2f 6769  ents](https://gi
+00001340: 7468 7562 2e63 6f6d 2f69 7465 7261 7469  thub.com/iterati
+00001350: 7665 2f76 7363 6f64 652d 6476 632f 626c  ve/vscode-dvc/bl
+00001360: 6f62 2f6d 6169 6e2f 6578 7465 6e73 696f  ob/main/extensio
+00001370: 6e2f 7265 736f 7572 6365 732f 7761 6c6b  n/resources/walk
+00001380: 7468 726f 7567 682f 6578 7065 7269 6d65  through/experime
+00001390: 6e74 732d 7461 626c 652e 6d64 290a 616e  nts-table.md).an
+000013a0: 640a 5b50 6c6f 7473 5d28 6874 7470 733a  d.[Plots](https:
+000013b0: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7465  //github.com/ite
+000013c0: 7261 7469 7665 2f76 7363 6f64 652d 6476  rative/vscode-dv
+000013d0: 632f 626c 6f62 2f6d 6169 6e2f 6578 7465  c/blob/main/exte
+000013e0: 6e73 696f 6e2f 7265 736f 7572 6365 732f  nsion/resources/
+000013f0: 7761 6c6b 7468 726f 7567 682f 706c 6f74  walkthrough/plot
+00001400: 732e 6d64 290a 7669 6577 733a 0a0a 215b  s.md).views:..![
+00001410: 5653 436f 6465 2045 7870 6572 696d 656e  VSCode Experimen
+00001420: 7473 5d28 2e2f 646f 6373 2f76 7363 6f64  ts](./docs/vscod
+00001430: 655f 6578 7065 7269 6d65 6e74 732e 706e  e_experiments.pn
+00001440: 6729 0a0a 215b 5653 436f 6465 2050 6c6f  g)..![VSCode Plo
+00001450: 7473 5d28 2e2f 646f 6373 2f76 7363 6f64  ts](./docs/vscod
+00001460: 655f 706c 6f74 732e 706e 6729 0a0a 5768  e_plots.png)..Wh
+00001470: 696c 6520 6578 7065 7269 6d65 6e74 7320  ile experiments 
+00001480: 6172 6520 7275 6e6e 696e 672c 206c 6976  are running, liv
+00001490: 6520 7570 6461 7465 7320 7769 6c6c 2062  e updates will b
+000014a0: 6520 6469 7370 6c61 7965 6420 696e 2062  e displayed in b
+000014b0: 6f74 6820 7669 6577 732e 0a0a 2323 2320  oth views...### 
+000014c0: 4456 4320 5374 7564 696f 0a0a 4966 2079  DVC Studio..If y
+000014d0: 6f75 2070 7573 6820 7468 6520 7265 7375  ou push the resu
+000014e0: 6c74 7320 746f 205b 4456 4320 5374 7564  lts to [DVC Stud
+000014f0: 696f 5d28 6874 7470 733a 2f2f 6476 632e  io](https://dvc.
+00001500: 6f72 672f 646f 632f 7374 7564 696f 292c  org/doc/studio),
+00001510: 2079 6f75 2063 616e 0a63 6f6d 7061 7265   you can.compare
+00001520: 2065 7870 6572 696d 656e 7473 2061 6761   experiments aga
+00001530: 696e 7374 2074 6865 2065 6e74 6972 6520  inst the entire 
+00001540: 7265 706f 2068 6973 746f 7279 3a0a 0a21  repo history:..!
+00001550: 5b53 7475 6469 6f20 436f 6d70 6172 655d  [Studio Compare]
+00001560: 282e 2f64 6f63 732f 7374 7564 696f 5f63  (./docs/studio_c
+00001570: 6f6d 7061 7265 2e70 6e67 290a 0a59 6f75  ompare.png)..You
+00001580: 2063 616e 2065 6e61 626c 650a 5b53 7475   can enable.[Stu
+00001590: 6469 6f20 4c69 7665 2045 7870 6572 696d  dio Live Experim
+000015a0: 656e 7473 5d28 6874 7470 733a 2f2f 6476  ents](https://dv
+000015b0: 632e 6f72 672f 646f 632f 7374 7564 696f  c.org/doc/studio
+000015c0: 2f75 7365 722d 6775 6964 652f 7072 6f6a  /user-guide/proj
+000015d0: 6563 7473 2d61 6e64 2d65 7870 6572 696d  ects-and-experim
+000015e0: 656e 7473 2f6c 6976 652d 6d65 7472 6963  ents/live-metric
+000015f0: 732d 616e 642d 706c 6f74 7329 0a74 6f20  s-and-plots).to 
+00001600: 7365 6520 6c69 7665 2075 7064 6174 6573  see live updates
+00001610: 2077 6869 6c65 2065 7870 6572 696d 656e   while experimen
+00001620: 7473 2061 7265 2072 756e 6e69 6e67 2e0a  ts are running..
+00001630: 0a5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ._______________
+00001640: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001650: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001660: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001670: 5f5f 5f5f 5f5f 5f0a 0a23 2043 6f6d 7061  _______..# Compa
+00001680: 7269 736f 6e20 746f 2072 656c 6174 6564  rison to related
+00001690: 2074 6563 686e 6f6c 6f67 6965 730a 0a2a   technologies..*
+000016a0: 2a44 5643 4c69 7665 2a2a 2069 7320 616e  *DVCLive** is an
+000016b0: 202a 4d4c 204c 6f67 6765 722a 2c20 7369   *ML Logger*, si
+000016c0: 6d69 6c61 7220 746f 3a0a 0a2d 205b 4d4c  milar to:..- [ML
+000016d0: 466c 6f77 5d28 6874 7470 733a 2f2f 6d6c  Flow](https://ml
+000016e0: 666c 6f77 2e6f 7267 2f29 0a2d 205b 5765  flow.org/).- [We
+000016f0: 6967 6874 7320 2620 4269 6173 6573 5d28  ights & Biases](
+00001700: 6874 7470 733a 2f2f 7761 6e64 622e 6169  https://wandb.ai
+00001710: 2f73 6974 6529 0a2d 205b 4e65 7074 756e  /site).- [Neptun
+00001720: 655d 2868 7474 7073 3a2f 2f6e 6570 7475  e](https://neptu
+00001730: 6e65 2e61 692f 290a 0a54 6865 206d 6169  ne.ai/)..The mai
+00001740: 6e20 6469 6666 6572 656e 6365 2077 6974  n difference wit
+00001750: 6820 7468 6f73 6520 2a4d 4c20 4c6f 6767  h those *ML Logg
+00001760: 6572 732a 2069 7320 7468 6174 202a 2a44  ers* is that **D
+00001770: 5643 4c69 7665 2a2a 2064 6f65 7320 6e6f  VCLive** does no
+00001780: 740a 2a2a 7265 7175 6972 652a 2a20 616e  t.**require** an
+00001790: 7920 6164 6469 7469 6f6e 616c 2073 6572  y additional ser
+000017a0: 7669 6365 7320 6f72 2073 6572 7665 7273  vices or servers
+000017b0: 2074 6f20 7275 6e2e 0a0a 4c6f 6767 6564   to run...Logged
+000017c0: 206d 6574 7269 6373 2c20 7061 7261 6d65   metrics, parame
+000017d0: 7465 7273 2c20 616e 6420 706c 6f74 7320  ters, and plots 
+000017e0: 6172 6520 7374 6f72 6564 2061 7320 706c  are stored as pl
+000017f0: 6169 6e20 7465 7874 2066 696c 6573 2074  ain text files t
+00001800: 6861 7420 6361 6e20 6265 0a76 6572 7369  hat can be.versi
+00001810: 6f6e 6564 2062 7920 746f 6f6c 7320 6c69  oned by tools li
+00001820: 6b65 2047 6974 206f 7220 7472 6163 6b65  ke Git or tracke
+00001830: 6420 6173 2070 6f69 6e74 6572 7320 746f  d as pointers to
+00001840: 2066 696c 6573 2069 6e20 4456 4320 7374   files in DVC st
+00001850: 6f72 6167 652e 0a0a 596f 7520 6361 6e20  orage...You can 
+00001860: 7468 656e 2075 7365 2064 6966 6665 7265  then use differe
+00001870: 6e74 205b 6f70 7469 6f6e 735d 2823 636f  nt [options](#co
+00001880: 6d70 6172 696e 6729 2074 6f20 7669 7375  mparing) to visu
+00001890: 616c 697a 6520 7468 6520 6d65 7472 6963  alize the metric
+000018a0: 732c 0a70 6172 616d 6574 6572 732c 2061  s,.parameters, a
+000018b0: 6e64 2070 6c6f 7473 2061 6372 6f73 7320  nd plots across 
+000018c0: 6578 7065 7269 6d65 6e74 732e 0a0a 5f5f  experiments...__
+000018d0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000018e0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000018f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001900: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001910: 5f5f 5f5f 0a0a 2320 436f 6e74 7269 6275  ____..# Contribu
+00001920: 7469 6e67 0a0a 436f 6e74 7269 6275 7469  ting..Contributi
+00001930: 6f6e 7320 6172 6520 7665 7279 2077 656c  ons are very wel
+00001940: 636f 6d65 2e20 546f 206c 6561 726e 206d  come. To learn m
+00001950: 6f72 652c 2073 6565 2074 6865 0a5b 436f  ore, see the.[Co
+00001960: 6e74 7269 6275 746f 7220 4775 6964 655d  ntributor Guide]
+00001970: 2843 4f4e 5452 4942 5554 494e 472e 7273  (CONTRIBUTING.rs
+00001980: 7429 2e0a 0a23 204c 6963 656e 7365 0a0a  t)...# License..
+00001990: 4469 7374 7269 6275 7465 6420 756e 6465  Distributed unde
+000019a0: 7220 7468 6520 7465 726d 7320 6f66 2074  r the terms of t
+000019b0: 6865 0a5b 4170 6163 6865 2032 2e30 206c  he.[Apache 2.0 l
+000019c0: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+000019d0: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+000019e0: 6963 656e 7365 732f 4170 6163 6865 2d32  icenses/Apache-2
+000019f0: 2e30 292c 202a 6476 636c 6976 652a 2069  .0), *dvclive* i
+00001a00: 730a 6672 6565 2061 6e64 206f 7065 6e20  s.free and open 
+00001a10: 736f 7572 6365 2073 6f66 7477 6172 652e  source software.
+00001a20: 0a                                       .
```

### Comparing `dvclive-2.6.4/docs/dvc_plots_diff.png` & `dvclive-2.7.0/docs/dvc_plots_diff.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/docs/studio_compare.png` & `dvclive-2.7.0/docs/studio_compare.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/docs/vscode_experiments.png` & `dvclive-2.7.0/docs/vscode_experiments.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/docs/vscode_plots.png` & `dvclive-2.7.0/docs/vscode_plots.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/pyproject.toml` & `dvclive-2.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/setup.cfg` & `dvclive-2.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 python_requires = >=3.8
 zip_safe = False
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	dvc>2.45.1
+	dvc-studio-client>=0.7.0,<1
 	funcy
 	ruamel.yaml
+	scmrepo
 
 [options.extras_require]
 image = 
 	numpy
 	pillow
 sklearn = 
 	scikit-learn
@@ -68,15 +70,15 @@
 	datasets
 catalyst = 
 	catalyst>22
 fastai = 
 	fastai
 pytorch_lightning = 
 	pytorch_lightning>=1.9
-	torch<1.13
+	torch<2.1
 optuna = 
 	optuna
 all = 
 	%(image)s
 	%(mmcv)s
 	%(tf)s
 	%(xgb)s
```

### Comparing `dvclive-2.6.4/src/dvclive/catalyst.py` & `dvclive-2.7.0/src/dvclive/catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/dvc.py` & `dvclive-2.7.0/src/dvclive/dvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # ruff: noqa: SLF001
 import logging
 import os
 import random
-from io import StringIO
 from pathlib import Path
 
 from dvclive import env
 from dvclive.plots import Image, Metric
-from dvclive.serialize import dump_yaml, get_yaml
+from dvclive.serialize import dump_yaml
 
 logging.basicConfig()
 logger = logging.getLogger("dvclive")
 logger.setLevel(os.getenv(env.DVCLIVE_LOGLEVEL, "INFO").upper())
 
 _CHECKPOINT_SLEEP = 0.1
 
@@ -73,20 +72,24 @@
     while os.path.exists(signal_file):
         sleep(_CHECKPOINT_SLEEP)
 
 
 def get_dvc_repo():
     from dvc.exceptions import NotDvcRepoError
     from dvc.repo import Repo
-    from dvc.scm import SCMError
+    from dvc.scm import Git, SCMError
+    from scmrepo.exceptions import SCMError as GitSCMError
 
     try:
         return Repo()
     except (NotDvcRepoError, SCMError):
-        return None
+        try:
+            return Repo.init(Git().root_dir)
+        except GitSCMError:
+            return None
 
 
 def make_dvcyaml(live):
     dvcyaml = {}
     if live._params:
         dvcyaml["params"] = [os.path.relpath(live.params_file, live.dir)]
     if live._metrics or live.summary:
@@ -103,14 +106,22 @@
     if live._plots:
         for plot in live._plots.values():
             plot_path = plot.output_path.relative_to(live.dir)
             plots.append({plot_path.as_posix(): plot.get_properties()})
     if plots:
         dvcyaml["plots"] = plots
 
+    if live._artifacts:
+        dvcyaml["artifacts"] = live._artifacts
+        for artifact in dvcyaml["artifacts"].values():
+            abs_path = os.path.realpath(artifact["path"])
+            abs_dir = os.path.realpath(live.dir)
+            relative_path = os.path.relpath(abs_path, abs_dir)
+            artifact["path"] = Path(relative_path).as_posix()
+
     dump_yaml(dvcyaml, live.dvc_file)
 
 
 def mark_dvclive_only_started():
     """
     Signal DVC VS Code extension that
     an experiment is running in the workspace.
@@ -153,27 +164,7 @@
     while True:
         adjective = random.choice(ADJECTIVES)  # noqa: S311
         noun = random.choice(NOUNS)  # noqa: S311
         name = f"{adjective}-{noun}"
         exp_ref = ExpRefInfo(baseline_sha=baseline_rev, name=name)
         if not scm.get_ref(str(exp_ref)):
             return name
-
-
-def get_dvc_stage_template(live):
-    stage = {
-        "cmd": "<python my_code_file.py my_args>",
-        "deps": ["<my_code_file.py>"],
-    }
-    if live._outs:
-        stage["outs"] = []
-    for o in live._outs:
-        artifact_path = Path(os.getcwd()) / o
-        artifact_path = artifact_path.relative_to(live._dvc_repo.root_dir).as_posix()
-        stage["outs"].append(artifact_path)
-    dvcyaml_dict = {"stages": {"dvclive": stage}}
-
-    output = StringIO()
-    get_yaml().dump(dvcyaml_dict, output)
-    dvcyaml = output.getvalue()
-    output.close()
-    return dvcyaml
```

### Comparing `dvclive-2.6.4/src/dvclive/error.py` & `dvclive-2.7.0/src/dvclive/error.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/fastai.py` & `dvclive-2.7.0/src/dvclive/fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/huggingface.py` & `dvclive-2.7.0/src/dvclive/huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/keras.py` & `dvclive-2.7.0/src/dvclive/keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/lgbm.py` & `dvclive-2.7.0/src/dvclive/lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/lightning.py` & `dvclive-2.7.0/src/dvclive/lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/live.py` & `dvclive-2.7.0/src/dvclive/live.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import json
 import logging
 import os
 import shutil
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Union
 
-from dvc_studio_client.env import STUDIO_TOKEN
+from dvc_studio_client.env import DVC_STUDIO_TOKEN, STUDIO_TOKEN
 from dvc_studio_client.post_live_metrics import post_live_metrics
 from funcy import set_in
 from pathspec import PathSpec
 from ruamel.yaml.representer import RepresenterError
 
 from . import env
 from .dvc import (
     get_dvc_repo,
-    get_dvc_stage_template,
     get_random_exp_name,
     make_checkpoint,
     make_dvcyaml,
     mark_dvclive_only_ended,
     mark_dvclive_only_started,
 )
 from .error import (
@@ -56,15 +55,15 @@
         self._resume: bool = resume or env2bool(env.DVCLIVE_RESUME)
         self._save_dvc_exp: bool = save_dvc_exp
         self._step: Optional[int] = None
         self._metrics: Dict[str, Any] = {}
         self._images: Dict[str, Any] = {}
         self._params: Dict[str, Any] = {}
         self._plots: Dict[str, Any] = {}
-        self._outs: Set[StrPath] = set()
+        self._artifacts: Dict[str, Dict] = {}
         self._inside_with = False
         self._dvcyaml = dvcyaml
 
         os.makedirs(self.dir, exist_ok=True)
 
         self._report_mode: Optional[str] = report
         self._report_notebook = None
@@ -121,31 +120,39 @@
                 )
                 self._save_dvc_exp = False
 
         self._dvc_repo = get_dvc_repo()
         if self._dvc_repo is None:
             if self._save_dvc_exp:
                 logger.warning(
-                    "Can't save experiment without a DVC Repo."
-                    "\nYou can create a DVC Repo by calling `dvc init`."
+                    "Can't save experiment without a Git Repo."
+                    "\nCreate a Git repo (`git init`) and commit (`git commit`)."
+                )
+                self._save_dvc_exp = False
+            return
+        if self._dvc_repo.scm.no_commits:
+            if self._save_dvc_exp:
+                logger.warning(
+                    "Can't save experiment to an empty Git Repo."
+                    "\nAdd a commit (`git commit`) to save experiments."
                 )
                 self._save_dvc_exp = False
             return
 
         if self._inside_dvc_exp:
             return
 
         self._baseline_rev = self._dvc_repo.scm.get_rev()
         if self._save_dvc_exp:
             self._exp_name = get_random_exp_name(self._dvc_repo.scm, self._baseline_rev)
             mark_dvclive_only_started()
             self._include_untracked.append(self.dir)
 
     def _init_studio(self):
-        if not os.getenv(STUDIO_TOKEN, None):
+        if not any((os.getenv(STUDIO_TOKEN, None), os.getenv(DVC_STUDIO_TOKEN, None))):
             logger.debug("Missing env var `STUDIO_TOKEN`, skipping `studio` report.")
             self._studio_events_to_skip.add("start")
             self._studio_events_to_skip.add("data")
             self._studio_events_to_skip.add("done")
         elif self._inside_dvc_exp:
             logger.debug("Skipping `studio` report `start` and `done` events.")
             self._studio_events_to_skip.add("start")
@@ -287,15 +294,15 @@
     def log_sklearn_plot(self, kind, labels, predictions, name=None, **kwargs):
         val = (labels, predictions)
 
         name = name or kind
         if name in self._plots:
             data = self._plots[name]
         elif kind in SKLEARN_PLOTS and SKLEARN_PLOTS[kind].could_log(val):
-            data = SKLEARN_PLOTS[kind](name, self.plots_dir)
+            data = SKLEARN_PLOTS[kind](name, self.plots_dir, **kwargs)
             self._plots[data.name] = data
         else:
             raise InvalidPlotTypeError(name)
 
         data.step = self.step
         data.dump(val, **kwargs)
         logger.debug(f"Logged {name}")
@@ -317,27 +324,50 @@
         self._dump_params()
         logger.debug(f"Logged {params} parameters to {self.params_file}")
 
     def log_param(self, name: str, val: ParamLike):
         """Saves the given parameter value to yaml"""
         self.log_params({name: val})
 
-    def log_artifact(self, path: StrPath):
+    def log_artifact(
+        self,
+        path: StrPath,
+        type: Optional[str] = None,  # noqa: A002
+        name: Optional[str] = None,
+        desc: Optional[str] = None,  # noqa: ARG002
+        labels: Optional[List[str]] = None,  # noqa: ARG002
+        meta: Optional[Dict[str, Any]] = None,  # noqa: ARG002
+    ):
         """Tracks a local file or directory with DVC"""
         if not isinstance(path, (str, Path)):
             raise InvalidDataTypeError(path, type(path))
 
         if self._dvc_repo is not None:
+            from dvc.repo.artifacts import name_is_compatible
+
             try:
                 stage = self._dvc_repo.add(path)
             except Exception as e:  # noqa: BLE001
                 logger.warning(f"Failed to dvc add {path}: {e}")
                 return
 
-            self._outs.add(path)
+            name = name or Path(path).stem
+            if name_is_compatible(name):
+                self._artifacts[name] = {
+                    k: v
+                    for k, v in locals().items()
+                    if k in ("path", "type", "desc", "labels", "meta") and v is not None
+                }
+            else:
+                logger.warning(
+                    "Can't use '%s' as artifact name (ID)."
+                    " It will not be included in the `artifacts` section.",
+                    name,
+                )
+
             dvc_file = stage[0].addressing
 
             if self._save_dvc_exp:
                 self._include_untracked.append(dvc_file)
                 self._include_untracked.append(
                     str(Path(dvc_file).parent / ".gitignore")
                 )
@@ -406,24 +436,14 @@
             if not response:
                 logger.warning("`post_to_studio` `done` event failed.")
             self._studio_events_to_skip.add("done")
             self._studio_events_to_skip.add("data")
         else:
             self.make_report()
 
-        if self._dvc_repo and not self._inside_dvc_exp:
-            from dvc.exceptions import DvcException
-
-            try:
-                path = os.path.join(self._dvc_repo.root_dir, "dvc.yaml")
-                yaml = get_dvc_stage_template(self)
-                logger.info(f"To run with DVC, add this to {path}:\n{yaml}")
-            except DvcException as e:
-                logger.warning(f"Failed to print DVC stage template:\n{e}")
-
     def make_checkpoint(self):
         if env2bool(env.DVC_CHECKPOINT):
             make_checkpoint()
 
     def read_step(self):
         if Path(self.metrics_file).exists():
             latest = self.read_latest()
```

### Comparing `dvclive-2.6.4/src/dvclive/optuna.py` & `dvclive-2.7.0/src/dvclive/optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/plots/base.py` & `dvclive-2.7.0/src/dvclive/plots/base.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/plots/image.py` & `dvclive-2.7.0/src/dvclive/plots/image.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/plots/metric.py` & `dvclive-2.7.0/src/dvclive/plots/metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/plots/sklearn.py` & `dvclive-2.7.0/src/dvclive/plots/sklearn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import copy
 from pathlib import Path
 
 from dvclive.serialize import dump_json
 
 from .base import Data
 
 
 class SKLearnPlot(Data):
     suffixes = [".json"]
     subfolder = "sklearn"
 
-    def __init__(self, name: str, output_folder: str) -> None:
+    def __init__(self, name: str, output_folder: str, **kwargs) -> None:  # noqa: ARG002
         super().__init__(name, output_folder)
         self.name = self.name.replace(".json", "")
 
     @property
     def output_path(self) -> Path:
         _path = Path(f"{self.output_folder / self.name}.json")
         _path.parent.mkdir(exist_ok=True, parents=True)
@@ -21,30 +22,30 @@
 
     @staticmethod
     def could_log(val: object) -> bool:
         if isinstance(val, tuple) and len(val) == 2:  # noqa: PLR2004
             return True
         return False
 
-    @staticmethod
-    def get_properties():
+    def get_properties(self):
         raise NotImplementedError
 
 
 class Roc(SKLearnPlot):
-    @staticmethod
-    def get_properties():
-        return {
-            "template": "simple",
-            "x": "fpr",
-            "y": "tpr",
-            "title": "Receiver operating characteristic (ROC)",
-            "x_label": "False Positive Rate",
-            "y_label": "True Positive Rate",
-        }
+    DEFAULT_PROPERTIES = {
+        "template": "simple",
+        "x": "fpr",
+        "y": "tpr",
+        "title": "Receiver operating characteristic (ROC)",
+        "x_label": "False Positive Rate",
+        "y_label": "True Positive Rate",
+    }
+
+    def get_properties(self):
+        return copy.deepcopy(self.DEFAULT_PROPERTIES)
 
     def dump(self, val, **kwargs) -> None:
         from sklearn import metrics
 
         fpr, tpr, roc_thresholds = metrics.roc_curve(
             y_true=val[0], y_score=val[1], **kwargs
         )
@@ -54,24 +55,25 @@
                 for fp, tp, t in zip(fpr, tpr, roc_thresholds)
             ]
         }
         dump_json(roc, self.output_path)
 
 
 class PrecisionRecall(SKLearnPlot):
-    @staticmethod
-    def get_properties():
-        return {
-            "template": "simple",
-            "x": "recall",
-            "y": "precision",
-            "title": "Precision-Recall Curve",
-            "x_label": "Recall",
-            "y_label": "Precision",
-        }
+    DEFAULT_PROPERTIES = {
+        "template": "simple",
+        "x": "recall",
+        "y": "precision",
+        "title": "Precision-Recall Curve",
+        "x_label": "Recall",
+        "y_label": "Precision",
+    }
+
+    def get_properties(self):
+        return copy.deepcopy(self.DEFAULT_PROPERTIES)
 
     def dump(self, val, **kwargs) -> None:
         from sklearn import metrics
 
         precision, recall, prc_thresholds = metrics.precision_recall_curve(
             y_true=val[0], probas_pred=val[1], **kwargs
         )
@@ -82,24 +84,25 @@
                 for p, r, t in zip(precision, recall, prc_thresholds)
             ]
         }
         dump_json(prc, self.output_path)
 
 
 class Det(SKLearnPlot):
-    @staticmethod
-    def get_properties():
-        return {
-            "template": "simple",
-            "x": "fpr",
-            "y": "fnr",
-            "title": "Detection error tradeoff (DET)",
-            "x_label": "False Positive Rate",
-            "y_label": "False Negative Rate",
-        }
+    DEFAULT_PROPERTIES = {
+        "template": "simple",
+        "x": "fpr",
+        "y": "fnr",
+        "title": "Detection error tradeoff (DET)",
+        "x_label": "False Positive Rate",
+        "y_label": "False Negative Rate",
+    }
+
+    def get_properties(self):
+        return copy.deepcopy(self.DEFAULT_PROPERTIES)
 
     def dump(self, val, **kwargs) -> None:
         from sklearn import metrics
 
         fpr, fnr, roc_thresholds = metrics.det_curve(
             y_true=val[0], y_score=val[1], **kwargs
         )
@@ -110,44 +113,53 @@
                 for fp, fn, t in zip(fpr, fnr, roc_thresholds)
             ]
         }
         dump_json(det, self.output_path)
 
 
 class ConfusionMatrix(SKLearnPlot):
-    @staticmethod
-    def get_properties():
-        return {
-            "template": "confusion",
-            "x": "actual",
-            "y": "predicted",
-            "title": "Confusion Matrix",
-            "x_label": "True Label",
-            "y_label": "Predicted Label",
-        }
+    DEFAULT_PROPERTIES = {
+        "template": "confusion",
+        "x": "actual",
+        "y": "predicted",
+        "title": "Confusion Matrix",
+        "x_label": "True Label",
+        "y_label": "Predicted Label",
+    }
+
+    def __init__(self, name: str, output_folder: str, **kwargs) -> None:
+        super().__init__(name, output_folder)
+        self.normalized = kwargs.get("normalized") or False
+
+    def get_properties(self):
+        properties = copy.deepcopy(self.DEFAULT_PROPERTIES)
+        if self.normalized:
+            properties["template"] = "confusion_normalized"
+        return properties
 
     def dump(self, val, **kwargs) -> None:  # noqa: ARG002
         cm = [
             {"actual": str(actual), "predicted": str(predicted)}
             for actual, predicted in zip(val[0], val[1])
         ]
         dump_json(cm, self.output_path)
 
 
 class Calibration(SKLearnPlot):
-    @staticmethod
-    def get_properties():
-        return {
-            "template": "simple",
-            "x": "prob_pred",
-            "y": "prob_true",
-            "title": "Calibration Curve",
-            "x_label": "Mean Predicted Probability",
-            "y_label": "Fraction of Positives",
-        }
+    DEFAULT_PROPERTIES = {
+        "template": "simple",
+        "x": "prob_pred",
+        "y": "prob_true",
+        "title": "Calibration Curve",
+        "x_label": "Mean Predicted Probability",
+        "y_label": "Fraction of Positives",
+    }
+
+    def get_properties(self):
+        return copy.deepcopy(self.DEFAULT_PROPERTIES)
 
     def dump(self, val, **kwargs) -> None:
         from sklearn import calibration
 
         prob_true, prob_pred = calibration.calibration_curve(
             y_true=val[0], y_prob=val[1], **kwargs
         )
```

### Comparing `dvclive-2.6.4/src/dvclive/plots/utils.py` & `dvclive-2.7.0/src/dvclive/plots/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/report.py` & `dvclive-2.7.0/src/dvclive/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,25 +89,20 @@
 def get_plot_renderers(plots_folder, live):
     renderers = []
     for suffix in SKLearnPlot.suffixes:
         for file in Path(plots_folder).rglob(f"*{suffix}"):
             name = file.relative_to(plots_folder).with_suffix("").as_posix()
             properties = {}
 
-            if name in SKLEARN_PLOTS:
-                properties = SKLEARN_PLOTS[name].get_properties()
-                data_field = name
-            else:
-                # Plot with custom name
-                logged_plot = live._plots[name]
-                for default_name, plot_class in SKLEARN_PLOTS.items():
-                    if isinstance(logged_plot, plot_class):
-                        properties = plot_class.get_properties()
-                        data_field = default_name
-                        break
+            logged_plot = live._plots[name]
+            for default_name, plot_class in SKLEARN_PLOTS.items():
+                if isinstance(logged_plot, plot_class):
+                    properties = logged_plot.get_properties()
+                    data_field = default_name
+                    break
 
             data = json.loads(file.read_text())
 
             if data_field in data:
                 data = data[data_field]
 
             for row in data:
```

### Comparing `dvclive-2.6.4/src/dvclive/serialize.py` & `dvclive-2.7.0/src/dvclive/serialize.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/studio.py` & `dvclive-2.7.0/src/dvclive/studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/utils.py` & `dvclive-2.7.0/src/dvclive/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive/xgb.py` & `dvclive-2.7.0/src/dvclive/xgb.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/src/dvclive.egg-info/PKG-INFO` & `dvclive-2.7.0/src/dvclive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6476 636c  : 2.1.Name: dvcl
-00000020: 6976 650a 5665 7273 696f 6e3a 2032 2e36  ive.Version: 2.6
-00000030: 2e34 0a53 756d 6d61 7279 3a20 4d65 7472  .4.Summary: Metr
+00000020: 6976 650a 5665 7273 696f 6e3a 2032 2e37  ive.Version: 2.7
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4d65 7472  .0.Summary: Metr
 00000040: 6963 206c 6f67 6765 7220 666f 7220 4d4c  ic logger for ML
 00000050: 2070 726f 6a65 6374 732e 0a48 6f6d 652d   projects..Home-
 00000060: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000070: 7468 7562 2e63 6f6d 2f69 7465 7261 7469  thub.com/iterati
 00000080: 7665 2f64 7663 6c69 7665 0a4d 6169 6e74  ve/dvclive.Maint
 00000090: 6169 6e65 722d 656d 6169 6c3a 2073 7570  ainer-email: sup
 000000a0: 706f 7274 4064 7663 2e6f 7267 0a4c 6963  port@dvc.org.Lic
@@ -154,323 +154,337 @@
 00000990: 672f 646f 632f 6476 636c 6976 652f 6d6c  g/doc/dvclive/ml
 000009a0: 2d66 7261 6d65 776f 726b 7329 0a0a 5f5f  -frameworks)..__
 000009b0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009c0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009d0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009e0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000009f0: 5f5f 5f5f 0a0a 2320 5175 6963 6b73 7461  ____..# Quicksta
-00000a00: 7274 0a0a 2323 2049 6e73 7461 6c6c 202a  rt..## Install *
-00000a10: 6476 636c 6976 652a 0a0a 6060 6063 6f6e  dvclive*..```con
-00000a20: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
-00000a30: 6c6c 2064 7663 6c69 7665 0a60 6060 0a0a  ll dvclive.```..
-00000a40: 2323 2049 6e69 7469 616c 697a 6520 4456  ## Initialize DV
-00000a50: 4320 5265 706f 7369 746f 7279 0a0a 6060  C Repository..``
-00000a60: 6063 6f6e 736f 6c65 0a24 2067 6974 2069  `console.$ git i
-00000a70: 6e69 740a 2420 6476 6320 696e 6974 0a24  nit.$ dvc init.$
-00000a80: 2067 6974 2063 6f6d 6d69 7420 2d6d 2022   git commit -m "
-00000a90: 4456 4320 696e 6974 220a 6060 600a 0a23  DVC init".```..#
-00000aa0: 2320 4578 616d 706c 6520 636f 6465 0a0a  # Example code..
-00000ab0: 436f 7079 2074 6865 2073 6e69 7070 6574  Copy the snippet
-00000ac0: 2062 656c 6f77 2061 7320 6120 6261 7369   below as a basi
-00000ad0: 6320 6578 616d 706c 6520 6f66 2074 6865  c example of the
-00000ae0: 2041 5049 2075 7361 6765 3a0a 0a60 6060   API usage:..```
-00000af0: 7079 7468 6f6e 0a23 2074 7261 696e 2e70  python.# train.p
-00000b00: 790a 696d 706f 7274 2072 616e 646f 6d0a  y.import random.
-00000b10: 696d 706f 7274 2073 7973 0a66 726f 6d20  import sys.from 
-00000b20: 6476 636c 6976 6520 696d 706f 7274 204c  dvclive import L
-00000b30: 6976 650a 0a77 6974 6820 4c69 7665 2873  ive..with Live(s
-00000b40: 6176 655f 6476 635f 6578 703d 5472 7565  ave_dvc_exp=True
-00000b50: 2920 6173 206c 6976 653a 0a20 2020 2065  ) as live:.    e
-00000b60: 706f 6368 7320 3d20 696e 7428 7379 732e  pochs = int(sys.
-00000b70: 6172 6776 5b31 5d29 0a20 2020 206c 6976  argv[1]).    liv
-00000b80: 652e 6c6f 675f 7061 7261 6d28 2265 706f  e.log_param("epo
-00000b90: 6368 7322 2c20 6570 6f63 6873 290a 2020  chs", epochs).  
-00000ba0: 2020 666f 7220 6570 6f63 6820 696e 2072    for epoch in r
-00000bb0: 616e 6765 2865 706f 6368 7329 3a0a 2020  ange(epochs):.  
-00000bc0: 2020 2020 2020 6c69 7665 2e6c 6f67 5f6d        live.log_m
-00000bd0: 6574 7269 6328 2274 7261 696e 2f61 6363  etric("train/acc
-00000be0: 7572 6163 7922 2c20 6570 6f63 6820 2b20  uracy", epoch + 
-00000bf0: 7261 6e64 6f6d 2e72 616e 646f 6d28 2929  random.random())
-00000c00: 0a20 2020 2020 2020 206c 6976 652e 6c6f  .        live.lo
-00000c10: 675f 6d65 7472 6963 2822 7472 6169 6e2f  g_metric("train/
-00000c20: 6c6f 7373 222c 2065 706f 6368 7320 2d20  loss", epochs - 
-00000c30: 6570 6f63 6820 2d20 7261 6e64 6f6d 2e72  epoch - random.r
-00000c40: 616e 646f 6d28 2929 0a20 2020 2020 2020  andom()).       
-00000c50: 206c 6976 652e 6c6f 675f 6d65 7472 6963   live.log_metric
-00000c60: 2822 7661 6c2f 6163 6375 7261 6379 222c  ("val/accuracy",
-00000c70: 6570 6f63 6820 2b20 7261 6e64 6f6d 2e72  epoch + random.r
-00000c80: 616e 646f 6d28 2920 290a 2020 2020 2020  andom() ).      
-00000c90: 2020 6c69 7665 2e6c 6f67 5f6d 6574 7269    live.log_metri
-00000ca0: 6328 2276 616c 2f6c 6f73 7322 2c20 6570  c("val/loss", ep
-00000cb0: 6f63 6873 202d 2065 706f 6368 202d 2072  ochs - epoch - r
-00000cc0: 616e 646f 6d2e 7261 6e64 6f6d 2829 290a  andom.random()).
-00000cd0: 2020 2020 2020 2020 6c69 7665 2e6e 6578          live.nex
-00000ce0: 745f 7374 6570 2829 0a60 6060 0a0a 5365  t_step().```..Se
-00000cf0: 6520 5b49 6e74 6567 7261 7469 6f6e 735d  e [Integrations]
-00000d00: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
-00000d10: 2f64 6f63 2f64 7663 6c69 7665 2f6d 6c2d  /doc/dvclive/ml-
-00000d20: 6672 616d 6577 6f72 6b73 2920 666f 7220  frameworks) for 
-00000d30: 6578 616d 706c 6573 2075 7369 6e67 0a44  examples using.D
-00000d40: 5643 4c69 7665 2061 6c6f 6e67 7369 6465  VCLive alongside
-00000d50: 2064 6966 6665 7265 6e74 204d 4c20 4672   different ML Fr
-00000d60: 616d 6577 6f72 6b73 2e0a 0a23 2320 5275  ameworks...## Ru
-00000d70: 6e6e 696e 670a 0a52 756e 2063 6f75 706c  nning..Run coupl
-00000d80: 6520 6f66 2074 696d 6573 2070 6173 7369  e of times passi
-00000d90: 6e67 2064 6966 6665 7265 6e74 2076 616c  ng different val
-00000da0: 7565 733a 0a0a 6060 6063 6f6e 736f 6c65  ues:..```console
-00000db0: 0a24 2070 7974 686f 6e20 7472 6169 6e2e  .$ python train.
-00000dc0: 7079 2035 0a24 2070 7974 686f 6e20 7472  py 5.$ python tr
-00000dd0: 6169 6e2e 7079 2035 0a24 2070 7974 686f  ain.py 5.$ pytho
-00000de0: 6e20 7472 6169 6e2e 7079 2037 0a60 6060  n train.py 7.```
-00000df0: 0a0a 2323 2043 6f6d 7061 7269 6e67 0a0a  ..## Comparing..
-00000e00: 4456 434c 6976 6520 6f75 7470 7574 7320  DVCLive outputs 
-00000e10: 6361 6e20 6265 2072 656e 6465 7265 6420  can be rendered 
-00000e20: 696e 2064 6966 6665 7265 6e74 2077 6179  in different way
-00000e30: 733a 0a0a 2323 2320 4456 4320 434c 490a  s:..### DVC CLI.
-00000e40: 0a59 6f75 2063 616e 2075 7365 205b 6476  .You can use [dv
-00000e50: 6320 6578 7020 7368 6f77 5d28 6874 7470  c exp show](http
-00000e60: 733a 2f2f 6476 632e 6f72 672f 646f 632f  s://dvc.org/doc/
-00000e70: 636f 6d6d 616e 642d 7265 6665 7265 6e63  command-referenc
-00000e80: 652f 6578 702f 7368 6f77 2920 616e 640a  e/exp/show) and.
-00000e90: 5b64 7663 2070 6c6f 7473 5d28 6874 7470  [dvc plots](http
-00000ea0: 733a 2f2f 6476 632e 6f72 672f 646f 632f  s://dvc.org/doc/
-00000eb0: 636f 6d6d 616e 642d 7265 6665 7265 6e63  command-referenc
-00000ec0: 652f 706c 6f74 7329 2074 6f20 636f 6d70  e/plots) to comp
-00000ed0: 6172 6520 616e 640a 7669 7375 616c 697a  are and.visualiz
-00000ee0: 6520 6d65 7472 6963 732c 2070 6172 616d  e metrics, param
-00000ef0: 6574 6572 7320 616e 6420 706c 6f74 7320  eters and plots 
-00000f00: 6163 726f 7373 2065 7870 6572 696d 656e  across experimen
-00000f10: 7473 3a0a 0a60 6060 636f 6e73 6f6c 650a  ts:..```console.
-00000f20: 2420 6476 6320 6578 7020 7368 6f77 0a60  $ dvc exp show.`
-00000f30: 6060 0a0a 6060 600a e294 80e2 9480 e294  ``..```.........
-00000f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000f50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000f60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000f70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000f80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000f90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000fa0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000fb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000fc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000fd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000fe0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000ff0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001000: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000a00: 7274 0a0a 3c70 2061 6c69 676e 3d27 6365  rt..<p align='ce
+00000a10: 6e74 6572 273e 0a3c 6120 6872 6566 3d22  nter'>.<a href="
+00000a20: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00000a30: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00000a40: 6d2f 6769 7468 7562 2f69 7465 7261 7469  m/github/iterati
+00000a50: 7665 2f64 7663 6c69 7665 2f62 6c6f 622f  ve/dvclive/blob/
+00000a60: 6d61 696e 2f65 7861 6d70 6c65 732f 4456  main/examples/DV
+00000a70: 434c 6976 652d 5175 6963 6b73 7461 7274  CLive-Quickstart
+00000a80: 2e69 7079 6e62 223e 3c69 6d67 2073 7263  .ipynb"><img src
+00000a90: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
+00000aa0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00000ab0: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+00000ac0: 2d62 6164 6765 2e73 7667 2220 2f3e 3c2f  -badge.svg" /></
+00000ad0: 613e 0a3c 2f70 3e0a 0a23 2320 496e 7374  a>.</p>..## Inst
+00000ae0: 616c 6c20 2a64 7663 6c69 7665 2a0a 0a60  all *dvclive*..`
+00000af0: 6060 636f 6e73 6f6c 650a 2420 7069 7020  ``console.$ pip 
+00000b00: 696e 7374 616c 6c20 6476 636c 6976 650a  install dvclive.
+00000b10: 6060 600a 0a23 2320 496e 6974 6961 6c69  ```..## Initiali
+00000b20: 7a65 2044 5643 2052 6570 6f73 6974 6f72  ze DVC Repositor
+00000b30: 790a 0a60 6060 636f 6e73 6f6c 650a 2420  y..```console.$ 
+00000b40: 6769 7420 696e 6974 0a24 2064 7663 2069  git init.$ dvc i
+00000b50: 6e69 740a 2420 6769 7420 636f 6d6d 6974  nit.$ git commit
+00000b60: 202d 6d20 2244 5643 2069 6e69 7422 0a60   -m "DVC init".`
+00000b70: 6060 0a0a 2323 2045 7861 6d70 6c65 2063  ``..## Example c
+00000b80: 6f64 650a 0a43 6f70 7920 7468 6520 736e  ode..Copy the sn
+00000b90: 6970 7065 7420 6265 6c6f 7720 6173 2061  ippet below as a
+00000ba0: 2062 6173 6963 2065 7861 6d70 6c65 206f   basic example o
+00000bb0: 6620 7468 6520 4150 4920 7573 6167 653a  f the API usage:
+00000bc0: 0a0a 6060 6070 7974 686f 6e0a 2320 7472  ..```python.# tr
+00000bd0: 6169 6e2e 7079 0a69 6d70 6f72 7420 7261  ain.py.import ra
+00000be0: 6e64 6f6d 0a69 6d70 6f72 7420 7379 730a  ndom.import sys.
+00000bf0: 6672 6f6d 2064 7663 6c69 7665 2069 6d70  from dvclive imp
+00000c00: 6f72 7420 4c69 7665 0a0a 7769 7468 204c  ort Live..with L
+00000c10: 6976 6528 7361 7665 5f64 7663 5f65 7870  ive(save_dvc_exp
+00000c20: 3d54 7275 6529 2061 7320 6c69 7665 3a0a  =True) as live:.
+00000c30: 2020 2020 6570 6f63 6873 203d 2069 6e74      epochs = int
+00000c40: 2873 7973 2e61 7267 765b 315d 290a 2020  (sys.argv[1]).  
+00000c50: 2020 6c69 7665 2e6c 6f67 5f70 6172 616d    live.log_param
+00000c60: 2822 6570 6f63 6873 222c 2065 706f 6368  ("epochs", epoch
+00000c70: 7329 0a20 2020 2066 6f72 2065 706f 6368  s).    for epoch
+00000c80: 2069 6e20 7261 6e67 6528 6570 6f63 6873   in range(epochs
+00000c90: 293a 0a20 2020 2020 2020 206c 6976 652e  ):.        live.
+00000ca0: 6c6f 675f 6d65 7472 6963 2822 7472 6169  log_metric("trai
+00000cb0: 6e2f 6163 6375 7261 6379 222c 2065 706f  n/accuracy", epo
+00000cc0: 6368 202b 2072 616e 646f 6d2e 7261 6e64  ch + random.rand
+00000cd0: 6f6d 2829 290a 2020 2020 2020 2020 6c69  om()).        li
+00000ce0: 7665 2e6c 6f67 5f6d 6574 7269 6328 2274  ve.log_metric("t
+00000cf0: 7261 696e 2f6c 6f73 7322 2c20 6570 6f63  rain/loss", epoc
+00000d00: 6873 202d 2065 706f 6368 202d 2072 616e  hs - epoch - ran
+00000d10: 646f 6d2e 7261 6e64 6f6d 2829 290a 2020  dom.random()).  
+00000d20: 2020 2020 2020 6c69 7665 2e6c 6f67 5f6d        live.log_m
+00000d30: 6574 7269 6328 2276 616c 2f61 6363 7572  etric("val/accur
+00000d40: 6163 7922 2c65 706f 6368 202b 2072 616e  acy",epoch + ran
+00000d50: 646f 6d2e 7261 6e64 6f6d 2829 2029 0a20  dom.random() ). 
+00000d60: 2020 2020 2020 206c 6976 652e 6c6f 675f         live.log_
+00000d70: 6d65 7472 6963 2822 7661 6c2f 6c6f 7373  metric("val/loss
+00000d80: 222c 2065 706f 6368 7320 2d20 6570 6f63  ", epochs - epoc
+00000d90: 6820 2d20 7261 6e64 6f6d 2e72 616e 646f  h - random.rando
+00000da0: 6d28 2929 0a20 2020 2020 2020 206c 6976  m()).        liv
+00000db0: 652e 6e65 7874 5f73 7465 7028 290a 6060  e.next_step().``
+00000dc0: 600a 0a53 6565 205b 496e 7465 6772 6174  `..See [Integrat
+00000dd0: 696f 6e73 5d28 6874 7470 733a 2f2f 6476  ions](https://dv
+00000de0: 632e 6f72 672f 646f 632f 6476 636c 6976  c.org/doc/dvcliv
+00000df0: 652f 6d6c 2d66 7261 6d65 776f 726b 7329  e/ml-frameworks)
+00000e00: 2066 6f72 2065 7861 6d70 6c65 7320 7573   for examples us
+00000e10: 696e 670a 4456 434c 6976 6520 616c 6f6e  ing.DVCLive alon
+00000e20: 6773 6964 6520 6469 6666 6572 656e 7420  gside different 
+00000e30: 4d4c 2046 7261 6d65 776f 726b 732e 0a0a  ML Frameworks...
+00000e40: 2323 2052 756e 6e69 6e67 0a0a 5275 6e20  ## Running..Run 
+00000e50: 636f 7570 6c65 206f 6620 7469 6d65 7320  couple of times 
+00000e60: 7061 7373 696e 6720 6469 6666 6572 656e  passing differen
+00000e70: 7420 7661 6c75 6573 3a0a 0a60 6060 636f  t values:..```co
+00000e80: 6e73 6f6c 650a 2420 7079 7468 6f6e 2074  nsole.$ python t
+00000e90: 7261 696e 2e70 7920 350a 2420 7079 7468  rain.py 5.$ pyth
+00000ea0: 6f6e 2074 7261 696e 2e70 7920 350a 2420  on train.py 5.$ 
+00000eb0: 7079 7468 6f6e 2074 7261 696e 2e70 7920  python train.py 
+00000ec0: 370a 6060 600a 0a23 2320 436f 6d70 6172  7.```..## Compar
+00000ed0: 696e 670a 0a44 5643 4c69 7665 206f 7574  ing..DVCLive out
+00000ee0: 7075 7473 2063 616e 2062 6520 7265 6e64  puts can be rend
+00000ef0: 6572 6564 2069 6e20 6469 6666 6572 656e  ered in differen
+00000f00: 7420 7761 7973 3a0a 0a23 2323 2044 5643  t ways:..### DVC
+00000f10: 2043 4c49 0a0a 596f 7520 6361 6e20 7573   CLI..You can us
+00000f20: 6520 5b64 7663 2065 7870 2073 686f 775d  e [dvc exp show]
+00000f30: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
+00000f40: 2f64 6f63 2f63 6f6d 6d61 6e64 2d72 6566  /doc/command-ref
+00000f50: 6572 656e 6365 2f65 7870 2f73 686f 7729  erence/exp/show)
+00000f60: 2061 6e64 0a5b 6476 6320 706c 6f74 735d   and.[dvc plots]
+00000f70: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
+00000f80: 2f64 6f63 2f63 6f6d 6d61 6e64 2d72 6566  /doc/command-ref
+00000f90: 6572 656e 6365 2f70 6c6f 7473 2920 746f  erence/plots) to
+00000fa0: 2063 6f6d 7061 7265 2061 6e64 0a76 6973   compare and.vis
+00000fb0: 7561 6c69 7a65 206d 6574 7269 6373 2c20  ualize metrics, 
+00000fc0: 7061 7261 6d65 7465 7273 2061 6e64 2070  parameters and p
+00000fd0: 6c6f 7473 2061 6372 6f73 7320 6578 7065  lots across expe
+00000fe0: 7269 6d65 6e74 733a 0a0a 6060 6063 6f6e  riments:..```con
+00000ff0: 736f 6c65 0a24 2064 7663 2065 7870 2073  sole.$ dvc exp s
+00001000: 686f 770a 6060 600a 0a60 6060 0ae2 9480  how.```..```....
 00001010: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001020: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001030: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001060: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001070: e294 80e2 9480 e294 80e2 9480 e294 800a  ................
-00001080: 4578 7065 7269 6d65 6e74 2020 2020 2020  Experiment      
-00001090: 2020 2020 2020 2020 2020 2043 7265 6174             Creat
-000010a0: 6564 2020 2020 7472 6169 6e2e 6163 6375  ed    train.accu
-000010b0: 7261 6379 2020 2074 7261 696e 2e6c 6f73  racy   train.los
-000010c0: 7320 2020 7661 6c2e 6163 6375 7261 6379  s   val.accuracy
-000010d0: 2020 2076 616c 2e6c 6f73 7320 2020 7374     val.loss   st
-000010e0: 6570 2020 2065 706f 6368 730a e294 80e2  ep   epochs.....
-000010f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001100: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001110: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001120: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001130: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001170: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000011a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000011b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000011c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001080: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000010a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000010b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000010c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000010d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000010e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000010f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001100: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001150: 80e2 9480 0a45 7870 6572 696d 656e 7420  .....Experiment 
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 4372 6561 7465 6420 2020 2074 7261 696e  Created    train
+00001180: 2e61 6363 7572 6163 7920 2020 7472 6169  .accuracy   trai
+00001190: 6e2e 6c6f 7373 2020 2076 616c 2e61 6363  n.loss   val.acc
+000011a0: 7572 6163 7920 2020 7661 6c2e 6c6f 7373  uracy   val.loss
+000011b0: 2020 2073 7465 7020 2020 6570 6f63 6873     step   epochs
+000011c0: 0ae2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000011d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000011e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000011f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001210: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001220: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001230: e294 800a 776f 726b 7370 6163 6520 2020  ....workspace   
-00001240: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 362e 3031 3039 2020 2020 2020 302e    6.0109      0.
-00001270: 3233 3331 3120 2020 2020 2020 2020 2036  23311          6
-00001280: 2e30 3632 2020 2020 302e 3234 3332 3120  .062    0.24321 
-00001290: 2020 2020 2036 2020 2037 0a6d 6173 7465       6   7.maste
-000012a0: 7220 2020 2020 2020 2020 2020 2020 2020  r               
-000012b0: 2020 2020 2020 3038 3a35 3020 504d 2020        08:50 PM  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-000012d0: 2020 2020 2020 2020 2020 202d 2020 2020             -    
-000012e0: 2020 2020 2020 2020 2020 2d20 2020 2020            -     
-000012f0: 2020 2020 202d 2020 2020 2020 2d20 2020       -      -   
-00001300: 2d0a e294 9ce2 9480 e294 8020 3434 3735  -.......... 4475
-00001310: 3834 3520 5b61 756c 6963 2d63 6869 765d  845 [aulic-chiv]
-00001320: 2020 2030 383a 3536 2050 4d20 2020 2020     08:56 PM     
-00001330: 2020 2020 2020 362e 3031 3039 2020 2020        6.0109    
-00001340: 2020 302e 3233 3331 3120 2020 2020 2020    0.23311       
-00001350: 2020 2036 2e30 3632 2020 2020 302e 3234     6.062    0.24
-00001360: 3332 3120 2020 2020 2036 2020 2037 0ae2  321      6   7..
-00001370: 949c e294 80e2 9480 2037 6434 6365 6637  ........ 7d4cef7
-00001380: 205b 7961 7265 722d 746f 6473 5d20 2020   [yarer-tods]   
-00001390: 3038 3a35 3620 504d 2020 2020 2020 2020  08:56 PM        
-000013a0: 2020 2034 2e38 3535 3120 2020 2020 2030     4.8551      0
-000013b0: 2e38 3230 3132 2020 2020 2020 2020 2034  .82012         4
-000013c0: 2e35 3535 3520 2020 302e 3033 3335 3333  .5555   0.033533
-000013d0: 2020 2020 2020 3420 2020 350a e294 94e2        4   5.....
-000013e0: 9480 e294 8020 6435 3033 6638 6520 5b63  ..... d503f8e [c
-000013f0: 7572 7374 2d63 6861 645d 2020 2030 383a  urst-chad]   08:
-00001400: 3536 2050 4d20 2020 2020 2020 2020 2020  56 PM           
-00001410: 342e 3937 3638 2020 2020 2030 2e30 3730  4.9768     0.070
-00001420: 3538 3520 2020 2020 2020 2020 342e 3037  585         4.07
-00001430: 3733 2020 2020 302e 3436 3633 3920 2020  73    0.46639   
-00001440: 2020 2034 2020 2035 0ae2 9480 e294 80e2     4   5........
-00001450: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001460: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001470: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001480: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000014a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000014b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000014c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000014d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000014e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000014f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001500: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001510: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001230: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001240: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001250: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001260: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001280: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000012a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000012b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000012c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000012d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000012e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000012f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001300: 9480 e294 80e2 9480 0a77 6f72 6b73 7061  .........workspa
+00001310: 6365 2020 2020 2020 2020 2020 2020 2020  ce              
+00001320: 2020 2020 2d20 2020 2020 2020 2020 2020      -           
+00001330: 2020 2020 2020 2036 2e30 3130 3920 2020         6.0109   
+00001340: 2020 2030 2e32 3333 3131 2020 2020 2020     0.23311      
+00001350: 2020 2020 362e 3036 3220 2020 2030 2e32      6.062    0.2
+00001360: 3433 3231 2020 2020 2020 3620 2020 370a  4321      6   7.
+00001370: 6d61 7374 6572 2020 2020 2020 2020 2020  master          
+00001380: 2020 2020 2020 2020 2020 2030 383a 3530             08:50
+00001390: 2050 4d20 2020 2020 2020 2020 2020 2020   PM             
+000013a0: 2020 202d 2020 2020 2020 2020 2020 2020     -            
+000013b0: 2d20 2020 2020 2020 2020 2020 2020 202d  -              -
+000013c0: 2020 2020 2020 2020 2020 2d20 2020 2020            -     
+000013d0: 202d 2020 202d 0ae2 949c e294 80e2 9480   -   -..........
+000013e0: 2034 3437 3538 3435 205b 6175 6c69 632d   4475845 [aulic-
+000013f0: 6368 6976 5d20 2020 3038 3a35 3620 504d  chiv]   08:56 PM
+00001400: 2020 2020 2020 2020 2020 2036 2e30 3130             6.010
+00001410: 3920 2020 2020 2030 2e32 3333 3131 2020  9      0.23311  
+00001420: 2020 2020 2020 2020 362e 3036 3220 2020          6.062   
+00001430: 2030 2e32 3433 3231 2020 2020 2020 3620   0.24321      6 
+00001440: 2020 370a e294 9ce2 9480 e294 8020 3764    7.......... 7d
+00001450: 3463 6566 3720 5b79 6172 6572 2d74 6f64  4cef7 [yarer-tod
+00001460: 735d 2020 2030 383a 3536 2050 4d20 2020  s]   08:56 PM   
+00001470: 2020 2020 2020 2020 342e 3835 3531 2020          4.8551  
+00001480: 2020 2020 302e 3832 3031 3220 2020 2020      0.82012     
+00001490: 2020 2020 342e 3535 3535 2020 2030 2e30      4.5555   0.0
+000014a0: 3333 3533 3320 2020 2020 2034 2020 2035  33533      4   5
+000014b0: 0ae2 9494 e294 80e2 9480 2064 3530 3366  .......... d503f
+000014c0: 3865 205b 6375 7273 742d 6368 6164 5d20  8e [curst-chad] 
+000014d0: 2020 3038 3a35 3620 504d 2020 2020 2020    08:56 PM      
+000014e0: 2020 2020 2034 2e39 3736 3820 2020 2020       4.9768     
+000014f0: 302e 3037 3035 3835 2020 2020 2020 2020  0.070585        
+00001500: 2034 2e30 3737 3320 2020 2030 2e34 3636   4.0773    0.466
+00001510: 3339 2020 2020 2020 3420 2020 350a e294  39      4   5...
 00001520: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001530: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001540: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001580: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001590: 0a60 6060 0a0a 6060 6063 6f6e 736f 6c65  .```..```console
-000015a0: 0a24 2064 7663 2070 6c6f 7473 2064 6966  .$ dvc plots dif
-000015b0: 6620 2428 6476 6320 6578 7020 6c69 7374  f $(dvc exp list
-000015c0: 202d 2d6e 616d 6573 2d6f 6e6c 7929 202d   --names-only) -
-000015d0: 2d6f 7065 6e0a 6060 600a 0a21 5b64 7663  -open.```..![dvc
-000015e0: 2070 6c6f 7473 2064 6966 665d 282e 2f64   plots diff](./d
-000015f0: 6f63 732f 6476 635f 706c 6f74 735f 6469  ocs/dvc_plots_di
-00001600: 6666 2e70 6e67 290a 0a23 2323 2044 5643  ff.png)..### DVC
-00001610: 2045 7874 656e 7369 6f6e 2066 6f72 2056   Extension for V
-00001620: 5320 436f 6465 0a0a 496e 7369 6465 2074  S Code..Inside t
-00001630: 6865 0a5b 4456 4320 4578 7465 6e73 696f  he.[DVC Extensio
-00001640: 6e20 666f 7220 5653 2043 6f64 655d 2868  n for VS Code](h
-00001650: 7474 7073 3a2f 2f6d 6172 6b65 7470 6c61  ttps://marketpla
-00001660: 6365 2e76 6973 7561 6c73 7475 6469 6f2e  ce.visualstudio.
-00001670: 636f 6d2f 6974 656d 733f 6974 656d 4e61  com/items?itemNa
-00001680: 6d65 3d49 7465 7261 7469 7665 2e64 7663  me=Iterative.dvc
-00001690: 292c 0a79 6f75 2063 616e 2063 6f6d 7061  ),.you can compa
-000016a0: 7265 2061 6e64 2076 6973 7561 6c69 7a65  re and visualize
-000016b0: 2072 6573 756c 7473 2075 7369 6e67 2074   results using t
-000016c0: 6865 0a5b 4578 7065 7269 6d65 6e74 735d  he.[Experiments]
-000016d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000016e0: 636f 6d2f 6974 6572 6174 6976 652f 7673  com/iterative/vs
-000016f0: 636f 6465 2d64 7663 2f62 6c6f 622f 6d61  code-dvc/blob/ma
-00001700: 696e 2f65 7874 656e 7369 6f6e 2f72 6573  in/extension/res
-00001710: 6f75 7263 6573 2f77 616c 6b74 6872 6f75  ources/walkthrou
-00001720: 6768 2f65 7870 6572 696d 656e 7473 2d74  gh/experiments-t
-00001730: 6162 6c65 2e6d 6429 0a61 6e64 0a5b 506c  able.md).and.[Pl
-00001740: 6f74 735d 2868 7474 7073 3a2f 2f67 6974  ots](https://git
-00001750: 6875 622e 636f 6d2f 6974 6572 6174 6976  hub.com/iterativ
-00001760: 652f 7673 636f 6465 2d64 7663 2f62 6c6f  e/vscode-dvc/blo
-00001770: 622f 6d61 696e 2f65 7874 656e 7369 6f6e  b/main/extension
-00001780: 2f72 6573 6f75 7263 6573 2f77 616c 6b74  /resources/walkt
-00001790: 6872 6f75 6768 2f70 6c6f 7473 2e6d 6429  hrough/plots.md)
-000017a0: 0a76 6965 7773 3a0a 0a21 5b56 5343 6f64  .views:..![VSCod
-000017b0: 6520 4578 7065 7269 6d65 6e74 735d 282e  e Experiments](.
-000017c0: 2f64 6f63 732f 7673 636f 6465 5f65 7870  /docs/vscode_exp
-000017d0: 6572 696d 656e 7473 2e70 6e67 290a 0a21  eriments.png)..!
-000017e0: 5b56 5343 6f64 6520 506c 6f74 735d 282e  [VSCode Plots](.
-000017f0: 2f64 6f63 732f 7673 636f 6465 5f70 6c6f  /docs/vscode_plo
-00001800: 7473 2e70 6e67 290a 0a57 6869 6c65 2065  ts.png)..While e
-00001810: 7870 6572 696d 656e 7473 2061 7265 2072  xperiments are r
-00001820: 756e 6e69 6e67 2c20 6c69 7665 2075 7064  unning, live upd
-00001830: 6174 6573 2077 696c 6c20 6265 2064 6973  ates will be dis
-00001840: 706c 6179 6564 2069 6e20 626f 7468 2076  played in both v
-00001850: 6965 7773 2e0a 0a23 2323 2044 5643 2053  iews...### DVC S
-00001860: 7475 6469 6f0a 0a49 6620 796f 7520 7075  tudio..If you pu
-00001870: 7368 2074 6865 2072 6573 756c 7473 2074  sh the results t
-00001880: 6f20 5b44 5643 2053 7475 6469 6f5d 2868  o [DVC Studio](h
-00001890: 7474 7073 3a2f 2f64 7663 2e6f 7267 2f64  ttps://dvc.org/d
-000018a0: 6f63 2f73 7475 6469 6f29 2c20 796f 7520  oc/studio), you 
-000018b0: 6361 6e0a 636f 6d70 6172 6520 6578 7065  can.compare expe
-000018c0: 7269 6d65 6e74 7320 6167 6169 6e73 7420  riments against 
-000018d0: 7468 6520 656e 7469 7265 2072 6570 6f20  the entire repo 
-000018e0: 6869 7374 6f72 793a 0a0a 215b 5374 7564  history:..![Stud
-000018f0: 696f 2043 6f6d 7061 7265 5d28 2e2f 646f  io Compare](./do
-00001900: 6373 2f73 7475 6469 6f5f 636f 6d70 6172  cs/studio_compar
-00001910: 652e 706e 6729 0a0a 596f 7520 6361 6e20  e.png)..You can 
-00001920: 656e 6162 6c65 0a5b 5374 7564 696f 204c  enable.[Studio L
-00001930: 6976 6520 4578 7065 7269 6d65 6e74 735d  ive Experiments]
-00001940: 2868 7474 7073 3a2f 2f64 7663 2e6f 7267  (https://dvc.org
-00001950: 2f64 6f63 2f73 7475 6469 6f2f 7573 6572  /doc/studio/user
-00001960: 2d67 7569 6465 2f70 726f 6a65 6374 732d  -guide/projects-
-00001970: 616e 642d 6578 7065 7269 6d65 6e74 732f  and-experiments/
-00001980: 6c69 7665 2d6d 6574 7269 6373 2d61 6e64  live-metrics-and
-00001990: 2d70 6c6f 7473 290a 746f 2073 6565 206c  -plots).to see l
-000019a0: 6976 6520 7570 6461 7465 7320 7768 696c  ive updates whil
-000019b0: 6520 6578 7065 7269 6d65 6e74 7320 6172  e experiments ar
-000019c0: 6520 7275 6e6e 696e 672e 0a0a 5f5f 5f5f  e running...____
-000019d0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000019e0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000019f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a00: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a10: 5f5f 0a0a 2320 436f 6d70 6172 6973 6f6e  __..# Comparison
-00001a20: 2074 6f20 7265 6c61 7465 6420 7465 6368   to related tech
-00001a30: 6e6f 6c6f 6769 6573 0a0a 2a2a 4456 434c  nologies..**DVCL
-00001a40: 6976 652a 2a20 6973 2061 6e20 2a4d 4c20  ive** is an *ML 
-00001a50: 4c6f 6767 6572 2a2c 2073 696d 696c 6172  Logger*, similar
-00001a60: 2074 6f3a 0a0a 2d20 5b4d 4c46 6c6f 775d   to:..- [MLFlow]
-00001a70: 2868 7474 7073 3a2f 2f6d 6c66 6c6f 772e  (https://mlflow.
-00001a80: 6f72 672f 290a 2d20 5b57 6569 6768 7473  org/).- [Weights
-00001a90: 2026 2042 6961 7365 735d 2868 7474 7073   & Biases](https
-00001aa0: 3a2f 2f77 616e 6462 2e61 692f 7369 7465  ://wandb.ai/site
-00001ab0: 290a 2d20 5b4e 6570 7475 6e65 5d28 6874  ).- [Neptune](ht
-00001ac0: 7470 733a 2f2f 6e65 7074 756e 652e 6169  tps://neptune.ai
-00001ad0: 2f29 0a0a 5468 6520 6d61 696e 2064 6966  /)..The main dif
-00001ae0: 6665 7265 6e63 6520 7769 7468 2074 686f  ference with tho
-00001af0: 7365 202a 4d4c 204c 6f67 6765 7273 2a20  se *ML Loggers* 
-00001b00: 6973 2074 6861 7420 2a2a 4456 434c 6976  is that **DVCLiv
-00001b10: 652a 2a20 646f 6573 206e 6f74 0a2a 2a72  e** does not.**r
-00001b20: 6571 7569 7265 2a2a 2061 6e79 2061 6464  equire** any add
-00001b30: 6974 696f 6e61 6c20 7365 7276 6963 6573  itional services
-00001b40: 206f 7220 7365 7276 6572 7320 746f 2072   or servers to r
-00001b50: 756e 2e0a 0a4c 6f67 6765 6420 6d65 7472  un...Logged metr
-00001b60: 6963 732c 2070 6172 616d 6574 6572 732c  ics, parameters,
-00001b70: 2061 6e64 2070 6c6f 7473 2061 7265 2073   and plots are s
-00001b80: 746f 7265 6420 6173 2070 6c61 696e 2074  tored as plain t
-00001b90: 6578 7420 6669 6c65 7320 7468 6174 2063  ext files that c
-00001ba0: 616e 2062 650a 7665 7273 696f 6e65 6420  an be.versioned 
-00001bb0: 6279 2074 6f6f 6c73 206c 696b 6520 4769  by tools like Gi
-00001bc0: 7420 6f72 2074 7261 636b 6564 2061 7320  t or tracked as 
-00001bd0: 706f 696e 7465 7273 2074 6f20 6669 6c65  pointers to file
-00001be0: 7320 696e 2044 5643 2073 746f 7261 6765  s in DVC storage
-00001bf0: 2e0a 0a59 6f75 2063 616e 2074 6865 6e20  ...You can then 
-00001c00: 7573 6520 6469 6666 6572 656e 7420 5b6f  use different [o
-00001c10: 7074 696f 6e73 5d28 2363 6f6d 7061 7269  ptions](#compari
-00001c20: 6e67 2920 746f 2076 6973 7561 6c69 7a65  ng) to visualize
-00001c30: 2074 6865 206d 6574 7269 6373 2c0a 7061   the metrics,.pa
-00001c40: 7261 6d65 7465 7273 2c20 616e 6420 706c  rameters, and pl
-00001c50: 6f74 7320 6163 726f 7373 2065 7870 6572  ots across exper
-00001c60: 696d 656e 7473 2e0a 0a5f 5f5f 5f5f 5f5f  iments..._______
-00001c70: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001c80: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001c90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001ca0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f0a  _______________.
-00001cb0: 0a23 2043 6f6e 7472 6962 7574 696e 670a  .# Contributing.
-00001cc0: 0a43 6f6e 7472 6962 7574 696f 6e73 2061  .Contributions a
-00001cd0: 7265 2076 6572 7920 7765 6c63 6f6d 652e  re very welcome.
-00001ce0: 2054 6f20 6c65 6172 6e20 6d6f 7265 2c20   To learn more, 
-00001cf0: 7365 6520 7468 650a 5b43 6f6e 7472 6962  see the.[Contrib
-00001d00: 7574 6f72 2047 7569 6465 5d28 434f 4e54  utor Guide](CONT
-00001d10: 5249 4255 5449 4e47 2e72 7374 292e 0a0a  RIBUTING.rst)...
-00001d20: 2320 4c69 6365 6e73 650a 0a44 6973 7472  # License..Distr
-00001d30: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
-00001d40: 2074 6572 6d73 206f 6620 7468 650a 5b41   terms of the.[A
-00001d50: 7061 6368 6520 322e 3020 6c69 6365 6e73  pache 2.0 licens
-00001d60: 655d 2868 7474 7073 3a2f 2f6f 7065 6e73  e](https://opens
-00001d70: 6f75 7263 652e 6f72 672f 6c69 6365 6e73  ource.org/licens
-00001d80: 6573 2f41 7061 6368 652d 322e 3029 2c20  es/Apache-2.0), 
-00001d90: 2a64 7663 6c69 7665 2a20 6973 0a66 7265  *dvclive* is.fre
-00001da0: 6520 616e 6420 6f70 656e 2073 6f75 7263  e and open sourc
-00001db0: 6520 736f 6674 7761 7265 2e0a            e software..
+00001590: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000015a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000015b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000015c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000015d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000015e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000015f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001600: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001610: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001620: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001630: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001640: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001650: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001660: 9480 e294 800a 6060 600a 0a60 6060 636f  ......```..```co
+00001670: 6e73 6f6c 650a 2420 6476 6320 706c 6f74  nsole.$ dvc plot
+00001680: 7320 6469 6666 2024 2864 7663 2065 7870  s diff $(dvc exp
+00001690: 206c 6973 7420 2d2d 6e61 6d65 732d 6f6e   list --names-on
+000016a0: 6c79 2920 2d2d 6f70 656e 0a60 6060 0a0a  ly) --open.```..
+000016b0: 215b 6476 6320 706c 6f74 7320 6469 6666  ![dvc plots diff
+000016c0: 5d28 2e2f 646f 6373 2f64 7663 5f70 6c6f  ](./docs/dvc_plo
+000016d0: 7473 5f64 6966 662e 706e 6729 0a0a 2323  ts_diff.png)..##
+000016e0: 2320 4456 4320 4578 7465 6e73 696f 6e20  # DVC Extension 
+000016f0: 666f 7220 5653 2043 6f64 650a 0a49 6e73  for VS Code..Ins
+00001700: 6964 6520 7468 650a 5b44 5643 2045 7874  ide the.[DVC Ext
+00001710: 656e 7369 6f6e 2066 6f72 2056 5320 436f  ension for VS Co
+00001720: 6465 5d28 6874 7470 733a 2f2f 6d61 726b  de](https://mark
+00001730: 6574 706c 6163 652e 7669 7375 616c 7374  etplace.visualst
+00001740: 7564 696f 2e63 6f6d 2f69 7465 6d73 3f69  udio.com/items?i
+00001750: 7465 6d4e 616d 653d 4974 6572 6174 6976  temName=Iterativ
+00001760: 652e 6476 6329 2c0a 796f 7520 6361 6e20  e.dvc),.you can 
+00001770: 636f 6d70 6172 6520 616e 6420 7669 7375  compare and visu
+00001780: 616c 697a 6520 7265 7375 6c74 7320 7573  alize results us
+00001790: 696e 6720 7468 650a 5b45 7870 6572 696d  ing the.[Experim
+000017a0: 656e 7473 5d28 6874 7470 733a 2f2f 6769  ents](https://gi
+000017b0: 7468 7562 2e63 6f6d 2f69 7465 7261 7469  thub.com/iterati
+000017c0: 7665 2f76 7363 6f64 652d 6476 632f 626c  ve/vscode-dvc/bl
+000017d0: 6f62 2f6d 6169 6e2f 6578 7465 6e73 696f  ob/main/extensio
+000017e0: 6e2f 7265 736f 7572 6365 732f 7761 6c6b  n/resources/walk
+000017f0: 7468 726f 7567 682f 6578 7065 7269 6d65  through/experime
+00001800: 6e74 732d 7461 626c 652e 6d64 290a 616e  nts-table.md).an
+00001810: 640a 5b50 6c6f 7473 5d28 6874 7470 733a  d.[Plots](https:
+00001820: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7465  //github.com/ite
+00001830: 7261 7469 7665 2f76 7363 6f64 652d 6476  rative/vscode-dv
+00001840: 632f 626c 6f62 2f6d 6169 6e2f 6578 7465  c/blob/main/exte
+00001850: 6e73 696f 6e2f 7265 736f 7572 6365 732f  nsion/resources/
+00001860: 7761 6c6b 7468 726f 7567 682f 706c 6f74  walkthrough/plot
+00001870: 732e 6d64 290a 7669 6577 733a 0a0a 215b  s.md).views:..![
+00001880: 5653 436f 6465 2045 7870 6572 696d 656e  VSCode Experimen
+00001890: 7473 5d28 2e2f 646f 6373 2f76 7363 6f64  ts](./docs/vscod
+000018a0: 655f 6578 7065 7269 6d65 6e74 732e 706e  e_experiments.pn
+000018b0: 6729 0a0a 215b 5653 436f 6465 2050 6c6f  g)..![VSCode Plo
+000018c0: 7473 5d28 2e2f 646f 6373 2f76 7363 6f64  ts](./docs/vscod
+000018d0: 655f 706c 6f74 732e 706e 6729 0a0a 5768  e_plots.png)..Wh
+000018e0: 696c 6520 6578 7065 7269 6d65 6e74 7320  ile experiments 
+000018f0: 6172 6520 7275 6e6e 696e 672c 206c 6976  are running, liv
+00001900: 6520 7570 6461 7465 7320 7769 6c6c 2062  e updates will b
+00001910: 6520 6469 7370 6c61 7965 6420 696e 2062  e displayed in b
+00001920: 6f74 6820 7669 6577 732e 0a0a 2323 2320  oth views...### 
+00001930: 4456 4320 5374 7564 696f 0a0a 4966 2079  DVC Studio..If y
+00001940: 6f75 2070 7573 6820 7468 6520 7265 7375  ou push the resu
+00001950: 6c74 7320 746f 205b 4456 4320 5374 7564  lts to [DVC Stud
+00001960: 696f 5d28 6874 7470 733a 2f2f 6476 632e  io](https://dvc.
+00001970: 6f72 672f 646f 632f 7374 7564 696f 292c  org/doc/studio),
+00001980: 2079 6f75 2063 616e 0a63 6f6d 7061 7265   you can.compare
+00001990: 2065 7870 6572 696d 656e 7473 2061 6761   experiments aga
+000019a0: 696e 7374 2074 6865 2065 6e74 6972 6520  inst the entire 
+000019b0: 7265 706f 2068 6973 746f 7279 3a0a 0a21  repo history:..!
+000019c0: 5b53 7475 6469 6f20 436f 6d70 6172 655d  [Studio Compare]
+000019d0: 282e 2f64 6f63 732f 7374 7564 696f 5f63  (./docs/studio_c
+000019e0: 6f6d 7061 7265 2e70 6e67 290a 0a59 6f75  ompare.png)..You
+000019f0: 2063 616e 2065 6e61 626c 650a 5b53 7475   can enable.[Stu
+00001a00: 6469 6f20 4c69 7665 2045 7870 6572 696d  dio Live Experim
+00001a10: 656e 7473 5d28 6874 7470 733a 2f2f 6476  ents](https://dv
+00001a20: 632e 6f72 672f 646f 632f 7374 7564 696f  c.org/doc/studio
+00001a30: 2f75 7365 722d 6775 6964 652f 7072 6f6a  /user-guide/proj
+00001a40: 6563 7473 2d61 6e64 2d65 7870 6572 696d  ects-and-experim
+00001a50: 656e 7473 2f6c 6976 652d 6d65 7472 6963  ents/live-metric
+00001a60: 732d 616e 642d 706c 6f74 7329 0a74 6f20  s-and-plots).to 
+00001a70: 7365 6520 6c69 7665 2075 7064 6174 6573  see live updates
+00001a80: 2077 6869 6c65 2065 7870 6572 696d 656e   while experimen
+00001a90: 7473 2061 7265 2072 756e 6e69 6e67 2e0a  ts are running..
+00001aa0: 0a5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ._______________
+00001ab0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001ac0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001ad0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001ae0: 5f5f 5f5f 5f5f 5f0a 0a23 2043 6f6d 7061  _______..# Compa
+00001af0: 7269 736f 6e20 746f 2072 656c 6174 6564  rison to related
+00001b00: 2074 6563 686e 6f6c 6f67 6965 730a 0a2a   technologies..*
+00001b10: 2a44 5643 4c69 7665 2a2a 2069 7320 616e  *DVCLive** is an
+00001b20: 202a 4d4c 204c 6f67 6765 722a 2c20 7369   *ML Logger*, si
+00001b30: 6d69 6c61 7220 746f 3a0a 0a2d 205b 4d4c  milar to:..- [ML
+00001b40: 466c 6f77 5d28 6874 7470 733a 2f2f 6d6c  Flow](https://ml
+00001b50: 666c 6f77 2e6f 7267 2f29 0a2d 205b 5765  flow.org/).- [We
+00001b60: 6967 6874 7320 2620 4269 6173 6573 5d28  ights & Biases](
+00001b70: 6874 7470 733a 2f2f 7761 6e64 622e 6169  https://wandb.ai
+00001b80: 2f73 6974 6529 0a2d 205b 4e65 7074 756e  /site).- [Neptun
+00001b90: 655d 2868 7474 7073 3a2f 2f6e 6570 7475  e](https://neptu
+00001ba0: 6e65 2e61 692f 290a 0a54 6865 206d 6169  ne.ai/)..The mai
+00001bb0: 6e20 6469 6666 6572 656e 6365 2077 6974  n difference wit
+00001bc0: 6820 7468 6f73 6520 2a4d 4c20 4c6f 6767  h those *ML Logg
+00001bd0: 6572 732a 2069 7320 7468 6174 202a 2a44  ers* is that **D
+00001be0: 5643 4c69 7665 2a2a 2064 6f65 7320 6e6f  VCLive** does no
+00001bf0: 740a 2a2a 7265 7175 6972 652a 2a20 616e  t.**require** an
+00001c00: 7920 6164 6469 7469 6f6e 616c 2073 6572  y additional ser
+00001c10: 7669 6365 7320 6f72 2073 6572 7665 7273  vices or servers
+00001c20: 2074 6f20 7275 6e2e 0a0a 4c6f 6767 6564   to run...Logged
+00001c30: 206d 6574 7269 6373 2c20 7061 7261 6d65   metrics, parame
+00001c40: 7465 7273 2c20 616e 6420 706c 6f74 7320  ters, and plots 
+00001c50: 6172 6520 7374 6f72 6564 2061 7320 706c  are stored as pl
+00001c60: 6169 6e20 7465 7874 2066 696c 6573 2074  ain text files t
+00001c70: 6861 7420 6361 6e20 6265 0a76 6572 7369  hat can be.versi
+00001c80: 6f6e 6564 2062 7920 746f 6f6c 7320 6c69  oned by tools li
+00001c90: 6b65 2047 6974 206f 7220 7472 6163 6b65  ke Git or tracke
+00001ca0: 6420 6173 2070 6f69 6e74 6572 7320 746f  d as pointers to
+00001cb0: 2066 696c 6573 2069 6e20 4456 4320 7374   files in DVC st
+00001cc0: 6f72 6167 652e 0a0a 596f 7520 6361 6e20  orage...You can 
+00001cd0: 7468 656e 2075 7365 2064 6966 6665 7265  then use differe
+00001ce0: 6e74 205b 6f70 7469 6f6e 735d 2823 636f  nt [options](#co
+00001cf0: 6d70 6172 696e 6729 2074 6f20 7669 7375  mparing) to visu
+00001d00: 616c 697a 6520 7468 6520 6d65 7472 6963  alize the metric
+00001d10: 732c 0a70 6172 616d 6574 6572 732c 2061  s,.parameters, a
+00001d20: 6e64 2070 6c6f 7473 2061 6372 6f73 7320  nd plots across 
+00001d30: 6578 7065 7269 6d65 6e74 732e 0a0a 5f5f  experiments...__
+00001d40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d60: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d70: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001d80: 5f5f 5f5f 0a0a 2320 436f 6e74 7269 6275  ____..# Contribu
+00001d90: 7469 6e67 0a0a 436f 6e74 7269 6275 7469  ting..Contributi
+00001da0: 6f6e 7320 6172 6520 7665 7279 2077 656c  ons are very wel
+00001db0: 636f 6d65 2e20 546f 206c 6561 726e 206d  come. To learn m
+00001dc0: 6f72 652c 2073 6565 2074 6865 0a5b 436f  ore, see the.[Co
+00001dd0: 6e74 7269 6275 746f 7220 4775 6964 655d  ntributor Guide]
+00001de0: 2843 4f4e 5452 4942 5554 494e 472e 7273  (CONTRIBUTING.rs
+00001df0: 7429 2e0a 0a23 204c 6963 656e 7365 0a0a  t)...# License..
+00001e00: 4469 7374 7269 6275 7465 6420 756e 6465  Distributed unde
+00001e10: 7220 7468 6520 7465 726d 7320 6f66 2074  r the terms of t
+00001e20: 6865 0a5b 4170 6163 6865 2032 2e30 206c  he.[Apache 2.0 l
+00001e30: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+00001e40: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+00001e50: 6963 656e 7365 732f 4170 6163 6865 2d32  icenses/Apache-2
+00001e60: 2e30 292c 202a 6476 636c 6976 652a 2069  .0), *dvclive* i
+00001e70: 730a 6672 6565 2061 6e64 206f 7065 6e20  s.free and open 
+00001e80: 736f 7572 6365 2073 6f66 7477 6172 652e  source software.
+00001e90: 0a                                       .
```

### Comparing `dvclive-2.6.4/src/dvclive.egg-info/SOURCES.txt` & `dvclive-2.7.0/src/dvclive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 .github/workflows/release.yml
 .github/workflows/tests.yml
 .github/workflows/update-template.yaml
 docs/dvc_plots_diff.png
 docs/studio_compare.png
 docs/vscode_experiments.png
 docs/vscode_plots.png
+examples/DVCLive-Quickstart.ipynb
 src/dvclive/__init__.py
 src/dvclive/catalyst.py
 src/dvclive/dvc.py
 src/dvclive/env.py
 src/dvclive/error.py
 src/dvclive/fastai.py
 src/dvclive/huggingface.py
```

### Comparing `dvclive-2.6.4/src/dvclive.egg-info/requires.txt` & `dvclive-2.7.0/src/dvclive.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 dvc>2.45.1
+dvc-studio-client<1,>=0.7.0
 funcy
 ruamel.yaml
+scmrepo
 
 [all]
 numpy
 pillow
 mmcv
 tensorflow
 xgboost
 lightgbm
 transformers
 datasets
 catalyst>22
 fastai
 pytorch_lightning>=1.9
-torch<1.13
+torch<2.1
 optuna
 scikit-learn
 matplotlib
 
 [catalyst]
 catalyst>22
 
@@ -37,15 +39,15 @@
 xgboost
 lightgbm
 transformers
 datasets
 catalyst>22
 fastai
 pytorch_lightning>=1.9
-torch<1.13
+torch<2.1
 optuna
 mypy>=1.1.1
 
 [fastai]
 fastai
 
 [huggingface]
@@ -69,15 +71,15 @@
 optuna
 
 [plots]
 scikit-learn
 
 [pytorch_lightning]
 pytorch_lightning>=1.9
-torch<1.13
+torch<2.1
 
 [sklearn]
 scikit-learn
 
 [tests]
 pytest==7.2.0
 pytest-sugar==0.9.5
```

### Comparing `dvclive-2.6.4/tests/conftest.py` & `dvclive-2.7.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # ruff: noqa: ARG002
 import sys
 
 import pytest
-from dvc_studio_client.env import STUDIO_ENDPOINT, STUDIO_REPO_URL, STUDIO_TOKEN
+from dvc_studio_client.env import DVC_STUDIO_TOKEN, DVC_STUDIO_URL, STUDIO_REPO_URL
 
 
 @pytest.fixture()
 def tmp_dir(tmp_path, monkeypatch):
     monkeypatch.chdir(tmp_path)
     return tmp_path
 
 
 @pytest.fixture()
 def mocked_dvc_repo(tmp_dir, mocker):
     _dvc_repo = mocker.MagicMock()
     _dvc_repo.index.stages = []
     _dvc_repo.scm.get_rev.return_value = "f" * 40
     _dvc_repo.scm.get_ref.return_value = None
+    _dvc_repo.scm.no_commits = False
     _dvc_repo.experiments.save.return_value = "e" * 40
     _dvc_repo.root_dir = tmp_dir
     mocker.patch("dvclive.live.get_dvc_repo", return_value=_dvc_repo)
     return _dvc_repo
 
 
 @pytest.fixture()
@@ -52,11 +53,11 @@
 
 
 @pytest.fixture()
 def mocked_studio_post(mocker, monkeypatch):
     valid_response = mocker.MagicMock()
     valid_response.status_code = 200
     mocked_post = mocker.patch("requests.post", return_value=valid_response)
-    monkeypatch.setenv(STUDIO_ENDPOINT, "https://0.0.0.0")
+    monkeypatch.setenv(DVC_STUDIO_URL, "https://0.0.0.0")
     monkeypatch.setenv(STUDIO_REPO_URL, "STUDIO_REPO_URL")
-    monkeypatch.setenv(STUDIO_TOKEN, "STUDIO_TOKEN")
+    monkeypatch.setenv(DVC_STUDIO_TOKEN, "STUDIO_TOKEN")
     return mocked_post, valid_response
```

### Comparing `dvclive-2.6.4/tests/plots/test_image.py` & `dvclive-2.7.0/tests/plots/test_image.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/plots/test_metric.py` & `dvclive-2.7.0/tests/plots/test_metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/plots/test_sklearn.py` & `dvclive-2.7.0/tests/plots/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_dvc.py` & `dvclive-2.7.0/tests/test_dvc.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,35 @@
 import pytest
 from dvc.repo import Repo
 from PIL import Image
 from ruamel.yaml import YAML
 from scmrepo.git import Git
 
 from dvclive import Live
-from dvclive.dvc import get_dvc_repo, get_dvc_stage_template, make_dvcyaml
+from dvclive.dvc import get_dvc_repo, make_dvcyaml
 from dvclive.env import DVC_EXP_BASELINE_REV, DVC_EXP_NAME
 from dvclive.serialize import load_yaml
 
 YAML_LOADER = YAML(typ="safe")
 
 
 def test_get_dvc_repo(tmp_dir):
     assert get_dvc_repo() is None
     Git.init(tmp_dir)
-    Repo.init(tmp_dir)
     assert isinstance(get_dvc_repo(), Repo)
 
 
+def test_get_dvc_repo_subdir(tmp_dir):
+    Git.init(tmp_dir)
+    subdir = tmp_dir / "sub"
+    subdir.mkdir()
+    os.chdir(subdir)
+    assert get_dvc_repo().root_dir == str(tmp_dir)
+
+
 def test_make_dvcyaml_empty(tmp_dir):
     live = Live()
     make_dvcyaml(live)
 
     assert load_yaml(live.dvc_file) == {}
 
 
@@ -61,14 +68,21 @@
 
 def test_make_dvcyaml_all_plots(tmp_dir):
     live = Live()
     live.log_param("foo", 1)
     live.log_metric("bar", 2)
     live.log_image("img.png", Image.new("RGB", (10, 10), (250, 250, 250)))
     live.log_sklearn_plot("confusion_matrix", [0, 0, 1, 1], [0, 1, 1, 0])
+    live.log_sklearn_plot(
+        "confusion_matrix",
+        [0, 0, 1, 1],
+        [0, 1, 1, 0],
+        name="confusion_matrix_normalized",
+        normalized=True,
+    )
     live.log_sklearn_plot("roc", [0, 0, 1, 1], [0.0, 0.5, 0.5, 0.0], "custom_name_roc")
     make_dvcyaml(live)
 
     assert load_yaml(live.dvc_file) == {
         "metrics": ["metrics.json"],
         "params": ["params.yaml"],
         "plots": [
@@ -81,14 +95,24 @@
                     "y": "predicted",
                     "title": "Confusion Matrix",
                     "x_label": "True Label",
                     "y_label": "Predicted Label",
                 },
             },
             {
+                "plots/sklearn/confusion_matrix_normalized.json": {
+                    "template": "confusion_normalized",
+                    "title": "Confusion Matrix",
+                    "x": "actual",
+                    "x_label": "True Label",
+                    "y": "predicted",
+                    "y_label": "Predicted Label",
+                }
+            },
+            {
                 "plots/sklearn/custom_name_roc.json": {
                     "template": "simple",
                     "x": "fpr",
                     "y": "tpr",
                     "title": "Receiver operating characteristic (ROC)",
                     "x_label": "False Positive Rate",
                     "y_label": "True Positive Rate",
@@ -133,14 +157,15 @@
 def test_exp_save_run_on_dvc_repro(tmp_dir, mocker):
     dvc_repo = mocker.MagicMock()
     dvc_stage = mocker.MagicMock()
     dvc_file = mocker.MagicMock()
     dvc_repo.index.stages = [dvc_stage, dvc_file]
     dvc_repo.scm.get_rev.return_value = "current_rev"
     dvc_repo.scm.get_ref.return_value = None
+    dvc_repo.scm.no_commits = False
     with mocker.patch("dvclive.live.get_dvc_repo", return_value=dvc_repo):
         live = Live(save_dvc_exp=True)
         assert live._save_dvc_exp
         assert live._baseline_rev is not None
         assert live._exp_name is not None
         live.end()
 
@@ -172,14 +197,15 @@
 def test_exp_save_with_dvc_files(tmp_dir, mocker):
     dvc_repo = mocker.MagicMock()
     dvc_file = mocker.MagicMock()
     dvc_file.is_data_source = True
     dvc_repo.index.stages = [dvc_file]
     dvc_repo.scm.get_rev.return_value = "current_rev"
     dvc_repo.scm.get_ref.return_value = None
+    dvc_repo.scm.no_commits = False
 
     with mocker.patch("dvclive.live.get_dvc_repo", return_value=dvc_repo):
         live = Live(save_dvc_exp=True)
         live.end()
 
     dvc_repo.experiments.save.assert_called_with(
         name=live._exp_name, include_untracked=[live.dir], force=True
@@ -196,67 +222,14 @@
     dvc_repo.experiments.save.side_effect = DvcException("foo")
     mocker.patch("dvclive.live.get_dvc_repo", return_value=dvc_repo)
 
     with Live(save_dvc_exp=True):
         pass
 
 
-def test_get_dvc_stage_template_empty(tmp_dir, mocked_dvc_repo):
-    live = Live()
-    template = get_dvc_stage_template(live)
-
-    assert YAML_LOADER.load(template) == {
-        "stages": {
-            "dvclive": {
-                "cmd": "<python my_code_file.py my_args>",
-                "deps": ["<my_code_file.py>"],
-            }
-        }
-    }
-
-
-def test_get_dvc_stage_template_artifacts(tmp_dir, mocked_dvc_repo):
-    live = Live()
-    live.log_artifact("artifact.txt")
-    template = get_dvc_stage_template(live)
-
-    assert YAML_LOADER.load(template) == {
-        "stages": {
-            "dvclive": {
-                "cmd": "<python my_code_file.py my_args>",
-                "deps": ["<my_code_file.py>"],
-                "outs": ["artifact.txt"],
-            }
-        }
-    }
-
-
-def test_get_dvc_stage_template_chdir(tmp_dir, mocked_dvc_repo, monkeypatch):
-    d = tmp_dir / "sub" / "dir"
-    d.mkdir(parents=True)
-    monkeypatch.chdir(d)
-    live = Live("live")
-    live.log_param("foo", 1)
-    live.log_metric("bar", 1)
-    live.log_image("img.png", Image.new("RGB", (10, 10), (250, 250, 250)))
-    live.log_sklearn_plot("confusion_matrix", [0, 0, 1, 1], [0, 1, 1, 0])
-    live.log_artifact("artifact.txt")
-    template = get_dvc_stage_template(live)
-
-    assert YAML_LOADER.load(template) == {
-        "stages": {
-            "dvclive": {
-                "cmd": "<python my_code_file.py my_args>",
-                "deps": ["<my_code_file.py>"],
-                "outs": ["sub/dir/artifact.txt"],
-            }
-        }
-    }
-
-
 def test_untracked_dvclive_files_inside_dvc_exp_run_are_added(
     tmp_dir, mocked_dvc_repo, monkeypatch
 ):
     monkeypatch.setenv(DVC_EXP_BASELINE_REV, "foo")
     monkeypatch.setenv(DVC_EXP_NAME, "bar")
     plot_file = os.path.join("dvclive", "plots", "metrics", "foo.tsv")
     mocked_dvc_repo.scm.untracked_files.return_value = [
```

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_catalyst.py` & `dvclive-2.7.0/tests/test_frameworks/test_catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_fastai.py` & `dvclive-2.7.0/tests/test_frameworks/test_fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_huggingface.py` & `dvclive-2.7.0/tests/test_frameworks/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_keras.py` & `dvclive-2.7.0/tests/test_frameworks/test_keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_lgbm.py` & `dvclive-2.7.0/tests/test_frameworks/test_lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_lightning.py` & `dvclive-2.7.0/tests/test_frameworks/test_lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_optuna.py` & `dvclive-2.7.0/tests/test_frameworks/test_optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_frameworks/test_xgboost.py` & `dvclive-2.7.0/tests/test_frameworks/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.4/tests/test_main.py` & `dvclive-2.7.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import os
-from io import StringIO
 
 import pytest
 
 from dvclive import Live, env
 from dvclive.error import InvalidDataTypeError, InvalidParameterTypeError
 from dvclive.plots import Metric
-from dvclive.serialize import get_yaml, load_yaml
+from dvclive.serialize import load_yaml
 from dvclive.utils import parse_metrics, parse_tsv
 
 
 def read_history(live, metric):
     history, _ = parse_metrics(live)
     steps = []
     values = []
@@ -449,14 +448,15 @@
 
     assert not os.path.exists(signal_file)
 
     dvc_repo = mocker.MagicMock()
     dvc_repo.index.stages = []
     dvc_repo.scm.get_rev.return_value = "current_rev"
     dvc_repo.scm.get_ref.return_value = None
+    dvc_repo.scm.no_commits = False
     with mocker.patch("dvclive.live.get_dvc_repo", return_value=dvc_repo), mocker.patch(
         "dvclive.live.os.getpid", return_value=test_pid
     ):
         dvclive = Live(save_dvc_exp=True)
 
     if dvc_root:
         assert os.path.exists(signal_file)
@@ -479,30 +479,7 @@
     dvclive = Live("logs", dvcyaml=dvcyaml)
     dvclive.log_metric("m1", 1)
     dvclive.make_dvcyaml()
 
     dvcyaml_path = tmp_dir / dvclive.dir / "dvc.yaml"
 
     assert dvcyaml_path.is_file()
-
-
-def test_get_dvc_stage_template(tmp_dir, mocker, mocked_dvc_repo):
-    logger = mocker.patch("dvclive.live.logger")
-    dvclive = Live()
-    dvclive.end()
-
-    template = {
-        "stages": {
-            "dvclive": {
-                "cmd": "<python my_code_file.py my_args>",
-                "deps": ["<my_code_file.py>"],
-            }
-        }
-    }
-
-    output = StringIO()
-    get_yaml().dump(template, output)
-    yaml_str = output.getvalue()
-    output.close()
-    path_str = os.path.join(tmp_dir, "dvc.yaml")
-    log_str = f"To run with DVC, add this to {path_str}:\n{yaml_str}"
-    logger.info.assert_called_with(log_str)
```

### Comparing `dvclive-2.6.4/tests/test_report.py` & `dvclive-2.7.0/tests/test_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,25 +158,25 @@
         plot_renderer = plot_renderers_dict[name]
         assert plot_renderer.datapoints == [
             {"fpr": 0.0, "rev": "workspace", "threshold": 2.0, "tpr": 0.0},
             {"fpr": 0.5, "rev": "workspace", "threshold": 1.0, "tpr": 0.5},
             {"fpr": 1.0, "rev": "workspace", "threshold": 0.1, "tpr": 0.5},
             {"fpr": 1.0, "rev": "workspace", "threshold": 0.0, "tpr": 1.0},
         ]
-        assert plot_renderer.properties == Roc.get_properties()
+        assert plot_renderer.properties == Roc.DEFAULT_PROPERTIES
 
     for name in ("confusion_matrix", "train/cm"):
         plot_renderer = plot_renderers_dict[name]
         assert plot_renderer.datapoints == [
             {"actual": "0", "rev": "workspace", "predicted": "1"},
             {"actual": "0", "rev": "workspace", "predicted": "0"},
             {"actual": "1", "rev": "workspace", "predicted": "0"},
             {"actual": "1", "rev": "workspace", "predicted": "1"},
         ]
-        assert plot_renderer.properties == ConfusionMatrix.get_properties()
+        assert plot_renderer.properties == ConfusionMatrix.DEFAULT_PROPERTIES
 
 
 def test_report_auto_doesnt_set_notebook(tmp_dir, mocker):
     mocker.patch("dvclive.live.inside_notebook", return_value=True)
     live = Live()
     assert live._report_mode != "notebook"
```

### Comparing `dvclive-2.6.4/tests/test_studio.py` & `dvclive-2.7.0/tests/test_studio.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     metrics_path = Path(live.metrics_file).as_posix()
     params_path = Path(live.params_file).as_posix()
     foo_path = (Path(live.plots_dir) / Metric.subfolder / "foo.tsv").as_posix()
 
     mocked_post, _ = mocked_studio_post
 
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "start",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": live._exp_name,
             "client": "dvclive",
         },
@@ -34,15 +34,15 @@
         timeout=5,
     )
 
     live.log_metric("foo", 1)
 
     live.next_step()
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "data",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": live._exp_name,
             "step": 0,
             "metrics": {metrics_path: {"data": {"step": 0, "foo": 1}}},
@@ -57,15 +57,15 @@
         timeout=5,
     )
 
     live.log_metric("foo", 2)
 
     live.next_step()
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "data",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": live._exp_name,
             "step": 1,
             "metrics": {metrics_path: {"data": {"step": 1, "foo": 2}}},
@@ -78,15 +78,15 @@
             "Content-type": "application/json",
         },
         timeout=5,
     )
 
     live.end()
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "done",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
             "experiment_rev": live._experiment_rev,
             "name": live._exp_name,
             "client": "dvclive",
@@ -116,15 +116,15 @@
     live.log_metric("foo", 1)
     live.next_step()
 
     mocked_post = mocker.patch("requests.post", return_value=valid_response)
     live.log_metric("foo", 2)
     live.next_step()
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "data",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": live._exp_name,
             "step": 1,
             "metrics": {metrics_path: {"data": {"step": 1, "foo": 2}}},
@@ -219,15 +219,15 @@
     live.next_step()
 
     dvc_path = Path(live.dvc_file).as_posix()
     metrics_path = Path(live.metrics_file).as_posix()
     foo_path = (Path(live.plots_dir) / Metric.subfolder / "foo.tsv").as_posix()
 
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "data",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": live._exp_name,
             "step": 0,
             "metrics": {metrics_path: {"data": {"step": 0, "foo": 1}}},
@@ -251,15 +251,15 @@
 
     dvc_path = Path(live.dvc_file).as_posix()
     metrics_path = Path(live.metrics_file).as_posix()
     plots_path = Path(live.plots_dir)
     loss_path = (plots_path / Metric.subfolder / "eval/loss.tsv").as_posix()
 
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "data",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
             "name": live._exp_name,
             "step": 0,
             "metrics": {metrics_path: {"data": {"step": 0, "eval": {"loss": 1}}}},
@@ -304,15 +304,15 @@
     live.next_step()
 
     dvc_path = Path(live.dvc_file).as_posix()
     metrics_path = Path(live.metrics_file).as_posix()
     foo_path = (Path(live.plots_dir) / Metric.subfolder / "foo.tsv").as_posix()
 
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "data",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": live._baseline_rev,
             "name": live._exp_name,
             "step": 0,
             "metrics": {f"subdir/{metrics_path}": {"data": {"step": 0, "foo": 1}}},
@@ -348,15 +348,15 @@
     live.next_step()
 
     dvc_path = Path(live.dvc_file).as_posix()
     metrics_path = Path(live.metrics_file).as_posix()
     foo_path = (Path(live.plots_dir) / Metric.subfolder / "foo.tsv").as_posix()
 
     mocked_post.assert_called_with(
-        "https://0.0.0.0",
+        "https://0.0.0.0/api/live",
         json={
             "type": "data",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": live._baseline_rev,
             "name": live._exp_name,
             "step": 0,
             "metrics": {f"subdir/{metrics_path}": {"data": {"step": 0, "foo": 1}}},
```

### Comparing `dvclive-2.6.4/tests/test_utils.py` & `dvclive-2.7.0/tests/test_utils.py`

 * *Files identical despite different names*

