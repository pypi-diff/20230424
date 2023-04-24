# Comparing `tmp/gretel-trainer-0.7.0.tar.gz` & `tmp/gretel-trainer-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gretel-trainer-0.7.0.tar", last modified: Wed Mar 22 19:31:21 2023, max compression
+gzip compressed data, was "gretel-trainer-0.8.0.tar", last modified: Mon Apr 24 18:10:12 2023, max compression
```

## Comparing `gretel-trainer-0.7.0.tar` & `gretel-trainer-0.8.0.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.849322 gretel-trainer-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.837322 gretel-trainer-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.837322 gretel-trainer-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-22 19:31:21.849322 gretel-trainer-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.837322 gretel-trainer-0.7.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/data/cpu_states.csv
--rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/data/mitre-synthea-health.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/img/gretel-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/img/gretel_logo_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/docs/trainer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/notebooks/benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/notebooks/conditional-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/notebooks/custom-example.py
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/notebooks/relational.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/notebooks/simple-conditional-generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/notebooks/simple-example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/notebooks/trainer-examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:31:21.849322 gretel-trainer-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.837322 gretel-trainer-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/src/gretel_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/custom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/custom/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/custom/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.845322 gretel-trainer-0.7.0/src/gretel_trainer/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36666 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/multi_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.845322 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/figures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/key_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report.css
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report_privacy_protection.css
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report_synthetic_quality.css
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/sdk_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.845322 gretel-trainer-0.7.0/src/gretel_trainer/relational/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/strategies/ancestral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/strategies/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/task_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.845322 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/synthetics_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/synthetics_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/transforms_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/relational/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    30567 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/src/gretel_trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.841322 gretel-trainer-0.7.0/src/gretel_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-22 19:31:21.000000 gretel-trainer-0.7.0/src/gretel_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-03-22 19:31:21.000000 gretel-trainer-0.7.0/src/gretel_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:31:21.000000 gretel-trainer-0.7.0/src/gretel_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-22 19:31:21.000000 gretel-trainer-0.7.0/src/gretel_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-22 19:31:21.000000 gretel-trainer-0.7.0/src/gretel_trainer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.845322 gretel-trainer-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.845322 gretel-trainer-0.7.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/data/core-221-train.csv
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/example_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.849322 gretel-trainer-0.7.0/tests/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:31:21.849322 gretel-trainer-0.7.0/tests/relational/example_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/example_dbs/art.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/example_dbs/ecom.sql
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/example_dbs/mutagenesis.sql
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/example_dbs/pets.sql
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/example_dbs/trips.sql
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_ancestral_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_independent_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_multi_table_config_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    25444 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_multi_table_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_synthetics_run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/relational/test_task_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-03-22 19:31:16.000000 gretel-trainer-0.7.0/tests/test_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.869338 gretel-trainer-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.869338 gretel-trainer-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.873338 gretel-trainer-0.8.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/data/cpu_states.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/data/mitre-synthea-health.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.873338 gretel-trainer-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.873338 gretel-trainer-0.8.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/img/gretel-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/img/gretel_logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/trainer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/conditional-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/custom-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15410 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/relational.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/simple-conditional-generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/simple-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/trainer-examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.869338 gretel-trainer-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.881338 gretel-trainer-0.8.0/src/gretel_trainer/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/multi_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.881338 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/key_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_privacy_protection.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_synthetic_quality.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/sdk_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.881338 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/ancestral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/task_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.885339 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.885339 gretel-trainer-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.885339 gretel-trainer-0.8.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/data/core-221-train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/example_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/tests/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/tests/relational/example_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/art.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/ecom.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/mutagenesis.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/pets.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/trips.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    17286 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_ancestral_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_independent_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_multi_table_config_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_multi_table_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_synthetics_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/test_strategy.py
```

### Comparing `gretel-trainer-0.7.0/.github/workflows/python-publish.yml` & `gretel-trainer-0.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/.gitignore` & `gretel-trainer-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/LICENSE` & `gretel-trainer-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/PKG-INFO` & `gretel-trainer-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.7.0
+Version: 0.8.0
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.7.0/README.md` & `gretel-trainer-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/data/cpu_states.csv` & `gretel-trainer-0.8.0/data/cpu_states.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/data/mitre-synthea-health.csv` & `gretel-trainer-0.8.0/data/mitre-synthea-health.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/docs/Makefile` & `gretel-trainer-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/docs/conf.py` & `gretel-trainer-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/docs/img/gretel-logo.png` & `gretel-trainer-0.8.0/docs/img/gretel-logo.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/docs/img/gretel_logo_white.png` & `gretel-trainer-0.8.0/docs/img/gretel_logo_white.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/docs/index.rst` & `gretel-trainer-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/docs/make.bat` & `gretel-trainer-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/docs/quickstart.rst` & `gretel-trainer-0.8.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/notebooks/benchmark.ipynb` & `gretel-trainer-0.8.0/notebooks/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/notebooks/conditional-generation.py` & `gretel-trainer-0.8.0/notebooks/conditional-generation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+from gretel_client import configure_session
 
 from gretel_trainer import Trainer
 from gretel_trainer.models import GretelLSTM, GretelACTGAN
 
 DATASET_PATH = 'https://gretel-public-website.s3.amazonaws.com/datasets/mitre-synthea-health.csv'
 MODEL_TYPE = [GretelLSTM(), GretelACTGAN()][1]
 
@@ -16,14 +17,17 @@
     ["asian", "chinese", "F"],
     ["asian", "chinese", "F"],
     ["asian", "chinese", "F"],
     ["asian", "chinese", "F"]
 ], columns=["RACE", "ETHNICITY", "GENDER"])
 
 
+# Configure Gretel credentials
+configure_session(api_key="prompt", cache="yes", validate=True)
+
 # Train a model and conditionally generate data
 seed_fields = seed_df.columns.values.tolist()
 model = Trainer(model_type=MODEL_TYPE)
 model.train(DATASET_PATH, seed_fields=seed_fields)
 print(model.generate(seed_df=seed_df))
 
 # Load a existing model and conditionally generate data
```

### Comparing `gretel-trainer-0.7.0/notebooks/custom-example.py` & `gretel-trainer-0.8.0/notebooks/custom-example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+from gretel_client import configure_session
+
 from gretel_trainer import Trainer
 from gretel_trainer.models import GretelLSTM, GretelACTGAN
 
 
+# Configure Gretel credentials
+configure_session(api_key="prompt", cache="yes", validate=True)
+
 dataset = "https://gretel-public-website.s3-us-west-2.amazonaws.com/datasets/USAdultIncome5k.csv"
 
 # Specify underlying model and config options.
 # configs can be either a string, dict, or path
 model_type = GretelACTGAN(
     config="synthetics/tabular-actgan",
     max_header_clusters=100,
```

### Comparing `gretel-trainer-0.7.0/notebooks/relational.ipynb` & `gretel-trainer-0.8.0/notebooks/relational.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967948717948718%*

 * *Differences: {"'cells'": "{insert: [(2, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['from gretel_client import "*

 * *            'configure_session\\n\', \'\\n\', \'configure_session(api_key="prompt", cache="yes", '*

 * *            "validate=True)'])]))]}"}*

```diff
@@ -17,14 +17,25 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from gretel_client import configure_session\n",
+                "\n",
+                "configure_session(api_key=\"prompt\", cache=\"yes\", validate=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# End-to-end synthetics example\n",
                 "\n",
                 "from gretel_trainer.relational import MultiTable, sqlite_conn\n",
                 "\n",
                 "\n",
                 "!curl -o \"ecom_xf.db\" \"https://gretel-blueprints-pub.s3.us-west-2.amazonaws.com/rdb/ecom_xf.db\"\n",
                 "\n",
```

### Comparing `gretel-trainer-0.7.0/notebooks/simple-conditional-generation.ipynb` & `gretel-trainer-0.8.0/notebooks/simple-conditional-generation.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'cells'": "{insert: [(2, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['# Configure Gretel "*

 * *            "credentials\\n', 'from gretel_client import configure_session\\n', '\\n', "*

 * *            '\'configure_session(api_key="prompt", cache="yes", validate=True)\'])]))]}'}*

```diff
@@ -29,14 +29,26 @@
                 "print(\"\\nPreviewing real world dataset\\n\")\n",
                 "pd.read_csv(DATASET_PATH)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Configure Gretel credentials\n",
+                "from gretel_client import configure_session\n",
+                "\n",
+                "configure_session(api_key=\"prompt\", cache=\"yes\", validate=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "id": "Gh10cM4SiHPM"
             },
             "outputs": [],
             "source": [
                 "# Train model\n",
                 "model = trainer.Trainer()\n",
```

### Comparing `gretel-trainer-0.7.0/notebooks/trainer-examples.ipynb` & `gretel-trainer-0.8.0/notebooks/trainer-examples.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'cells'": "{insert: [(1, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['# Configure Gretel "*

 * *            "credentials\\n', 'from gretel_client import configure_session\\n', '\\n', "*

 * *            '\'configure_session(api_key="prompt", cache="yes", validate=True)\'])]))]}'}*

```diff
@@ -10,14 +10,26 @@
             "source": [
                 "#!pip install -Uqq gretel-trainer"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Configure Gretel credentials\n",
+                "from gretel_client import configure_session\n",
+                "\n",
+                "configure_session(api_key=\"prompt\", cache=\"yes\", validate=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "id": "rNI6TSbOCrEo"
             },
             "outputs": [],
             "source": [
                 "from gretel_trainer import Trainer\n",
                 "\n",
```

### Comparing `gretel-trainer-0.7.0/setup.py` & `gretel-trainer-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/__init__.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/compare.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/compare.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/core.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/core.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/custom/datasets.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,16 +141,16 @@
             valid_datatypes = [datatype.value for datatype in Datatype]
             raise BenchmarkException(
                 f"Invalid datatype: {datatype}. Must be one of: {valid_datatypes}"
             )
 
     if source_type == pd.DataFrame:
         return DataFramesDataset(
-            dfs=sources,
+            dfs=sources,  # type:ignore
             datatype=datatype,
             local_dir=local_dir,
             namespace=namespace or "DataFrames",
         )
     else:
         return FilesDataset(
-            paths=sources, datatype=datatype, delimiter=delimiter, namespace=namespace
+            paths=sources, datatype=datatype, delimiter=delimiter, namespace=namespace  # type:ignore
         )
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/custom/executor.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/datasets.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/executor.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 import pandas as pd
 
-import gretel_trainer
 
 from gretel_trainer.benchmark.core import DataSource
 from gretel_trainer.benchmark.gretel.models import GretelModel
 from gretel_trainer.benchmark.gretel.sdk import GretelSDK
 from gretel_trainer.benchmark.gretel.trainer import TrainerFactory
+from gretel_trainer.models import _BaseConfig
 
 
 class _GretelTrainerExecutor:
     def __init__(
         self,
         project_name: str,
-        trainer_model_type: Optional[gretel_trainer.models._BaseConfig],
+        trainer_model_type: Optional[_BaseConfig],
         trainer_factory: TrainerFactory,
         benchmark_dir: str,
     ):
         self.project_name = project_name
         self.trainer_model_type = trainer_model_type
         self.trainer_factory = trainer_factory
         self.benchmark_dir = benchmark_dir
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/models.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
-import gretel_trainer
-
 from gretel_client.projects.exceptions import ModelConfigError
 from gretel_client.projects.models import read_model_config
 from gretel_trainer import models
 from gretel_trainer.benchmark.core import BenchmarkException, DataSource, Datatype
