# Comparing `tmp/syngen-0.0.94.tar.gz` & `tmp/syngen-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.94.tar", last modified: Fri Apr 21 11:16:12 2023, max compression
+gzip compressed data, was "syngen-0.0.95.tar", last modified: Mon Apr 24 07:03:08 2023, max compression
```

## Comparing `syngen-0.0.94.tar` & `syngen-0.0.95.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-21 11:14:52.000000 syngen-0.0.94/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-21 11:14:52.000000 syngen-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-21 11:14:52.000000 syngen-0.0.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-21 11:16:12.375892 syngen-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-21 11:14:52.000000 syngen-0.0.94/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-21 11:14:52.000000 syngen-0.0.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-21 11:16:12.379892 syngen-0.0.94/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.367893 syngen-0.0.94/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.367893 syngen-0.0.94/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.367893 syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6256 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15923 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    28464 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10390 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.375892 syngen-0.0.94/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12935 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-21 11:14:52.000000 syngen-0.0.94/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:16:12.371893 syngen-0.0.94/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-21 11:16:12.000000 syngen-0.0.94/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-21 11:16:12.000000 syngen-0.0.94/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 11:16:12.000000 syngen-0.0.94/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-21 11:16:12.000000 syngen-0.0.94/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-21 11:16:12.000000 syngen-0.0.94/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-21 11:16:12.000000 syngen-0.0.94/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-24 07:01:37.000000 syngen-0.0.95/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-24 07:01:37.000000 syngen-0.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-24 07:01:37.000000 syngen-0.0.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-24 07:03:08.776894 syngen-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-24 07:01:37.000000 syngen-0.0.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-24 07:01:37.000000 syngen-0.0.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-24 07:03:08.776894 syngen-0.0.95/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.760894 syngen-0.0.95/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.764894 syngen-0.0.95/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.760894 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6256 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15923 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.772894 syngen-0.0.95/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28464 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10390 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11009 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.776894 syngen-0.0.95/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-24 07:01:37.000000 syngen-0.0.95/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:03:08.768894 syngen-0.0.95/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-24 07:03:08.000000 syngen-0.0.95/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.94/LICENSE` & `syngen-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/PKG-INFO` & `syngen-0.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.94
+Version: 0.0.95
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.94 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.95 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.94/README.md` & `syngen-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/setup.cfg` & `syngen-0.0.95/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/infer.py` & `syngen-0.0.95/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/config/configurations.py` & `syngen-0.0.95/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/convertor/convertor.py` & `syngen-0.0.95/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.0.95/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/__init__.py` & `syngen-0.0.95/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.0.95/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.0.95/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.0.95/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/metrics/utils.py` & `syngen-0.0.95/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/reporters/reporters.py` & `syngen-0.0.95/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/strategies/strategies.py` & `syngen-0.0.95/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.0.95/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/utils/utils.py` & `syngen-0.0.95/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.0.95/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/vae/models/dataset.py` & `syngen-0.0.95/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/vae/models/features.py` & `syngen-0.0.95/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/vae/models/model.py` & `syngen-0.0.95/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.0.95/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.0.95/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen/ml/worker/worker.py` & `syngen-0.0.95/src/syngen/ml/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,17 @@
         if len(table_names) == 1 and "keys" not in config_of_tables[table_names[0]]:
             # case with one table without any keys
             chain_of_tables = table_names
         else:
             if kwargs.get("type_of_process") in ("infer", "all"):
                 config_of_tables = self._split_pk_fk_metadata(config_of_tables, list(config_of_tables.keys()))
             pk_tables = self._get_tables(config_of_tables, "PK")
+            uq_tables = self._get_tables(config_of_tables, "UQ")
             fk_tables = self._get_tables(config_of_tables, "FK")
-            chain_of_tables = list(dict.fromkeys([*pk_tables, *fk_tables]))
+            chain_of_tables = list(dict.fromkeys([*pk_tables, *uq_tables, *fk_tables]))
 
         return chain_of_tables, config_of_tables
 
     def _split_pk_fk_metadata(self, config, tables):
         for table in tables:
             types_of_keys = [value["type"] for key, value in config[table]["keys"].items()]
             if "PK" in types_of_keys and "FK" in types_of_keys:
```

### Comparing `syngen-0.0.94/src/syngen/train.py` & `syngen-0.0.95/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.94/src/syngen.egg-info/PKG-INFO` & `syngen-0.0.95/src/syngen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.94
+Version: 0.0.95
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.94 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.95 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.94/src/syngen.egg-info/SOURCES.txt` & `syngen-0.0.95/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