+from gretel_trainer.models import _BaseConfig
 
 GretelModelConfig = Union[str, Path, Dict]
 
 
 TRAINER_MODEL_TYPE_CONSTRUCTORS = {
     "actgan": models.GretelACTGAN,
     "amplify": models.GretelAmplify,
@@ -49,15 +48,15 @@
             raise BenchmarkException(f"Invalid Gretel model config")
 
     @property
     def use_trainer(self) -> bool:
         return self.model_key in TRAINER_MODEL_TYPE_CONSTRUCTORS.keys()
 
     @property
-    def trainer_model_type(self) -> Optional[gretel_trainer.models._BaseConfig]:
+    def trainer_model_type(self) -> Optional[_BaseConfig]:
         return TRAINER_MODEL_TYPE_CONSTRUCTORS[self.model_key](self.config)
 
     def runnable(self, source: DataSource) -> bool:
         return _is_compatible(self.model_key, source)
 
 
 class GretelLSTM(GretelModel):
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/benchmark/gretel/sdk.py` & `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/sdk.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/models.py` & `gretel-trainer-0.8.0/src/gretel_trainer/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     """This should be overridden on concrete classes"""
     _max_header_clusters_limit: int
     _max_rows_limit: int
     _model_slug: str
 
     # Should be set by concrete constructors
-    config: Union[str, dict]
+    config: dict
     max_rows: int
     max_header_clusters: int
 
     def __init__(
         self,
         config: Union[str, dict],
         max_rows: int,
@@ -97,16 +97,14 @@
     def _replace_nested_key(self, data, key, value) -> dict:
         """Replace nested keys"""
         if isinstance(data, dict):
             return {
                 k: value if k == key else self._replace_nested_key(v, key, value)
                 for k, v in data.items()
             }
-        elif isinstance(data, list):
-            return [self._replace_nested_key(v, key, value) for v in data]
         else:
             return data
 
 
 class GretelLSTM(_BaseConfig):
     """
     This model works for a variety of synthetic data tasks including time-series, tabular, and text data. Generally useful for a few thousand records and upward. Dataset generally has a mix of categorical, continuous, and numerical values
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/README.md` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/ancestry.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/ancestry.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/artifacts.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/artifacts.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 
 from gretel_client.projects import Project
 
 
 @dataclass
 class ArtifactCollection:
+    hybrid: bool
     gretel_debug_summary: Optional[str] = None
     source_archive: Optional[str] = None
     synthetics_training_archive: Optional[str] = None
     synthetics_outputs_archive: Optional[str] = None
     transforms_outputs_archive: Optional[str] = None
 
     def upload_gretel_debug_summary(self, project: Project, path: str) -> None:
@@ -33,15 +34,23 @@
         existing = self.synthetics_outputs_archive
         self.synthetics_outputs_archive = self._upload_file(project, path, existing)
 
     def upload_transforms_outputs_archive(self, project: Project, path: str) -> None:
         existing = self.transforms_outputs_archive
         self.transforms_outputs_archive = self._upload_file(project, path, existing)
 
-    def _upload_file(self, project: Project, path: str, existing: Optional[str]) -> str:
+    def _upload_file(
+        self, project: Project, path: str, existing: Optional[str]
+    ) -> Optional[str]:
+        # We do not upload any of these artifacts in hybrid contexts because they are intended to be
+        # "singleton" objects, but we cannot list or delete items in users' artifact endpoints, so
+        # we would end up polluting their endpoints with many nearly-duplicative copies of these files.
+        if self.hybrid:
+            return None
+
         latest = project.upload_artifact(path)
         if existing is not None:
             project.delete_artifact(existing)
         return latest
 
 
 def add_to_tar(targz: Path, src: Path, arcname: str) -> None:
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/backup.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/backup.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/connectors.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/connectors.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/core.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/core.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/model_config.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/model_config.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/multi_table.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/multi_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import requests
 import smart_open
-from gretel_client import configure_session
+from gretel_client.config import RunnerMode, get_session_config
 from gretel_client.projects import Project, create_project, get_project
 from gretel_client.projects.jobs import ACTIVE_STATES, END_STATES, Job, Status
 from gretel_client.projects.models import Model, read_model_config
 from gretel_client.projects.records import RecordHandler
 
 from gretel_trainer.relational.artifacts import ArtifactCollection, add_to_tar
 from gretel_trainer.relational.backup import (
@@ -35,29 +35,22 @@
 )
 from gretel_trainer.relational.core import (
     GretelModelConfig,
     MultiTableException,
     RelationalData,
     TableEvaluation,
 )
+from gretel_trainer.relational.log import silent_logs
 from gretel_trainer.relational.model_config import (
     make_evaluate_config,
     make_synthetics_config,
     make_transform_config,
 )
 from gretel_trainer.relational.report.report import ReportPresenter, ReportRenderer
-from gretel_trainer.relational.sdk_extras import (
-    cautiously_refresh_status,
-    delete_data_source,
-    download_file_artifact,
-    download_tar_artifact,
-    get_job_id,
-    room_in_project,
-    sqs_score_from_full_report,
-)
+from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 from gretel_trainer.relational.strategies.ancestral import AncestralStrategy
 from gretel_trainer.relational.strategies.independent import IndependentStrategy
 from gretel_trainer.relational.task_runner import run_task
 from gretel_trainer.relational.tasks import (
     SyntheticsEvaluateTask,
     SyntheticsRunTask,
     SyntheticsTrainTask,
@@ -97,27 +90,25 @@
         backup: Optional[Backup] = None,
     ):
         self._strategy = _validate_strategy(strategy)
         model_name, model_config = self._validate_gretel_model(gretel_model)
         self._gretel_model = model_name
         self._model_config = model_config
         self._set_refresh_interval(refresh_interval)
-
         self.relational_data = relational_data
-        self._artifact_collection = ArtifactCollection()
+        self._artifact_collection = ArtifactCollection(hybrid=self._hybrid)
+        self._extended_sdk = ExtendedGretelSDK(hybrid=self._hybrid)
         self._latest_backup: Optional[Backup] = None
         self._transforms_train = TransformsTrain()
         self.transform_output_tables: Dict[str, pd.DataFrame] = {}
         self._synthetics_train = SyntheticsTrain()
         self._synthetics_run: Optional[SyntheticsRun] = None
         self.synthetic_output_tables: Dict[str, pd.DataFrame] = {}
         self.evaluations = defaultdict(lambda: TableEvaluation())
 
-        configure_session(api_key="prompt", cache="yes", validate=True)
-
         if backup is None:
             self._complete_fresh_init(project_display_name)
         else:
             self._complete_init_from_backup(backup)
 
     def _complete_fresh_init(self, project_display_name: Optional[str]) -> None:
         project_display_name = project_display_name or "multi-table"
@@ -136,25 +127,26 @@
         logger.info(
             f"Connected to existing project `{self._project.display_name}` with unique name `{self._project.name}`."
         )
         self._working_dir = _mkdir(backup.working_dir)
         self._artifact_collection = backup.artifact_collection
 
         # RelationalData
+        source_archive_path = self._working_dir / "source_tables.tar.gz"
         source_archive_id = backup.artifact_collection.source_archive
-        if source_archive_id is None:
+        if source_archive_id is not None:
+            self._extended_sdk.download_tar_artifact(
+                self._project,
+                source_archive_id,
+                source_archive_path,
+            )
+        if not source_archive_path.exists():
             raise MultiTableException(
                 "Cannot restore from backup: source archive is missing."
             )
-        source_archive_path = self._working_dir / "source_tables.tar.gz"
-        download_tar_artifact(
-            self._project,
-            source_archive_id,
-            source_archive_path,
-        )
         with tarfile.open(source_archive_path, "r:gz") as tar:
             tar.extractall(path=self._working_dir)
         for table_name, table_backup in backup.relational_data.tables.items():
             source_data = pd.read_csv(self._working_dir / f"source_{table_name}.csv")
             self.relational_data.add_table(
                 name=table_name, primary_key=table_backup.primary_key, data=source_data
             )
@@ -162,15 +154,15 @@
             self.relational_data.add_foreign_key(
                 foreign_key=fk_backup.foreign_key, referencing=fk_backup.referencing
             )
 
         # Debug summary
         debug_summary_id = backup.artifact_collection.gretel_debug_summary
         if debug_summary_id is not None:
-            download_file_artifact(
+            self._extended_sdk.download_file_artifact(
                 self._project,
                 debug_summary_id,
                 self._working_dir / "_gretel_debug_summary.json",
             )
 
         # Transforms Train
         backup_transforms_train = backup.transforms_train
@@ -189,26 +181,27 @@
             logger.info(
                 "No synthetics training data found in backup. From here, your next step is to call `train`."
             )
             return None
 
         logger.info("Restoring synthetics models")
 
+        synthetics_training_archive_path = (
+            self._working_dir / "synthetics_training.tar.gz"
+        )
         synthetics_training_archive_id = (
             self._artifact_collection.synthetics_training_archive
         )
         if synthetics_training_archive_id is not None:
-            synthetics_training_archive_path = (
-                self._working_dir / "synthetics_training.tar.gz"
-            )
-            download_tar_artifact(
+            self._extended_sdk.download_tar_artifact(
                 self._project,
                 synthetics_training_archive_id,
                 synthetics_training_archive_path,
             )
+        if synthetics_training_archive_path.exists():
             with tarfile.open(synthetics_training_archive_path, "r:gz") as tar:
                 tar.extractall(path=self._working_dir)
 
         self._synthetics_train.training_columns = (
             backup_synthetics_train.training_columns
         )
         self._synthetics_train.lost_contact = backup_synthetics_train.lost_contact
@@ -233,45 +226,49 @@
         training_succeeded = [
             table
             for table, model in self._synthetics_train.models.items()
             if model.status == Status.COMPLETED
         ]
         for table in training_succeeded:
             model = self._synthetics_train.models[table]
-            self._strategy.update_evaluation_from_model(
-                table, self.evaluations, model, self._working_dir
-            )
+            with silent_logs():
+                self._strategy.update_evaluation_from_model(
+                    table,
+                    self.evaluations,
+                    model,
+                    self._working_dir,
+                    self._extended_sdk,
+                )
 
         training_failed = [
             table
             for table, model in self._synthetics_train.models.items()
             if model.status in END_STATES and table not in training_succeeded
         ]
         if len(training_failed) > 0:
             logger.info(
                 f"Training failed for tables: {training_failed}. From here, your next step is to try retraining them with modified data by calling `retrain_tables`."
             )
             return None
 
         # Synthetics Generate
         ## First, download the outputs archive if present and extract the data.
+        synthetics_output_archive_path = self._working_dir / "synthetics_outputs.tar.gz"
         synthetics_outputs_archive_id = (
             self._artifact_collection.synthetics_outputs_archive
         )
         any_outputs = False
         if synthetics_outputs_archive_id is not None:
-            any_outputs = True
-            synthetics_output_archive_path = (
-                self._working_dir / "synthetics_outputs.tar.gz"
-            )
-            download_tar_artifact(
+            self._extended_sdk.download_tar_artifact(
                 self._project,
                 synthetics_outputs_archive_id,
                 synthetics_output_archive_path,
             )
+        if synthetics_output_archive_path.exists():
+            any_outputs = True
             with tarfile.open(synthetics_output_archive_path, "r:gz") as tar:
                 tar.extractall(path=self._working_dir)
 
         ## Then, restore latest, potentially in-progress run data if present
         backup_generate = backup.generate
         if backup_generate is None:
             if any_outputs:
@@ -321,15 +318,15 @@
             return None
         else:
             # Latest run was still in progress. Download any seeds we may have previously created.
             for table, rh in record_handlers.items():
                 data_source = rh.data_source
                 if data_source is not None:
                     try:
-                        download_file_artifact(
+                        self._extended_sdk.download_file_artifact(
                             self._project,
                             data_source,
                             self._working_dir
                             / backup_generate.identifier
                             / f"synthetics_seed_{table}.csv",
                         )
                     except:
@@ -362,15 +359,15 @@
             return None
 
         # write to local directory
         backup_path = self._working_dir / "_gretel_backup.json"
         with open(backup_path, "w") as bak:
             json.dump(backup.as_dict, bak)
 
-        _upload_gretel_backup(self._project, str(backup_path))
+        _upload_gretel_backup(self._project, str(backup_path), self._hybrid)
 
         self._latest_backup = backup
 
     def _build_backup(self) -> Backup:
         backup = Backup(
             project_name=self._project.name,
             strategy=self._strategy.name,
@@ -416,14 +413,18 @@
                     table: rh.record_id
                     for table, rh in self._synthetics_run.record_handlers.items()
                 },
             )
 
         return backup
 
+    @property
+    def _hybrid(self) -> bool:
+        return get_session_config().default_runner == RunnerMode.HYBRID
+
     def _set_refresh_interval(self, interval: Optional[int]) -> None:
         if interval is None:
             self._refresh_interval = 60
         else:
             if interval < 30:
                 logger.warning(
                     "Refresh interval must be at least 30 seconds. Setting to 30."
@@ -464,15 +465,15 @@
 
         self._backup()
 
         task = TransformsTrainTask(
             transforms_train=self._transforms_train,
             multitable=self,
         )
-        run_task(task)
+        run_task(task, self._extended_sdk)
 
     def run_transforms(
         self,
         identifier: Optional[str] = None,
         in_place: bool = False,
         data: Optional[Dict[str, pd.DataFrame]] = None,
     ) -> None:
@@ -522,15 +523,15 @@
             )
             transforms_record_handlers[table_name] = record_handler
 
         task = TransformsRunTask(
             record_handlers=transforms_record_handlers,
             multitable=self,
         )
-        run_task(task)
+        run_task(task, self._extended_sdk)
 
         output_tables = self._strategy.label_encode_keys(
             self.relational_data, task.output_tables
         )
 
         if in_place:
             for table_name, transformed_table in output_tables.items():
@@ -579,20 +580,20 @@
 
         self._backup()
 
         task = SyntheticsTrainTask(
             synthetics_train=self._synthetics_train,
             multitable=self,
         )
-        run_task(task)
+        run_task(task, self._extended_sdk)
 
         for table in task.completed:
             model = self._synthetics_train.models[table]
             self._strategy.update_evaluation_from_model(
-                table, self.evaluations, model, self._working_dir
+                table, self.evaluations, model, self._working_dir, self._extended_sdk
             )
 
         # TODO: consider moving this to before running the task
         archive_path = self._working_dir / "synthetics_training.tar.gz"
         for table_name, csv_path in training_data.items():
             add_to_tar(archive_path, csv_path, csv_path.name)
         self._artifact_collection.upload_synthetics_training_archive(
@@ -706,15 +707,15 @@
 
         task = SyntheticsRunTask(
             synthetics_run=self._synthetics_run,
             synthetics_train=self._synthetics_train,
             run_dir=run_dir,
             multitable=self,
         )
-        run_task(task)
+        run_task(task, self._extended_sdk)
 
         output_tables = self._strategy.post_process_synthetic_results(
             task.output_tables, self._synthetics_run.preserved, self.relational_data
         )
 
         for table, synth_df in output_tables.items():
             synth_csv_path = run_dir / f"synth_{table}.csv"
@@ -743,22 +744,23 @@
             )
 
         synthetics_evaluate_task = SyntheticsEvaluateTask(
             evaluate_models=evaluate_models,
             project=evaluate_project,
             multitable=self,
         )
-        run_task(synthetics_evaluate_task)
+        run_task(synthetics_evaluate_task, self._extended_sdk)
 
         for table in synthetics_evaluate_task.completed:
             self._strategy.update_evaluation_from_evaluate(
                 table_name=table,
                 evaluate_model=evaluate_models[table],
                 evaluations=self.evaluations,
                 working_dir=self._working_dir,
+                extended_sdk=self._extended_sdk,
             )
 
         evaluate_project.delete()
 
         for table_name in output_tables:
             for eval_type in ["individual", "cross_table"]:
                 for ext in ["html", "json"]:
@@ -871,15 +873,17 @@
 
 def _mkdir(name: str) -> Path:
     d = Path(name)
     os.makedirs(d, exist_ok=True)
     return d
 
 
-def _upload_gretel_backup(project: Project, path: str) -> None:
+def _upload_gretel_backup(project: Project, path: str, hybrid: bool) -> None:
+    if hybrid:
+        return None
     latest = project.upload_artifact(path)
     for artifact in project.artifacts:
         key = artifact["key"]
         if key != latest and key.endswith("__gretel_backup.json"):
             project.delete_artifact(key)
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/report/figures.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/figures.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/report/key_highlight.js` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/key_highlight.js`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report.css` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report_privacy_protection.css` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_privacy_protection.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report_synthetic_quality.css` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_synthetic_quality.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/report/report_template.html` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_template.html`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/strategies/ancestral.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/ancestral.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import gretel_trainer.relational.ancestry as ancestry
 import gretel_trainer.relational.strategies.common as common
 from gretel_trainer.relational.core import (
     MultiTableException,
     RelationalData,
     TableEvaluation,
 )
+from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 
 logger = logging.getLogger(__name__)
 
 
 class AncestralStrategy:
     @property
     def name(self) -> str:
@@ -272,18 +273,19 @@
 
     def update_evaluation_from_model(
         self,
         table_name: str,
         evaluations: Dict[str, TableEvaluation],
         model: Model,
         working_dir: Path,
+        extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading cross_table evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_cross_table_evaluation_{table_name}"
-        common.download_artifacts(model, out_filepath, table_name)
+        common.download_artifacts(model, out_filepath, extended_sdk)
 
         evaluation = evaluations[table_name]
         evaluation.cross_table_report_json = common.read_report_json_data(
             model, out_filepath
         )
 
     def get_evaluate_model_data(
@@ -299,18 +301,19 @@
 
     def update_evaluation_from_evaluate(
         self,
         table_name: str,
         evaluations: Dict[str, TableEvaluation],
         evaluate_model: Model,
         working_dir: Path,
+        extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading individual evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_individual_evaluation_{table_name}"
-        common.download_artifacts(evaluate_model, out_filepath, table_name)
+        common.download_artifacts(evaluate_model, out_filepath, extended_sdk)
 
         evaluation = evaluations[table_name]
         evaluation.individual_report_json = common.read_report_json_data(
             evaluate_model, out_filepath
         )
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/strategies/common.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 
 import pandas as pd
 import smart_open
 from gretel_client.projects.models import Model
 from sklearn import preprocessing
 
 from gretel_trainer.relational.core import RelationalData
-from gretel_trainer.relational.sdk_extras import download_file_artifact
+from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 
 logger = logging.getLogger(__name__)
 
 
-def download_artifacts(model: Model, out_filepath: Path, table_name: str) -> None:
+def download_artifacts(
+    model: Model, out_filepath: Path, extended_sdk: ExtendedGretelSDK
+) -> None:
     """
     Downloads all model artifacts to a subdirectory in the working directory.
-    Returns the artifact directory path when successful.
     """
     legend = {"html": "report", "json": "report_json"}
 
     for filetype, artifact_name in legend.items():
         out_path = f"{out_filepath}.{filetype}"
-        download_file_artifact(model, artifact_name, out_path)
+        extended_sdk.download_file_artifact(model, artifact_name, out_path)
 
 
 def read_report_json_data(model: Model, report_path: Path) -> Optional[Dict]:
     full_path = f"{report_path}.json"
     try:
         return json.loads(smart_open.open(full_path).read())
     except:
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/strategies/independent.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/independent.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import gretel_trainer.relational.ancestry as ancestry
 import gretel_trainer.relational.strategies.common as common
 from gretel_trainer.relational.core import (
     MultiTableException,
     RelationalData,
     TableEvaluation,
 )
+from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 
 logger = logging.getLogger(__name__)
 
 
 class IndependentStrategy:
     @property
     def name(self) -> str:
@@ -146,18 +147,19 @@
 
     def update_evaluation_from_model(
         self,
         table_name: str,
         evaluations: Dict[str, TableEvaluation],
         model: Model,
         working_dir: Path,
+        extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading individual evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_individual_evaluation_{table_name}"
-        common.download_artifacts(model, out_filepath, table_name)
+        common.download_artifacts(model, out_filepath, extended_sdk)
 
         evaluation = evaluations[table_name]
         evaluation.individual_report_json = common.read_report_json_data(
             model, out_filepath
         )
 
     def get_evaluate_model_data(
@@ -188,18 +190,19 @@
 
     def update_evaluation_from_evaluate(
         self,
         table_name: str,
         evaluations: Dict[str, TableEvaluation],
         evaluate_model: Model,
         working_dir: Path,
+        extended_sdk: ExtendedGretelSDK,
     ) -> None:
         logger.info(f"Downloading cross table evaluation reports for `{table_name}`.")
         out_filepath = working_dir / f"synthetics_cross_table_evaluation_{table_name}"
-        common.download_artifacts(evaluate_model, out_filepath, table_name)
+        common.download_artifacts(evaluate_model, out_filepath, extended_sdk)
 
         evaluation = evaluations[table_name]
         evaluation.cross_table_report_json = common.read_report_json_data(
             evaluate_model, out_filepath
         )
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/task_runner.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/task_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,15 @@
 from collections import defaultdict
 from typing import Dict, List
 
 from gretel_client.projects.jobs import ACTIVE_STATES, END_STATES, Job, Status
 from gretel_client.projects.projects import Project
 from typing_extensions import Protocol
 
-from gretel_trainer.relational.sdk_extras import (
-    cautiously_refresh_status,
-    delete_data_source,
-    get_job_id,
-    room_in_project,
-    start_job_if_possible,
-)
+from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 
 MAX_REFRESH_ATTEMPTS = 3
 
 logger = logging.getLogger(__name__)
 
 
 class Task(Protocol):
@@ -59,55 +53,57 @@
     def handle_lost_contact(self, table: str) -> None:
         ...
 
     def each_iteration(self) -> None:
         ...
 
 
-def run_task(task: Task) -> None:
+def run_task(task: Task, extended_sdk: ExtendedGretelSDK) -> None:
     refresh_attempts: Dict[str, int] = defaultdict(int)
     first_pass = True
 
     while task.more_to_do():
         if first_pass:
             first_pass = False
         else:
             _wait(task.refresh_interval)
 
         for table_name in task.table_collection:
             if task.is_finished(table_name):
                 continue
 
             job = task.get_job(table_name)
-            if get_job_id(job) is None:
-                start_job_if_possible(
+            if extended_sdk.get_job_id(job) is None:
+                extended_sdk.start_job_if_possible(
                     job=job,
                     table_name=table_name,
                     action=task.action,
                     project=task.project,
                     number_of_artifacts=task.artifacts_per_job,
                 )
                 continue
 
-            status = cautiously_refresh_status(job, table_name, refresh_attempts)
+            status = extended_sdk.cautiously_refresh_status(
+                job, table_name, refresh_attempts
+            )
 
             if refresh_attempts[table_name] >= MAX_REFRESH_ATTEMPTS:
                 _log_lost_contact(table_name)
                 task.handle_lost_contact(table_name)
-                delete_data_source(task.project, job)
+                extended_sdk.delete_data_source(task.project, job)
                 continue
 
             if status == Status.COMPLETED:
                 _log_success(table_name, task.action)
                 task.handle_completed(table_name, job)
-                delete_data_source(task.project, job)
+                extended_sdk.delete_data_source(task.project, job)
             elif status in END_STATES:
                 _log_failed(table_name, task.action)
                 task.handle_failed(table_name)
-                delete_data_source(task.project, job)
+                extended_sdk.delete_data_source(task.project, job)
             else:
                 _log_in_progress(table_name, status, task.action)
 
         task.each_iteration()
 
 
 def _wait(seconds: int) -> None:
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/synthetics_run.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 
 import pandas as pd
 from gretel_client.projects.jobs import ACTIVE_STATES, Job
 from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
 from gretel_client.projects.records import RecordHandler
 
-from gretel_trainer.relational.sdk_extras import (
-    get_record_handler_data,
-    start_job_if_possible,
-)
 from gretel_trainer.relational.tasks.common import _MultiTable
 from gretel_trainer.relational.workflow_state import SyntheticsRun, SyntheticsTrain
 
 logger = logging.getLogger(__name__)
 
 
 class SyntheticsRunTask:
@@ -79,15 +75,15 @@
     def is_finished(self, table: str) -> bool:
         return table in self.working_tables
 
     def get_job(self, table: str) -> Job:
         return self.synthetics_run.record_handlers[table]
 
     def handle_completed(self, table: str, job: Job) -> None:
-        record_handler_data = get_record_handler_data(job)
+        record_handler_data = self.multitable._extended_sdk.get_record_handler_data(job)
         post_processed_data = (
             self.multitable._strategy.post_process_individual_synthetic_result(
                 table, self.multitable.relational_data, record_handler_data
             )
         )
         self.working_tables[table] = post_processed_data
 
@@ -135,15 +131,15 @@
                 self.synthetics_train.training_columns[table_name],
             )
             model = self.synthetics_train.models[table_name]
             record_handler = model.create_record_handler_obj(**table_job)
             self.synthetics_run.record_handlers[table_name] = record_handler
             # Attempt starting the record handler right away. If it can't start right at this moment,
             # the regular task runner check will handle starting it when possible.
-            start_job_if_possible(
+            self.multitable._extended_sdk.start_job_if_possible(
                 job=record_handler,
                 table_name=table_name,
                 action=self.action,
                 project=self.project,
                 number_of_artifacts=self.artifacts_per_job,
             )
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/synthetics_train.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_train.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/transforms_run.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Dict, List, Optional
 
 import pandas as pd
 from gretel_client.projects.jobs import Job
 from gretel_client.projects.projects import Project
 from gretel_client.projects.records import RecordHandler
 
-from gretel_trainer.relational.sdk_extras import get_record_handler_data
 from gretel_trainer.relational.tasks.common import _MultiTable
 
 
 class TransformsRunTask:
     def __init__(
         self,
         record_handlers: Dict[str, RecordHandler],
@@ -53,15 +52,17 @@
     def is_finished(self, table: str) -> bool:
         return table in self.working_tables
 
     def get_job(self, table: str) -> Job:
         return self.record_handlers[table]
 
     def handle_completed(self, table: str, job: Job) -> None:
-        self.working_tables[table] = get_record_handler_data(job)
+        self.working_tables[
+            table
+        ] = self.multitable._extended_sdk.get_record_handler_data(job)
 
     def handle_failed(self, table: str) -> None:
         self.working_tables[table] = None
 
     def handle_lost_contact(self, table: str) -> None:
         self.working_tables[table] = None
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/tasks/transforms_train.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_train.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/relational/workflow_state.py` & `gretel-trainer-0.8.0/src/gretel_trainer/relational/workflow_state.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/runner.py` & `gretel-trainer-0.8.0/src/gretel_trainer/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from collections import Counter
 from concurrent.futures import ALL_COMPLETED, ThreadPoolExecutor, wait
 from copy import deepcopy
 from dataclasses import dataclass
 from functools import wraps
 from pathlib import Path
 from random import choice
-from typing import List, Optional, Union
+from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 import smart_open
 from gretel_client.projects import Project
 from gretel_client.projects.jobs import ACTIVE_STATES
 from gretel_client.projects.models import Model, Status
 from gretel_client.projects.records import RecordHandler
@@ -70,56 +70,44 @@
 class GenPayload:
     num_records: int
     seed_df: Optional[pd.DataFrame] = None
     seed_artifact_id: Optional[str] = None
     max_invalid: Optional[int] = None
 
 
-def _needs_load(func):
-    @wraps(func)
-    def wrapper(inst: StrategyRunner, *args, **kwargs):
-        if not inst._loaded:
-            inst.load()
-        return func(inst, *args, **kwargs)
-
-    return wrapper
-
-
 @dataclass
 class RemoteDFPayload:
     partition: int
     slot: int
     job_type: str
-    uid: str
-    handler_uid: str
+    uid: Optional[str]
+    handler_uid: Optional[str]
     project: Project
     artifact_type: str
-    df: pd.DataFrame = None
 
 
-def _remote_dataframe_fetcher(payload: RemoteDFPayload) -> RemoteDFPayload:
+def _remote_dataframe_fetcher(payload: RemoteDFPayload) -> Tuple[RemoteDFPayload, pd.DataFrame]:
     # We need the model object no matter what
     model = Model(payload.project, model_id=payload.uid)
     job = model
 
     # if we are downloading handler data, we reset our job
     # to the specific handler object
     if payload.job_type == "run":
         job = RecordHandler(model, record_id=payload.handler_uid)
 
     download_url = job.get_artifact_link(payload.artifact_type)
-    payload.df = pd.read_csv(download_url, compression="gzip")
-    return payload
+    return payload, pd.read_csv(download_url, compression="gzip")
 
 
 def _maybe_submit_job(
     job: Union[Model, RecordHandler]
 ) -> Optional[Union[Model, RecordHandler]]:
     try:
-        job = job.submit_cloud()
+        job = job.submit()
     except ApiException as err:
         if "Maximum number of" in str(err):
             logger.warning(
                 "Rate limiting: Max jobs created, skipping new job for now..."
             )
             return None
         else:
@@ -128,20 +116,19 @@
     return job
 
 
 class StrategyRunner:
 
     _df: pd.DataFrame
     _cache_file: Path
-    _constraints = PartitionConstraints
-    _strategy = PartitionStrategy
+    _constraints: PartitionConstraints
+    _strategy: PartitionStrategy
     _model_config: dict
     _max_jobs_active: int
     _project: Project
-    _loaded: bool
     _artifacts: List[str]
     _cache_overwrite: bool
     _max_artifacts: int = 25
     _status_counter: Counter
     _handler_status_counter: Counter
     _error_retry_limit: int
     strategy_id: str
@@ -152,70 +139,46 @@
         strategy_id: str,
         df: pd.DataFrame,
         cache_file: Union[str, Path],
         cache_overwrite: bool = False,
         model_config: dict,
         partition_constraints: PartitionConstraints,
         project: Project,
+        hybrid: bool,
         error_retry_limit: int = 3,
     ):
         self._df = df
         self._cache_file = Path(cache_file)
         self._constraints = partition_constraints
         self._model_config = model_config
         self._project = project
-        self._loaded = False
         self._cache_overwrite = cache_overwrite
         self._artifacts = []
         self.strategy_id = strategy_id
         self._status_counter = Counter()
+        self._hybrid = hybrid
         self._error_retry_limit = error_retry_limit
+        self._strategy = self._load_strategy()
 
-    def load(self):
-        """Hydrate the instance before we can start
-        doing work, must be called after init
-        """
-        if self._loaded:
-            return
-
+    def _load_strategy(self) -> PartitionStrategy:
         self._refresh_max_job_capacity()
 
         # If the cache file exists, we'll try and load an existing
         # strategy. If not, we'll create a new strategy with the
         # provided constraints.
 
         if self._cache_file.exists() and not self._cache_overwrite:
-            self._strategy = PartitionStrategy.from_disk(self._cache_file)
+            strategy = PartitionStrategy.from_disk(self._cache_file)
         else:
-            self._strategy = PartitionStrategy.from_dataframe(
+            strategy = PartitionStrategy.from_dataframe(
                 self.strategy_id, self._df, self._constraints
             )
 
-        self._strategy.save_to(self._cache_file, overwrite=True)
-
-        self._loaded = True
-
-    @classmethod
-    def from_completed(
-        cls, project: Project, cache_file: Union[str, Path]
-    ) -> StrategyRunner:
-        cache_file = Path(cache_file)
-        if not cache_file.exists():
-            raise ValueError("cache file does not exist")
-
-        inst = cls(
-            strategy_id="__none__",
-            df=None,
-            cache_file=cache_file,
-            model_config=None,
-            partition_constraints=None,
-            project=project,
-        )
-        inst.load()
-        return inst
+        strategy.save_to(self._cache_file, overwrite=True)
+        return strategy
 
     def _update_job_status(self):
         # Get all jobs that have been created, we can do this
         # by just searching for any partitions have have a "model_id"
         # set
         partitions = self._strategy.query_glob(MODEL_ID, "*")
         # logger.info(f"Fetching updates for {len(partitions)} models...")
@@ -303,36 +266,38 @@
                 logger.info(
                     f"Partition {partition.idx} record generation status change from {last_status} to {current_handler.status}"
                 )
 
             partition.ctx[HANDLER][STATUS] = current_handler.status
             self._strategy.save()
 
-    @_needs_load
     def cancel_all(self):
         partitions = self._strategy.query_glob(MODEL_ID, "*")
         for partition in partitions:
             model_id = partition.ctx.get(MODEL_ID)
 
             # Hydrate a Model object from the remote API
             current_model = Model(self._project, model_id=model_id)
             logger.warning(f"Cancelling: {current_model.id}")
             current_model.cancel()
 
     def _refresh_max_job_capacity(self):
         self._max_jobs_active = get_me()["service_limits"]["max_jobs_active"]
 
     @property
-    @_needs_load
     def has_capacity(self) -> bool:
         num_active = len(self._gather_statuses(ACTIVE_STATES))
         self._refresh_max_job_capacity()
         return num_active < self._max_jobs_active
 
     def _remove_unused_artifact(self) -> Optional[str]:
+        # Artifact eviction is both unnecessary and unsupported in hybrid deployments
+        if self._hybrid:
+            return "__none__"
+
         project_artifacts = self._project.artifacts
         curr_artifacts = set()
 
         if len(project_artifacts) < self._max_artifacts:
             return "__none__"
 
         # First we try and remove an artifact from this strategy by
@@ -402,15 +367,14 @@
     def _df_to_artifact(self, df: pd.DataFrame, filename: str) -> ArtifactResult:
         with tempfile.TemporaryDirectory() as tmp:
             target_file = str(Path(tmp) / filename)
             df.to_csv(target_file, index=False)
             artifact_id = self._project.upload_artifact(target_file)
             return ArtifactResult(id=artifact_id, record_count=len(df))
 
-    @_needs_load
     def train_partition(
         self, partition: Partition, artifact: ArtifactResult
     ) -> Optional[str]:
         attempt = partition.ctx.get(ATTEMPT, 0) + 1
         model_config = deepcopy(self._model_config)
         data_source = None
 
@@ -460,28 +424,27 @@
         )
         self._strategy.save()
         logger.info(
             f"Started model: {model.print_obj['model_name']} " f"source: {artifact.id}"
         )
         return model.model_id
 
-    @_needs_load
     def run_partition(
         self, partition: Partition, gen_payload: GenPayload
     ) -> Optional[str]:
         """
         Run a record handler for a model and return the job id.
 
         NOTE: This assumes the partition is successfully trained and has an
         available model.
         """
         handler_dict = partition.ctx.get(HANDLER)
         if handler_dict is None:
             partition.ctx[HANDLER] = {}
-        attempt = partition.ctx.get(HANDLER).get(ATTEMPT, 0) + 1
+        attempt = partition.ctx.get(HANDLER, {}).get(ATTEMPT, 0) + 1
         model_id = partition.ctx.get(MODEL_ID)
 
         # Hydrate our trained model so we can start the handler
         model_obj = Model(self._project, model_id=model_id)
 
         # Create and start our handler to generate data
         handler_obj = model_obj.create_record_handler_obj(
@@ -506,15 +469,14 @@
         partition.ctx[HANDLER].update(_ctx_update)
         self._strategy.save()
         logger.info(
             f"Generating {gen_payload.num_records} records from model: {model_obj.print_obj['model_name']}"
         )
         return handler_obj.record_id
 
-    @_needs_load
     def train_next_partition(self) -> Optional[str]:
         start_job = False
         for partition in self._strategy.partitions:
             status = partition.ctx.get(STATUS)  # type: Status
 
             # If we've never done a job for this partition, we should start one
             if status is None:
@@ -531,19 +493,18 @@
                 logger.info(
                     f"Partition {partition.idx} status: {status.value}, re-attempting job"
                 )
                 start_job = True
 
             if start_job:
                 artifact = self._partition_to_artifact(partition)
-                if artifact.id is None:
+                if artifact is None or artifact.id is None:
                     return None
                 return self.train_partition(partition, artifact)
 
-    @_needs_load
     def run_next_partition(self, gen_payload: GenPayload) -> Optional[str]:
         start_job = False
         for partition in self._strategy.partitions:
             status = partition.ctx.get(HANDLER, {}).get(STATUS)  # type: Status
             attempt_count = partition.ctx.get(HANDLER, {}).get(ATTEMPT, 0)
 
             if status is None:
@@ -556,15 +517,15 @@
             ):
                 logger.info(
                     f"Partition {partition.idx} has status {status.value}, re-attempting generation"
                 )
                 start_job = True
 
             if start_job:
-                use_seeds = False
+                seed_artifact_id = None
                 # If this partition has seed fields and we were given seeds, we need to upload
                 # the artifact first.
                 if partition.columns.seed_headers and isinstance(
                     gen_payload.seed_df, pd.DataFrame
                 ):
                     # NOTE(jm): If we've tried N-1 attempts with seeds and the handler has continued
                     # fail then we should not use seeds to at least let the handler try to succeed.
@@ -574,34 +535,33 @@
                         logger.info(
                             f"WARNING: Disabling seeds for partition {partition.idx} due to previous failed generation attempts..."
                         )
                     else:
                         logger.info(
                             "Partition has seed fields, uploading seed artifact..."
                         )
-                        use_seeds = True
                         removed_artifact = self._remove_unused_artifact()
                         if removed_artifact is None:
                             logger.info(
                                 "Could not start generation with seeds, an old artifact could not be removed"
                             )
                             return None
 
                         filename = f"{self.strategy_id}-seeds-{partition.idx}.csv"
                         artifact = self._df_to_artifact(gen_payload.seed_df, filename)
+                        seed_artifact_id = artifact.id
 
                 new_payload = GenPayload(
                     num_records=gen_payload.num_records,
                     max_invalid=gen_payload.max_invalid,
-                    seed_artifact_id=artifact.id if use_seeds else None,
+                    seed_artifact_id=seed_artifact_id,
                 )
 
                 return self.run_partition(partition, new_payload)
 
-    @_needs_load
     def clear_partition_runs(self):
         """
         Partitions should only be trained until they are 'completed', however we can run
         a partition any number of times. Before we do that, we want to go through and
         """
         for partition in self._strategy.partitions:
             partition.ctx[HANDLER] = {}
@@ -612,15 +572,14 @@
             status = partition.ctx.get(STATUS)
             if status is None:
                 continue
             if status in statuses:
                 out.append(partition)
         return out
 
-    @_needs_load
     def is_done(self, *, handler: bool = False) -> bool:
         done = 0
         for p in self._strategy.partitions:
             if handler:
                 ctx_base = p.ctx.get(HANDLER, {})
             else:
                 ctx_base = p.ctx
@@ -636,15 +595,14 @@
                 status in (Status.ERROR, Status.LOST)
                 and attempt >= self._error_retry_limit
             ):
                 done += 1
 
         return done == len(self._strategy.partitions)
 
-    @_needs_load
     def train_all_partitions(self):
         logger.info(f"Processing {len(self._strategy.partitions)} partitions")
         while True:
             self._update_job_status()
             if not self.has_capacity:
                 logger.debug("At active capacity, waiting for more...")
                 time.sleep(10)
@@ -657,15 +615,14 @@
             if self.is_done():
                 break
 
             time.sleep(10)
 
         logger.info(dict(self._status_counter))
 
-    @_needs_load
     def _get_synthetic_data(self, job_type: str, artifact_type: str) -> pd.DataFrame:
         if job_type == "model":
             self._update_job_status()
             num_completed = self._status_counter.get(Status.COMPLETED, 0)
         elif job_type == "run":
             self._update_handler_status()
             num_completed = self._handler_status_counter.get(Status.COMPLETED, 0)
@@ -699,18 +656,18 @@
                 artifact_type=artifact_type,
             )
             futures.append(pool.submit(_remote_dataframe_fetcher, payload))
 
         wait(futures, return_when=ALL_COMPLETED)
 
         for future in futures:
-            payload = future.result()  # type: RemoteDFPayload
+            payload, this_df = future.result()
 
             curr_df = df_chunks[payload.slot]
-            df_chunks[payload.slot] = pd.concat([curr_df, payload.df]).reset_index(
+            df_chunks[payload.slot] = pd.concat([curr_df, this_df]).reset_index(
                 drop=True
             )
 
         df = pd.concat(list(df_chunks.values()), axis=1)
         return df
 
     def _maybe_restore_df_headers(self, df) -> pd.DataFrame:
@@ -732,30 +689,32 @@
 
     def get_sqs_information(self) -> List[dict]:
         return [
             partition.ctx[SQS]
             for partition in self._strategy.partitions
         ]
 
-    @_needs_load
     def generate_data(
         self,
         *,
         seed_df: Optional[pd.DataFrame] = None,
         num_records: Optional[int] = None,
         max_invalid: Optional[int] = None,
         clear_cache: bool = False,
     ):
 
         if seed_df is None and not num_records:
             raise ValueError("must provide a seed_df or num_records to generate")
 
-        if isinstance(seed_df, pd.DataFrame) and num_records:
+        if seed_df is not None and num_records:
             raise ValueError("must use one of seed_df or num_records only")
 
+        # Pyright's type-narrowing doesn't understand that at this point exactly one of num_records and seed_df is None
+        num_records = num_records or len(seed_df)  # type:ignore
+
         # Refresh all of the trained models
         logger.info("Loading existing model information...")
         self._update_job_status()
 
         # We can't generate a dataset if any of the models are in a bad state, so we check that here
         completed_count = self._status_counter[Status.COMPLETED]
         if completed_count != self._strategy.partition_count:
@@ -767,16 +726,14 @@
         if clear_cache:
             self.clear_partition_runs()
 
         # If we have seeds, then we use the number of seeds as the number of records
         # to generate from each model.
         found_seeds = False
         if isinstance(seed_df, pd.DataFrame):
-            num_records = len(seed_df)
-
             # Loop through all of the partitions and make sure we have some that
             # take seed values, if we don't have any partitions set for seeds
             # and we recieved a seed DF, we should error.
             for partition in self._strategy.partitions:
                 if partition.columns.seed_headers:
                     found_seeds = True
                     break
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/strategy.py` & `gretel-trainer-0.8.0/src/gretel_trainer/strategy.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,41 +22,33 @@
     seed_headers: Optional[List[str]]
     idx: int
 
 
 class Partition(BaseModel):
     idx: int
     rows: RowPartition
-    columns: Optional[ColumnPartition]
+    columns: ColumnPartition
     ctx: dict = Field(default_factory=dict)
 
     def extract_df(self, df: pd.DataFrame) -> pd.DataFrame:
-        if self.columns is not None:
+        if self.columns.headers is not None:
             df = df[self.columns.headers]
 
         return df.iloc[self.rows.start : self.rows.end]  # noqa
 
     def update_ctx(self, update: dict):
         self.ctx.update(update)
 
 
 @dataclass
 class PartitionConstraints:
-    max_row_count: Optional[int] = None
-    max_row_partitions: Optional[int] = None
+    max_row_count: int
     header_clusters: Optional[List[List[str]]] = None
     seed_headers: Optional[List[str]] = None
 
-    def __post_init__(self):
-        if self.max_row_count is not None and self.max_row_partitions is not None:
-            raise AttributeError("cannot use both max_row_count and max_row_partitions")
-
-        if self.max_row_count is None and self.max_row_partitions is None:
-            raise AttributeError("must use one of max_row_count or max_row_partitions")
-
     @property
     def header_cluster_count(self) -> int:
         if self.header_clusters is None:
             return 1
         return len(self.header_clusters)
 
 
@@ -67,19 +59,15 @@
 
     header_clusters = constraints.header_clusters
     if header_clusters is None:
         header_clusters = [list(df.columns)]
 
     partitions = []
     partition_idx = 0
-
-    if constraints.max_row_partitions is not None:
-        partition_count = constraints.max_row_partitions
-    elif constraints.max_row_count is not None:
-        partition_count = math.ceil(total_rows / constraints.max_row_count)
+    partition_count = math.ceil(total_rows / constraints.max_row_count)
 
     # We need to break up the number of rows into roughly even chunks
     chunk_size, remain = divmod(total_rows, partition_count)
 
     # each item in this array is the size of the chunk
     chunks = [chunk_size] * partition_count
 
@@ -106,30 +94,31 @@
         curr_start += chunk_size
 
     return partitions
 
 
 class PartitionStrategy(BaseModel):
     id: str
-    partitions: Optional[List[Partition]]
+    partitions: List[Partition]
     header_cluster_count: int
     original_headers: Optional[List[str]]
     status_counter: Optional[dict]
     _disk_location: Path = PrivateAttr(default=None)
 
     @classmethod
     def from_dataframe(
         cls, id: str, df: pd.DataFrame, constraints: PartitionConstraints
     ) -> PartitionStrategy:
         partitions = _build_partitions(df, constraints)
         return cls(
             id=id,
             partitions=partitions,
             header_cluster_count=constraints.header_cluster_count,
-            original_headers=list(df),
+            original_headers=list(df.columns),
+            status_counter=None,
         )
 
     @classmethod
     def from_disk(cls, src: Union[Path, str]) -> PartitionStrategy:
         location = Path(src)
         if not location.exists():
             raise ValueError("File does not exist")
@@ -142,15 +131,15 @@
 
     @property
     def partition_count(self) -> int:
         return len(self.partitions)
 
     @property
     def row_partition_count(self) -> int:
-        return len(self.partitions) / self.header_cluster_count
+        return math.ceil(len(self.partitions) / self.header_cluster_count)
 
     def save_to(self, dest: Union[Path, str], overwrite: bool = False):
         location = Path(dest)
         if location.suffix != ".json":
             raise ValueError("file must end in .json")
         if location.exists() and not overwrite:
             raise RuntimeError("destination already exists")
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer/trainer.py` & `gretel-trainer-0.8.0/src/gretel_trainer/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Main Trainer Module"""
 
+from __future__ import annotations
+
 import json
 import logging
 import os.path
 from pathlib import Path
 from typing import Optional
 
 import pandas as pd
-from gretel_client import configure_session
+from gretel_client.config import get_session_config, RunnerMode
 from gretel_client.projects import create_or_get_unique_project
 from gretel_synthetics.utils.header_clusters import cluster
 
 from gretel_trainer import runner, strategy
 from gretel_trainer.models import _BaseConfig, determine_best_model
 
 logger = logging.getLogger(__name__)
@@ -42,61 +44,77 @@
         model_type (_BaseConfig, optional): Options include GretelLSTM(), GretelACTGAN(). If unspecified, the best option will be chosen at train time based on the training dataset.
         cache_file (str, optional): Select a path to save or load the cache file. Default is `[project_name]-runner.json`.
         overwrite (bool, optional): Overwrite previous progress. Defaults to True.
     """
 
     def __init__(
         self,
-        project_name: str = "trainer",
-        model_type: _BaseConfig = None,
-        cache_file: str = None,
+        project_name: str = DEFAULT_PROJECT,
+        model_type: Optional[_BaseConfig] = None,
+        cache_file: Optional[str] = None,
         overwrite: bool = True,
     ):
-        configure_session(api_key="prompt", cache="yes", validate=True)
-
-        self.df = None
         self.dataset_path: Optional[Path] = None
         self.run = None
         self.project_name = project_name
         self.project = create_or_get_unique_project(name=project_name)
         self.overwrite = overwrite
+        cache_file = cache_file or f"{project_name}-runner.json"
         self.cache_file = self._get_cache_file(cache_file)
         self.model_type = model_type
 
         if self.overwrite:
             if self.model_type is None:
                 logger.debug("Deferring model configuration to optimize based on training data.")
             else:
                 logger.debug(json.dumps(self.model_type.config, indent=2))
 
     @classmethod
     def load(
         cls, cache_file: str = DEFAULT_CACHE, project_name: str = DEFAULT_PROJECT
-    ) -> runner.StrategyRunner:
+    ) -> Trainer:
         """Load an existing project from a cache.
 
         Args:
             cache_file (str, optional): Valid file path to load the cache file from. Defaults to `[project-name]-runner.json`
+            project_name (str, optional): Gretel project name. This should match the original project. Defaults to "trainer"
 
         Returns:
-            Trainer: returns an initialized StrategyRunner class.
+            Trainer: returns a Trainer instance with an initialized StrategyRunner class.
         """
-        project = create_or_get_unique_project(name=project_name)
-        model = cls(cache_file=cache_file, project_name=project_name, overwrite=False)
-
         if not os.path.exists(cache_file):
             raise ValueError(
                 f"Unable to find `{cache_file}`. Please specify a valid cache_file."
             )
 
-        model.run = model._initialize_run(df=None, overwrite=model.overwrite)
-        return model
+        project = create_or_get_unique_project(name=project_name)
+        trainer = cls(cache_file=cache_file, project_name=project_name, overwrite=False)
+
+        # Cache file does not store all the data needed to fully rehydrate a StrategyRunner, but
+        # 1) we don't need all the attributes to generate data from existing trained models, and
+        # 2) if we do want to train from scratch, Trainer#train will create a new StrategyRunner
+        #    with legitimate values for these attributes.
+        empty_df = pd.DataFrame()
+        empty_model_config = {}
+        empty_partition_constraints = strategy.PartitionConstraints(max_row_count=0)
+        trainer.run = runner.StrategyRunner(
+            df=empty_df,
+            model_config=empty_model_config,
+            partition_constraints=empty_partition_constraints,
+            strategy_id=_sanitize_name(trainer._get_strategy_id()),
+            cache_file=trainer.cache_file,
+            cache_overwrite=trainer.overwrite,
+            project=trainer.project,
+            hybrid=trainer._hybrid,
+        )
+
+        return trainer
 
     def train(
-        self, dataset_path: str, delimiter: str = ",", round_decimals: int = 4, seed_fields: list = None,
+        self, dataset_path: str, delimiter: str = ",", round_decimals: int = 4, seed_fields: Optional[list] = None,
     ):
         """Train a model on the dataset
 
         Args:
             dataset_path (str): Path or URL to CSV
             delimiter (str, optional): Delimiter to use when reading the dataset. Defaults to comma (",").
             round_decimals (int, optional): Round decimals in CSV as preprocessing step. Defaults to `4`.
@@ -108,49 +126,63 @@
         )
         self.run = self._initialize_run(
             df=self.df, overwrite=self.overwrite, seed_fields=seed_fields
         )
         self.run.train_all_partitions()
 
     def generate(
-        self, num_records: int = 500, seed_df: pd.DataFrame = None
+        self, num_records: int = 500, seed_df: Optional[pd.DataFrame] = None
     ) -> pd.DataFrame:
         """Generate synthetic data
 
         Args:
             num_records (int, optional): Number of records to generate from model. Defaults to 500.
             seed_df (pd.DataFrame, optional): Pandas DataFrame of values to seed the model with. Defaults to None.
 
         Returns:
             pd.DataFrame: Synthetic data.
         """
+        if self.run is None:
+            raise RuntimeError(
+                "Cannot generate data without training information. Train a model via `train` or try loading an existing project from cache via `load`."
+            )
+
         self.run.generate_data(
             num_records=num_records if seed_df is None else None,
             max_invalid=None,
             clear_cache=True,
             seed_df=seed_df,
         )
         return self.run.get_synthetic_data()
 
     def get_sqs_score(self) -> int:
         """Return the average SQS synthetic data quality score.
 
         Requires the model has been trained.
         """
+        if self.run is None:
+            raise RuntimeError(
+                "Cannot generate data without training information. Train a model via `train` or try loading an existing project from cache via `load`."
+            )
+
         scores = [
             sqs["synthetic_data_quality_score"]["score"]
             for sqs in self.run.get_sqs_information()
         ]
         return int(sum(scores) / len(scores))
 
+    @property
+    def _hybrid(self) -> bool:
+        return get_session_config().default_runner == RunnerMode.HYBRID
+
     def _preprocess_data(
-        self, dataset_path: Path, delimiter: str, round_decimals: int = 4
+        self, dataset_path: str, delimiter: str, round_decimals: int = 4
     ) -> pd.DataFrame:
         """Preprocess input data"""
-        tmp = pd.read_csv(str(dataset_path), sep=delimiter, low_memory=False)
+        tmp = pd.read_csv(dataset_path, sep=delimiter, low_memory=False)
         tmp = tmp.round(round_decimals)
         return tmp
 
     def _get_cache_file(self, cache_file: str) -> str:
         """Select a path to store the runtime cache to initialize a model"""
         if cache_file is None:
             cache_file = f"{self.project_name}-runner.json"
@@ -161,55 +193,52 @@
             else:
                 logger.info(f"Using existing run cache: {cache_file}.")
         else:
             logger.info(f"Creating new run cache: {cache_file}.")
         return cache_file
 
     def _initialize_run(
-        self, df: pd.DataFrame = None, overwrite: bool = True, seed_fields: list = None
+        self, df: pd.DataFrame, overwrite: bool, seed_fields: Optional[list]
     ) -> runner.StrategyRunner:
         """Create training jobs"""
-        constraints = None
-        model_config = None
-
-        if df is None:
-            df = pd.DataFrame()
-
-        if not df.empty:
-            if self.model_type is None:
-                self.model_type = determine_best_model(df)
-                logger.debug(json.dumps(self.model_type.config, indent=2))
-
-            model_config = self.model_type.config
-
-            header_clusters = cluster(
-                df,
-                maxsize=self.model_type.max_header_clusters,
-                header_prefix=seed_fields,
-                plot=False,
-            )
-            logger.info(
-                f"Header clustering created {len(header_clusters)} cluster(s) "
-                f"of length(s) {[len(x) for x in header_clusters]}"
-            )
+        if self.model_type is None:
+            self.model_type = determine_best_model(df)
+            logger.debug(json.dumps(self.model_type.config, indent=2))
+
+        model_config = self.model_type.config
+
+        header_clusters = cluster(
+            df,
+            maxsize=self.model_type.max_header_clusters,
+            header_prefix=seed_fields,
+            plot=False,
+        )
+        logger.info(
+            f"Header clustering created {len(header_clusters)} cluster(s) "
+            f"of length(s) {[len(x) for x in header_clusters]}"
+        )
 
-            constraints = strategy.PartitionConstraints(
-                header_clusters=header_clusters,
-                max_row_count=self.model_type.max_rows,
-                seed_headers=seed_fields,
-            )
+        constraints = strategy.PartitionConstraints(
+            header_clusters=header_clusters,
+            max_row_count=self.model_type.max_rows,
+            seed_headers=seed_fields,
+        )
 
-        if self.dataset_path is None:
-            strategy_id = f"{self.project_name}"
-        else:
-            strategy_id = f"{self.project_name}-{self.dataset_path.stem}"
+        strategy_id = self._get_strategy_id()
 
         run = runner.StrategyRunner(
             strategy_id=_sanitize_name(strategy_id),
             df=self.df,
             cache_file=self.cache_file,
             cache_overwrite=overwrite,
             model_config=model_config,
             partition_constraints=constraints,
             project=self.project,
+            hybrid=self._hybrid,
         )
         return run
+
+    def _get_strategy_id(self) -> str:
+        strategy_id = self.project_name
+        if self.dataset_path is not None:
+            strategy_id += f"-{self.dataset_path.stem}"
+        return strategy_id
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer.egg-info/PKG-INFO` & `gretel-trainer-0.8.0/src/gretel_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.7.0
+Version: 0.8.0
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.7.0/src/gretel_trainer.egg-info/SOURCES.txt` & `gretel-trainer-0.8.0/src/gretel_trainer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 src/gretel_trainer/relational/__init__.py
 src/gretel_trainer/relational/ancestry.py
 src/gretel_trainer/relational/artifacts.py
 src/gretel_trainer/relational/backup.py
 src/gretel_trainer/relational/connectors.py
 src/gretel_trainer/relational/core.py
 src/gretel_trainer/relational/drawing.py
+src/gretel_trainer/relational/log.py
 src/gretel_trainer/relational/model_config.py
 src/gretel_trainer/relational/multi_table.py
 src/gretel_trainer/relational/sdk_extras.py
 src/gretel_trainer/relational/task_runner.py
 src/gretel_trainer/relational/workflow_state.py
 src/gretel_trainer/relational/report/figures.py
 src/gretel_trainer/relational/report/key_highlight.js
```

### Comparing `gretel-trainer-0.7.0/tests/data/core-221-train.csv` & `gretel-trainer-0.8.0/tests/data/core-221-train.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/mocks.py` & `gretel-trainer-0.8.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/conftest.py` & `gretel-trainer-0.8.0/tests/relational/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 import pandas as pd
 import pytest
 from sqlalchemy import create_engine
 
 from gretel_trainer.relational.connectors import Connector
 from gretel_trainer.relational.core import RelationalData
+from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 
 EXAMPLE_DBS = Path(__file__).parent.resolve() / "example_dbs"
 
 
-@pytest.fixture(autouse=True)
-def patch_configure_session():
-    with patch("gretel_trainer.relational.multi_table.configure_session"):
-        yield
+@pytest.fixture()
+def extended_sdk():
+    return ExtendedGretelSDK(hybrid=False)
 
 
 @pytest.fixture()
 def project():
     with patch(
         "gretel_trainer.relational.multi_table.create_project"
     ) as create_project, patch(
```

### Comparing `gretel-trainer-0.7.0/tests/relational/example_dbs/art.sql` & `gretel-trainer-0.8.0/tests/relational/example_dbs/art.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/example_dbs/ecom.sql` & `gretel-trainer-0.8.0/tests/relational/example_dbs/ecom.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/example_dbs/mutagenesis.sql` & `gretel-trainer-0.8.0/tests/relational/example_dbs/mutagenesis.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/example_dbs/pets.sql` & `gretel-trainer-0.8.0/tests/relational/example_dbs/pets.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/test_ancestral_strategy.py` & `gretel-trainer-0.8.0/tests/relational/test_ancestral_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,17 @@
         }
     )
 
     pdtest.assert_frame_equal(expected_events, processed_tables["events"])
     pdtest.assert_frame_equal(expected_users, processed_tables["users"])
 
 
-def test_uses_trained_model_to_update_cross_table_scores(report_json_dict):
+def test_uses_trained_model_to_update_cross_table_scores(
+    report_json_dict, extended_sdk
+):
     strategy = AncestralStrategy()
     evaluations = {
         "table_1": TableEvaluation(),
         "table_2": TableEvaluation(),
     }
     model = Mock()
 
@@ -508,28 +510,28 @@
         working_dir = Path(working_dir)
         with open(
             working_dir / "synthetics_cross_table_evaluation_table_1.json", "w"
         ) as f:
             f.write(json.dumps(report_json_dict))
 
         strategy.update_evaluation_from_model(
-            "table_1", evaluations, model, working_dir
+            "table_1", evaluations, model, working_dir, extended_sdk
         )
 
     evaluation = evaluations["table_1"]
 
     assert evaluation.cross_table_sqs == 95
     assert evaluation.cross_table_report_json == report_json_dict
 
     assert evaluation.individual_sqs is None
     assert evaluation.individual_report_json is None
 
 
 def test_falls_back_to_fetching_report_json_when_download_artifacts_fails(
-    report_json_dict,
+    report_json_dict, extended_sdk
 ):
     strategy = AncestralStrategy()
     evaluations = {
         "table_1": TableEvaluation(),
         "table_2": TableEvaluation(),
     }
     model = Mock()
@@ -540,15 +542,15 @@
         "gretel_trainer.relational.strategies.ancestral.common._get_report_json"
     ) as get_json:
         working_dir = Path(working_dir)
         download_artifacts.return_value = None
         get_json.return_value = report_json_dict
 
         strategy.update_evaluation_from_model(
-            "table_1", evaluations, model, working_dir
+            "table_1", evaluations, model, working_dir, extended_sdk
         )
 
     evaluation = evaluations["table_1"]
 
     assert evaluation.cross_table_sqs == 95
     assert evaluation.cross_table_report_json == report_json_dict
```

### Comparing `gretel-trainer-0.7.0/tests/relational/test_ancestry.py` & `gretel-trainer-0.8.0/tests/relational/test_ancestry.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/test_backup.py` & `gretel-trainer-0.8.0/tests/relational/test_backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             "customer": "555444666",
             "address": "333111222",
         },
     )
     artifact_collection = ArtifactCollection(
         gretel_debug_summary="gretel_abc__gretel_debug_summary.json",
         source_archive="gretel_abc_source_tables.tar.gz",
+        hybrid=False,
     )
     backup = Backup(
         project_name="my-project",
         strategy="independent",
         gretel_model="amplify",
         working_dir="workdir",
         refresh_interval=120,
```

### Comparing `gretel-trainer-0.7.0/tests/relational/test_connectors.py` & `gretel-trainer-0.8.0/tests/relational/test_connectors.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/test_independent_strategy.py` & `gretel-trainer-0.8.0/tests/relational/test_independent_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         fk_value_counts[fk_value] = fk_value_counts[fk_value] + 1
 
     fk_value_counts = sorted(list(fk_value_counts.values()))
 
     assert fk_value_counts == [5, 5, 15, 30, 35, 60]
 
 
-def test_uses_trained_model_to_update_individual_scores(report_json_dict):
+def test_uses_trained_model_to_update_individual_scores(report_json_dict, extended_sdk):
     strategy = IndependentStrategy()
     evaluations = {
         "table_1": TableEvaluation(),
         "table_2": TableEvaluation(),
     }
     model = Mock()
 
@@ -196,28 +196,28 @@
         working_dir = Path(working_dir)
         with open(
             working_dir / "synthetics_individual_evaluation_table_1.json", "w"
         ) as f:
             f.write(json.dumps(report_json_dict))
 
         strategy.update_evaluation_from_model(
-            "table_1", evaluations, model, working_dir
+            "table_1", evaluations, model, working_dir, extended_sdk
         )
 
     evaluation = evaluations["table_1"]
 
     assert evaluation.individual_sqs == 95
     assert evaluation.individual_report_json == report_json_dict
 
     assert evaluation.cross_table_sqs is None
     assert evaluation.cross_table_report_json is None
 
 
 def test_falls_back_to_fetching_report_json_when_download_artifacts_fails(
-    report_json_dict,
+    report_json_dict, extended_sdk
 ):
     strategy = IndependentStrategy()
     evaluations = {
         "table_1": TableEvaluation(),
         "table_2": TableEvaluation(),
     }
     model = Mock()
@@ -228,15 +228,15 @@
         "gretel_trainer.relational.strategies.independent.common._get_report_json"
     ) as get_json:
         working_dir = Path(working_dir)
         download_artifacts.return_value = None
         get_json.return_value = report_json_dict
 
         strategy.update_evaluation_from_model(
-            "table_1", evaluations, model, working_dir
+            "table_1", evaluations, model, working_dir, extended_sdk
         )
 
     evaluation = evaluations["table_1"]
 
     assert evaluation.individual_sqs == 95
     assert evaluation.individual_report_json == report_json_dict
```

### Comparing `gretel-trainer-0.7.0/tests/relational/test_model_config.py` & `gretel-trainer-0.8.0/tests/relational/test_model_config.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/test_multi_table_config_options.py` & `gretel-trainer-0.8.0/tests/relational/test_multi_table_config_options.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/test_multi_table_restore.py` & `gretel-trainer-0.8.0/tests/relational/test_multi_table_restore.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     training_archive_present: bool = False,
     output_archive_present: bool = False,
     transforms_models: Dict[str, Mock] = {},
 ) -> str:
     artifact_collection = ArtifactCollection(
         gretel_debug_summary=ARTIFACTS["debug_summary"]["artifact_id"],
         source_archive=ARTIFACTS["source_archive"]["artifact_id"],
+        hybrid=False,
     )
     if training_archive_present:
         artifact_collection.synthetics_training_archive = ARTIFACTS[
             "synthetics_training_archive"
         ]["artifact_id"]
     if output_archive_present:
         artifact_collection.synthetics_outputs_archive = ARTIFACTS[
@@ -313,394 +314,434 @@
     project.get_model = make_mock_get_model(models)
     download_tar_artifact.side_effect = make_mock_download_tar_artifact(
         setup_path,
         working_path,
     )
 
 
-def test_restore_not_yet_trained(project, pets):
-    with tempfile.TemporaryDirectory() as working_dir, tempfile.TemporaryDirectory() as testsetup_dir, patch(
-        "gretel_trainer.relational.multi_table.download_tar_artifact"
+@pytest.fixture(autouse=True)
+def download_tar_artifact():
+    with patch(
+        "gretel_trainer.relational.sdk_extras.ExtendedGretelSDK.download_tar_artifact"
     ) as download_tar_artifact:
-        working_dir = Path(working_dir)
-        testsetup_dir = Path(testsetup_dir)
+        yield download_tar_artifact
 
-        create_standin_project_artifacts(pets, testsetup_dir)
-        configure_mocks(project, download_tar_artifact, testsetup_dir, working_dir)
-        backup_file = create_backup(pets, working_dir)
 
-        # Restore a MultiTable instance, starting with only the backup file present in working_dir
-        assert os.listdir(working_dir) == ["_gretel_backup.json"]
-        mt = MultiTable.restore(backup_file)
+@pytest.fixture(autouse=True)
+def working_dir():
+    with tempfile.TemporaryDirectory() as working_dir:
+        yield Path(working_dir)
+
+
+@pytest.fixture(autouse=True)
+def testsetup_dir():
+    with tempfile.TemporaryDirectory() as testsetup_dir:
+        yield Path(testsetup_dir)
+
+
+def test_restore_not_yet_trained(
+    project, pets, download_tar_artifact, working_dir, testsetup_dir
+):
+    create_standin_project_artifacts(pets, testsetup_dir)
+    configure_mocks(project, download_tar_artifact, testsetup_dir, working_dir)
+    backup_file = create_backup(pets, working_dir)
+
+    # Restore a MultiTable instance, starting with only the backup file present in working_dir
+    assert os.listdir(working_dir) == ["_gretel_backup.json"]
+    mt = MultiTable.restore(backup_file)
+
+    # Backup + Debug summary + Source archive + (2) Source CSVs
+    assert len(os.listdir(working_dir)) == 5
+
+    # Debug summary is restored
+    assert os.path.exists(local_file(working_dir, "debug_summary"))
+    with open(local_file(working_dir, "debug_summary"), "r") as dbg:
+        assert json.load(dbg) == DEBUG_SUMMARY_CONTENT
+
+    # RelationalData is restored
+    assert os.path.exists(working_dir / "source_humans.csv")
+    assert os.path.exists(working_dir / "source_pets.csv")
+    assert mt.relational_data.debug_summary() == pets.debug_summary()
+
+
+def test_restore_transforms(
+    project, pets, download_tar_artifact, working_dir, testsetup_dir
+):
+    transforms_models = {
+        "humans": make_mock_model(
+            name="humans",
+            status="completed",
+            setup_path=testsetup_dir,
+        ),
+        "pets": make_mock_model(
+            name="pets",
+            status="completed",
+            setup_path=testsetup_dir,
+        ),
+    }
+
+    create_standin_project_artifacts(pets, testsetup_dir)
+    configure_mocks(
+        project,
+        download_tar_artifact,
+        testsetup_dir,
+        working_dir,
+        transforms_models,
+    )
+    backup_file = create_backup(pets, working_dir, transforms_models=transforms_models)
 
-        # Backup + Debug summary + Source archive + (2) Source CSVs
-        assert len(os.listdir(working_dir)) == 5
+    mt = MultiTable.restore(backup_file)
 
-        # Debug summary is restored
-        assert os.path.exists(local_file(working_dir, "debug_summary"))
-        with open(local_file(working_dir, "debug_summary"), "r") as dbg:
-            assert json.load(dbg) == DEBUG_SUMMARY_CONTENT
-
-        # RelationalData is restored
-        assert os.path.exists(working_dir / "source_humans.csv")
-        assert os.path.exists(working_dir / "source_pets.csv")
-        assert mt.relational_data.debug_summary() == pets.debug_summary()
-
-
-def test_restore_transforms(project, pets):
-    with tempfile.TemporaryDirectory() as working_dir, tempfile.TemporaryDirectory() as testsetup_dir, patch(
-        "gretel_trainer.relational.multi_table.download_tar_artifact"
-    ) as download_tar_artifact:
-        working_dir = Path(working_dir)
-        testsetup_dir = Path(testsetup_dir)
+    # Backup + Debug summary + Source archive + (2) Source CSVs
+    assert len(os.listdir(working_dir)) == 5
 
-        transforms_models = {
-            "humans": make_mock_model(
-                name="humans",
-                status="completed",
-                setup_path=testsetup_dir,
-            ),
-            "pets": make_mock_model(
-                name="pets",
-                status="completed",
-                setup_path=testsetup_dir,
-            ),
-        }
-
-        create_standin_project_artifacts(pets, testsetup_dir)
-        configure_mocks(
-            project,
-            download_tar_artifact,
-            testsetup_dir,
-            working_dir,
-            transforms_models,
-        )
-        backup_file = create_backup(
-            pets, working_dir, transforms_models=transforms_models
-        )
+    # Transforms state is restored
+    assert len(mt._transforms_train.models) == 2
+    assert len(mt._transforms_train.lost_contact) == 0
+
+
+def test_restore_synthetics_training_still_in_progress(
+    project, pets, download_tar_artifact, working_dir, testsetup_dir
+):
+    synthetics_models = {
+        "humans": make_mock_model(
+            name="humans",
+            status="active",
+            setup_path=testsetup_dir,
+        ),
+        "pets": make_mock_model(
+            name="pets",
+            status="pending",
+            setup_path=testsetup_dir,
+        ),
+    }
+
+    create_standin_project_artifacts(pets, testsetup_dir)
+    configure_mocks(
+        project,
+        download_tar_artifact,
+        testsetup_dir,
+        working_dir,
+        synthetics_models,
+    )
+    backup_file = create_backup(pets, working_dir, synthetics_models=synthetics_models)
 
+    with pytest.raises(MultiTableException):
         mt = MultiTable.restore(backup_file)
 
-        # Backup + Debug summary + Source archive + (2) Source CSVs
-        assert len(os.listdir(working_dir)) == 5
-
-        # Transforms state is restored
-        assert len(mt._transforms_train.models) == 2
-        assert len(mt._transforms_train.lost_contact) == 0
 
+def test_restore_training_complete(
+    project, pets, report_json_dict, download_tar_artifact, working_dir, testsetup_dir
+):
+    synthetics_models = {
+        "humans": make_mock_model(
+            name="humans",
+            status="completed",
+            setup_path=testsetup_dir,
+            report_json=report_json_dict,
+        ),
+        "pets": make_mock_model(
+            name="pets",
+            status="completed",
+            setup_path=testsetup_dir,
+            report_json=report_json_dict,
+        ),
+    }
+
+    create_standin_project_artifacts(pets, testsetup_dir)
+    configure_mocks(
+        project,
+        download_tar_artifact,
+        testsetup_dir,
+        working_dir,
+        synthetics_models,
+    )
+    backup_file = create_backup(
+        pets,
+        working_dir,
+        synthetics_models=synthetics_models,
+        training_archive_present=True,
+    )
 
-def test_restore_synthetics_training_still_in_progress(project, pets):
-    with tempfile.TemporaryDirectory() as working_dir, tempfile.TemporaryDirectory() as testsetup_dir, patch(
-        "gretel_trainer.relational.multi_table.download_tar_artifact"
-    ) as download_tar_artifact:
-        working_dir = Path(working_dir)
-        testsetup_dir = Path(testsetup_dir)
+    mt = MultiTable.restore(backup_file)
 
-        synthetics_models = {
-            "humans": make_mock_model(
-                name="humans",
-                status="active",
-                setup_path=testsetup_dir,
-            ),
-            "pets": make_mock_model(
-                name="pets",
-                status="pending",
-                setup_path=testsetup_dir,
-            ),
-        }
-
-        create_standin_project_artifacts(pets, testsetup_dir)
-        configure_mocks(
-            project,
-            download_tar_artifact,
-            testsetup_dir,
-            working_dir,
-            synthetics_models,
-        )
-        backup_file = create_backup(
-            pets, working_dir, synthetics_models=synthetics_models
-        )
-
-        with pytest.raises(MultiTableException):
-            mt = MultiTable.restore(backup_file)
-
-
-def test_restore_training_complete(project, pets, report_json_dict):
-    with tempfile.TemporaryDirectory() as working_dir, tempfile.TemporaryDirectory() as testsetup_dir, patch(
-        "gretel_trainer.relational.multi_table.download_tar_artifact"
-    ) as download_tar_artifact:
-        working_dir = Path(working_dir)
-        testsetup_dir = Path(testsetup_dir)
+    # Backup + Debug summary + Source archive + (2) Source CSVs
+    # + Training archive + (2) Train CSVs + (4) Reports from models
+    assert len(os.listdir(working_dir)) == 12
+
+    # Training state is restored
+    assert os.path.exists(local_file(working_dir, "synthetics_training_archive"))
+    assert os.path.exists(local_file(working_dir, "train_humans"))
+    assert os.path.exists(working_dir / "synthetics_individual_evaluation_humans.json")
+    assert os.path.exists(working_dir / "synthetics_individual_evaluation_humans.html")
+    assert os.path.exists(local_file(working_dir, "train_pets"))
+    assert os.path.exists(working_dir / "synthetics_individual_evaluation_pets.json")
+    assert os.path.exists(working_dir / "synthetics_individual_evaluation_pets.html")
+    assert len(mt._synthetics_train.models) == 2
+
+    assert mt.evaluations["humans"].individual_sqs == 95
+    assert mt.evaluations["humans"].cross_table_sqs is None
+    assert mt.evaluations["pets"].individual_sqs == 95
+    assert mt.evaluations["pets"].cross_table_sqs is None
+
+
+def test_restore_training_one_failed(
+    project, pets, report_json_dict, download_tar_artifact, working_dir, testsetup_dir
+):
+    synthetics_models = {
+        "humans": make_mock_model(
+            name="humans",
+            status="error",
+            setup_path=testsetup_dir,
+        ),
+        "pets": make_mock_model(
+            name="pets",
+            status="completed",
+            setup_path=testsetup_dir,
+            report_json=report_json_dict,
+        ),
+    }
+
+    create_standin_project_artifacts(pets, testsetup_dir)
+    configure_mocks(
+        project,
+        download_tar_artifact,
+        testsetup_dir,
+        working_dir,
+        synthetics_models,
+    )
+    backup_file = create_backup(
+        pets,
+        working_dir,
+        synthetics_models=synthetics_models,
+        training_archive_present=True,
+    )
 
-        synthetics_models = {
-            "humans": make_mock_model(
-                name="humans",
-                status="completed",
-                setup_path=testsetup_dir,
-                report_json=report_json_dict,
-            ),
-            "pets": make_mock_model(
-                name="pets",
-                status="completed",
-                setup_path=testsetup_dir,
-                report_json=report_json_dict,
-            ),
-        }
-
-        create_standin_project_artifacts(pets, testsetup_dir)
-        configure_mocks(
-            project,
-            download_tar_artifact,
-            testsetup_dir,
-            working_dir,
-            synthetics_models,
-        )
-        backup_file = create_backup(
-            pets,
-            working_dir,
-            synthetics_models=synthetics_models,
-            training_archive_present=True,
-        )
+    mt = MultiTable.restore(backup_file)
 
-        mt = MultiTable.restore(backup_file)
+    # Backup + Debug summary + Source archive + (2) Source CSVs
+    # Training archive + (2) Train CSVs + (2) Reports from model
+    assert len(os.listdir(working_dir)) == 10
+
+    # Training state is restored
+    assert os.path.exists(local_file(working_dir, "synthetics_training_archive"))
+    ## We do expect the training CSV to be present, extracted from the training archive...
+    assert os.path.exists(local_file(working_dir, "train_humans"))
+    ## ...but we should not see evaluation reports because the table failed to train.
 
-        # Backup + Debug summary + Source archive + (2) Source CSVs
-        # + Training archive + (2) Train CSVs + (4) Reports from models
-        assert len(os.listdir(working_dir)) == 12
-
-        # Training state is restored
-        assert os.path.exists(local_file(working_dir, "synthetics_training_archive"))
-        assert os.path.exists(local_file(working_dir, "train_humans"))
-        assert os.path.exists(
-            working_dir / "synthetics_individual_evaluation_humans.json"
-        )
-        assert os.path.exists(
-            working_dir / "synthetics_individual_evaluation_humans.html"
-        )
-        assert os.path.exists(local_file(working_dir, "train_pets"))
-        assert os.path.exists(
-            working_dir / "synthetics_individual_evaluation_pets.json"
-        )
-        assert os.path.exists(
-            working_dir / "synthetics_individual_evaluation_pets.html"
-        )
-        assert len(mt._synthetics_train.models) == 2
-
-        # FIXME have {'humans': TableEvaluation(), 'pets': TableEvaluation()} here
-        assert mt.evaluations["humans"].individual_sqs == 95
-        assert mt.evaluations["humans"].cross_table_sqs is None
-        assert mt.evaluations["pets"].individual_sqs == 95
-        assert mt.evaluations["pets"].cross_table_sqs is None
-
-
-def test_restore_training_one_failed(project, pets, report_json_dict):
-    with tempfile.TemporaryDirectory() as working_dir, tempfile.TemporaryDirectory() as testsetup_dir, patch(
-        "gretel_trainer.relational.multi_table.download_tar_artifact"
-    ) as download_tar_artifact:
-        working_dir = Path(working_dir)
-        testsetup_dir = Path(testsetup_dir)
+    assert not os.path.exists(
+        working_dir / "synthetics_individual_evaluation_humans.json"
+    )
+    assert not os.path.exists(
+        working_dir / "synthetics_individual_evaluation_humans.html"
+    )
 
-        synthetics_models = {
-            "humans": make_mock_model(
-                name="humans",
-                status="error",
-                setup_path=testsetup_dir,
-            ),
-            "pets": make_mock_model(
-                name="pets",
-                status="completed",
-                setup_path=testsetup_dir,
-                report_json=report_json_dict,
-            ),
-        }
-
-        create_standin_project_artifacts(pets, testsetup_dir)
-        configure_mocks(
-            project,
-            download_tar_artifact,
-            testsetup_dir,
-            working_dir,
-            synthetics_models,
-        )
-        backup_file = create_backup(
-            pets,
-            working_dir,
-            synthetics_models=synthetics_models,
-            training_archive_present=True,
-        )
+    assert os.path.exists(local_file(working_dir, "train_pets"))
+    assert os.path.exists(working_dir / "synthetics_individual_evaluation_pets.json")
+    assert os.path.exists(working_dir / "synthetics_individual_evaluation_pets.html")
+    assert len(mt._synthetics_train.models) == 2
+
+    assert mt.evaluations["humans"].individual_sqs is None
+    assert mt.evaluations["humans"].cross_table_sqs is None
+    assert mt.evaluations["pets"].individual_sqs == 95
+    assert mt.evaluations["pets"].cross_table_sqs is None
+
+
+def test_restore_generate_completed(
+    project, pets, report_json_dict, download_tar_artifact, working_dir, testsetup_dir
+):
+    synthetics_record_handlers = {
+        "humans": make_mock_record_handler(name="humans", status="completed"),
+        "pets": make_mock_record_handler(name="pets", status="completed"),
+    }
+
+    synthetics_models = {
+        "humans": make_mock_model(
+            name="humans",
+            status="completed",
+            setup_path=testsetup_dir,
+            record_handler=synthetics_record_handlers["humans"],
+            report_json=report_json_dict,
+        ),
+        "pets": make_mock_model(
+            name="pets",
+            status="completed",
+            setup_path=testsetup_dir,
+            record_handler=synthetics_record_handlers["pets"],
+            report_json=report_json_dict,
+        ),
+    }
+
+    create_standin_project_artifacts(pets, testsetup_dir)
+    configure_mocks(
+        project,
+        download_tar_artifact,
+        testsetup_dir,
+        working_dir,
+        synthetics_models,
+    )
+    backup_file = create_backup(
+        pets,
+        working_dir,
+        synthetics_models=synthetics_models,
+        synthetics_record_handlers=synthetics_record_handlers,
+        training_archive_present=True,
+        output_archive_present=True,
+    )
 
-        mt = MultiTable.restore(backup_file)
+    mt = MultiTable.restore(backup_file)
 
-        # Backup + Debug summary + Source archive + (2) Source CSVs
-        # Training archive + (2) Train CSVs + (2) Reports from model
-        assert len(os.listdir(working_dir)) == 10
-
-        # Training state is restored
-        assert os.path.exists(local_file(working_dir, "synthetics_training_archive"))
-        ## We do expect the training CSV to be present, extracted from the training archive...
-        assert os.path.exists(local_file(working_dir, "train_humans"))
-        ## ...but we should not see evaluation reports because the table failed to train.
-
-        assert not os.path.exists(
-            working_dir / "synthetics_individual_evaluation_humans.json"
-        )
-        assert not os.path.exists(
-            working_dir / "synthetics_individual_evaluation_humans.html"
-        )
-
-        assert os.path.exists(local_file(working_dir, "train_pets"))
-        assert os.path.exists(
-            working_dir / "synthetics_individual_evaluation_pets.json"
-        )
-        assert os.path.exists(
-            working_dir / "synthetics_individual_evaluation_pets.html"
-        )
-        assert len(mt._synthetics_train.models) == 2
-
-        assert mt.evaluations["humans"].individual_sqs is None
-        assert mt.evaluations["humans"].cross_table_sqs is None
-        assert mt.evaluations["pets"].individual_sqs == 95
-        assert mt.evaluations["pets"].cross_table_sqs is None
-
-
-def test_restore_generate_completed(project, pets, report_json_dict):
-    with tempfile.TemporaryDirectory() as working_dir, tempfile.TemporaryDirectory() as testsetup_dir, patch(
-        "gretel_trainer.relational.multi_table.download_tar_artifact"
-    ) as download_tar_artifact:
-        working_dir = Path(working_dir)
-        testsetup_dir = Path(testsetup_dir)
+    # Backup + Debug summary + Source archive + (2) Source CSVs
+    # + Training archive + (2) Train CSVs + (4) Reports from models
+    # + Outputs archive + Previous run subdirectory
+    assert len(os.listdir(working_dir)) == 14
+
+    # Generate state is restored
+    assert os.path.exists(working_dir / "run-id" / "synth_humans.csv")
+    assert os.path.exists(
+        working_dir / "run-id" / "synthetics_cross_table_evaluation_humans.json"
+    )
+    assert os.path.exists(
+        working_dir / "run-id" / "synthetics_cross_table_evaluation_humans.html"
+    )
+    assert os.path.exists(working_dir / "run-id" / "synth_pets.csv")
+    assert os.path.exists(
+        working_dir / "run-id" / "synthetics_cross_table_evaluation_pets.json"
+    )
+    assert os.path.exists(
+        working_dir / "run-id" / "synthetics_cross_table_evaluation_pets.html"
+    )
+    assert mt._synthetics_run is not None
+    assert len(mt.synthetic_output_tables) == 2
+    assert mt.evaluations["humans"].individual_sqs == 95
+    assert mt.evaluations["humans"].cross_table_sqs == 95
+    assert mt.evaluations["pets"].individual_sqs == 95
+    assert mt.evaluations["pets"].cross_table_sqs == 95
+
+
+def test_restore_generate_in_progress(
+    project, pets, report_json_dict, download_tar_artifact, working_dir, testsetup_dir
+):
+    synthetics_record_handlers = {
+        "humans": make_mock_record_handler(name="humans", status="completed"),
+        "pets": make_mock_record_handler(name="pets", status="completed"),
+    }
+
+    synthetics_models = {
+        "humans": make_mock_model(
+            name="humans",
+            status="completed",
+            setup_path=testsetup_dir,
+            record_handler=synthetics_record_handlers["humans"],
+            report_json=report_json_dict,
+        ),
+        "pets": make_mock_model(
+            name="pets",
+            status="completed",
+            setup_path=testsetup_dir,
+            record_handler=synthetics_record_handlers["pets"],
+            report_json=report_json_dict,
+        ),
+    }
+
+    create_standin_project_artifacts(pets, testsetup_dir)
+    configure_mocks(
+        project,
+        download_tar_artifact,
+        testsetup_dir,
+        working_dir,
+        synthetics_models,
+    )
+    backup_file = create_backup(
+        pets,
+        working_dir,
+        synthetics_models=synthetics_models,
+        synthetics_record_handlers=synthetics_record_handlers,
+        training_archive_present=True,
+        output_archive_present=False,
+    )
 
-        synthetics_record_handlers = {
-            "humans": make_mock_record_handler(name="humans", status="completed"),
-            "pets": make_mock_record_handler(name="pets", status="completed"),
-        }
-
-        synthetics_models = {
-            "humans": make_mock_model(
-                name="humans",
-                status="completed",
-                setup_path=testsetup_dir,
-                record_handler=synthetics_record_handlers["humans"],
-                report_json=report_json_dict,
-            ),
-            "pets": make_mock_model(
-                name="pets",
-                status="completed",
-                setup_path=testsetup_dir,
-                record_handler=synthetics_record_handlers["pets"],
-                report_json=report_json_dict,
-            ),
-        }
-
-        create_standin_project_artifacts(pets, testsetup_dir)
-        configure_mocks(
-            project,
-            download_tar_artifact,
-            testsetup_dir,
-            working_dir,
-            synthetics_models,
-        )
-        backup_file = create_backup(
-            pets,
-            working_dir,
-            synthetics_models=synthetics_models,
-            synthetics_record_handlers=synthetics_record_handlers,
-            training_archive_present=True,
-            output_archive_present=True,
-        )
+    mt = MultiTable.restore(backup_file)
 
-        mt = MultiTable.restore(backup_file)
+    # Backup + Debug summary + Source archive + (2) Source CSVs
+    # + Training archive + (2) Train CSVs + (4) Reports from models
+    assert len(os.listdir(working_dir)) == 12
+
+    # Generate state is partially restored
+    assert mt._synthetics_run == SyntheticsRun(
+        identifier="run-id",
+        preserved=[],
+        record_size_ratio=1.0,
+        lost_contact=[],
+        missing_model=[],
+        record_handlers=synthetics_record_handlers,
+    )
+    assert len(mt.synthetic_output_tables) == 0
+    assert mt.evaluations["humans"].individual_sqs == 95
+    assert mt.evaluations["humans"].cross_table_sqs is None
+    assert mt.evaluations["pets"].individual_sqs == 95
+    assert mt.evaluations["pets"].cross_table_sqs is None
+
+
+def test_restore_hybrid_run(project, pets, report_json_dict, working_dir):
+    # In hybrid contexts, the ArtifactCollection does not track or upload anything to the project.
+    # We are entirely reliant upon the local directory for those artifacts.
+    # For testing, this means we set up everything in the working directory already.
+
+    synthetics_record_handlers = {
+        "humans": make_mock_record_handler(name="humans", status="completed"),
+        "pets": make_mock_record_handler(name="pets", status="completed"),
+    }
+
+    synthetics_models = {
+        "humans": make_mock_model(
+            name="humans",
+            status="completed",
+            setup_path=working_dir,
+            record_handler=synthetics_record_handlers["humans"],
+            report_json=report_json_dict,
+        ),
+        "pets": make_mock_model(
+            name="pets",
+            status="completed",
+            setup_path=working_dir,
+            record_handler=synthetics_record_handlers["pets"],
+            report_json=report_json_dict,
+        ),
+    }
+
+    create_standin_project_artifacts(pets, working_dir)
+    download_tar_artifact = Mock()
+    configure_mocks(
+        project,
+        download_tar_artifact,
+        working_dir,
+        working_dir,
+        synthetics_models,
+    )
 
-        # Backup + Debug summary + Source archive + (2) Source CSVs
-        # + Training archive + (2) Train CSVs + (4) Reports from models
-        # + Outputs archive + Previous run subdirectory
-        assert len(os.listdir(working_dir)) == 14
-
-        # Generate state is restored
-        assert os.path.exists(working_dir / "run-id" / "synth_humans.csv")
-        assert os.path.exists(
-            working_dir / "run-id" / "synthetics_cross_table_evaluation_humans.json"
-        )
-        assert os.path.exists(
-            working_dir / "run-id" / "synthetics_cross_table_evaluation_humans.html"
-        )
-        assert os.path.exists(working_dir / "run-id" / "synth_pets.csv")
-        assert os.path.exists(
-            working_dir / "run-id" / "synthetics_cross_table_evaluation_pets.json"
-        )
-        assert os.path.exists(
-            working_dir / "run-id" / "synthetics_cross_table_evaluation_pets.html"
-        )
-        assert mt._synthetics_run is not None
-        assert len(mt.synthetic_output_tables) == 2
-        assert mt.evaluations["humans"].individual_sqs == 95
-        assert mt.evaluations["humans"].cross_table_sqs == 95
-        assert mt.evaluations["pets"].individual_sqs == 95
-        assert mt.evaluations["pets"].cross_table_sqs == 95
-
-
-def test_restore_generate_in_progress(project, pets, report_json_dict):
-    with tempfile.TemporaryDirectory() as working_dir, tempfile.TemporaryDirectory() as testsetup_dir, patch(
-        "gretel_trainer.relational.multi_table.download_tar_artifact"
-    ) as download_tar_artifact:
-        working_dir = Path(working_dir)
-        testsetup_dir = Path(testsetup_dir)
+    backup_object = make_backup(
+        rel_data=pets,
+        working_dir=working_dir,
+        artifact_collection=ArtifactCollection(hybrid=True),
+        transforms_models={},
+        synthetics_models=synthetics_models,
+        synthetics_record_handlers=synthetics_record_handlers,
+    )
+    backup_file = write_backup(backup_object, working_dir)
 
-        synthetics_record_handlers = {
-            "humans": make_mock_record_handler(name="humans", status="completed"),
-            "pets": make_mock_record_handler(name="pets", status="completed"),
-        }
-
-        synthetics_models = {
-            "humans": make_mock_model(
-                name="humans",
-                status="completed",
-                setup_path=testsetup_dir,
-                record_handler=synthetics_record_handlers["humans"],
-                report_json=report_json_dict,
-            ),
-            "pets": make_mock_model(
-                name="pets",
-                status="completed",
-                setup_path=testsetup_dir,
-                record_handler=synthetics_record_handlers["pets"],
-                report_json=report_json_dict,
-            ),
-        }
-
-        create_standin_project_artifacts(pets, testsetup_dir)
-        configure_mocks(
-            project,
-            download_tar_artifact,
-            testsetup_dir,
-            working_dir,
-            synthetics_models,
-        )
-        backup_file = create_backup(
-            pets,
-            working_dir,
-            synthetics_models=synthetics_models,
-            synthetics_record_handlers=synthetics_record_handlers,
-            training_archive_present=True,
-            output_archive_present=False,
-        )
+    mt = MultiTable.restore(backup_file)
 
-        mt = MultiTable.restore(backup_file)
+    # No need to assert artifacts are present in working_dir because we set it up that way
+    # and hybrid restore would not work otherwise.
 
-        # Backup + Debug summary + Source archive + (2) Source CSVs
-        # + Training archive + (2) Train CSVs + (4) Reports from models
-        assert len(os.listdir(working_dir)) == 12
-
-        # Generate state is partially restored
-        assert mt._synthetics_run == SyntheticsRun(
-            identifier="run-id",
-            preserved=[],
-            record_size_ratio=1.0,
-            lost_contact=[],
-            missing_model=[],
-            record_handlers=synthetics_record_handlers,
-        )
-        assert len(mt.synthetic_output_tables) == 0
-        assert mt.evaluations["humans"].individual_sqs == 95
-        assert mt.evaluations["humans"].cross_table_sqs is None
-        assert mt.evaluations["pets"].individual_sqs == 95
-        assert mt.evaluations["pets"].cross_table_sqs is None
+    assert len(mt._synthetics_train.models) == 2
+    assert mt._synthetics_run is not None
+    assert len(mt.synthetic_output_tables) == 2
+    assert mt.evaluations["humans"].individual_sqs == 95
+    assert mt.evaluations["humans"].cross_table_sqs == 95
+    assert mt.evaluations["pets"].individual_sqs == 95
+    assert mt.evaluations["pets"].cross_table_sqs == 95
+
+    # The ArtifactCollection will not have uploaded any archive files,
+    # so restore will not try to download any.
+    download_tar_artifact.assert_not_called()
```

### Comparing `gretel-trainer-0.7.0/tests/relational/test_relational_data.py` & `gretel-trainer-0.8.0/tests/relational/test_relational_data.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/test_report.py` & `gretel-trainer-0.8.0/tests/relational/test_report.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.7.0/tests/relational/test_synthetics_run_task.py` & `gretel-trainer-0.8.0/tests/relational/test_synthetics_run_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 
 import pandas as pd
 import pandas.testing as pdtest
 import pytest
 from gretel_client.projects.projects import Project
 
 from gretel_trainer.relational.core import RelationalData
-from gretel_trainer.relational.sdk_extras import MAX_PROJECT_ARTIFACTS
+from gretel_trainer.relational.sdk_extras import (
+    MAX_PROJECT_ARTIFACTS,
+    ExtendedGretelSDK,
+)
 from gretel_trainer.relational.strategies.ancestral import AncestralStrategy
 from gretel_trainer.relational.strategies.independent import IndependentStrategy
 from gretel_trainer.relational.tasks import SyntheticsRunTask
 from gretel_trainer.relational.workflow_state import SyntheticsRun, SyntheticsTrain
 
 
 @dataclass
 class MockMultiTable:
     relational_data: RelationalData
     _refresh_interval: int = 0
     _project: Project = Mock(artifacts=[])
     _strategy: Union[AncestralStrategy, IndependentStrategy] = AncestralStrategy()
+    _extended_sdk: ExtendedGretelSDK = ExtendedGretelSDK(hybrid=False)
 
     def _backup(self) -> None:
         pass
 
 
 @pytest.fixture(autouse=True)
 def tmpdir():
@@ -48,15 +52,15 @@
             lost_contact=[],
             preserved=preserved or [],
             missing_model=missing_model or [],
             record_size_ratio=1.0,
         ),
         synthetics_train=SyntheticsTrain(
             training_columns={
-                table: rel_data.get_table_data(table).columns
+                table: list(rel_data.get_table_data(table).columns)
                 for table in rel_data.list_all_tables()
             },
             models={
                 table: Mock(create_record_handler=Mock())
                 for table in rel_data.list_all_tables()
             },
         ),
@@ -100,35 +104,37 @@
     class MockStrategy:
         def post_process_individual_synthetic_result(self, table, rel_data, rh_data):
             return rh_data.head(1)
 
     task.multitable._strategy = MockStrategy()  # type:ignore
 
     with patch(
-        "gretel_trainer.relational.tasks.synthetics_run.get_record_handler_data"
+        "gretel_trainer.relational.sdk_extras.ExtendedGretelSDK.get_record_handler_data"
     ) as get_rh_data:
         get_rh_data.return_value = raw_df
         task.handle_completed("table", Mock())
 
-    pdtest.assert_frame_equal(task.working_tables["table"], raw_df.head(1))
+    post_processed = task.working_tables["table"]
+    assert post_processed is not None
+    pdtest.assert_frame_equal(post_processed, raw_df.head(1))
 
 
 def test_starts_jobs_for_ready_tables(pets, tmpdir):
     task = make_task(pets, tmpdir)
 
     assert len(task.synthetics_run.record_handlers) == 0
 
     task.each_iteration()
 
     assert len(task.synthetics_run.record_handlers) == 1
     assert "humans" in task.synthetics_run.record_handlers
     task.synthetics_train.models[
         "humans"
     ].create_record_handler_obj.assert_called_once()
-    task.synthetics_run.record_handlers["humans"].submit_cloud.assert_called_once()
+    task.synthetics_run.record_handlers["humans"].submit.assert_called_once()
 
 
 def test_defers_jobs_if_no_room(pets, tmpdir):
     task = make_task(pets, tmpdir)
     task.multitable._project.artifacts = ["art"] * MAX_PROJECT_ARTIFACTS
 
     assert len(task.synthetics_run.record_handlers) == 0
@@ -140,15 +146,15 @@
     # and therefore wouldn't be deferred; in this context, though, the record handler object
     # is a Mock and calling the `data_source` property returns another mock object, not None
     assert len(task.synthetics_run.record_handlers) == 1
     assert "humans" in task.synthetics_run.record_handlers
     task.synthetics_train.models[
         "humans"
     ].create_record_handler_obj.assert_called_once()
-    task.synthetics_run.record_handlers["humans"].submit_cloud.assert_not_called()
+    task.synthetics_run.record_handlers["humans"].submit.assert_not_called()
 
 
 def test_does_not_restart_existing_deferred_jobs(pets, tmpdir):
     task = make_task(pets, tmpdir)
     task.multitable._project.artifacts = ["art"] * MAX_PROJECT_ARTIFACTS
 
     assert len(task.synthetics_run.record_handlers) == 0
@@ -157,14 +163,14 @@
 
     # We create the record handler, but defer submitting it
     assert len(task.synthetics_run.record_handlers) == 1
     assert "humans" in task.synthetics_run.record_handlers
     task.synthetics_train.models[
         "humans"
     ].create_record_handler_obj.assert_called_once()
-    task.synthetics_run.record_handlers["humans"].submit_cloud.assert_not_called()
+    task.synthetics_run.record_handlers["humans"].submit.assert_not_called()
 
     task.synthetics_train.models["humans"].reset_mock()
 
     # On next iteration, we do not *re-create* a record handler object for humans
     task.each_iteration()
     task.synthetics_train.models["humans"].create_record_handler_obj.assert_not_called()
```

### Comparing `gretel-trainer-0.7.0/tests/relational/test_task_runner.py` & `gretel-trainer-0.8.0/tests/relational/test_task_runner.py`

 * *Files 21% similar despite different names*

```diff
@@ -53,131 +53,137 @@
 
     def each_iteration(self) -> None:
         self.iteration_count += 1
 
 
 @pytest.fixture(autouse=True)
 def get_job_id():
-    with patch("gretel_trainer.relational.task_runner.get_job_id") as _get_job_id:
+    with patch(
+        "gretel_trainer.relational.sdk_extras.ExtendedGretelSDK.get_job_id"
+    ) as _get_job_id:
         yield _get_job_id
 
 
 @pytest.fixture(autouse=True)
 def delete_data_source():
     with patch(
-        "gretel_trainer.relational.task_runner.delete_data_source"
+        "gretel_trainer.relational.sdk_extras.ExtendedGretelSDK.delete_data_source"
     ) as _delete_data_source:
         yield _delete_data_source
 
 
-def test_one_successful_model(get_job_id, delete_data_source):
+def test_one_successful_model(get_job_id, delete_data_source, extended_sdk):
     get_job_id.side_effect = [None, "id"]
 
     project = Mock(artifacts=[])
     model = Mock(status=Status.COMPLETED)
     models = {"table": model}
 
     task = MockTask(
         project=project,
         models=models,
     )
-    run_task(task)
+    run_task(task, extended_sdk)
 
     assert task.iteration_count == 2
     assert task.completed == ["table"]
     assert task.failed == []
     delete_data_source.assert_called_once()
 
 
-def test_one_failed_model(get_job_id, delete_data_source):
+def test_one_failed_model(get_job_id, delete_data_source, extended_sdk):
     get_job_id.side_effect = [None, "id"]
 
     project = Mock(artifacts=[])
     model = Mock(status=Status.ERROR)
     models = {"table": model}
 
     task = MockTask(
         project=project,
         models=models,
     )
-    run_task(task)
+    run_task(task, extended_sdk)
 
     assert task.iteration_count == 2
     assert task.completed == []
     assert task.failed == ["table"]
     delete_data_source.assert_called_once()
 
 
-def test_model_taking_awhile(get_job_id, delete_data_source):
+def test_model_taking_awhile(get_job_id, delete_data_source, extended_sdk):
     get_job_id.side_effect = [None, "id", "id"]
 
     project = Mock(artifacts=[])
     model = Mock()
     status = PropertyMock(side_effect=[Status.ACTIVE, Status.COMPLETED])
     type(model).status = status
     models = {"table": model}
 
     task = MockTask(
         project=project,
         models=models,
     )
-    run_task(task)
+    run_task(task, extended_sdk)
 
     assert task.iteration_count == 3
     assert task.completed == ["table"]
     assert task.failed == []
     delete_data_source.assert_called_once()
 
 
-def test_lose_contact_with_model(get_job_id, delete_data_source):
+def test_lose_contact_with_model(get_job_id, delete_data_source, extended_sdk):
     get_job_id.side_effect = [None, "id", "id", "id"]
 
     project = Mock(artifacts=[])
     model = Mock(status=Status.ACTIVE)
     model.refresh.side_effect = Exception()
     models = {"table": model}
 
     task = MockTask(
         project=project,
         models=models,
     )
-    run_task(task)
+    run_task(task, extended_sdk)
 
     # Bail after refresh fails MAX_REFRESH_ATTEMPTS times
     assert task.iteration_count == 4
     assert task.completed == []
     assert task.failed == []
     assert task.lost_contact == ["table"]
     delete_data_source.assert_called_once()
 
 
-def test_refresh_status_can_tolerate_blips(get_job_id, delete_data_source):
+def test_refresh_status_can_tolerate_blips(
+    get_job_id, delete_data_source, extended_sdk
+):
     get_job_id.side_effect = [None, "id", "id"]
 
     project = Mock(artifacts=[])
     model = Mock()
     status = PropertyMock(side_effect=[Status.ACTIVE, Status.COMPLETED])
     type(model).status = status
     model.refresh.side_effect = [Exception(), None]
     models = {"table": model}
 
     task = MockTask(
         project=project,
         models=models,
     )
-    run_task(task)
+    run_task(task, extended_sdk)
 
     assert task.iteration_count == 3
     assert task.completed == ["table"]
     assert task.failed == []
     assert task.lost_contact == []
     delete_data_source.assert_called_once()
 
 
-def test_defers_submission_if_no_room_in_project(get_job_id, delete_data_source):
+def test_defers_submission_if_no_room_in_project(
+    get_job_id, delete_data_source, extended_sdk
+):
     get_job_id.side_effect = [None, None, None, "id"]
     project = Mock()
     # First time through, we're at the project limit
     # Second time through, we're below the limit, but still not enough room for this task
     # Third time through, there is enough space
     artifacts = PropertyMock(
         side_effect=[
@@ -190,22 +196,22 @@
     model = Mock(status=Status.COMPLETED)
     models = {"table": model}
 
     task = MockTask(
         project=project,
         models=models,
     )
-    run_task(task)
+    run_task(task, extended_sdk)
 
     assert task.iteration_count == 4
     assert task.completed == ["table"]
     delete_data_source.assert_called_once()
 
 
-def test_several_models(delete_data_source):
+def test_several_models(delete_data_source, extended_sdk):
     project = Mock(artifacts=[])
 
     completed_model = Mock(status=Status.COMPLETED)
     error_model = Mock(status=Status.ERROR)
     cancelled_model = Mock(status=Status.CANCELLED)
     lost_model = Mock(status=Status.LOST)
 
@@ -216,15 +222,15 @@
         "lost": lost_model,
     }
 
     task = MockTask(
         project=project,
         models=models,
     )
-    run_task(task)
+    run_task(task, extended_sdk)
 
     assert task.completed == ["completed"]
     assert set(task.failed) == {"error", "cancelled", "lost"}
     delete_data_source.assert_has_calls(
         [
             call(project, completed_model),
             call(project, error_model),
```

### Comparing `gretel-trainer-0.7.0/tests/test_benchmark.py` & `gretel-trainer-0.8.0/tests/test_benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         ],
         runtime_config=TEST_RUNTIME_CONFIG,
         gretel_sdk=_make_gretel_sdk(),
         gretel_trainer_factory=mock_gretel_trainer_factory(get_sqs_score=84),
     ).wait()
 
     def _unique_results(col: str):
-        unique_results = list(set(comparison.results[col].values.tolist()))
+        unique_results = list(set(comparison.results[col].values))
         unique_results.sort()
         return unique_results
 
     assert len(comparison.results) == 8
     assert _unique_results("Input data") == [
         f"{csv}",
         "DataFrames::0",
@@ -139,19 +139,19 @@
             DoNothingModel,
         ],
         runtime_config=TEST_RUNTIME_CONFIG,
         gretel_sdk=_make_gretel_sdk(evaluate=_fail),
         gretel_trainer_factory=mock_gretel_trainer_factory(),
     ).wait()
 
-    assert comparison.results["Status"].values.tolist() == [
+    assert set(comparison.results["Status"].values) == {
         "Failed (train)",
         "Failed (generate)",
         "Failed (evaluate)",
-    ]
+    }
 
 
 def test_failures_during_cleanup_are_ignored(csv):
     def _failing_search(_):
         raise Exception("failed")
 
     csv_dataset = _make_dataset([csv])
@@ -162,15 +162,15 @@
             GretelAuto,
         ],
         runtime_config=TEST_RUNTIME_CONFIG,
         gretel_sdk=_make_gretel_sdk(search_projects=_failing_search),
         gretel_trainer_factory=mock_gretel_trainer_factory(),
     ).wait()
 
-    assert comparison.results["Status"].values.tolist() == ["Completed"]
+    assert set(comparison.results["Status"].values) == {"Completed"}
 
 
 @pytest.mark.parametrize(
     "model,expected_model_type",
     [
         (GretelAuto, None),
         (GretelACTGAN, tm.GretelACTGAN),
@@ -246,16 +246,16 @@
 
     mock_trainer_factory.assert_not_called()
     mock_project_factory.assert_called_with("benchmark-proj-0")
     mock_model.submit_cloud.assert_called_once()
     mock_record_handler.submit_cloud.assert_called_once()
     mock_record_handler.get_artifact_link.assert_called_once_with("data")
     assert mock_poll.call_count == 2
-    assert comparison.results["Status"].values.tolist() == ["Completed"]
-    assert comparison.results["SQS"].values.tolist() == [94]
+    assert set(comparison.results["Status"].values) == {"Completed"}
+    assert set(comparison.results["SQS"].values) == {94}
 
 
 def test_gretel_model_with_bad_custom_config_fails_before_execution_starts(csv):
     class BadGretelConfig(GretelModel):
         config = {"hello": "world", "hola": "mundo"}
 
     mock_trainer_factory = Mock()
@@ -309,16 +309,16 @@
             GretelAuto,
         ],
         runtime_config=TEST_RUNTIME_CONFIG,
         gretel_sdk=_make_gretel_sdk(),
         gretel_trainer_factory=mock_gretel_trainer_factory(get_sqs_score=84),
     ).wait()
 
-    assert comparison.results["Input data"].values.tolist() == ["iris/data.csv"]
-    assert comparison.results["Status"].values.tolist() == ["Completed"]
+    assert set(comparison.results["Input data"].values) == {"iris/data.csv"}
+    assert set(comparison.results["Status"].values) == {"Completed"}
 
     with suppress(FileNotFoundError):
         assert len(os.listdir(TEST_BENCHMARK_DIR)) == 0
         shutil.rmtree(TEST_BENCHMARK_DIR)
 
 
 def test_benchmark_cleans_up_after_failures(csv):
@@ -333,15 +333,15 @@
             GretelAuto,
         ],
         runtime_config=TEST_RUNTIME_CONFIG,
         gretel_sdk=_make_gretel_sdk(search_projects=mock_search_projects),
         gretel_trainer_factory=mock_gretel_trainer_factory(fail="train"),
     ).wait()
 
-    assert comparison.results["Status"].values.tolist() == ["Failed (train)"]
+    assert set(comparison.results["Status"].values) == {"Failed (train)"}
 
     mock_project.delete.assert_called()
 
 
 def test_make_dataset_with_different_datatypes(csv):
     _make_dataset([csv], datatype=Datatype.TABULAR_MIXED)
     _make_dataset([csv], datatype="tabular_mixed")
@@ -375,15 +375,15 @@
         datasets=[too_many_columns, wrong_datatype],
         models=[GretelGPTX],
         runtime_config=TEST_RUNTIME_CONFIG,
         gretel_sdk=_make_gretel_sdk(),
         gretel_trainer_factory=Mock(),
     ).wait()
 
-    assert comparison.results["Status"].values.tolist() == ["Skipped", "Skipped"]
+    assert set(comparison.results["Status"].values) == {"Skipped", "Skipped"}
 
 
 def test_runs_with_lstm_are_skipped_when_over_150_columns():
     too_many_columns = _make_dataset(
         [pd.DataFrame(index=range(151), columns=range(151))]
     )
 
@@ -391,15 +391,15 @@
         datasets=[too_many_columns],
         models=[GretelLSTM],
         runtime_config=TEST_RUNTIME_CONFIG,
         gretel_sdk=_make_gretel_sdk(),
         gretel_trainer_factory=Mock(),
     ).wait()
 
-    assert comparison.results["Status"].values.tolist() == ["Skipped"]
+    assert set(comparison.results["Status"].values) == {"Skipped"}
 
 
 def test_skip_cleanup_when_requested():
     with suppress(FileNotFoundError):
         shutil.rmtree(TEST_BENCHMARK_DIR)
 
     runtime_config = TEST_RUNTIME_CONFIG
```

### Comparing `gretel-trainer-0.7.0/tests/test_strategy.py` & `gretel-trainer-0.8.0/tests/test_strategy.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,42 +30,28 @@
 @pytest.fixture(scope="module")
 def header_clusters_seed(test_df) -> ClusterData:
     seeds = ["goal", "goal_type", "goals"]
     clusters = cluster(test_df, header_prefix=seeds)
     return ClusterData(clusters=clusters, seeds=seeds)
 
 
-def test_invalid_partition_constraints():
-    with pytest.raises(AttributeError):
-        PartitionConstraints(max_row_count=1, max_row_partitions=1)
-
-    with pytest.raises(AttributeError):
-        PartitionConstraints()
-
-
 @pytest.mark.parametrize(
     "constraints",
     [
-        PartitionConstraints(max_row_partitions=3),
-        PartitionConstraints(max_row_partitions=20),
         PartitionConstraints(max_row_count=1000),
         PartitionConstraints(max_row_count=100),
     ],
 )
 def test_strategy_all_columns(constraints: PartitionConstraints, test_df):
     strategy = PartitionStrategy.from_dataframe("foo", test_df, constraints)
-    if constraints.max_row_partitions:
-        assert constraints.max_row_partitions == strategy.partition_count
-
-    if constraints.max_row_count:
-        assert (
-            len(test_df) // constraints.max_row_count
-            <= strategy.partition_count
-            <= len(test_df) // constraints.max_row_count + 1
-        )
+    assert (
+        len(test_df) // constraints.max_row_count
+        <= strategy.partition_count
+        <= len(test_df) // constraints.max_row_count + 1
+    )
 
     # partitions are of roughly equal size
     extracted_df_lengths = [len(partition.extract_df(test_df)) for partition in strategy.partitions]
     assert max(extracted_df_lengths) - min(extracted_df_lengths) <= 1
 
     # re-assemble all partitions and compare
     compare = pd.DataFrame()
@@ -77,38 +63,29 @@
 
     assert compare.shape == test_df.shape
 
 
 @pytest.mark.parametrize(
     "constraints",
     [
-        PartitionConstraints(max_row_partitions=3),
-        PartitionConstraints(max_row_partitions=20),
         PartitionConstraints(max_row_count=1000),
         PartitionConstraints(max_row_count=100),
     ],
 )
 def test_strategy_column_batches(
     constraints: PartitionConstraints, test_df, header_clusters
 ):
     constraints.header_clusters = header_clusters
 
     strategy = PartitionStrategy.from_dataframe("foo", test_df, constraints)
-    if constraints.max_row_partitions:
-        assert (
-            constraints.max_row_partitions * len(header_clusters)
-            == strategy.partition_count
-        )
-
-    if constraints.max_row_count:
-        assert (
-            len(test_df) // constraints.max_row_count
-            <= strategy.partition_count / len(header_clusters)
-            <= len(test_df) // constraints.max_row_count + 1
-        )
+    assert (
+        len(test_df) // constraints.max_row_count
+        <= strategy.partition_count / len(header_clusters)
+        <= len(test_df) // constraints.max_row_count + 1
+    )
 
     # partitions are of roughly equal size
     extracted_df_lengths = [len(partition.extract_df(test_df)) for partition in strategy.partitions]
     assert max(extracted_df_lengths) - min(extracted_df_lengths) <= 1
 
     part1 = pd.DataFrame()
     part2 = pd.DataFrame()
@@ -120,36 +97,30 @@
         else:
             part2 = pd.concat([part2, tmp_df]).reset_index(drop=True)
 
     final = pd.concat([part1, part2], axis=1)
     assert final.shape == test_df.shape
 
 
-@pytest.mark.parametrize(
-    "constraints",
-    [
-        PartitionConstraints(max_row_partitions=3),
-        PartitionConstraints(max_row_count=100),
-    ],
-)
-def test_strategy_seeds(constraints: PartitionConstraints, test_df, header_clusters_seed: ClusterData):
+def test_strategy_seeds(test_df, header_clusters_seed: ClusterData):
+    constraints = PartitionConstraints(max_row_count=100)
     constraints.header_clusters = header_clusters_seed.clusters
     constraints.seed_headers = header_clusters_seed.seeds
     strategy = PartitionStrategy.from_dataframe("foo", test_df, constraints)
     for partition in strategy.partitions:
         if partition.columns.idx == 0:
             assert partition.columns.seed_headers == header_clusters_seed.seeds
         else:
             assert not partition.columns.seed_headers
 
 
 def test_read_write(test_df, header_clusters, tmpdir):
     save_location = Path(tmpdir) / "data.json"
     constraints = PartitionConstraints(
-        max_row_partitions=3, header_clusters=header_clusters
+        max_row_count=100, header_clusters=header_clusters
     )
     strategy = PartitionStrategy.from_dataframe("foo", test_df, constraints)
 
     # Inproper filename
     with pytest.raises(ValueError):
         strategy.save_to("foo.txt")
```

