# Comparing `tmp/Renate-0.1.0.tar.gz` & `tmp/Renate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Renate-0.1.0.tar", last modified: Mon Nov 28 16:23:17 2022, max compression
+gzip compressed data, was "Renate-0.2.0.tar", last modified: Mon Apr 24 16:17:52 2023, max compression
```

## Comparing `Renate-0.1.0.tar` & `Renate-0.2.0.tar`

### file list

```diff
@@ -1,177 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.624804 Renate-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.596802 Renate-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.604803 Renate-0.1.0/.github/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      488 2022-11-28 16:23:05.000000 Renate-0.1.0/.github/hooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.604803 Renate-0.1.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2022-11-28 16:23:05.000000 Renate-0.1.0/.github/scripts/build_docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2022-11-28 16:23:05.000000 Renate-0.1.0/.github/scripts/prepend_license.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.604803 Renate-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2022-11-28 16:23:05.000000 Renate-0.1.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2022-11-28 16:23:05.000000 Renate-0.1.0/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-11-28 16:23:05.000000 Renate-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2022-11-28 16:23:05.000000 Renate-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-11-28 16:23:05.000000 Renate-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-11-28 16:23:05.000000 Renate-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2022-11-28 16:23:17.624804 Renate-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2022-11-28 16:23:05.000000 Renate-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-11-28 16:23:05.000000 Renate-0.1.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-11-28 16:23:05.000000 Renate-0.1.0/dev_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.604803 Renate-0.1.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.604803 Renate-0.1.0/doc/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    35105 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/_images/improvement_renate.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34694 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/_images/improvement_tuning.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.604803 Renate-0.1.0/doc/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/benchmarking/custom_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      957 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/benchmarking/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/benchmarking/renate_benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.604803 Renate-0.1.0/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/examples/train_classifier_sagemaker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/examples/train_mlp_locally.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.608803 Renate-0.1.0/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/getting_started/how_to_renate_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/getting_started/how_to_run_training.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      585 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/getting_started/output.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/getting_started/supported_algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-11-28 16:23:05.000000 Renate-0.1.0/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.600803 Renate-0.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.608803 Renate-0.1.0/examples/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/benchmarking/class_incremental_learning_cifar10_der.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.608803 Renate-0.1.0/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/getting_started/renate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.608803 Renate-0.1.0/examples/simple_classifier_cifar10/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/simple_classifier_cifar10/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/simple_classifier_cifar10/start_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/simple_classifier_cifar10/start_without_hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.608803 Renate-0.1.0/examples/train_mlp_locally/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/train_mlp_locally/renate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/train_mlp_locally/start_training_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2022-11-28 16:23:05.000000 Renate-0.1.0/examples/train_mlp_locally/start_training_without_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2022-11-28 16:23:05.000000 Renate-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2022-11-28 16:23:05.000000 Renate-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-28 16:23:17.624804 Renate-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.600803 Renate-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.608803 Renate-0.1.0/src/Renate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2022-11-28 16:23:17.000000 Renate-0.1.0/src/Renate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2022-11-28 16:23:17.000000 Renate-0.1.0/src/Renate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 16:23:17.000000 Renate-0.1.0/src/Renate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-11-28 16:23:17.000000 Renate-0.1.0/src/Renate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-11-28 16:23:17.000000 Renate-0.1.0/src/Renate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.608803 Renate-0.1.0/src/renate/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.612803 Renate-0.1.0/src/renate/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.612803 Renate-0.1.0/src/renate/benchmark/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/datasets/nlp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/datasets/vision_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/experimentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.612803 Renate-0.1.0/src/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/models/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/benchmark/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.612803 Renate-0.1.0/src/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/cli/parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/cli/run_experiment_with_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/cli/run_remote_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/cli/run_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.612803 Renate-0.1.0/src/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/data/data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.612803 Renate-0.1.0/src/renate/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.612803 Renate-0.1.0/src/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/evaluation/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/evaluation/metrics/performance_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/evaluation/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.616804 Renate-0.1.0/src/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/memory/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.616804 Renate-0.1.0/src/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.616804 Renate-0.1.0/src/renate/models/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/models/layers/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/models/renate_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.616804 Renate-0.1.0/src/renate/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/tuning/config_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    24898 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/tuning/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.616804 Renate-0.1.0/src/renate/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.616804 Renate-0.1.0/src/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48135 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/experimental/er.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/experimental/gdumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/experimental/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/experimental/offline_er.py
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/experimental/repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)    18691 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.616804 Renate-0.1.0/src/renate/updaters/learner_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/learner_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/learner_components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/learner_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/learner_components/reinitialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/updaters/model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/src/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/utils/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/utils/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2022-11-28 16:23:05.000000 Renate-0.1.0/src/renate/utils/syne_tune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2022-11-28 16:23:05.000000 Renate-0.1.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2022-11-28 16:23:05.000000 Renate-0.1.0/test/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/renate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/renate/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/renate/benchmark/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/benchmark/models/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/benchmark/models/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/benchmark/models/test_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/benchmark/test_experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/benchmark/test_experimentation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/benchmark/test_scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/renate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/cli/test_parsing_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/renate/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/data/test_data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/data/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.600803 Renate-0.1.0/test/renate/evaluation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/renate/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/evaluation/metrics/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/evaluation/metrics/test_regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.620804 Renate-0.1.0/test/renate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/memory/test_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.624804 Renate-0.1.0/test/renate/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/models/test_renate_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.624804 Renate-0.1.0/test/renate/renate_config_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/renate_config_files/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/test_renate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.624804 Renate-0.1.0/test/renate/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/tuning/test_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.624804 Renate-0.1.0/test/renate/updaters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.624804 Renate-0.1.0/test/renate/updaters/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/updaters/experimental/test_er.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/updaters/experimental/test_joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/updaters/experimental/test_repeated_distill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/updaters/test_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/updaters/test_model_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 16:23:17.624804 Renate-0.1.0/test/renate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/utils/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/utils/test_metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/utils/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/utils/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-11-28 16:23:05.000000 Renate-0.1.0/test/renate/utils/test_syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/hooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       98 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/scripts/build_docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/scripts/prepend_license.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/integration_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/run_renate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-24 16:17:43.000000 Renate-0.2.0/.github/workflows/test_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 16:17:43.000000 Renate-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 16:17:43.000000 Renate-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-24 16:17:43.000000 Renate-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 16:17:43.000000 Renate-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-24 16:17:43.000000 Renate-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-24 16:17:52.039463 Renate-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-24 16:17:43.000000 Renate-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 16:17:43.000000 Renate-0.2.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 16:17:43.000000 Renate-0.2.0/dev_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.007463 Renate-0.2.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    35105 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/_images/improvement_renate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/_images/improvement_tuning.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/benchmarking/custom_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/benchmarking/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/benchmarking/renate_benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/examples/train_classifier_sagemaker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/examples/train_mlp_locally.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/avalanche.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/how_to_renate_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/how_to_run_training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/getting_started/supported_algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 16:17:43.000000 Renate-0.2.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/benchmarking/class_incremental_learning_cifar10_der.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/getting_started/renate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/nlp_finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/nlp_finetuning/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/nlp_finetuning/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/simple_classifier_cifar10/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/start_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/simple_classifier_cifar10/start_without_hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.011463 Renate-0.2.0/examples/train_mlp_locally/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/renate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/start_training_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-24 16:17:43.000000 Renate-0.2.0/examples/train_mlp_locally/start_training_without_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-24 16:17:43.000000 Renate-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 16:17:43.000000 Renate-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:17:52.039463 Renate-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/Renate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:17:51.000000 Renate-0.2.0/src/Renate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/benchmark/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/datasets/nlp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/datasets/vision_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/experimentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/models/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/benchmark/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.015463 Renate-0.2.0/src/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    37040 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/run_experiment_with_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/run_remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/cli/run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/data/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/performance_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/evaluation/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/memory/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/memory/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/layers/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/prediction_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/models/renate_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25819 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.019463 Renate-0.2.0/src/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/avalanche/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.023463 Renate-0.2.0/src/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/gdumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/offline_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/experimental/repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.023463 Renate-0.2.0/src/renate/updaters/learner_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/learner_components/reinitialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/updaters/model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.023463 Renate-0.2.0/src/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/config_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-24 16:17:43.000000 Renate-0.2.0/src/renate/utils/syne_tune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-04-24 16:17:43.000000 Renate-0.2.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-24 16:17:43.000000 Renate-0.2.0/test/dummy_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/test/integration_tests/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/configs/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/cifar10.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/cifar100.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/fashionmnist.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/datasets/mnist.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/configs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/models/mlp-200.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/models/resnet18-cifar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.027463 Renate-0.2.0/test/integration_tests/configs/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/class-incremental-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/feature-sorting-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/hue-shift-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/iid-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/permutation-2updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/rotation-10updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/scenarios/rotation-2updates.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/test/integration_tests/configs/suites/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.031463 Renate-0.2.0/test/integration_tests/configs/suites/quick/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-icarl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/cls-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/der.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/gdumb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/offline-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/pod-er.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/suites/quick/super-er.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/integration_tests/configs/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-ewc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-icarl-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/avalanche-lwf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/cls-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/der-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/fine-tuning.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/gdumb-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/joint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/offline-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/pod-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/configs/updaters/super-er-buffer500.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-24 16:17:43.000000 Renate-0.2.0/test/integration_tests/run_quick_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/benchmark/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/models/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/models/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/models/test_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/test_experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/test_experimentation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/benchmark/test_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/cli/test_parsing_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/data/test_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/data/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.003463 Renate-0.2.0/test/renate/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/evaluation/metrics/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/evaluation/metrics/test_regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/memory/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/memory/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.035463 Renate-0.2.0/test/renate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/models/test_renate_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/renate_config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/renate_config_files/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/test_renate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/training/
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/training/test_run_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/updaters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/updaters/avalanche/
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_model_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/avalanche/test_avalanche_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/updaters/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/experimental/test_repeated_distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/test_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/updaters/test_model_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:17:52.039463 Renate-0.2.0/test/renate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 16:17:43.000000 Renate-0.2.0/test/renate/utils/test_syne_tune.py
```

### Comparing `Renate-0.1.0/.github/workflows/pypi_publish.yml` & `Renate-0.2.0/.github/workflows/pypi_publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python 3.10
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: "3.10"
 
     - name: Install pypa/build
       run: >-
         python -m
         pip install
```

### Comparing `Renate-0.1.0/.github/workflows/run_unit_tests.yml` & `Renate-0.2.0/.github/workflows/test_docs.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,34 @@
 
-name: Run unit tests on push and PR
+name: Sphinx Doc Building
 
 on:
   push:
     branches: [ "main", "dev" ]
   pull_request:
     branches: [ "main", "dev" ]
 
-  workflow_dispatch:
-
-
 jobs:
   test:
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ["3.8", "3.9"]
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
-          
+
       - name: Switch to Current Branch
         run: git checkout ${{ env.BRANCH }}
-              
-      - name: Set up Python ${{ matrix.python-version }}
+
+      - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: "3.9"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
-          pip install -e .[dev]
+          pip install -r doc/requirements.txt
 
-      - name: Lint with flake8
+      - name: Build docs
         run: |
-          # stop the build if there are Python syntax errors or undefined names
-          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-
-      - name: Run unit tests
-        run: PYTHONPATH=test python -m pytest test/
+          bash .github/scripts/build_docs.sh
```

### Comparing `Renate-0.1.0/CONTRIBUTING.md` & `Renate-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/LICENSE` & `Renate-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/PKG-INFO` & `Renate-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,128 @@
 Metadata-Version: 2.1
 Name: Renate
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library for Continual Learning for Practitioners
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <=3.10,>=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: avalanche
 Provides-Extra: dev
 License-File: LICENSE
+License-File: NOTICE
 
 .. image:: https://img.shields.io/pypi/status/Renate
+    :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.1.0
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
-   :alt: PyPI - Downloads
+    :target: https://pypistats.org/packages/renate
+    :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
 .. image:: https://readthedocs.org/projects/renate/badge/?version=latest
     :target: https://renate.readthedocs.io
     :alt: Documentation Status
+.. image:: https://raw.githubusercontent.com/awslabs/Renate/python-coverage-comment-action-data/badge.svg
+    :target: https://htmlpreview.github.io/?https://github.com/awslabs/Renate/blob/python-coverage-comment-action-data/htmlcov/index.html
+    :alt: Coverage Badge
 
-Renate - Automatic Neural Networks Retraining and Continual Learning in Python
+Renate: Automatic Neural Networks Retraining and Continual Learning in Python
 ******************************************************************************
 
 Renate is a Python package for automatic retraining of neural networks models.
 It uses advanced Continual Learning and Lifelong Learning algorithms to achieve this purpose. 
 The implementation is based on `PyTorch <https://pytorch.org>`_
 and `Lightning <https://www.pytorchlightning.ai>`_ for deep learning, and
 `Syne Tune <https://github.com/awslabs/syne-tune>`_ for hyperparameter optimization.
 
+Quick links
+===========
+* Install renate with ``pip install renate`` or look at `these instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
+* Examples for `local training <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_ and `training on Amazon SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_.
+* `Documentation <https://renate.readthedocs.io>`_
+* `Supported Algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
+
 
 Who needs Renate?
 =================
 
 In many applications data is made available over time and retraining from scratch for
 every new batch of data is prohibitively expensive. In these cases, we would like to use
 the new batch of data provided to update our previous model with limited costs.
 Unfortunately, since data in different chunks is not sampled according to the same distribution,
 just fine-tuning the old model creates problems like *catastrophic forgetting*.
 The algorithms in Renate help mitigating the negative impact of forgetting and increase the 
 model performance overall. 
 
 .. figure:: https://raw.githubusercontent.com/awslabs/Renate/main/doc/_images/improvement_renate.svg
-    :scale: 80%
     :align: center
     :alt: Renate vs Model Fine-Tuning.
 
     Renate's update mechanisms improve over naive fine-tuning approaches. [#]_
 
 Renate also offers hyperparameter optimization (HPO), a functionality that can heavily impact
 the performance of the model when continuously updated. To do so, Renate employs
 `Syne Tune <https://github.com/awslabs/syne-tune>`_ under the hood, and can offer
 advanced HPO methods such multi-fidelity algorithms (ASHA) and transfer learning algorithms
 (useful for speeding up the retuning).
 
 .. figure:: https://raw.githubusercontent.com/awslabs/Renate/main/doc/_images/improvement_tuning.svg
-    :scale: 80%
     :align: center
     :alt: Impact of HPO on Renate's Updating Algorithms.
 
     Renate will benefit from hyperparameter tuning compared to Renate with default settings. [#]_
 
 
 Key features
 ============
 
 * Easy to scale and run in the cloud
 * Designed for real-world retraining pipelines
 * Advanced HPO functionalities available out-of-the-box
 * Open for experimentation 
 
+Blog posts
+==========
+
+* `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+
 
 What are you looking for?
 =========================
 
 * `Installation Instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
-
     .. code-block:: bash
 
       pip install renate
 
-* Examples
-    We provide examples to train your model
-    `locally <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_
-    or `using Amazon SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_.
-* `Documentation <https://renate.readthedocs.io>`_
-* `Supported Algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
-* `Experimenting with Renate <https://renate.readthedocs.io/en/latest/benchmarking/index.html>`_
+* Examples:
+    * `Train an MLP locally on MNIST <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_
+    * `Train a ResNet on SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_
+* `Documentation website with API doc and examples <https://renate.readthedocs.io>`_
+* `List of the supported algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
+* `How to run continual learning experiments using Renate <https://renate.readthedocs.io/en/latest/benchmarking/index.html>`_
 * `Guidelines for Contributors <https://github.com/awslabs/renate/tree/master/CONTRIBUTING.md>`_
-* You did not find what you were looking for?
-    Open an `issue <https://github.com/awslabs/Renate/issues/new>`_ and we will do our best
-    to improve the documentation.
+
+If you did not find what you were looking for, open an `issue <https://github.com/awslabs/Renate/issues/new>`_ and
+we will do our best to improve the documentation.
 
 
 .. [#] To create this plot, we simulated class-incremental learning with CIFAR-10.
     The training data was divided into 5 partitions, and we trained sequentially on them.
     Fine-tuning refers to the strategy to learn on the first partition from scratch, and
     train on each of the subsequent partitions for few epochs only.
     We compare to Experience Replay with a memory size of 500.
     For both methods we use the same number of epochs and choose the best checkpoint
     using a validation set.
     Results reported are on the test set.
+
 .. [#] The setup is the same as in the last experiment. However, this time we compare
     Experience Replay against a version in which its hyperparameters were tuned.
```

### Comparing `Renate-0.1.0/README.rst` & `Renate-0.2.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,111 @@
 .. image:: https://img.shields.io/pypi/status/Renate
+    :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.1.0
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
-   :alt: PyPI - Downloads
+    :target: https://pypistats.org/packages/renate
+    :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
 .. image:: https://readthedocs.org/projects/renate/badge/?version=latest
     :target: https://renate.readthedocs.io
     :alt: Documentation Status
+.. image:: https://raw.githubusercontent.com/awslabs/Renate/python-coverage-comment-action-data/badge.svg
+    :target: https://htmlpreview.github.io/?https://github.com/awslabs/Renate/blob/python-coverage-comment-action-data/htmlcov/index.html
+    :alt: Coverage Badge
 
-Renate - Automatic Neural Networks Retraining and Continual Learning in Python
+Renate: Automatic Neural Networks Retraining and Continual Learning in Python
 ******************************************************************************
 
 Renate is a Python package for automatic retraining of neural networks models.
 It uses advanced Continual Learning and Lifelong Learning algorithms to achieve this purpose. 
 The implementation is based on `PyTorch <https://pytorch.org>`_
 and `Lightning <https://www.pytorchlightning.ai>`_ for deep learning, and
 `Syne Tune <https://github.com/awslabs/syne-tune>`_ for hyperparameter optimization.
 
+Quick links
+===========
+* Install renate with ``pip install renate`` or look at `these instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
+* Examples for `local training <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_ and `training on Amazon SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_.
+* `Documentation <https://renate.readthedocs.io>`_
+* `Supported Algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
+
 
 Who needs Renate?
 =================
 
 In many applications data is made available over time and retraining from scratch for
 every new batch of data is prohibitively expensive. In these cases, we would like to use
 the new batch of data provided to update our previous model with limited costs.
 Unfortunately, since data in different chunks is not sampled according to the same distribution,
 just fine-tuning the old model creates problems like *catastrophic forgetting*.
 The algorithms in Renate help mitigating the negative impact of forgetting and increase the 
 model performance overall. 
 
 .. figure:: https://raw.githubusercontent.com/awslabs/Renate/main/doc/_images/improvement_renate.svg
-    :scale: 80%
     :align: center
     :alt: Renate vs Model Fine-Tuning.
 
     Renate's update mechanisms improve over naive fine-tuning approaches. [#]_
 
 Renate also offers hyperparameter optimization (HPO), a functionality that can heavily impact
 the performance of the model when continuously updated. To do so, Renate employs
 `Syne Tune <https://github.com/awslabs/syne-tune>`_ under the hood, and can offer
 advanced HPO methods such multi-fidelity algorithms (ASHA) and transfer learning algorithms
 (useful for speeding up the retuning).
 
 .. figure:: https://raw.githubusercontent.com/awslabs/Renate/main/doc/_images/improvement_tuning.svg
-    :scale: 80%
     :align: center
     :alt: Impact of HPO on Renate's Updating Algorithms.
 
     Renate will benefit from hyperparameter tuning compared to Renate with default settings. [#]_
 
 
 Key features
 ============
 
 * Easy to scale and run in the cloud
 * Designed for real-world retraining pipelines
 * Advanced HPO functionalities available out-of-the-box
 * Open for experimentation 
 
+Blog posts
+==========
+
+* `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+
 
 What are you looking for?
 =========================
 
 * `Installation Instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
-
     .. code-block:: bash
 
       pip install renate
 
-* Examples
-    We provide examples to train your model
-    `locally <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_
-    or `using Amazon SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_.
-* `Documentation <https://renate.readthedocs.io>`_
-* `Supported Algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
-* `Experimenting with Renate <https://renate.readthedocs.io/en/latest/benchmarking/index.html>`_
+* Examples:
+    * `Train an MLP locally on MNIST <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_
+    * `Train a ResNet on SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_
+* `Documentation website with API doc and examples <https://renate.readthedocs.io>`_
+* `List of the supported algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
+* `How to run continual learning experiments using Renate <https://renate.readthedocs.io/en/latest/benchmarking/index.html>`_
 * `Guidelines for Contributors <https://github.com/awslabs/renate/tree/master/CONTRIBUTING.md>`_
-* You did not find what you were looking for?
-    Open an `issue <https://github.com/awslabs/Renate/issues/new>`_ and we will do our best
-    to improve the documentation.
+
+If you did not find what you were looking for, open an `issue <https://github.com/awslabs/Renate/issues/new>`_ and
+we will do our best to improve the documentation.
 
 
 .. [#] To create this plot, we simulated class-incremental learning with CIFAR-10.
     The training data was divided into 5 partitions, and we trained sequentially on them.
     Fine-tuning refers to the strategy to learn on the first partition from scratch, and
     train on each of the subsequent partitions for few epochs only.
     We compare to Experience Replay with a memory size of 500.
     For both methods we use the same number of epochs and choose the best checkpoint
     using a validation set.
     Results reported are on the test set.
+
 .. [#] The setup is the same as in the last experiment. However, this time we compare
     Experience Replay against a version in which its hyperparameters were tuned.
```

### Comparing `Renate-0.1.0/doc/_images/improvement_renate.svg` & `Renate-0.2.0/doc/_images/improvement_renate.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/doc/_images/improvement_tuning.svg` & `Renate-0.2.0/doc/_images/improvement_tuning.svg`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/doc/benchmarking/custom_benchmarks.rst` & `Renate-0.2.0/doc/benchmarking/custom_benchmarks.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Create Custom Benchmarks
 ************************
 
-There are several reasons to create a custom benchmark.
+There are several reasons to create a *custom* benchmark.
 For example, you want to use your own dataset, your own model, your own scenario or
 your own data splits.
 Creating a benchmark config file is very similar to creating the
 :doc:`Renate config file <../getting_started/how_to_renate_config>`.
 It is not required to build it from scratch but can be build on top of
 :py:mod:`~renate.benchmark.experiment_config` in case you want to reuse parts of the
 Renate benchmarks.
-The main difference is that the object returned by the :code:`model_fn` needs to
-follow a slightly different interface.
 
 
+Your Own Function Arguments
+===========================
+Benchmarking still relies on the functions :code:`model_fn` and :code:`data_module_fn`. You can add further
+arguments as long as you use typing and data of type ``bool``, ``float``, ``int``, ``str``, ``list``, and ``tuple``.
+A more detailed explanation is provided in the
+:ref:`Renate config chapter <getting_started/how_to_renate_config:custom function arguments>`.
+
 Your Own Model
 ==============
 
 If you want to use your own model, simply provide the :code:`model_fn` function as explained in the
 :ref:`Renate config chapter <getting_started/how_to_renate_config:model definition>`.
 
 Your Own Data
@@ -31,20 +36,20 @@
 in the last chapter.
 For example, you can combine the :py:class:`~renate.benchmark.scenarios.ClassIncrementalScenario`
 with your data module as follows.
 
 .. code-block:: python
 
     def data_module_fn(
-        data_path: Union[Path, str], chunk_id: int, seed: int
+        data_path: Union[Path, str], chunk_id: int, seed: int, class_groupings: Tuple[Tuple[int]]
     ):
         data_module = CustomDataModule(data_path=data_path, seed=seed)
         return ClassIncrementalScenario(
             data_module=data_module,
-            class_groupings=[[0, 1], [2, 3]],
+            class_groupings=class_groupings,
             chunk_id=chunk_id,
         )
 
 Please note, that :code:`data_module_fn` takes :code:`chunk_id` as a special argument which indicates
 the partition id. The :code:`chunk_id` will be in range :math:`0\ldots\text{num_updates}-1`
 and indicates the partition that should be loaded as training and validation data.
 
@@ -53,12 +58,13 @@
 =================
 
 If you want to use a custom scenario, create your own class extending
 :py:class:`~renate.benchmark.scenarios.Scenario`.
 You will need to implement :py:meth:`~renate.benchmark.scenarios.Scenario.prepare_data()`
 such that it assigns the right subset of your data to :code:`self._train_data` and
 :code:`self._val_data` based on :code:`self._chunk_id`.
-By default, your model will be evaluated on the entire test data after each update step.
-If you want to change that, please override :py:meth:`~renate.benchmark.scenarios.Scenario.test_data()`
-as well.
-Please check the implementation of :py:class:`~renate.benchmark.scenarios.TransformScenario`
-for an example.
+Assign a list of datasets to :code:`self._test_data` where each entry of the list corresponds to one
+:code:`self._chunk_id`.
+At each update step, your model will be evaluated on the test datasets up to :code:`self._chunk_id`.
+You can modify this behavior to assign different values to :code:`self._test_data`.
+Please check the implementation of :py:class:`~renate.benchmark.scenarios.IIDScenario`
+for a simple example.
```

### Comparing `Renate-0.1.0/doc/benchmarking/index.rst` & `Renate-0.2.0/doc/benchmarking/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Renate provides a feature to simulate continual learning offline.
 By providing a dataset, you will be able to split it into smaller parts and simulate the behavior of updating your model
 on a regular basis.
 Among other things, Renate will support you in evaluating different optimizers, hyperparameters and the expected
 performance on your historic data or public benchmark data.
 At the core of this feature is the function :py:func:`~renate.benchmark.experimentation.execute_experiment_job`.
-For the reader familiar with the function :py:func:`~renate.tuning.tuning.execute_tuning_job`, the use will be very
+For the reader familiar with the function :py:func:`~renate.training.training.run_training_job`, the use will be very
 intuitive.
 
 In the following chapters, we will discuss how this interface can be used to experiment on
 :doc:`Renate benchmarks <renate_benchmarks>` as well as
 :doc:`custom benchmarks <custom_benchmarks>`.
 
 .. toctree::
```

### Comparing `Renate-0.1.0/doc/conf.py` & `Renate-0.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 import os
 import shutil
 import sys
 
 sys.path.insert(0, os.path.abspath("../src/"))
 
-import renate
+import renate  # noqa: E402
 
 
 def run_apidoc(app):
     """Generate doc stubs using sphinx-apidoc."""
     module_dir = os.path.join(app.srcdir, "../src/")
     output_dir = os.path.join(app.srcdir, "_apidoc")
     excludes = []
@@ -48,29 +48,31 @@
     app.connect("builder-inited", run_apidoc)
 
 
 # Sphinx configuration below.
 project = "Renate"
 version = renate.__version__
 release = renate.__version__
-copyright = f"{datetime.datetime.now().year}, Amazon"
+copyright = f"2022-{datetime.datetime.now().year}, Amazon"
 
 
 extensions = [
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.napoleon",
     "sphinx.ext.autodoc",
+    "sphinx_autodoc_typehints",  # typing shown in api reference
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx.ext.coverage",
     "hoverxref.extension",  # show reference preview
     "sphinx_copybutton",
     "sphinxext.opengraph",
+    "sphinx_paramlinks",  # lightning uses it, we get warnings otherwise
 ]
 coverage_show_missing_items = True
 
 # Make sure the target is unique
 autosectionlabel_prefix_document = True
 
 hoverxref_auto_ref = True  # Enable preview for all refs
@@ -84,25 +86,25 @@
 autodoc_member_order = "bysource"
 default_role = "py:obj"
 
 html_theme = "pydata_sphinx_theme"
 html_sidebars = {"**": ["sidebar-nav-bs"]}
 html_theme_options = {
     "primary_sidebar_end": [],
-    "footer_items": ["copyright"],
+    "footer_start": ["copyright"],
+    "footer_end": [],
     "icon_links": [
         {
             "name": "GitHub",
             "url": "https://github.com/awslabs/Renate",  # required
             "icon": "fa-brands fa-square-github",
             "type": "fontawesome",
         }
     ],
     "use_edit_page_button": True,
-    "announcement": "<p>Renate 0.1.0 is released. See you at NeurIPS!</p>",
     "collapse_navigation": True,
 }
 html_context = {
     "github_user": "awslabs",
     "github_repo": "Renate",
     "github_version": "dev",
     "doc_path": "doc",
```

### Comparing `Renate-0.1.0/doc/examples/train_classifier_sagemaker.rst` & `Renate-0.2.0/doc/examples/train_classifier_sagemaker.rst`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,20 @@
     it was useful for us to create a simple example using a single dataset :)
 
 In the :code:`renate_config.py` file we also create some simple transformations to
 normalize and augment the dataset. More transformations can be added if needed,
 details on how to write a configuration file are available in :doc:`../getting_started/how_to_renate_config`.
 
 .. literalinclude:: ../../examples/simple_classifier_cifar10/renate_config.py
+    :lines: 3-
+
+The configuration file uses a scenario in the definition of the data module function.
+The scenario is just splitting the dataset in several chunks and allows us to train the model on
+different parts of the dataset without adding complex code to the example. For most practical purposes
+the definition of the scenario can just be removed from the function.
 
 Training
 ========
 
 The example also contains :code:`start_with_hpo.py`,
 which launches a training job with integrated hyperparameters optimization.
 To this purpose, in the file we define a dictionary containing the
@@ -43,28 +49,31 @@
 in :code:`next_state_url`, to simplify the example in this case we provide two variables
 that can be used to set AWS Account ID and AWS region used, but any accessible S3 bucket can be
 used for storing the output.
 The description of the other arguments and a high level overview of how to run a
 training jobs are available in :doc:`../getting_started/how_to_run_training`.
 
 .. literalinclude:: ../../examples/simple_classifier_cifar10/start_with_hpo.py
+    :lines: 3-
 
 Once the training job terminates, the output will be available in the S3 bucket indicated
 in :code:`next_state_url`. For more information about how to interpret the output, see
 :doc:`../getting_started/output`.
 
 To simulate an application where data are made available incrementally over time,
 after the first training job has been executed, it is possible to re-train the model
 on the second chunk of the dataset that we left intentionally untouched during
 the first training process.
 
-To do this, it is sufficient to modifying the arguments passed to the :code:`execute_tuning_job` function.
+To do this, it is sufficient to modifying the arguments passed to the :py:func:`~renate.training.training.run_training_job` function.
 In particular:
 
 1. select the second part of the datasets by setting :code:`chunk-id = 1`.
 
 2. load the model trained in the first training job by adding the :code:`state_url`
 argument pointing to the same S3 location. In this case it will be useful to change the
 url for the :code:`next_state_url` to avoid overwriting the old artefacts.
 
-
+Note that in our example we specified :code:`requirements_file="requirements.txt"`
+even if it is not necessary since the only dependency in the file is Renate itself.
+The only purpose of this is to show how additional dependencies can be added when needed.
```

### Comparing `Renate-0.1.0/doc/examples/train_mlp_locally.rst` & `Renate-0.2.0/doc/examples/train_mlp_locally.rst`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 In the :code:`renate_config.py` file we also create a simple transformation flattening
 the input images (matrices 28x28) into vectors. Transformations do not provide
 only the ability to reshape the inputs, but they can be used for normalization,
 augmentation, and several other purposes. More details on how to write a
 configuration file are available in :doc:`../getting_started/how_to_renate_config`.
 
 .. literalinclude:: ../../examples/train_mlp_locally/renate_config.py
+    :lines: 3-
+    
+The configuration file uses a scenario in the definition of the data module function.
+The scenario is just splitting the dataset in several chunks and allows us to train the model on
+different parts of the dataset without adding complex code to the example. For most practical purposes
+the definition of the scenario can be removed from the function.
 
 Training
 ========
 
 The example also contains :code:`start_training_without_hpo.py`,
 which is the one launching the training jobs. In the file we defined a
 configuration using the :code:`config_space` dictionary and pass it to
@@ -41,14 +47,15 @@
 There are also parameters that we pass directly like
 the folder in which the learner state will be saved (via :code:`next_state_url`).
 In order to update an existing model, it will also be necessary to provide the path
 to the previously saved state using :code:`state_url`, as done in our example.
 More details about running training jobs are available in :doc:`../getting_started/how_to_run_training`.
 
 .. literalinclude:: ../../examples/train_mlp_locally/start_training_without_hpo.py
+    :lines: 3-
 
 Results
 =======
 
 The results obtained by running this simple example are usually quite good
 with an almost-perfect accuracy on the first chunk of data and an accuracy
 still above 90% after processing the second one.
```

### Comparing `Renate-0.1.0/doc/getting_started/how_to_run_training.rst` & `Renate-0.2.0/doc/getting_started/how_to_run_training.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 How to Run a Training Job
 *************************
 
 Renate offers possibility to run training jobs using both CLIs and functions that can be called
 programmatically in python. The best choice may be different depending on the requirements (e.g.,
 a CLI can be convenient to run remote jobs). In the following we illustrate the solution that we
 find to be the simplest and more convenient. The complete documentation is available in
-:py:func:`~renate.tuning.tuning.execute_tuning_job`.
+:py:func:`~renate.training.training.run_training_job`.
 
 
 Setup
 =====
 
 The first step that needs to be completed before running a training job is to define which model needs
 to be trained and on which data. This is explained in :doc:`how_to_renate_config`.
 
 Once completed the first step, a simple way to run a training job is to use the
-:py:func:`~renate.tuning.tuning.execute_tuning_job`,
+:py:func:`~renate.training.training.run_training_job`,
 this can work for most training needs: it can launch trainings with and without HPO,
 either locally or on Amazon SageMaker.
 
 
 Run a local training job
 ========================
 
@@ -44,42 +44,43 @@
         "memory_batch_size": 32,
         "memory_size": 500,
     }
 
 
 
 Once the configuration of the learning algorithm is specified, we need to set another couple of arguments
-in the :py:func:`~renate.tuning.tuning.execute_tuning_job` function to make sure we obtain the desired behavior:
+in the :py:func:`~renate.training.training.run_training_job` function to make sure we obtain the desired behavior:
 
 * :code:`mode`: it can be either :code:`min` or :code:`max` and define if the aim is to minimize or maximize the metric
 * :code:`metric`: it is the target metric. Metrics measured on the validation set are prefixed with :code:`val_`,
   while the ones measured on the training set are prefixed with :code:`train_`. Mode an metric will be used to checkpoint
   the best model if a validation set is provided, otherwise do not pass these arguments.
 * :code:`updater`: the name of the algorithm to be used for updating the model. See :doc:`supported_algorithms` for more info.
 * :code:`max_epochs`: the maximum number of training epochs.
-* :code:`state_url`: this is the location at which the state of learner and the model to be updated are made available.
+* :code:`input_state_url`: this is the location at which the state of learner and the model to be updated are made available.
   If this argument is not passed, the model will be trained from scratch.
-* :code:`next_state_url`: this is the location at which the output of the training job (e.g., model, state) will be stored.
+* :code:`output_state_url`: this is the location at which the output of the training job (e.g., model, state) will be stored.
 * :code:`backend`: when set to :code:`local` will run the training job on the local machine
 
 In both cases the urls can point to local folders or S3 locations.
 
 Putting everything together will result in a script like the following.
 
 .. literalinclude:: ../../examples/train_mlp_locally/start_training_with_er_without_hpo.py
+    :lines: 3-
 
 Once the training has been executed you will see some metrics printed on the screen (e.g., validation accuracy)
 and you will find the output of the training process in the folder specified. For more information about the
 output see :doc:`output`.
 
 Run a training job on SageMaker
 ===============================
 
 Running a job on SageMaker is very similar to run the training job locally, but it will require a few changes
-to the arguments passed to :py:func:`~renate.tuning.tuning.execute_tuning_job`:
+to the arguments passed to :py:func:`~renate.training.training.run_training_job`:
 
 * :code:`backend`: the backend will have to be set to :code:`sagemaker`.
 * :code:`role`: an `execution role <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`_ will need to be passed.
 * :code:`instance_type`: the type of machine to be used for the training. AWS provides a `list of training instances available <https://aws.amazon.com/sagemaker/pricing/>`_.
 * :code:`job_name`: (optional) a prefix used to name the training job to make it recognizable in the SageMaker jobs list.
 
 When using the SageMaker training you should use a S3 location as :code:`next_state_url` to make sure
@@ -111,32 +112,55 @@
     }
 
 
 
 For more suggestions and details about how to design a search space,
 see the `Syne Tune documentation <https://github.com/awslabs/syne-tune/blob/main/docs/search_space.md>`_.
 If you do not know which search space to use, you can adopt a default one by calling
-:py:func:`~renate.tuning.config_spaces.config_space` and passing the name of your algorithm to it.
+:py:func:`~renate.utils.config_spaces.config_space` and passing the name of your algorithm to it.
 
 .. code-block:: python
 
-    from renate.tuning.config_spaces import config_space
+    from renate.utils.config_spaces import config_space
 
     config_space("ER")
 
 After configuring the search space, it will be sufficient to add a few more arguments to
-the :py:func:`~renate.tuning.tuning.execute_tuning_job` function.
+the :py:func:`~renate.training.training.run_training_job` function.
 To start, please make sure that :code:`mode` and :code:`metric` (already introduced above) reflect your aim.
 Also, please make sure that in :code:`data_module_fn` a reasonable
 fraction of the data is assigned to the validation set, otherwise it will not be possible to measure validation performance reliably
 (:code:`val_size` is controlling that).
 
 It also possible to define more aspects of the HPO process:
 
 * :code:`n_workers`: the number of workers evaluating configurations in parallel (useful for multi-cpu or multi-gpu machines).
 * :code:`scheduler`: to decide which optimizer to use for the hyperparameters (e.g., "bo", "asha").
 * specify one of the stopping criteria available, for example :code:`max_time` stops the tuning job after a certain amount of time.
 
 After defining these arguments it will be sufficient to run the script and wait :)
-The output will be available in the location specified in :code:`next_state_url`.
+The output will be available in the location specified in :code:`output_state_url`.
 
 We provide an example of training on SageMaker with HPO at :doc:`../examples/train_classifier_sagemaker`.
+
+Custom Function Arguments
+=========================
+Now that we know how to run basic training jobs, we can discuss how to use custom defined function arguments.
+We are building upon the linear model example introduced in the
+:ref:`previous chapter <getting_started/how_to_renate_config:custom function arguments>` where we added
+``num_inputs`` and ``num_outputs`` to :code:`data_module_fn`.
+The values for these inputs are passed via the configuration alongside the other arguments.
+
+.. code-block:: python
+
+    config_space = {
+        # Define all remaining standard arguments as well
+        "num_inputs": 28 * 28,
+        "num_outputs": 10,
+    }
+
+While it does not make any sense for this example, we can also define ranges for our custom function arguments and
+automatically optimize them during hyperparameter optimization.
+
+.. note::
+    If you have functions defined with the same argument name, the value defined in the configuration will be passed
+    to both.
```

### Comparing `Renate-0.1.0/doc/getting_started/output.rst` & `Renate-0.2.0/doc/getting_started/output.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 .. list-table:: Renate Dataset Overview
     :header-rows: 1
 
     * - File
       - Description
     * - model.ckpt
       - This is the checkpoint of the trained model and the only file required for deployment.
-        Use and [load this file](#loading-the-updated-model) to make predictions.
+        Use and `load this file <loading the updated model_>`_ to make predictions.
     * - learner.ckpt
       - This contains the state of the Renate updater. Only used by Renate.
     * - hpo.csv
       - A summary of all previous updates. The :code:`update_id` with highest value refers to the last update step.
         Among other things, it contains information about selected hyperparameters and logged metrics.
         It might be used in the next update step to accelerate the hyperparameter tuning step.
 
 Loading the Updated Model
 =========================
 
-In the following, we refer with :code:`model_fn` to the function defined by the user in the [Renate config file](./how_to_renate_config.rst).
+In the following, we refer with :code:`model_fn` to the function defined by the user in the
+:doc:`Renate config file <how_to_renate_config>`.
 
 Output Saved Locally
 ~~~~~~~~~~~~~~~~~~~~
 
 If :code:`next_state_url` is a path to a local folder, loading the updated model can be done as follows:
 
 .. code-block:: python
```

### Comparing `Renate-0.1.0/doc/getting_started/supported_algorithms.rst` & `Renate-0.2.0/doc/getting_started/supported_algorithms.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Supported Algorithms
 ********************
 
 Renate provides implementations of various continual learning methods. The following table provides
 an overview with links to the documentation, and a short description. When initiating model updates
-using Renate (e.g., using :py:func:`renate.tuning.tuning.execute_tuning_job`; see
+using Renate (e.g., using :py:func:`~renate.training.training.run_training_job`; see
 :doc:`how_to_run_training`), a method may be selected using the shorthand provided below.
 
 .. list-table:: Supported Algorithms
    :header-rows: 1
 
    * - Shorthand
      - Implementation
@@ -17,19 +17,34 @@
      - A simple replay-based method, where the model is finetuned using minibatches combining new data and points sampled from a rehearsal memory. The memory is updated after each minibatch. [`Paper <https://arxiv.org/abs/1902.10486>`__]
    * - ``"DER"``
      - :py:class:`DarkExperienceReplayLearner <renate.updaters.experimental.er.DarkExperienceReplayLearner>`
      - A version of experience replay which augments the loss by a distillation term using logits produced by previous model states. The implementation also includes the DER++ variant of the algorithm. [`Paper <https://arxiv.org/abs/2004.07211>`__]
    * - ``"Super-ER"``
      - :py:class:`SuperExperienceReplayLearner <renate.updaters.experimental.er.SuperExperienceReplayLearner>`
      - An experimental method combining various of the ER variants listed above.
-   * - ``"OfflineER"``
+   * - ``"Offline-ER"``
      - :py:class:`OfflineExperienceReplayLearner <renate.updaters.experimental.offline_er.OfflineExperienceReplayLearner>`
      - An offline version of experience replay, where the rehearsal memory is only updated at the end of training.
    * - ``"RD"``
      - :py:class:`RepeatedDistillationLearner <renate.updaters.experimental.repeated_distill.RepeatedDistillationLearner>`
      - A distillation-based method inspired by (but not identical to) Deep Model Consolidation. An expert model is trained on the new data and then combined with the previous model state in a distillation phase. [`DMC Paper <https://arxiv.org/abs/1903.07864>`__]
    * - ``"GDumb"``
      - :py:class:`GDumbLearner <renate.updaters.experimental.gdumb.GDumbLearner>`
      - A strong baseline that trains the model from scratch on a memory, which is maintained using a greedy class-balancing strategy. [`Paper <https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123470511.pdf>`__]
    * - ``"Joint"``
      - :py:class:`JointLearner <renate.updaters.experimental.joint.JointLearner>`
-     - Retraining from scratch on all data seen so far. Used as an "upper bound" in experiments, inefficient for practical use.
+     - This method retrains a randomly initialized model each time from scratch on all data seen so far. Used as "upper bound" in experiments, inefficient for practical use.
+   * - ``"FineTuning"``
+     - :py:class:`Learner <renate.updaters.learner.Learner>`
+     - A simple method which trains the current model on only the new data without any sort of mitigation for forgetting. Used as "lower bound" baseline in experiments.
+   * - ``"Avalanche-ER"``
+     - :py:class:`AvalancheReplayLearner <renate.updaters.avalanche.learner.AvalancheReplayLearner>`
+     - A wrapper which gives access to Experience Replay as implemented in the Avalanche library. This method is the equivalent to our Offline-ER.
+   * - ``"Avalanche-EWC"``
+     - :py:class:`AvalancheEWCLearner <renate.updaters.avalanche.learner.AvalancheEWCLearner>`
+     - A wrapper which gives access to Elastic Weight Consolidation as implemented in the Avalanche library. EWC updates the model in such a way that the parameters after the update remain close to the parameters before the update to avoid catastrophic forgetting. [`Paper <https://arxiv.org/abs/1612.00796>`__]
+   * - ``"Avalanche-LwF"``
+     - :py:class:`AvalancheLwFLearner <renate.updaters.avalanche.learner.AvalancheLwFLearner>`
+     - A wrapper which gives access to Learning without Forgetting as implemented in the Avalanche library. LwF does not require to retain old data. It assumes that each new data chunk is its own task. A common backbone is shared across all task and each task has its own prediction head. [`Paper <https://arxiv.org/abs/1606.09282>`__]
+   * - ``"Avalanche-iCaRL"``
+     - :py:class:`AvalancheICaRLLearner <renate.updaters.avalanche.learner.AvalancheICaRLLearner>`
+     - A wrapper which gives access to iCaRL as implemented in the Avalanche library. This method is limited to class-incremental learning and combines knowledge distillation with nearest neighbors classification. [`Paper <https://arxiv.org/abs/1611.07725>`__]
```

### Comparing `Renate-0.1.0/examples/benchmarking/class_incremental_learning_cifar10_der.py` & `Renate-0.2.0/examples/benchmarking/class_incremental_learning_cifar10_der.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,31 @@
+# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 from renate.benchmark.experimentation import execute_experiment_job, experiment_config_file
 
 
-def to_dense_str(value):
-    return str(value).replace(" ", "")
-
-
-dataset_name = "CIFAR10"
 config_space = {
     "updater": "DER",
     "optimizer": "SGD",
     "momentum": 0.0,
     "weight_decay": 0.0,
     "learning_rate": 0.03,
     "alpha": 0.2,
     "beta": 0.5,
     "batch_size": 32,
     "memory_batch_size": 32,
     "memory_size": 500,
     "max_epochs": 50,
     "loss_normalization": 0,
     "loss_weight": 1.0,
-    "model_fn_model_name": "ResNet18CIFAR",
-    "data_module_fn_scenario_name": "ClassIncrementalScenario",
-    "data_module_fn_dataset_name": dataset_name,
-    "data_module_fn_val_size": 0,
-    "data_module_fn_class_groupings": to_dense_str([[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]),
-    "transform_dataset_name": dataset_name,
+    "model_name": "ResNet18CIFAR",
+    "scenario_name": "ClassIncrementalScenario",
+    "dataset_name": "CIFAR10",
+    "val_size": 0,
+    "class_groupings": ((0, 1), (2, 3), (4, 5), (6, 7), (8, 9)),
 }
 
 for seed in range(10):
     execute_experiment_job(
         backend="local",
         config_file=experiment_config_file(),
         config_space=config_space,
```

### Comparing `Renate-0.1.0/examples/getting_started/renate_config.py` & `Renate-0.2.0/examples/getting_started/renate_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from pathlib import Path
-from typing import Callable, Literal, Optional, Union
+# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
+from typing import Callable, Dict, Literal, Optional
 
 import torch
 import torchvision
+from torchmetrics import Accuracy
 from torchvision.transforms import transforms
 
 from renate.data.data_module import RenateDataModule
 from renate.models import RenateModule
 
 
 class MyMNISTMLP(RenateModule):
@@ -21,28 +23,29 @@
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self._fc1(x)
         x = torch.nn.functional.relu(x)
         return self._fc2(x)
 
 
-def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
     if model_state_url is None:
-        # If no model state is given, we create the model from scratch with initial model hyperparameters.
+        # If no model state is given, we create the model from scratch with initial model
+        # hyperparameters.
         model = MyMNISTMLP(num_hidden=100)
     else:
         # If a model state is passed, we reload the model using PyTorch's load_state_dict.
         # In this case, model hyperparameters are restored from the saved state.
-        state_dict = torch.load(str(model_state_url))
+        state_dict = torch.load(model_state_url)
         model = MyMNISTMLP.from_state_dict(state_dict)
     return model
 
 
 class MyMNISTDataModule(RenateDataModule):
-    def __init__(self, data_path: Union[Path, str], val_size: float, seed: int = 42) -> None:
+    def __init__(self, data_path: str, val_size: float, seed: int = 42) -> None:
         super().__init__(data_path, val_size=val_size, seed=seed)
 
     def prepare_data(self) -> None:
         # This is only to download the data. We separate downloading from the remaining set-up to
         # streamline data loading when using multiple training jobs during HPO.
         torchvision.datasets.MNIST(self._data_path, download=True)
 
@@ -62,15 +65,15 @@
                 self._data_path,
                 train=False,
                 transform=transforms.ToTensor(),
                 target_transform=transforms.Lambda(lambda x: torch.tensor(x, dtype=torch.long)),
             )
 
 
-def data_module_fn(data_path: Union[Path, str], seed: int) -> RenateDataModule:
+def data_module_fn(data_path: str, seed: int) -> RenateDataModule:
     return MyMNISTDataModule(val_size=0.2, seed=seed)
 
 
 def train_transform() -> Callable:
     return torchvision.transforms.Compose(
         [torchvision.transforms.RandomCrop((28, 28), padding=4), torch.nn.Flatten()]
     )
@@ -84,7 +87,11 @@
     return torchvision.transforms.Compose(
         [
             torchvision.transforms.RandomCrop((28, 28), padding=4),
             torchvision.transforms.RandomRotation(degrees=15),
             torch.nn.Flatten(),
         ]
     )
+
+
+def metrics_fn() -> Dict:
+    return {"my_accuracy": Accuracy()}
```

### Comparing `Renate-0.1.0/examples/simple_classifier_cifar10/renate_config.py` & `Renate-0.2.0/examples/simple_classifier_cifar10/renate_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
-from typing import Optional, Union
+from typing import Callable, Optional, Union
 
 import torch
 from torchvision import transforms
 
 import renate.defaults as defaults
 from renate.benchmark.datasets.vision_datasets import TorchVisionDataModule
-from renate.benchmark.models.resnet import ResNet18CIFAR
+from renate.benchmark.models import ResNet18CIFAR
 from renate.benchmark.scenarios import ClassIncrementalScenario, Scenario
 from renate.models import RenateModule
 
 
 def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
     """Returns a model instance."""
     if model_state_url is None:
         model = ResNet18CIFAR()
     else:
         state_dict = torch.load(str(model_state_url))
         model = ResNet18CIFAR.from_state_dict(state_dict)
     return model
 
 
-def data_module_fn(
-    data_path: Union[Path, str], chunk_id: int, seed: int = defaults.SEED
-) -> Scenario:
+def data_module_fn(data_path: str, chunk_id: int, seed: int = defaults.SEED) -> Scenario:
     """Returns a class-incremental scenario instance.
 
     The transformations passed to prepare the input data are required to convert the data to
     PyTorch tensors.
     """
     data_module = TorchVisionDataModule(
-        str(data_path),
+        data_path,
         dataset_name="CIFAR10",
         val_size=0.2,
         seed=seed,
     )
     class_incremental_scenario = ClassIncrementalScenario(
         data_module=data_module,
         class_groupings=[[0, 1, 2, 3, 4], [5, 6, 7, 8, 9]],
         chunk_id=chunk_id,
     )
     return class_incremental_scenario
 
 
-def train_transform() -> transforms.Compose:
+def train_transform() -> Callable:
     """Returns a transform function to be used in the training."""
     return transforms.Compose(
         [
             transforms.RandomCrop(32, padding=4),
             transforms.RandomHorizontalFlip(),
             transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2470, 0.2435, 0.2615)),
         ]
     )
 
 
-def test_transform() -> transforms.Compose:
+def test_transform() -> Callable:
     """Returns a transform function to be used for validation or testing."""
     return transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2470, 0.2435, 0.2615))
 
 
-def buffer_transform() -> transforms.Compose:
+def buffer_transform() -> Callable:
     """Returns a transform function to be used in the Memory Buffer."""
     return train_transform()
```

### Comparing `Renate-0.1.0/examples/simple_classifier_cifar10/start_with_hpo.py` & `Renate-0.2.0/examples/simple_classifier_cifar10/start_with_hpo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-
+import boto3
 from syne_tune.backend.sagemaker_backend.sagemaker_utils import get_execution_role
 from syne_tune.config_space import choice, loguniform, uniform
 
-from renate.tuning import execute_tuning_job
+from renate.training import run_training_job
 
 config_space = {
     "optimizer": "SGD",
     "momentum": uniform(0.1, 0.9),
     "weight_decay": 0.0,
     "learning_rate": loguniform(1e-4, 1e-1),
     "alpha": uniform(0.0, 1.0),
@@ -16,34 +16,37 @@
     "memory_batch_size": 32,
     "memory_size": 1000,
     "loss_normalization": 0,
     "loss_weight": uniform(0.0, 1.0),
 }
 
 if __name__ == "__main__":
-
-    AWS_ID = "0123456789"  # use your AWS account id here
+    AWS_ID = boto3.client("sts").get_caller_identity().get("Account")
     AWS_REGION = "us-west-2"  # use your AWS preferred region here
 
-    execute_tuning_job(
+    run_training_job(
         config_space=config_space,
         mode="max",
         metric="val_accuracy",
         updater="ER",  # we train with Experience Replay
         max_epochs=50,
-        chunk_id=0,  # we select the first chunk of our dataset, you will probably not need this in practice
+        # we select the first chunk of our dataset, you will probably not need this in practice
+        chunk_id=0,
         config_file="renate_config.py",
         requirements_file="requirements.txt",
-        # replace the url below with a different one if you already ran it and you want to avoid overwriting
-        next_state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-training-cifar10-1st-model/",
-        # uncomment the line below only if you already created a model with this script and you want to update it
-        # state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-training-cifar10-1st-model/",
-        backend="sagemaker",  # we will run this on SageMaker, but you can select "local" to run this locally
+        # replace the url below with a different one if you already ran it and you want to avoid
+        # overwriting
+        output_state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-cifar10/",
+        # uncomment the line below only if you already created a model with this script and you want
+        # to update it
+        # input_state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-cifar10/",
+        backend="sagemaker",  # run on SageMaker, select "local" to run this locally
         role=get_execution_role(),
         instance_count=1,
         instance_type="ml.g4dn.xlarge",
         max_num_trials_finished=100,
-        scheduler="asha",  # we will run ASHA to optimize our hyperparameters
-        # if you use a big instance with multiple GPUs you can multiple workers evaluating configuration in parallel
+        scheduler="asha",  # run ASHA to optimize our hyperparameters
+        # if you use a big instance with multiple GPUs you can multiple workers evaluating
+        # configuration in parallel
         # n_workers=4,
-        job_name="job_name",
+        job_name="job-name",
     )
```

### Comparing `Renate-0.1.0/examples/simple_classifier_cifar10/start_without_hpo.py` & `Renate-0.2.0/examples/simple_classifier_cifar10/start_without_hpo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-
+import boto3
 from syne_tune.backend.sagemaker_backend.sagemaker_utils import get_execution_role
 
-from renate.tuning import execute_tuning_job
+from renate.training import run_training_job
 
 config_space = {
     "optimizer": "SGD",
     "momentum": 0.0,
     "weight_decay": 0.0,
     "learning_rate": 0.1,
     "alpha": 0.5,
@@ -15,30 +15,32 @@
     "memory_batch_size": 32,
     "memory_size": 300,
     "loss_normalization": 0,
     "loss_weight": 0.5,
 }
 
 if __name__ == "__main__":
-
-    AWS_ID = "0123456789"  # use your AWS account id here
+    AWS_ID = boto3.client("sts").get_caller_identity().get("Account")
     AWS_REGION = "us-west-2"  # use your AWS preferred region here
 
-    execute_tuning_job(
+    run_training_job(
         config_space=config_space,
         mode="max",
         metric="val_accuracy",
         updater="ER",  # we train with Experience Replay
         max_epochs=50,
-        chunk_id=0,  # we select the first chunk of our dataset, you will probably not need this in practice
+        # we select the first chunk of our dataset, you will probably not need this in practice
+        chunk_id=0,
         config_file="renate_config.py",
         requirements_file="requirements.txt",
-        # replace the url below with a different one if you already ran it and you want to avoid overwriting
-        next_state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-training-cifar10-1st-model/",
-        # uncomment the line below only if you already created a model with this script and you want to update it
-        # state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-training-cifar10-1st-model/",
-        backend="sagemaker",  # we will run this on SageMaker, but you can select "local" to run this locally
+        # replace the url below with a different one if you already ran it and you want to avoid
+        # overwriting
+        output_state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-cifar10/",
+        # uncomment the line below only if you already created a model with this script and you want
+        # to update it
+        # input_state_url=f"s3://sagemaker-{AWS_REGION}-{AWS_ID}/renate-cifar10/",
+        backend="sagemaker",  # run on SageMaker, select "local" to run this locally
         role=get_execution_role(),
         instance_count=1,
         instance_type="ml.g4dn.xlarge",
-        job_name="job_name",
+        job_name="job-name",
     )
```

### Comparing `Renate-0.1.0/examples/train_mlp_locally/renate_config.py` & `Renate-0.2.0/examples/train_mlp_locally/renate_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
-from typing import Union, Optional
+from typing import Callable, Optional, Union
 
 import torch
 from torchvision.transforms import transforms
 
-from renate.benchmark.models.mlp import MultiLayerPerceptron
-
-from renate.models import RenateModule
-
 from renate import defaults
 from renate.benchmark.datasets.vision_datasets import TorchVisionDataModule
+from renate.benchmark.models.mlp import MultiLayerPerceptron
 from renate.benchmark.scenarios import ClassIncrementalScenario, Scenario
+from renate.models import RenateModule
 
 
-def data_module_fn(
-    data_path: Union[Path, str], chunk_id: int, seed: int = defaults.SEED
-) -> Scenario:
+def data_module_fn(data_path: str, chunk_id: int, seed: int = defaults.SEED) -> Scenario:
     """Returns a class-incremental scenario instance.
 
     The transformations passed to prepare the input data are required to convert the data to
     PyTorch tensors.
     """
     data_module = TorchVisionDataModule(
-        str(data_path),
+        data_path,
         dataset_name="MNIST",
         val_size=0.1,
         seed=seed,
     )
 
     class_incremental_scenario = ClassIncrementalScenario(
         data_module=data_module,
@@ -44,10 +42,10 @@
         )
     else:
         state_dict = torch.load(str(model_state_url))
         model = MultiLayerPerceptron.from_state_dict(state_dict)
     return model
 
 
-def train_transform() -> transforms.Compose:
+def train_transform() -> Callable:
     """Returns a transform function to be used in the training."""
     return transforms.Lambda(lambda x: torch.flatten(x))
```

### Comparing `Renate-0.1.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py` & `Renate-0.2.0/examples/train_mlp_locally/start_training_with_er_without_hpo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from renate.tuning import execute_tuning_job
+# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
+from renate.training import run_training_job
 
 configuration = {
     "optimizer": "SGD",
     "momentum": 0.0,
     "weight_decay": 1e-2,
     "learning_rate": 0.05,
     "batch_size": 32,
     "max_epochs": 50,
     "memory_batch_size": 32,
     "memory_size": 500,
 }
 
 if __name__ == "__main__":
-
-    execute_tuning_job(
+    run_training_job(
         config_space=configuration,
         mode="max",
         metric="val_accuracy",
         updater="ER",
         max_epochs=50,
         chunk_id=0,
         config_file="renate_config.py",
-        next_state_url="./output_folder/",  # this is where the model will be stored
+        output_state_url="./output_folder/",  # this is where the model will be stored
         backend="local",  # the training job will run on the local machine
     )
```

### Comparing `Renate-0.1.0/examples/train_mlp_locally/start_training_with_hpo.py` & `Renate-0.2.0/examples/train_mlp_locally/start_training_with_hpo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-from renate.tuning import execute_tuning_job
-from renate.tuning.config_spaces import config_space
+# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
+from renate.training import run_training_job
+from renate.utils.config_spaces import config_space
 
 if __name__ == "__main__":
-
     # we run the first training job on the MNIST classes [0-4]
-    execute_tuning_job(
+    run_training_job(
         config_space=config_space("RD"),  # getting the default search space
         mode="max",
         metric="val_accuracy",
         updater="RD",  # use the RepeatedDistillationModelUpdater
         max_epochs=50,
         chunk_id=0,  # this selects the first chunk of the dataset
         config_file="renate_config.py",
-        next_state_url="./state_dump_first_model_rd/",  # this is where the model will be stored
+        # location where the new model is saved to
+        output_state_url="./state_dump_first_model_rd/",
         backend="local",  # the training job will run on the local machine
         scheduler="asha",
-        # using only 5 trials will not give great performance but this is just an example
+        # using only 5 trials will not give great performance -- just an example
         max_num_trials_finished=5,
     )
 
-    # retrieve the model from `./state_dump_first_model_rd/` if you want -- don't delete it
+    # retrieve the model from `./state_dump_first_model_rd/` if you want
+    # do not delete it, we will need it in the remaining of this example
 
-    execute_tuning_job(
+    run_training_job(
         config_space=config_space("RD"),
         mode="max",
         metric="val_accuracy",
         updater="RD",
         max_epochs=50,
         chunk_id=1,  # this time we use the second chunk of the dataset
         config_file="renate_config.py",
-        state_url="./state_dump_first_model_rd/",  # the output of the first training job is loaded
-        next_state_url="./state_dump_second_model_rd/",  # the new model will be stored in this folder
+        # the output of the first training job is loaded
+        input_state_url="./state_dump_first_model_rd/",
+        # location where the new model is saved to
+        output_state_url="./state_dump_second_model_rd/",
         backend="local",
         scheduler="asha",
         max_num_trials_finished=5,
     )
```

### Comparing `Renate-0.1.0/examples/train_mlp_locally/start_training_without_hpo.py` & `Renate-0.2.0/examples/train_mlp_locally/start_training_without_hpo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-from renate.tuning import execute_tuning_job
+# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# SPDX-License-Identifier: Apache-2.0
+from renate.training import run_training_job
 
 
 config_space = {
     "optimizer": "SGD",
     "momentum": 0.0,
     "weight_decay": 0.0,
     "learning_rate": 0.1,
     "alpha": 0.5,
     "batch_size": 32,
     "memory_batch_size": 32,
     "memory_size": 500,
     "loss_normalization": 0,
     "loss_weight": 0.5,
-    "enable_early_stopping": True,
+    "early_stopping": True,
 }
 
 if __name__ == "__main__":
-
     # we run the first training job on the MNIST classes [0-4]
-    execute_tuning_job(
+    run_training_job(
         config_space=config_space,
         mode="max",
         metric="val_accuracy",
         updater="ER",
         max_epochs=50,
         chunk_id=0,  # this selects the first chunk of the dataset
         config_file="renate_config.py",
-        next_state_url="./state_dump_first_model/",  # this is where the model will be stored
-        backend="local",  # the training job will run on the local machine
+        # this is where the model will be stored
+        output_state_url="./state_dump_first_model/",
+        # the training job will run on the local machine
+        backend="local",
     )
 
-    # retrieve the model from `./state_dump_first_model/` if you want -- don't delete it
+    # retrieve the model from `./state_dump_first_model/` if you want
+    # do not delete the model, we are going to use it below
 
-    execute_tuning_job(
+    run_training_job(
         config_space=config_space,
         mode="max",
         metric="val_accuracy",
         updater="ER",
         max_epochs=50,
         chunk_id=1,  # this time we use the second chunk of the dataset
         config_file="renate_config.py",
-        state_url="./state_dump_first_model/",  # the output of the first training job is loaded
-        next_state_url="./state_dump_second_model/",  # the new model will be stored in this folder
+        # the output of the first training job is loaded
+        input_state_url="./state_dump_first_model/",
+        # the new model will be stored in this folder
+        output_state_url="./state_dump_second_model/",
         backend="local",
     )
```

### Comparing `Renate-0.1.0/pyproject.toml` & `Renate-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -9,24 +9,30 @@
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
 ]
-requires-python = ">=3.8, <=3.10"
+requires-python = ">=3.8, <3.11"
 dynamic = ["version", "readme", "dependencies"]
 
 [project.optional-dependencies]
+avalanche = [
+    "avalanche_lib==0.3.1",
+    "torch>=1.10.0, <1.12.2",
+]
 dev = [
-    "black",
+    "black==23.1.0",
+    "avalanche_lib==0.3.1",
+    "torch>=1.10.0, <1.12.2",
     # PyTest Dependencies
-    "pytest>=7.0, <=7.1.2",
-    "pytest-cov <=3.0.0",
-    "pytest-helpers-namespace",
+    "pytest==7.2.2",
+    "pytest-cov==4.0.0",
+    "pytest-helpers-namespace==2021.12.29",
     ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
 version = {attr = "renate.__version__"}
@@ -35,11 +41,12 @@
 
 [tool.black]
 line-length = 100
 target-version = ["py38", "py39", "py310"]
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
-addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 80"
+addopts = "--cov --cov-fail-under 80"
 
 [tool.coverage.run]
 source = ["src"]
+relative_files = true
```

### Comparing `Renate-0.1.0/src/Renate.egg-info/PKG-INFO` & `Renate-0.2.0/src/Renate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,128 @@
 Metadata-Version: 2.1
 Name: Renate
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library for Continual Learning for Practitioners
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <=3.10,>=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: avalanche
 Provides-Extra: dev
 License-File: LICENSE
+License-File: NOTICE
 
 .. image:: https://img.shields.io/pypi/status/Renate
+    :target: #
     :alt: PyPI - Status
 .. image:: https://img.shields.io/github/v/release/awslabs/Renate
+    :target: https://github.com/awslabs/Renate/releases/tag/v0.1.0
     :alt: Latest Release
 .. image:: https://img.shields.io/pypi/dm/Renate
-   :alt: PyPI - Downloads
+    :target: https://pypistats.org/packages/renate
+    :alt: PyPI - Downloads
 .. image:: https://img.shields.io/github/license/awslabs/Renate
     :target: https://github.com/awslabs/Renate/blob/main/LICENSE
     :alt: License
 .. image:: https://readthedocs.org/projects/renate/badge/?version=latest
     :target: https://renate.readthedocs.io
     :alt: Documentation Status
+.. image:: https://raw.githubusercontent.com/awslabs/Renate/python-coverage-comment-action-data/badge.svg
+    :target: https://htmlpreview.github.io/?https://github.com/awslabs/Renate/blob/python-coverage-comment-action-data/htmlcov/index.html
+    :alt: Coverage Badge
 
-Renate - Automatic Neural Networks Retraining and Continual Learning in Python
+Renate: Automatic Neural Networks Retraining and Continual Learning in Python
 ******************************************************************************
 
 Renate is a Python package for automatic retraining of neural networks models.
 It uses advanced Continual Learning and Lifelong Learning algorithms to achieve this purpose. 
 The implementation is based on `PyTorch <https://pytorch.org>`_
 and `Lightning <https://www.pytorchlightning.ai>`_ for deep learning, and
 `Syne Tune <https://github.com/awslabs/syne-tune>`_ for hyperparameter optimization.
 
+Quick links
+===========
+* Install renate with ``pip install renate`` or look at `these instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
+* Examples for `local training <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_ and `training on Amazon SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_.
+* `Documentation <https://renate.readthedocs.io>`_
+* `Supported Algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
+
 
 Who needs Renate?
 =================
 
 In many applications data is made available over time and retraining from scratch for
 every new batch of data is prohibitively expensive. In these cases, we would like to use
 the new batch of data provided to update our previous model with limited costs.
 Unfortunately, since data in different chunks is not sampled according to the same distribution,
 just fine-tuning the old model creates problems like *catastrophic forgetting*.
 The algorithms in Renate help mitigating the negative impact of forgetting and increase the 
 model performance overall. 
 
 .. figure:: https://raw.githubusercontent.com/awslabs/Renate/main/doc/_images/improvement_renate.svg
-    :scale: 80%
     :align: center
     :alt: Renate vs Model Fine-Tuning.
 
     Renate's update mechanisms improve over naive fine-tuning approaches. [#]_
 
 Renate also offers hyperparameter optimization (HPO), a functionality that can heavily impact
 the performance of the model when continuously updated. To do so, Renate employs
 `Syne Tune <https://github.com/awslabs/syne-tune>`_ under the hood, and can offer
 advanced HPO methods such multi-fidelity algorithms (ASHA) and transfer learning algorithms
 (useful for speeding up the retuning).
 
 .. figure:: https://raw.githubusercontent.com/awslabs/Renate/main/doc/_images/improvement_tuning.svg
-    :scale: 80%
     :align: center
     :alt: Impact of HPO on Renate's Updating Algorithms.
 
     Renate will benefit from hyperparameter tuning compared to Renate with default settings. [#]_
 
 
 Key features
 ============
 
 * Easy to scale and run in the cloud
 * Designed for real-world retraining pipelines
 * Advanced HPO functionalities available out-of-the-box
 * Open for experimentation 
 
+Blog posts
+==========
+
+* `Automatically retrain neural networks with Renate <https://aws.amazon.com/blogs/machine-learning/automatically-retrain-neural-networks-with-renate/>`_
+
 
 What are you looking for?
 =========================
 
 * `Installation Instructions <https://renate.readthedocs.io/en/latest/getting_started/install.html>`_
-
     .. code-block:: bash
 
       pip install renate
 
-* Examples
-    We provide examples to train your model
-    `locally <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_
-    or `using Amazon SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_.
-* `Documentation <https://renate.readthedocs.io>`_
-* `Supported Algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
-* `Experimenting with Renate <https://renate.readthedocs.io/en/latest/benchmarking/index.html>`_
+* Examples:
+    * `Train an MLP locally on MNIST <https://renate.readthedocs.io/en/latest/examples/train_mlp_locally.html>`_
+    * `Train a ResNet on SageMaker <https://renate.readthedocs.io/en/latest/examples/train_classifier_sagemaker.html>`_
+* `Documentation website with API doc and examples <https://renate.readthedocs.io>`_
+* `List of the supported algorithms <https://renate.readthedocs.io/en/latest/getting_started/supported_algorithms.html>`_
+* `How to run continual learning experiments using Renate <https://renate.readthedocs.io/en/latest/benchmarking/index.html>`_
 * `Guidelines for Contributors <https://github.com/awslabs/renate/tree/master/CONTRIBUTING.md>`_
-* You did not find what you were looking for?
-    Open an `issue <https://github.com/awslabs/Renate/issues/new>`_ and we will do our best
-    to improve the documentation.
+
+If you did not find what you were looking for, open an `issue <https://github.com/awslabs/Renate/issues/new>`_ and
+we will do our best to improve the documentation.
 
 
 .. [#] To create this plot, we simulated class-incremental learning with CIFAR-10.
     The training data was divided into 5 partitions, and we trained sequentially on them.
     Fine-tuning refers to the strategy to learn on the first partition from scratch, and
     train on each of the subsequent partitions for few epochs only.
     We compare to Experience Replay with a memory size of 500.
     For both methods we use the same number of epochs and choose the best checkpoint
     using a validation set.
     Results reported are on the test set.
+
 .. [#] The setup is the same as in the last experiment. However, this time we compare
     Experience Replay against a version in which its hyperparameters were tuned.
```

### Comparing `Renate-0.1.0/src/renate/__init__.py` & `Renate-0.2.0/src/renate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,8 @@
     _handler = logging.StreamHandler()
     _handler.setFormatter(
         logging.Formatter("[%(asctime)s] %(levelname)s [%(name)s:%(lineno)s] %(message)s")
     )
     _renate_logger.addHandler(_handler)
     _renate_logger.propagate = False
 
-
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

### Comparing `Renate-0.1.0/src/renate/benchmark/datasets/vision_datasets.py` & `Renate-0.2.0/src/renate/benchmark/datasets/vision_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import os
 from pathlib import Path
-from typing import Callable, List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import torch
-from torch.utils.data import Dataset
 import torchvision
+from torch.utils.data import Dataset
 from torchvision import transforms
 
 from renate import defaults
 from renate.data import ImageDataset
 from renate.data.data_module import RenateDataModule
 from renate.utils.file import download_and_unzip_file, download_folder_from_s3
 
@@ -98,15 +98,16 @@
 
 
 class TorchVisionDataModule(RenateDataModule):
     """Data module wrapping torchvision datasets.
 
     Args:
         data_path: the path to the folder containing the dataset files.
-        src_bucket: the name of the s3 bucket. If not provided, downloads the data from original source.
+        src_bucket: the name of the s3 bucket. If not provided, downloads the data from original
+            source.
         src_object_name: the folder path in the s3 bucket.
         dataset_name: Name of the torchvision dataset.
         val_size: Fraction of the training data to be used for validation.
         seed: Seed used to fix random number generation.
     """
 
     dataset_dict = {
@@ -185,20 +186,20 @@
 class CLEARDataModule(RenateDataModule):
     """Datamodule that process CLEAR datasets: CLEAR10 and CLEAR100.
 
     Source: https://clear-benchmark.github.io/.
 
     Args:
         data_path: the path to the folder containing the dataset files.
-        src_bucket: the name of the s3 bucket. If not provided, downloads the data from original source.
+        src_bucket: the name of the s3 bucket. If not provided, downloads the data from original
+            source.
         src_object_name: the folder path in the s3 bucket.
-        transform: Transformation or augmentation to perform on the sample.
-        target_transform: Transformation or augmentation to perform on the target.
         dataset_name: CLEAR dataset name, options are clear10 and clear100.
-        chunk_id: Used to define the CLEAR dataset splits. There are 10 splits in total with ids from 0 to 9.
+        chunk_id: Used to define the CLEAR dataset splits. There are 10 splits in total with ids
+            from 0 to 9.
         val_size: Fraction of the training data to be used for validation.
         seed: Seed used to fix random number generation.
     """
 
     md5s = {
         "clear10-train-image-only.zip": "5171f720810d60b471c308dee595d430",
         "clear100-train-image-only.zip": "ea85cdba9efcb3abf77eaab5554052c8",
```

### Comparing `Renate-0.1.0/src/renate/benchmark/experiment_config.py` & `Renate-0.2.0/src/renate/benchmark/experiment_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-import ast
-from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 import torch
 from torchvision.transforms import transforms
 
-from renate.benchmark.datasets.nlp_datasets import TorchTextDataModule
 from renate.benchmark.datasets.vision_datasets import CLEARDataModule, TorchVisionDataModule
 from renate.benchmark.models import (
     MultiLayerPerceptron,
     ResNet18,
     ResNet18CIFAR,
     ResNet34,
     ResNet34CIFAR,
@@ -23,21 +20,24 @@
     VisionTransformerH14,
     VisionTransformerL16,
     VisionTransformerL32,
 )
 from renate.benchmark.scenarios import (
     BenchmarkScenario,
     ClassIncrementalScenario,
+    FeatureSortingScenario,
+    HueShiftScenario,
+    IIDScenario,
     ImageRotationScenario,
     PermutationScenario,
     Scenario,
 )
 from renate.data.data_module import RenateDataModule
 from renate.models import RenateModule
-
+from renate.models.prediction_strategies import ICaRLClassificationStrategy
 
 models = {
     "MultiLayerPerceptron": MultiLayerPerceptron,
     "ResNet18CIFAR": ResNet18CIFAR,
     "ResNet34CIFAR": ResNet34CIFAR,
     "ResNet50CIFAR": ResNet50CIFAR,
     "ResNet18": ResNet18,
@@ -49,78 +49,83 @@
     "VisionTransformerL16": VisionTransformerL16,
     "VisionTransformerL32": VisionTransformerL32,
     "VisionTransformerH14": VisionTransformerH14,
 }
 
 
 def model_fn(
-    model_state_url: Optional[Union[Path, str]] = None,
-    model_fn_model_name: Optional[str] = None,
-    model_fn_num_inputs: Optional[str] = None,
-    model_fn_num_outputs: Optional[str] = None,
-    model_fn_num_hidden_layers: Optional[str] = None,
-    model_fn_hidden_size: Optional[str] = None,
+    model_state_url: Optional[str] = None,
+    updater: Optional[str] = None,
+    model_name: Optional[str] = None,
+    num_inputs: Optional[int] = None,
+    num_outputs: Optional[int] = None,
+    num_hidden_layers: Optional[int] = None,
+    hidden_size: Optional[Tuple[int]] = None,
 ) -> RenateModule:
     """Returns a model instance."""
-    if model_fn_model_name not in models:
-        raise ValueError(f"Unknown model `{model_fn_model_name}`")
-    model_class = models[model_fn_model_name]
+    if model_name not in models:
+        raise ValueError(f"Unknown model `{model_name}`")
+    model_class = models[model_name]
     model_kwargs = {}
-    if model_fn_model_name == "MultiLayerPerceptron":
+    if updater == "Avalanche-iCaRL":
+        model_kwargs["prediction_strategy"] = ICaRLClassificationStrategy()
+    if model_name == "MultiLayerPerceptron":
         model_kwargs = {
-            "num_inputs": int(model_fn_num_inputs),
-            "num_outputs": int(model_fn_num_outputs),
-            "num_hidden_layers": int(model_fn_num_hidden_layers),
-            "hidden_size": ast.literal_eval(model_fn_hidden_size),
+            "num_inputs": num_inputs,
+            "num_hidden_layers": num_hidden_layers,
+            "hidden_size": hidden_size,
         }
+    if num_outputs is not None:
+        model_kwargs["num_outputs"] = num_outputs
     if model_state_url is None:
         model = model_class(**model_kwargs)
     else:
-        state_dict = torch.load(str(model_state_url))
+        state_dict = torch.load(model_state_url)
         model = model_class.from_state_dict(state_dict)
     return model
 
 
 def get_data_module(
     data_path: str, dataset_name: str, val_size: float, seed: int
 ) -> RenateDataModule:
     if dataset_name in TorchVisionDataModule.dataset_dict:
         return TorchVisionDataModule(
             data_path, dataset_name=dataset_name, val_size=val_size, seed=seed
         )
     if dataset_name in ["CLEAR10", "CLEAR100"]:
         return CLEARDataModule(data_path, dataset_name=dataset_name, val_size=val_size, seed=seed)
-    if dataset_name in TorchTextDataModule.dataset_dict:
-        return TorchTextDataModule(
-            data_path, dataset_name=dataset_name, val_size=val_size, seed=seed
-        )
     raise ValueError(f"Unknown dataset `{dataset_name}`.")
 
 
 def get_scenario(
     scenario_name: str,
     data_module: RenateDataModule,
     chunk_id: int,
     seed: int,
     num_tasks: Optional[int] = None,
-    class_groupings: Optional[List[List[int]]] = None,
+    class_groupings: Optional[Tuple[Tuple[int]]] = None,
     degrees: Optional[List[int]] = None,
     input_dim: Optional[Union[List[int], Tuple[int], int]] = None,
+    feature_idx: Optional[int] = None,
+    randomness: Optional[float] = None,
 ) -> Scenario:
     """Function to create scenario based on name and arguments.
 
     Args:
         scenario_name: Name to identify scenario.
         data_module: The base data module.
         chunk_id: The data chunk to load in for the training or validation data.
         seed: A random seed to fix the created scenario.
         num_tasks: The total number of expected tasks for experimentation.
-        class_groupings: Used for scenario `ClassIncrementalScenario`. Partitions classes into different chunks
+        class_groupings: Used for scenario `ClassIncrementalScenario`. Partitions classes into
+            different chunks.
         degrees: Used for scenario `ImageRotationScenario`. Rotations applied for each chunk.
         input_dim: Used for scenario `PermutationScenario`. Input dimensionality.
+        feature_idx: Used for scenario `SoftSortingScenario`. Index of feature to sort by.
+        randomness: Used for all `_SortingScenario`. Randomness strength in [0, 1].
 
     Returns:
         An instance of the requested scenario.
 
     Raises:
         ValueError: If scenario name is unknown.
     """
@@ -133,90 +138,107 @@
             class_groupings=class_groupings,
             chunk_id=chunk_id,
         )
     if scenario_name == "BenchmarkScenario":
         return BenchmarkScenario(
             data_module=data_module, num_tasks=num_tasks, chunk_id=chunk_id, seed=seed
         )
+    if scenario_name == "IIDScenario":
+        return IIDScenario(
+            data_module=data_module, num_tasks=num_tasks, chunk_id=chunk_id, seed=seed
+        )
     if scenario_name == "ImageRotationScenario":
         return ImageRotationScenario(
             data_module=data_module, degrees=degrees, chunk_id=chunk_id, seed=seed
         )
     if scenario_name == "PermutationScenario":
         return PermutationScenario(
             data_module=data_module,
             num_tasks=num_tasks,
             input_dim=input_dim,
             chunk_id=chunk_id,
             seed=seed,
         )
+    if scenario_name == "FeatureSortingScenario":
+        return FeatureSortingScenario(
+            data_module=data_module,
+            num_tasks=num_tasks,
+            feature_idx=feature_idx,
+            randomness=randomness,
+            chunk_id=chunk_id,
+            seed=seed,
+        )
+    if scenario_name == "HueShiftScenario":
+        return HueShiftScenario(
+            data_module=data_module,
+            num_tasks=num_tasks,
+            randomness=randomness,
+            chunk_id=chunk_id,
+            seed=seed,
+        )
     raise ValueError(f"Unknown scenario `{scenario_name}`.")
 
 
 def data_module_fn(
-    data_path: Union[Path, str],
+    data_path: str,
     chunk_id: int,
     seed: int,
-    data_module_fn_scenario_name: str,
-    data_module_fn_dataset_name: str,
-    data_module_fn_val_size: str = "0.0",
-    data_module_fn_num_tasks: Optional[str] = None,
-    data_module_fn_class_groupings: Optional[str] = None,
-    data_module_fn_degrees: Optional[str] = None,
-    data_module_fn_input_dim: Optional[str] = None,
+    scenario_name: str,
+    dataset_name: str,
+    val_size: float = 0.0,
+    num_tasks: Optional[int] = None,
+    class_groupings: Optional[Tuple[Tuple[int]]] = None,
+    degrees: Optional[Tuple[int]] = None,
+    input_dim: Optional[Tuple[int]] = None,
+    feature_idx: Optional[int] = None,
+    randomness: Optional[float] = None,
 ):
     data_module = get_data_module(
-        data_path=str(data_path),
-        dataset_name=data_module_fn_dataset_name,
-        val_size=float(data_module_fn_val_size),
+        data_path=data_path,
+        dataset_name=dataset_name,
+        val_size=val_size,
         seed=seed,
     )
-    if data_module_fn_num_tasks is not None:
-        data_module_fn_num_tasks = int(data_module_fn_num_tasks)
-    if data_module_fn_class_groupings is not None:
-        data_module_fn_class_groupings = ast.literal_eval(data_module_fn_class_groupings)
-    if data_module_fn_degrees is not None:
-        data_module_fn_degrees = ast.literal_eval(data_module_fn_degrees)
-    if data_module_fn_input_dim is not None:
-        data_module_fn_input_dim = ast.literal_eval(data_module_fn_input_dim)
     return get_scenario(
-        scenario_name=data_module_fn_scenario_name,
+        scenario_name=scenario_name,
         data_module=data_module,
         chunk_id=chunk_id,
         seed=seed,
-        num_tasks=data_module_fn_num_tasks,
-        class_groupings=data_module_fn_class_groupings,
-        degrees=data_module_fn_degrees,
-        input_dim=data_module_fn_input_dim,
+        num_tasks=num_tasks,
+        class_groupings=class_groupings,
+        degrees=degrees,
+        input_dim=input_dim,
+        feature_idx=feature_idx,
+        randomness=randomness,
     )
 
 
 def _get_normalize_transform(dataset_name):
     if dataset_name in TorchVisionDataModule.dataset_stats:
         return transforms.Normalize(
             TorchVisionDataModule.dataset_stats[dataset_name]["mean"],
             TorchVisionDataModule.dataset_stats[dataset_name]["std"],
         )
 
 
-def train_transform(transform_dataset_name: str) -> Optional[transforms.Compose]:
+def train_transform(dataset_name: str) -> Optional[transforms.Compose]:
     """Returns a transform function to be used in the training."""
-    if transform_dataset_name in ["MNIST", "FashionMNIST"]:
+    if dataset_name in ["MNIST", "FashionMNIST"]:
         return None
-    elif transform_dataset_name in ["CIFAR10", "CIFAR100"]:
+    elif dataset_name in ["CIFAR10", "CIFAR100"]:
         return transforms.Compose(
             [
                 transforms.RandomCrop(32, padding=4),
                 transforms.RandomHorizontalFlip(),
-                _get_normalize_transform(transform_dataset_name),
+                _get_normalize_transform(dataset_name),
             ]
         )
-    raise ValueError(f"Unknown dataset `{transform_dataset_name}`.")
+    raise ValueError(f"Unknown dataset `{dataset_name}`.")
 
 
-def test_transform(transform_dataset_name: str) -> Optional[transforms.Normalize]:
+def test_transform(dataset_name: str) -> Optional[transforms.Normalize]:
     """Returns a transform function to be used for validation or testing."""
-    if transform_dataset_name in ["MNIST", "FashionMNIST"]:
+    if dataset_name in ["MNIST", "FashionMNIST"]:
         return None
-    elif transform_dataset_name in ["CIFAR10", "CIFAR100"]:
-        return _get_normalize_transform(transform_dataset_name)
-    raise ValueError(f"Unknown dataset `{transform_dataset_name}`.")
+    elif dataset_name in ["CIFAR10", "CIFAR100"]:
+        return _get_normalize_transform(dataset_name)
+    raise ValueError(f"Unknown dataset `{dataset_name}`.")
```

### Comparing `Renate-0.1.0/src/renate/benchmark/experimentation.py` & `Renate-0.2.0/src/renate/benchmark/experimentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 import pandas as pd
 import torch
 from pytorch_lightning import seed_everything
 
 import renate
 import renate.defaults as defaults
 from renate.cli.parsing_functions import (
-    get_data_module_fn_args,
-    get_model_fn_args,
+    get_data_module_fn_kwargs,
+    get_model_fn_kwargs,
     get_scheduler_kwargs,
     get_transforms_kwargs,
 )
 from renate.evaluation.metrics.classification import (
     average_accuracy,
     backward_transfer,
     forgetting,
     forward_transfer,
 )
-from renate.tuning import execute_tuning_job
-from renate.tuning.tuning import submit_remote_job
+from renate.training import run_training_job
+from renate.training.training import submit_remote_job
 from renate.utils.file import (
     copy_to_uri,
     is_s3_uri,
     move_to_uri,
     save_pandas_df_to_csv,
 )
 from renate.utils.module import (
@@ -44,16 +44,16 @@
 
 
 def experiment_config_file():
     return str(Path(renate.__path__[0]) / "benchmark" / "experiment_config.py")
 
 
 def create_cumulative_metrics(task: defaults.SUPPORTED_TASKS_TYPE) -> List[Tuple[str, Callable]]:
-    """Gets the cumulative metrics for a given task along with a name of the metric to include in any potential results
-    table.
+    """Gets the cumulative metrics for a given task along with a name of the metric to include in
+    any potential results table.
 
     Args:
         task: Whether classification or regression, for now.
     """
     if task == "classification":
         return [
             ("Average Accuracy", average_accuracy),
@@ -66,18 +66,20 @@
 
 
 def cumulative_metrics_summary(
     results: Dict[str, List[List[float]]],
     cumulative_metrics: List[Tuple[str, Callable]],
     num_tasks: int,
 ) -> pd.DataFrame:
-    """Creates a pandas DataFrame summary with respect to the observed tasks, specified by `num_tasks`.
+    """Creates a pandas DataFrame summary with respect to the observed tasks, specified by
+    `num_tasks`.
 
     Args:
-        results: The results dictionary holding all the results with respect to all recorded metrics.
+        results: The results dictionary holding all the results with respect to all recorded
+            metrics.
         cumulative_metrics: The list of (name, metric) tuples.
         num_tasks: The total number of tasks.
     """
     data = []
     for task_id in range(num_tasks + 1):
         row = [task_id + 1]
         for _, metric in cumulative_metrics:
@@ -90,18 +92,20 @@
 
 
 def individual_metrics_summary(
     results: Dict[str, List[List[float]]],
     current_task: int,
     num_tasks: int,
 ) -> pd.DataFrame:
-    """Creates a pandas DataFrame summary for all individual metrics with respect to all observed tasks.
+    """Creates a pandas DataFrame summary for all individual metrics with respect to all observed
+    tasks.
 
     Args:
-        results: The results dictionary holding all the results with respect to all recorded metrics.
+        results: The results dictionary holding all the results with respect to all recorded
+            metrics.
         current_task: The current task ID.
         num_tasks: The total number of tasks.
     """
     data = []
     metric_columns = [k for k in results.keys() if "_init" not in k]
 
     for task_id in range(current_task):
@@ -137,23 +141,25 @@
     max_num_trials_started: Optional[int] = None,
     max_num_trials_completed: Optional[int] = None,
     max_num_trials_finished: Optional[int] = None,
     n_workers: int = defaults.N_WORKERS,
     seed: int = defaults.SEED,
     accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
     devices: int = defaults.DEVICES,
+    deterministic_trainer: bool = True,
     job_name: str = defaults.JOB_NAME,
 ) -> None:
     """Executes the experiment job.
 
     Args:
         backend: Backend of the experiment job.
         config_file: Path to the Renate config file.
         config_space: Details for defining your own search space is provided in the
-            `Syne Tune Documentation <https://github.com/awslabs/syne-tune/blob/main/docs/search_space.md>`_.
+            `Syne Tune Documentation
+            <https://github.com/awslabs/syne-tune/blob/main/docs/search_space.md>`_.
         experiment_outputs_url: Path to the experiment outputs.
         mode: Whether to minimize or maximize the metric.
         metric: Metric of the experiment job.
         num_updates: Number of updates of the experiment job.
         working_directory: Path to the working directory.
         requirements_file: Path to the requirements file.
         role: Role of the experiment job.
@@ -164,14 +170,16 @@
         max_num_trials_started: Max number of trials started of the experiment job.
         max_num_trials_completed: Max number of trials completed of the experiment job.
         max_num_trials_finished: Max number of trials finished of the experiment job.
         n_workers: Number of workers of the experiment job.
         seed: Seed of the experiment job.
         accelerator: Type of accelerator to use.
         devices: Number of devices to use.
+        deterministic_trainer: When true the Trainer adopts a deterministic behaviour also on GPU.
+            In this function this parameter is set to True by default.
         job_name: Name of the experiment job.
     """
     assert (
         mode in defaults.SUPPORTED_TUNING_MODE
     ), f"Mode {mode} is not in {defaults.SUPPORTED_TUNING_MODE}."
     assert (
         backend in defaults.SUPPORTED_BACKEND
@@ -188,14 +196,15 @@
             max_time=max_time,
             max_num_trials_started=max_num_trials_started,
             max_num_trials_completed=max_num_trials_completed,
             max_num_trials_finished=max_num_trials_finished,
             n_workers=n_workers,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
             seed=seed,
         )
     _execute_experiment_job_remotely(
         job_name=job_name,
         config_file=config_file,
         experiment_outputs_url=experiment_outputs_url,
         mode=mode,
@@ -206,14 +215,15 @@
         max_time=max_time,
         max_num_trials_started=max_num_trials_started,
         max_num_trials_completed=max_num_trials_completed,
         max_num_trials_finished=max_num_trials_finished,
         n_workers=n_workers,
         accelerator=accelerator,
         devices=devices,
+        deterministic_trainer=deterministic_trainer,
         seed=seed,
         requirements_file=requirements_file,
         role=role,
         instance_type=instance_type,
         instance_count=instance_count,
         instance_max_time=instance_max_time,
     )
@@ -231,46 +241,47 @@
     accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE,
     devices: int,
     max_time: float,
     max_num_trials_started: int,
     max_num_trials_completed: int,
     max_num_trials_finished: int,
     n_workers: int,
+    deterministic_trainer: bool,
 ) -> None:
     """Runs an experiment, combining hyperparameter tuning and model for multiple updates.
 
     See renate.benchmark.experimentation.execute_experiment_job for more details.
     """
     logger.info("Start experiment.")
     seed_everything(seed)
 
-    state_url = defaults.current_state_folder(working_directory)
-    next_state_url = defaults.next_state_folder(working_directory)
+    input_state_url = defaults.input_state_folder(working_directory)
+    output_state_url = defaults.output_state_folder(working_directory)
     data_url = defaults.data_folder(working_directory)
-    model_url = defaults.model_file(state_url)
+    model_url = defaults.model_file(input_state_url)
     logs_url = defaults.logs_folder(working_directory)
 
-    for url in [state_url, next_state_url, logs_url]:
+    for url in [input_state_url, output_state_url, logs_url]:
         if os.path.exists(url):
             shutil.rmtree(url)
         Path(url).mkdir(parents=True, exist_ok=True)
 
     config_module = import_module("config_module", config_file)
     scheduler, scheduler_kwargs = get_scheduler_kwargs(config_module)
-    model_fn_args = get_model_fn_args(config_space)
-    logger.info(f"Loading model {model_fn_args.get('model_fn_model_name', '')}")
-    model = get_model(config_module, **model_fn_args)
-    data_module_fn_args = get_data_module_fn_args(config_space)
-    logger.info(f"Prepare dataset {data_module_fn_args.get('data_module_fn_dataset_name', '')}")
+    model_fn_kwargs = get_model_fn_kwargs(config_module, config_space)
+    logger.info(f"Loading model {model_fn_kwargs.get('model_name', '')}")
+    model = get_model(config_module, **model_fn_kwargs)
+    data_module_fn_kwargs = get_data_module_fn_kwargs(config_module, config_space)
+    logger.info(f"Prepare dataset {data_module_fn_kwargs.get('dataset_name', '')}")
     data_module = get_and_prepare_data_module(
         config_module,
         data_path=data_url,
         chunk_id=defaults.CHUNK_ID,
         seed=seed,
-        **data_module_fn_args,
+        **data_module_fn_kwargs,
     )
     data_module.setup()
     assert num_updates == len(
         data_module.test_data()
     ), f"The dataset has {len(data_module.test_data())} chunks, expected {num_updates}."
     transforms = get_transforms_kwargs(config_module, config_space)
     metrics = get_metrics(config_module)
@@ -292,60 +303,59 @@
         accelerator=accelerator,
         devices=devices,
     )
 
     for update_id in range(num_updates):
         logger.info(f"Starting Update {update_id + 1}/{num_updates}.")
         update_url = os.path.join(experiment_outputs_url, f"update_{update_id}")
-        execute_tuning_job(
+        run_training_job(
             mode=mode,
             config_space=config_space,
             metric=metric,
             backend="local",
             updater=config_space["updater"],
             max_epochs=config_space["max_epochs"],
             chunk_id=update_id,
-            state_url=state_url,
-            next_state_url=next_state_url,
+            input_state_url=input_state_url,
+            output_state_url=output_state_url,
             working_directory=working_directory,
             config_file=config_file,
             max_time=max_time,
             max_num_trials_started=max_num_trials_started,
             max_num_trials_completed=max_num_trials_completed,
             max_num_trials_finished=max_num_trials_finished,
             n_workers=n_workers,
             scheduler=scheduler,
             scheduler_kwargs=scheduler_kwargs,
             seed=seed,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
-        move_to_uri(next_state_url, state_url)
-        copy_to_uri(state_url, update_url)
+        move_to_uri(output_state_url, input_state_url)
+        copy_to_uri(input_state_url, update_url)
         model = get_model(
-            config_module, model_state_url=model_url, **get_model_fn_args(config_space)
+            config_module,
+            model_state_url=model_url,
+            **get_model_fn_kwargs(config_module, config_space),
         )
 
         evaluate_and_record_results(
             results,
             model=model,
             data_module=data_module,
             transform=transforms.get("test_transform"),
             target_transform=transforms.get("target_test_transform"),
             logged_metrics=metrics,
             accelerator=accelerator,
             devices=devices,
         )
         df = individual_metrics_summary(results, update_id + 1, num_updates)
         save_pandas_df_to_csv(
-            df,
-            defaults.metric_summary_file(
-                logs_url,
-                special_str=f"_update_{update_id}_" + defaults.current_timestamp(),
-            ),
+            df, defaults.metric_summary_file(logs_url, special_str=f"_update_{update_id}")
         )
         logger.info(f"### Results after update {update_id + 1}: ###")
         logger.info(df)
 
     cumulative_metrics = create_cumulative_metrics("classification")
     df = cumulative_metrics_summary(results, cumulative_metrics, num_updates - 1)
     save_pandas_df_to_csv(df, defaults.metric_summary_file(logs_url))
```

### Comparing `Renate-0.1.0/src/renate/benchmark/models/mlp.py` & `Renate-0.2.0/src/renate/benchmark/models/mlp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from typing import List, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
-import torch
 import torch.nn as nn
 
-from renate.defaults import TASK_ID
-from renate.models.renate_module import RenateModule
+from renate.benchmark.models.base import RenateBenchmarkingModule
+from renate.models.prediction_strategies import PredictionStrategy
 
 
-class MultiLayerPerceptron(RenateModule):
-    """A simple Multi Layer Perceptron with hidden layers, activation and Batch Normalization if enabled.
+class MultiLayerPerceptron(RenateBenchmarkingModule):
+    """A simple Multi Layer Perceptron with hidden layers, activation and Batch Normalization if
+    enabled.
 
     Args:
         num_inputs: Number of input nodes.
         num_outputs: Number of output nodes.
         num_hidden_layers: Number of hidden layers.
-        hidden_size: Uniform hidden size or the list or tuple of hidden sizes for individual hidden layers.
+        hidden_size: Uniform hidden size or the list or tuple of hidden sizes for individual hidden
+            layers.
         loss: Loss function to be used for training.
-        activation: Activation name, matching activation name in `torch.nn` to be used between the hidden layers.
-        batch_normalization: Whether to use Batch Normalization after the activation. By default the Batch Normalization
-            tracks the running statistics.
+        activation: Activation name, matching activation name in `torch.nn` to be used between the
+            hidden layers.
+        batch_normalization: Whether to use Batch Normalization after the activation. By default the
+            Batch Normalization tracks the running statistics.
+        prediction_strategy: Continual learning strategies may alter the prediction at train or test
+            time.
+        add_icarl_class_means: If ``True``, additional parameters used only by the
+            ``ICaRLModelUpdater`` are added. Only required when using that updater.
     """
 
     def __init__(
         self,
         num_inputs: int,
         num_outputs: int,
         num_hidden_layers: int,
         hidden_size: Union[int, List[int], Tuple[int]],
         loss: nn.Module = nn.CrossEntropyLoss(),
         activation: str = "ReLU",
         batch_normalization: bool = False,
+        prediction_strategy: Optional[PredictionStrategy] = None,
+        add_icarl_class_means: bool = True,
     ) -> None:
+        embedding_size = hidden_size if type(hidden_size) == int else hidden_size[-1]
         super().__init__(
+            embedding_size=embedding_size,
+            num_outputs=num_outputs,
             constructor_arguments={
                 "num_inputs": num_inputs,
-                "num_outputs": num_outputs,
                 "num_hidden_layers": num_hidden_layers,
                 "hidden_size": hidden_size,
                 "activation": activation,
                 "batch_normalization": batch_normalization,
             },
             loss_fn=loss,
+            prediction_strategy=prediction_strategy,
+            add_icarl_class_means=add_icarl_class_means,
         )
         if isinstance(hidden_size, int):
             hidden_size = [hidden_size for _ in range(num_hidden_layers + 1)]
         assert len(hidden_size) == num_hidden_layers + 1
 
         activation = getattr(nn, activation)
 
@@ -54,28 +66,8 @@
         layers = [nn.Flatten()]
         for i in range(num_hidden_layers + 1):
             layers.append(nn.Linear(hidden_size[i], hidden_size[i + 1]))
             layers.append(activation())
             if batch_normalization:
                 layers.append(nn.BatchNorm1d(hidden_size[i + 1]))
 
-        self._last_hidden_size = hidden_size[-1]
-        self._num_outputs = num_outputs
-
-        self._model = nn.Sequential(*layers)
-        self._tasks_params: nn.ModuleDict = nn.ModuleDict()
-        self.add_task_params(TASK_ID)
-
-    def forward(self, x: torch.Tensor, task_id: str = TASK_ID) -> torch.Tensor:
-        """Performs a forward pass on the inputs and returns the predictions."""
-        return self._tasks_params[task_id](self._model(x))
-
-    def _add_task_params(self, task_id: str = TASK_ID) -> None:
-        """Adds new parameters associated to a specific task to the model."""
-        self._tasks_params[task_id] = nn.Linear(
-            self._last_hidden_size,
-            self._num_outputs,
-        )
-
-    def get_params(self, task_id: str = TASK_ID) -> List[nn.Parameter]:
-        """Returns the list of parameters for the core model and a specific `task_id`."""
-        return list(self._model.parameters()) + list(self._tasks_params[task_id].parameters())
+        self._backbone = nn.Sequential(*layers)
```

### Comparing `Renate-0.1.0/src/renate/benchmark/models/resnet.py` & `Renate-0.2.0/src/renate/benchmark/models/resnet.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,96 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List, Optional, Type, Union
 
-import torch
 import torch.nn as nn
 from torchvision.models.resnet import BasicBlock, Bottleneck
 from torchvision.models.resnet import ResNet as _ResNet
 
-from renate.defaults import TASK_ID
-from renate.models.renate_module import RenateModule
+from renate.benchmark.models.base import RenateBenchmarkingModule
+from renate.models.prediction_strategies import PredictionStrategy
 
 
-class ResNet(RenateModule):
+class ResNet(RenateBenchmarkingModule):
     """ResNet model base class.
 
     TODO: Fix citation
     Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun:
     Deep Residual Learning for Image Recognition. CVPR 2016: 770-778
 
     Args:
         block: The type of the block to use as the core building block.
         layers: The number of blocks in the respective parts of ResNet.
         num_outputs: The number of output units.
-        zero_init_residual: Whether to set the initial weights of the residual blocks
-                            to zero through initializing the Batch Normalization parameters at the end of the block to zero.
+        zero_init_residual: Whether to set the initial weights of the residual blocks to zero
+            through initializing the Batch Normalization parameters at the end of the block to zero.
         groups: The number of groups to be used for the group convolution.
         width_per_group: The width of the group convolution.
         replace_stride_with_dilation: Whether to replace the stride with a dilation to save memory.
         norm_layer: What kind of normalization layer to use, following convolutions.
         cifar_stem: Whether to use a stem for CIFAR-sized images.
         loss: Loss function to be used for training.
+        prediction_strategy: Continual learning strategies may alter the prediction at train or test
+            time.
+        add_icarl_class_means: If ``True``, additional parameters used only by the
+            ``ICaRLModelUpdater`` are added. Only required when using that updater.
     """
 
     def __init__(
         self,
         block: Type[Union[BasicBlock, Bottleneck]],
         layers: List[int],
         num_outputs: int = 10,
         zero_init_residual: bool = False,
         groups: int = 1,
         width_per_group: int = 64,
         replace_stride_with_dilation: Optional[List[bool]] = None,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
         cifar_stem: bool = True,
         loss: nn.Module = nn.CrossEntropyLoss(),
+        prediction_strategy: Optional[PredictionStrategy] = None,
+        add_icarl_class_means: bool = True,
     ) -> None:
-        RenateModule.__init__(
-            self,
+        model = _ResNet(
+            block=block,
+            layers=layers,
+            num_classes=num_outputs,
+            zero_init_residual=zero_init_residual,
+            groups=groups,
+            width_per_group=width_per_group,
+            replace_stride_with_dilation=replace_stride_with_dilation,
+            norm_layer=norm_layer,
+        )
+        super().__init__(
+            embedding_size=model.fc.in_features,
+            num_outputs=num_outputs,
             constructor_arguments={
                 "block": block,
                 "layers": layers,
-                "num_outputs": num_outputs,
                 "zero_init_residual": zero_init_residual,
                 "groups": groups,
                 "width_per_group": width_per_group,
                 "replace_stride_with_dilation": replace_stride_with_dilation,
                 "norm_layer": norm_layer,
                 "cifar_stem": cifar_stem,
             },
             loss_fn=loss,
+            prediction_strategy=prediction_strategy,
+            add_icarl_class_means=add_icarl_class_means,
         )
-        self._model = _ResNet(
-            block=block,
-            layers=layers,
-            num_classes=num_outputs,
-            zero_init_residual=zero_init_residual,
-            groups=groups,
-            width_per_group=width_per_group,
-            replace_stride_with_dilation=replace_stride_with_dilation,
-            norm_layer=norm_layer,
-        )
+        self._backbone = model
         if cifar_stem:
-            self._model.conv1 = nn.Conv2d(3, 64, kernel_size=3, stride=1, padding=1, bias=False)
-            self._model.maxpool = nn.Identity()
-
-        self._last_hidden_size = self._model.fc.in_features
-        self._num_outputs = num_outputs
-        self._model.fc = nn.Identity()
-        self._tasks_params: nn.ModuleDict = nn.ModuleDict()
-        self.add_task_params(TASK_ID)
+            self._backbone.conv1 = nn.Conv2d(3, 64, kernel_size=3, stride=1, padding=1, bias=False)
+            self._backbone.maxpool = nn.Identity()
+        self._backbone.fc = nn.Identity()
 
         for m in self.modules():
             if hasattr(m, "reset_parameters"):
                 m.reset_parameters()
 
-    def forward(self, x: torch.Tensor, task_id: str = TASK_ID) -> torch.Tensor:
-        """Performs a forward pass on the inputs and returns the predictions."""
-        x = self._model(x)
-        return self._tasks_params[task_id](x)
-
-    def _add_task_params(self, task_id: str = TASK_ID) -> None:
-        """Adds new parameters associated to a specific task to the model."""
-        self._tasks_params[task_id] = nn.Linear(self._last_hidden_size, self._num_outputs)
-
-    def get_params(self, task_id: str = TASK_ID) -> List[nn.Parameter]:
-        """Returns the list of parameters for the core model and a specific `task_id`."""
-        return list(self._model.parameters()) + list(self._tasks_params[task_id].parameters())
-
 
 class ResNet18CIFAR(ResNet):
     def __init__(self, block=BasicBlock, layers=[2, 2, 2, 2], cifar_stem=True, **kwargs) -> None:
         super().__init__(block=block, layers=layers, cifar_stem=cifar_stem, **kwargs)
 
 
 class ResNet34CIFAR(ResNet):
```

### Comparing `Renate-0.1.0/src/renate/benchmark/models/vision_transformer.py` & `Renate-0.2.0/src/renate/benchmark/models/vision_transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 from functools import partial
 from typing import Any, Callable, List, Optional
 
-import torch
 import torch.nn as nn
 from torchvision.models.vision_transformer import ConvStemConfig, WeightsEnum
 from torchvision.models.vision_transformer import VisionTransformer as _VisionTransformer
 
-from renate.defaults import TASK_ID
-from renate.models.renate_module import RenateModule
+from renate.benchmark.models.base import RenateBenchmarkingModule
+from renate.models.prediction_strategies import PredictionStrategy
 
 
-class VisionTransformer(RenateModule):
+class VisionTransformer(RenateBenchmarkingModule):
     """Vision Transformer base model.
 
     TODO: Fix citation
-    Dosovitskiy, Alexey, et al. "An image is worth 16x16 words: Transformers for image recognition at scale."
+    Dosovitskiy, Alexey, et al. "An image is worth 16x16 words: Transformers for image recognition
+    at scale."
     arXiv preprint arXiv:2010.11929 (2020).
 
     Args:
         image_size: Size of the input image.
         patch_size: Size of the patches.
         num_layers: Number of Encoder layers.
         num_heads: Number of Attention heads.
         hidden_dim: Size of the Encoder's hidden state.
         mlp_dim: Size of the intermediate Multi-layer Perceptron in the Encoder.
         dropout: Dropout probability.
         attention_dropout: Dropout probability for the attention in the Multi-head Attention layer.
         num_outputs: Size of the output.
-        representation_size: If specified, the model will return a linear projection of the last hidden state.
+        representation_size: If specified, the model will return a linear projection of the last
+            hidden state.
         norm_layer: Normalization layer.
-        conv_stem_configs: List of ConvStemConfig. Each ConvStemConfig corresponds to a convolutional stem.
+        conv_stem_configs: List of ConvStemConfig. Each ConvStemConfig corresponds to a
+            convolutional stem.
         loss: Loss function.
+        prediction_strategy: Continual learning strategies may alter the prediction at train or test
+            time.
+        add_icarl_class_means: If ``True``, additional parameters used only by the
+            ``ICaRLModelUpdater`` are added. Only required when using that updater.
     """
 
     def __init__(
         self,
         image_size: int = 32,
         patch_size: int = 4,
         num_layers: int = 12,
@@ -47,68 +53,55 @@
         attention_dropout: float = 0.1,
         num_outputs: int = 10,
         representation_size: Optional[int] = None,
         norm_layer: Callable[..., nn.Module] = partial(nn.LayerNorm, eps=1e-6),
         conv_stem_configs: Optional[List[ConvStemConfig]] = None,
         weights: Optional[WeightsEnum] = None,
         loss: nn.Module = nn.CrossEntropyLoss(),
+        prediction_strategy: Optional[PredictionStrategy] = None,
+        add_icarl_class_means: bool = True,
     ) -> None:
-        RenateModule.__init__(
-            self,
+        model = _VisionTransformer(
+            image_size=image_size,
+            patch_size=patch_size,
+            num_layers=num_layers,
+            num_heads=num_heads,
+            hidden_dim=hidden_dim,
+            mlp_dim=mlp_dim,
+            dropout=dropout,
+            attention_dropout=attention_dropout,
+            num_classes=num_outputs,
+            representation_size=representation_size,
+            norm_layer=norm_layer,
+            conv_stem_configs=conv_stem_configs,
+        )
+        super().__init__(
+            embedding_size=model.heads.head.in_features,
+            num_outputs=num_outputs,
             constructor_arguments={
                 "image_size": image_size,
                 "patch_size": patch_size,
                 "num_layers": num_layers,
                 "num_heads": num_heads,
                 "hidden_dim": hidden_dim,
                 "mlp_dim": mlp_dim,
                 "dropout": dropout,
                 "attention_dropout": attention_dropout,
-                "num_outputs": num_outputs,
                 "representation_size": representation_size,
                 "norm_layer": norm_layer,
                 "conv_stem_configs": conv_stem_configs,
             },
             loss_fn=loss,
+            prediction_strategy=prediction_strategy,
+            add_icarl_class_means=add_icarl_class_means,
         )
-        self._model = _VisionTransformer(
-            image_size=image_size,
-            patch_size=patch_size,
-            num_layers=num_layers,
-            num_heads=num_heads,
-            hidden_dim=hidden_dim,
-            mlp_dim=mlp_dim,
-            dropout=dropout,
-            attention_dropout=attention_dropout,
-            num_classes=num_outputs,
-            representation_size=representation_size,
-            norm_layer=norm_layer,
-            conv_stem_configs=conv_stem_configs,
-        )
+        self._backbone = model
         if weights:
-            self._model.load_state_dict(weights.get_state_dict())
-
-        self._last_hidden_size = self._model.heads.head.in_features
-        self._num_outputs = num_outputs
-        self._model.heads.head = nn.Identity()
-        self._tasks_params: nn.ModuleDict = nn.ModuleDict()
-        self.add_task_params(TASK_ID)
-
-    def forward(self, x: torch.Tensor, task_id: str = TASK_ID) -> torch.Tensor:
-        """Performs a forward pass on the inputs and returns the predictions."""
-        x = self._model(x)
-        return self._tasks_params[task_id](x)
-
-    def _add_task_params(self, task_id: str = TASK_ID) -> None:
-        """Adds new parameters associated to a specific task to the model."""
-        self._tasks_params[task_id] = nn.Linear(self._last_hidden_size, self._num_outputs)
-
-    def get_params(self, task_id: str = TASK_ID) -> List[nn.Parameter]:
-        """Returns the list of parameters for the core model and a specific `task_id`."""
-        return list(self._model.parameters()) + list(self._tasks_params[task_id].parameters())
+            self._backbone.load_state_dict(weights.get_state_dict())
+        self._backbone.heads.head = nn.Identity()
 
 
 class VisionTransformerCIFAR(VisionTransformer):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(
             image_size=32,
             patch_size=4,
```

### Comparing `Renate-0.1.0/src/renate/cli/run_experiment_with_scenario.py` & `Renate-0.2.0/src/renate/cli/run_experiment_with_scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
-This script is used to launch an experiment on SageMaker. Previously passed arguments on a different machine are loaded
-from S3 and the update process is started with these parameters.
-Arguments expected are described in renate.benchmark.execute_experiment_job.
+This script is used to launch an experiment on SageMaker. Previously passed arguments on a different
+machine are loaded from S3 and the update process is started with these parameters. Arguments
+expected are described in renate.benchmark.execute_experiment_job.
 """
 import argparse
 
 import renate.defaults as defaults
 from renate.benchmark.experimentation import execute_experiment_job
 
 
 class ExperimentCLI:
     """Entry point to perform an experiment from start to end including evaluation.
 
     Given a dataset, optionally wrapped in a scenario, a model and a training configuration,
-    this script will find the best hyper-parameters per each data chunk, update the model and evaluate it
-    on all the provided test data.
+    this script will find the best hyper-parameters per each data chunk, update the model and
+    evaluate it on all the provided test data.
     """
 
     def run(self):
         parser = argparse.ArgumentParser()
         argument_group = parser.add_argument_group("Required Parameters")
 
         argument_group.add_argument(
             "--config_file",
             type=str,
             required=True,
-            help="File containing the definition of model_fn, data_module_fn, config_space_fn and scheduler_fn.",
+            help="File containing the definition of model_fn, data_module_fn, config_space_fn and "
+            "scheduler_fn.",
         )
         argument_group.add_argument(
             "--experiment_outputs_url",
             type=str,
             required=True,
             help="Location where to store the experimental results and the final model and state.",
         )
         argument_group.add_argument(
             "--num_updates",
             type=int,
             required=True,
-            help="How many updates or chunk IDs should be passed to the updater to update the model.",
+            help="How many updates or chunk IDs should be passed to the updater to update the "
+            "model.",
         )
         argument_group.add_argument(
             "--mode",
             choices=defaults.SUPPORTED_TUNING_MODE,
             required=True,
             help=f"Declares the type of optimization problem: {defaults.SUPPORTED_TUNING_MODE}",
         )
@@ -85,15 +87,16 @@
             default=defaults.N_WORKERS,
             help=f"Number of workers running in parallel. Default: {defaults.N_WORKERS}.",
         )
         parser.add_argument(
             "--working_directory",
             type=str,
             default=defaults.WORKING_DIRECTORY,
-            help=f"Folder used by Renate to store files temporarily. Default: {defaults.WORKING_DIRECTORY}.",
+            help="Folder used by Renate to store files temporarily. Default: "
+            f"{defaults.WORKING_DIRECTORY}.",
         )
 
         argument_group = parser.add_argument_group("Optional Parameters")
         argument_group.add_argument(
             "--max_epochs",
             type=int,
             default=defaults.MAX_EPOCHS,
@@ -156,14 +159,23 @@
         argument_group.add_argument(
             "--job_name",
             type=str,
             default=None,
             help="Name of the SageMaker job.",
         )
 
+        argument_group.add_argument(
+            "--deterministic_trainer",
+            type=str,
+            default=str(defaults.DETERMINISTIC_TRAINER),
+            choices=["True", "False"],
+            help="When True forces the trainer to be deterministic. Default: "
+            f"{defaults.DETERMINISTIC_TRAINER}.",
+        )
+
         args = parser.parse_args()
 
         execute_experiment_job(
             **vars(args),
         )
```

### Comparing `Renate-0.1.0/src/renate/cli/run_remote_job.py` & `Renate-0.2.0/src/renate/cli/run_remote_job.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 """
-This script is used to launch model tuning on SageMaker. Previously passed arguments on a different machine are loaded
-again and the update process is started with these parameters.
-Arguments expected are described in renate.tuning.execute_tuning_job.
+This script is used to launch model run on SageMaker. Previously passed arguments on a different
+machine are loaded again and the update process is started with these parameters. Arguments expected
+are described in renate.training.run_training_job.
 """
 import json
 
 import renate.defaults as defaults
 from renate.benchmark.experimentation import execute_experiment_job
-from renate.tuning import execute_tuning_job
+from renate.training import run_training_job
 from renate.utils.syne_tune import config_space_from_dict
 
 if __name__ == "__main__":
     with open(defaults.JOB_KWARGS_FILE, "r") as f:
         job_kwargs = json.load(f)
     job_kwargs["config_space"] = config_space_from_dict(job_kwargs["config_space"])
     if "experiment_outputs_url" in job_kwargs:
         execute_experiment_job(backend="local", **job_kwargs)
     else:
-        execute_tuning_job(backend="local", **job_kwargs)
+        run_training_job(backend="local", **job_kwargs)
```

### Comparing `Renate-0.1.0/src/renate/data/data_module.py` & `Renate-0.2.0/src/renate/data/data_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 
 class RenateDataModule(abc.ABC):
     """Data modules bundle code for data loading and preparation.
 
     A data module implements two methods for data preparation:
     - `prepare_data()` downloads the data to the local machine and unpacks it.
-    - `setup()` creates pytorch dataset objects that return training, test and (possibly) validation data.
+    - `setup()` creates pytorch dataset objects that return training, test and (possibly) validation
+    data.
     These two steps are separated to streamline the process when launching multiple training jobs
     simultaneously, e.g., for hyperparameter optimization. In this case, `prepare_data()` is only
     called once per machine.
 
     After these two methods have been called, the data can be accessed using
     - `train_data()`
     - `test_data()`
@@ -79,15 +80,17 @@
         return self._val_data
 
     def test_data(self) -> Dataset:
         """Returns test dataset."""
         return self._test_data
 
     def _verify_file(self, file_name: str) -> bool:
-        """A helper function that verifies that the required dataset files are downloaded and correct."""
+        """A helper function that verifies that the required dataset files are downloaded and
+        correct.
+        """
         return check_integrity(
             os.path.join(self._data_path, self._dataset_name, file_name),
             self.md5s[file_name],
         )
 
     def _split_train_val_data(self, train_data: Dataset) -> Tuple[Dataset, Dataset]:
         """A helper function that splits the train data into train and validation sets."""
```

### Comparing `Renate-0.1.0/src/renate/defaults.py` & `Renate-0.2.0/src/renate/defaults.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,23 +22,22 @@
 BATCH_SIZE = 32
 LOSS_WEIGHT = 1.0
 SEED = 0
 EMA_MEMORY_UPDATE_GAMMA = 1.0
 VALIDATION_SIZE = 0.0
 LOSS_NORMALIZATION = 1
 EARLY_STOPPING = False
+DETERMINISTIC_TRAINER = False
 
 ACCELERATOR = "auto"
 SUPPORTED_ACCELERATORS = ["auto", "cpu", "gpu", "tpu"]
 SUPPORTED_ACCELERATORS_TYPE = Literal["auto", "cpu", "gpu", "tpu"]
 DEVICES = 1
 VOLUME_SIZE = 60
 
-BUFFER_STORAGE_MODE = "in_memory"
-SUPPORTED_BUFFER_STORAGE_MODES = Literal["in_memory"]
 LEARNER = "ER"
 INSTANCE_COUNT = 1
 INSTANCE_MAX_TIME = 3 * 24 * 3600
 N_WORKERS = 1
 INSTANCE_TYPE = "ml.c5.xlarge"
 PYTHON_VERSION = "py38"
 FRAMEWORK_VERSION = "1.12.0"
@@ -91,16 +90,26 @@
 SER_POD_NORMALIZE = 1
 SER_CLS_ALPHA = 0.1
 SER_CLS_STABLE_MODEL_UPDATE_WEIGHT = 0.999
 SER_CLS_STABLE_MODEL_UPDATE_PROBABILITY = 0.7
 SER_CLS_PLASTIC_MODEL_UPDATE_WEIGHT = 0.999
 SER_CLS_PLASTIC_MODEL_UPDATE_PROBABILITY = 0.9
 
+# EWC
+EWC_LAMBDA = 0.4
+
+# LwF
+LWF_ALPHA = 1
+LWF_TEMPERATURE = 2
+
 MEMORY_SIZE = 32
 
+# Benchmark datasets/models
+TOKENIZER_KWARGS = dict(padding="max_length", max_length=128, truncation=True)
+
 
 def scheduler(config_space: Dict[str, Any], mode: str, metric: str):
     return FIFOScheduler(
         config_space=config_space,
         searcher="random",
         mode=mode,
         metric=metric,
@@ -111,32 +120,40 @@
     return str(datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S-%f"))
 
 
 def data_folder(working_directory: str):
     return os.path.join(working_directory, "data")
 
 
-def current_state_folder(working_directory: str):
-    return os.path.join(working_directory, "state")
+def input_state_folder(working_directory: str):
+    return os.path.join(working_directory, "input_state")
 
 
-def next_state_folder(working_directory: str):
-    return os.path.join(working_directory, "next_state")
+def output_state_folder(working_directory: str):
+    return os.path.join(working_directory, "output_state")
 
 
 def logs_folder(working_directory: str):
     return os.path.join(working_directory, "logs")
 
 
 def model_file(state_folder: str):
     return os.path.join(state_folder, "model.ckpt")
 
 
+LEARNER_CHECKPOINT_NAME = "learner.ckpt"
+AVALANCHE_CHECKPOINT_NAME = "avalanche.ckpt"
+
+
 def learner_state_file(state_folder: str):
-    return os.path.join(state_folder, "learner.ckpt")
+    return os.path.join(state_folder, LEARNER_CHECKPOINT_NAME)
+
+
+def avalanche_state_file(state_folder: str):
+    return os.path.join(state_folder, AVALANCHE_CHECKPOINT_NAME)
 
 
 def metric_summary_file(logs_folder: str, special_str: str = ""):
     return os.path.join(logs_folder, f"metrics_summary{special_str}.csv")
 
 
 def hpo_file(state_folder: str):
```

### Comparing `Renate-0.1.0/src/renate/evaluation/evaluator.py` & `Renate-0.2.0/src/renate/evaluation/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from pytorch_lightning import LightningModule, Trainer
 from pytorch_lightning.loggers.logger import Logger
 from torch.utils.data import DataLoader, Dataset
 
 from renate import defaults
 from renate.data.datasets import _TransformedDataset
 from renate.evaluation.metrics.utils import create_metrics
-from renate.models.renate_module import RenateModule
+from renate.models import RenateModule
 
 
 class Evaluator(LightningModule, abc.ABC):
     """A general Evaluator module for collection of quantitative metrics on the test dataset.
 
     This is an abstract interface which can be called with respect to a PyTorch Lightning `Trainer`.
-    and its `.test()` function. It collects quantitative observations with respect to a single dataset. The
-    metrics that are being collected are defined in the `create_metrics` function.
+    and its `.test()` function. It collects quantitative observations with respect to a single
+    dataset. The metrics that are being collected are defined in the `create_metrics` function.
 
     Args:
         model: A `RenateModule` to be evaluated.
         task: The machine learning problem considered.
         batch_size: The batch size to be used when creating the test data loader.
         transform: The transformation applied for evaluation.
         target_transform: The target transformation applied for evaluation.
@@ -81,15 +81,17 @@
         Logs the metrics and resets the metric collection.
         """
         self.log_dict(self._metric_collection.compute(), on_step=False, on_epoch=True)
         self._metric_collection.reset()
 
 
 class ClassificationEvaluator(Evaluator):
-    """A classification Evaluator module for collection of quantitative metrics on the test dataset."""
+    """A classification Evaluator module for collection of quantitative metrics on the test
+    dataset.
+    """
 
     def __init__(self, **kwargs: Any):
         super().__init__(task="classification", **kwargs)
 
     def forward(self, x, task_id: Optional[str] = None) -> torch.Tensor:
         """Forward pass of the model.
 
@@ -109,32 +111,35 @@
     transform: Optional[Callable] = None,
     target_transform: Optional[Callable] = None,
     logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
     logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
     accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
     devices: Optional[int] = None,
 ) -> Dict[str, List[float]]:
-    """Evaluate the model on the test dataset or a set of test datasets corresponding to distinct tasks.
+    """Evaluate the model on the test dataset or a set of test datasets corresponding to distinct
+    tasks.
 
-    If the `test_dataset` are specified as a list of datasets, it is assumed to be ordered. Similarly, in a case
-    the `task_id` are specified as a list, it is assumed to be ordered. A task ID list can be used to set specific
-    model part to be used, for example, an output head with some specific test dataset in the input sequence.
+    If the `test_dataset` are specified as a list of datasets, it is assumed to be ordered.
+    Similarly, in a case the `task_id` are specified as a list, it is assumed to be ordered. A task
+    ID list can be used to set specific model part to be used, for example, an output head with some
+    specific test dataset in the input sequence.
 
     Args:
         model: A `RenateModule` to be evaluated.
         test_dataset: The test dataset(s) to be evaluated.
         task_id: The task id(s) of the test dataset(s).
         batch_size: The batch size to be used when creating the test data loader.
         transform: The transformation applied for evaluation.
         target_transform: The target transformation applied for evaluation.
         logged_metrics: Metrics logged additional to the default ones.
         logger: Logger used by PyTorch Lightning to log intermediate results.
         accelerator: Accelerator used by PyTorch Lightning to train the model.
-        devices: Devices used by PyTorch Lightning to train the model. If the devices flag is not defined,
-                 it will assume devices to be "auto" and fetch the `auto_device_count` from the `accelerator`.
+        devices: Devices used by PyTorch Lightning to train the model. If the devices flag is not
+            defined, it will assume devices to be "auto" and fetch the `auto_device_count` from the
+            `accelerator`.
     """
     if isinstance(test_dataset, Dataset):
         test_dataset = [test_dataset]
 
     if isinstance(task_id, str):
         task_id = [task_id] * len(test_dataset)
```

### Comparing `Renate-0.1.0/src/renate/evaluation/metrics/classification.py` & `Renate-0.2.0/src/renate/evaluation/metrics/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     .. math::
         \\frac{1}{T}  sum_{i=1}^T  a_{T,i}
 
     where :math:`T` is the number of tasks, :math:`a_{T,i}` is the accuracy
     of the model on task :math:`i`, while having learned all tasks up to :math:`T`.
 
     Args:
-        results: The results dictionary holding all the results with respect to all recorded metrics.
+        results: The results dictionary holding all the results with respect to all recorded
+            metrics.
         task_id: The task index.
     """
     return sum(results["accuracy"][task_id][: task_id + 1]) / (task_id + 1)
 
 
 def forgetting(results: Dict[str, List[List[float]]], task_id: int) -> float:
     """Compute the forgetting measure of the model.
@@ -28,22 +29,23 @@
 
     .. math::
         \\frac{1}{T-1}  sum_{i=1}^{T-1}  f_{T,i}
 
     where :math:`f_{j,i}` is defined as:
 
     .. math::
-        f_{j,i} = \\max_{k\\in\{1, \\ldots, j=i\\}} a_{k,i} - a_{j,i}
+        f_{j,i} = \\max_{k\\in\\{1, \\ldots, j=i\\}} a_{k,i} - a_{j,i}
 
     where :math:`T` is the final task index, :math:`a_{n,i}` is the test classification accuracy
-    on task :math:`i` after sequentially learning the nth task and :math:`f_{j,i}` is a measure of forgetting
-    on task :math:`i` after training up to task :math:`j`.
+    on task :math:`i` after sequentially learning the nth task and :math:`f_{j,i}` is a measure of
+    forgetting on task :math:`i` after training up to task :math:`j`.
 
     Args:
-        results: The results dictionary holding all the results with respect to all recorded metrics.
+        results: The results dictionary holding all the results with respect to all recorded
+            metrics.
         task_id: The task index.
     """
     if task_id == 0:
         return 0.0
 
     def f(results: Dict[str, List[List[float]]], j: int, i: int) -> float:
         """A Helper function to compute the: math:`f_{j,i}`."""
@@ -65,15 +67,16 @@
     .. math::
         \\frac{1}{T-1}  sum_{i=1}^{T-1}  a_{T,i} - a_{i,i}
 
     where :math:`T` is the final task index, :math:`a_{n,i}` is the test classification accuracy
     on task :math:`i` after sequentially learning the nth task.
 
     Args:
-        results: The results dictionary holding all the results with respect to all recorded metrics.
+        results: The results dictionary holding all the results with respect to all recorded
+            metrics.
         task_id: The task index.
     """
     if task_id == 0:
         return 0.0
     return (
         sum([results["accuracy"][task_id][i] - results["accuracy"][i][i] for i in range(task_id)])
         / task_id
@@ -85,19 +88,20 @@
 
     This measure is defined by:
 
     .. math::
         \\frac{1}{T-1}  sum_{i=2}^{T}  a_{i-1,i} - b_{i}
 
     where :math:`T` is the final task index, :math:`a_{n,i}` is the test classification accuracy
-    on task :math:`i` after sequentially learning the nth task. :math:`b_{i}` is the accuracy for all
-    :math:`T` tasks recorded at initialisation prior to observing any task.
+    on task :math:`i` after sequentially learning the nth task. :math:`b_{i}` is the accuracy for
+    all :math:`T` tasks recorded at initialisation prior to observing any task.
 
     Args:
-        results: The results dictionary holding all the results with respect to all recorded metrics.
+        results: The results dictionary holding all the results with respect to all recorded
+            metrics.
         task_id: The task index.
     """
     if task_id == 0:
         return 0.0
     return sum(
         [
             results["accuracy"][i - 1][i] - results["accuracy_init"][0][i]
```

### Comparing `Renate-0.1.0/src/renate/evaluation/metrics/performance_regression_metrics.py` & `Renate-0.2.0/src/renate/evaluation/metrics/performance_regression_metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import torch
 from torchmetrics import Metric
 
 _DESCRIPTION = """
-    In classification tasks, sample-wise inconsistencies between models appear as “negative flips”:
+    In classification tasks, sample-wise inconsistencies between models appear as "negative flips":
     A new model incorrectly predicts the output for a test sample that was correctly
     classified by the old (reference) model. The fraction of the total number of negative flips
     and the total number of examples in the test set is called negative flip rate (NFR).
     Another metric for measuring regression is negative flip impact (NFI).
     Negative Flip Impact (NFI) measures the fraction of the total number of negative flips
     and the total number of errors in the test set. The difference between NFR and NFI
     is how they are normalized.
 """
 
 _CITATION = """
     @article{Yan2021PositiveCongruentTT,
         title={Positive-Congruent Training: Towards Regression-Free Model Updates},
-        author={Sijie Yan and Yuanjun Xiong and Kaustav Kundu and Shuo Yang 
+        author={Sijie Yan and Yuanjun Xiong and Kaustav Kundu and Shuo Yang
         and Siqi Deng and Meng Wang and Wei Xia and Stefano Soatto},
         journal={2021 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
         year={2021},
         pages={14294-14303}
     }
     @inproceedings{Xie2021RegressionBugs,
-        title={Regression Bugs Are In Your Model! Measuring, Reducing and Analyzing Regressions In NLP Model Updates},
-        author={Yuqing Xie and Yi{-}An Lai and Yuanjun Xiong and Yi Zhang and Shuo Yang and Stefano Soatto},
-        journal={Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics and 
-        the 11th International Joint Conference on Natural Language Processing (Volume 1: Long Papers)},
+        title={Regression Bugs Are In Your Model! Measuring, Reducing and Analyzing Regressions In
+            NLP Model Updates},
+        author={Yuqing Xie and Yi{-}An Lai and Yuanjun Xiong and Yi Zhang and Shuo Yang and Stefano
+            Soatto},
+        journal={Proceedings of the 59th Annual Meeting of the Association for Computational
+            Linguistics and the 11th International Joint Conference on Natural Language Processing
+            (Volume 1: Long Papers)},
         year={2021},
         pages={6589-6602}
         }
     @article{Cai2022MeasuringAR,
         title={Measuring and Reducing Model Update Regression in Structured Prediction for NLP},
         author={Deng Cai and Elman Mansimov and Yi-An Lai and Yixuan Su and Lei Shu and Yi Zhang},
         journal={ArXiv},
@@ -41,31 +44,33 @@
 """
 
 
 class NegativeFlipRateMetric(Metric):
     """Compute Negative Flip Rate (NFR) between new and old models' predictions,
 
     NFR = len((pred_old == labels) and (pred_new != labels)) / len(test_set).
-
-    Args:
-        new_pred: a 1-D torch tensor contains new model's predicted labels.
-        old_pred: a 1-D torch tensor contains old model's predicted labels.
-        labels: a 1-D torch tensor contains ground truth labels.
     """
 
     full_state_update: bool = False
     higher_is_better: bool = False
     is_differentiable: bool = False
 
     def __init__(self):
         super().__init__()
         self.add_state("neg_flip_num", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
     def update(self, new_pred: torch.Tensor, old_pred: torch.Tensor, labels: torch.Tensor):
+        """Update the metric.
+
+        Args:
+            new_pred: a 1-D torch tensor contains new model's predicted labels.
+            old_pred: a 1-D torch tensor contains old model's predicted labels.
+            labels: a 1-D torch tensor contains ground truth labels.
+        """
         assert (
             new_pred.shape == old_pred.shape == labels.shape
         ), "dim of new_pred, old_pred, and labels are not matched!"
         assert len(new_pred) > 0, "input tensor is empty!"
         neg_flip_samples = (old_pred == labels) & (new_pred != labels)
         self.neg_flip_num += torch.sum(neg_flip_samples)
         self.total += len(labels)
@@ -74,31 +79,33 @@
         return self.neg_flip_num.float() / self.total
 
 
 class NegativeFlipImpactMetric(Metric):
     """Compute Negative Flip Impact (NFI) between new and old models' predictions,
 
     NFI = len((pred_old == labels) and (pred_new != labels)) / len(pred_new != labels).
-
-    Args:
-        new_pred: a 1-D torch tensor contains new model's predicted labels.
-        old_pred: a 1-D torch tensor contains old model's predicted labels.
-        labels: a 1-D torch tensor contains ground truth labels.
     """
 
     full_state_update: bool = False
     higher_is_better: bool = False
     is_differentiable: bool = False
 
     def __init__(self):
         super().__init__()
         self.add_state("new_num_errors", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("neg_flip_num", default=torch.tensor(0), dist_reduce_fx="sum")
 
     def update(self, new_pred: torch.Tensor, old_pred: torch.Tensor, labels: torch.Tensor):
+        """Updates the metric.
+
+        Args:
+            new_pred: a 1-D torch tensor contains new model's predicted labels.
+            old_pred: a 1-D torch tensor contains old model's predicted labels.
+            labels: a 1-D torch tensor contains ground truth labels.
+        """
         assert (
             new_pred.shape == old_pred.shape == labels.shape
         ), "dim of new_pred, old_pred, and labels are not matched!"
         assert len(new_pred) > 0, "input tensor is empty!"
         neg_flip_samples = (old_pred == labels) & (new_pred != labels)
         self.neg_flip_num += torch.sum(neg_flip_samples)
         self.new_num_errors += torch.sum(new_pred != labels)
@@ -107,31 +114,33 @@
         return self.neg_flip_num.float() / self.new_num_errors
 
 
 class PositiveFlipRateMetric(Metric):
     """Compute Positive Flip Rate (PFR) between new and old models' predictions,
 
     PFR = len((pred_old != labels) and (pred_new == labels)) / len(test_set).
-
-    Args:
-        new_pred: a 1-D torch tensor contains new model's predicted labels.
-        old_pred: a 1-D torch tensor contains old model's predicted labels.
-        labels: a 1-D torch tensor contains ground truth labels.
     """
 
     full_state_update: bool = False
     higher_is_better: bool = True
     is_differentiable: bool = False
 
     def __init__(self):
         super().__init__()
         self.add_state("pos_flip_num", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
     def update(self, new_pred: torch.Tensor, old_pred: torch.Tensor, labels: torch.Tensor):
+        """Updates the metric.
+
+        Args:
+            new_pred: a 1-D torch tensor contains new model's predicted labels.
+            old_pred: a 1-D torch tensor contains old model's predicted labels.
+            labels: a 1-D torch tensor contains ground truth labels.
+        """
         assert (
             new_pred.shape == old_pred.shape == labels.shape
         ), "dim of new_pred, old_pred, and labels are not matched!"
         assert len(new_pred) > 0, "input tensor is empty!"
         pos_flip_samples = (old_pred != labels) & (new_pred == labels)
         self.pos_flip_num += torch.sum(pos_flip_samples)
         self.total += len(labels)
@@ -140,31 +149,33 @@
         return self.pos_flip_num.float() / self.total
 
 
 class PositiveFlipImpactMetric(Metric):
     """Compute Positive Flip Impact (PFI) between new and old models' predictions,
 
     PFI = len((pred_old != labels) and (pred_new == labels)) / len(pred_new == labels).
-
-    Args:
-        new_pred: a 1-D torch tensor contains new model's predicted labels.
-        old_pred: a 1-D torch tensor contains old model's predicted labels.
-        labels: a 1-D torch tensor contains ground truth labels.
     """
 
     full_state_update: bool = False
     higher_is_better: bool = True
     is_differentiable: bool = False
 
     def __init__(self):
         super().__init__()
         self.add_state("new_num_correct", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("pos_flip_num", default=torch.tensor(0), dist_reduce_fx="sum")
 
     def update(self, new_pred: torch.Tensor, old_pred: torch.Tensor, labels: torch.Tensor):
+        """Updates the metric.
+
+        Args:
+            new_pred: a 1-D torch tensor contains new model's predicted labels.
+            old_pred: a 1-D torch tensor contains old model's predicted labels.
+            labels: a 1-D torch tensor contains ground truth labels.
+        """
         assert (
             new_pred.shape == old_pred.shape == labels.shape
         ), "dim of new_pred, old_pred, and labels are not matched!"
         assert len(new_pred) > 0, "input tensor is empty!"
         pos_flip_samples = (old_pred != labels) & (new_pred == labels)
         self.pos_flip_num += torch.sum(pos_flip_samples)
         self.new_num_correct += torch.sum(new_pred == labels)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Renate-0.1.0/src/renate/evaluation/metrics/utils.py` & `Renate-0.2.0/src/renate/evaluation/metrics/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,24 +11,25 @@
     task: defaults.SUPPORTED_TASKS_TYPE,
     additional_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
 ) -> torchmetrics.MetricCollection:
     """Creates task-specific metrics including all additional metrics.
 
     Args:
         task: Whether classification or regression, for now.
-        additional_metrics: Dictionary of additionally metrics to be added to the returned `MetricCollection`.
+        additional_metrics: Dictionary of additionally metrics to be added to the returned
+            `MetricCollection`.
     """
     if task == "classification":
         metric_collection = {
             "accuracy": torchmetrics.Accuracy(),
         }
     elif task == "regression":
         metric_collection = {"mean_squared_error": torchmetrics.MeanSquaredError()}
     else:
         raise NotImplementedError(f"Task {task} not implemented.")
     if additional_metrics:
         assert set(metric_collection).isdisjoint(set(additional_metrics)), (
-            f"Use a different name for your custom metrics. Following names are reserved for the default metrics: "
-            f"{set(metric_collection)}."
+            "Use a different name for your custom metrics. Following names are reserved for the "
+            f"default metrics: {set(metric_collection)}."
         )
         metric_collection.update(additional_metrics)
     return torchmetrics.MetricCollection(metric_collection)
```

### Comparing `Renate-0.1.0/src/renate/memory/buffer.py` & `Renate-0.2.0/src/renate/memory/buffer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,356 +1,340 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from abc import ABC, abstractmethod
 from collections import defaultdict
-from typing import Any, Callable, Dict, Optional, Tuple
+import copy
+from typing import Callable, Dict, Optional
 
 import torch
 from torch.utils.data import Dataset
 
 from renate import defaults
+from renate.memory.storage import MemoryMappedTensorStorage
+from renate.types import NestedTensors
 from renate.utils.pytorch import get_generator
 
-DataTuple = Tuple[torch.Tensor, ...]
 DataDict = Dict[str, torch.Tensor]
 
 
-class DataBuffer(Dataset, ABC):
+class DataBuffer(Dataset):
     """A memory buffer storing data points.
 
-    The buffer functions as a torch dataset, i.e., it implements `__len__` and
-    `__getitem__`. Pytorch data loaders can be used to sample from or iterate
-    over the buffer.
-
-    Extracting an element from the buffer will return a tuple,
-    `data_point, metadata = buffer[i]`, where `data_point` is the raw data point
-    and `metadata` is a dictionary containing associated metadata (identical
-    keys for all data points, possibly empty) and the index `idx` of the currently
-    sampled data sample, referring to the ordering inside of the buffer.
-    It is assumed that all passed in data are PyTorch tensors.
-    Metadata can be passed externally when calling `Buffer.update` and
-    additional fields of metadata might be added by some buffering methods, e.g.,
-    instance weights in coreset methods.
-
-    Note that the buffer does not change the device placement of data passed to it.
-    Please ensure that the data passed to `DataBuffer.update` resides on the CPU.
-
-    Note that, in order to apply transformations, the buffer assumes that the datapoints
-    are tuples of exactly 2 tensors i.e. `(x, y)` where `x` is the input and `y` is some target.
-
-    Args:
-        max_size: Maximal size of the buffer.
-        storage_mode: How to store the data in the buffer. Currently, we only
-           support `in_memory`.
-        seed: Seed for the random number generator used in the buffer.
-        transform: The transformation to be applied to the memory buffer data samples.
-        target_transform: The target transformation to be applied to the memory buffer target samples.
+    The buffer functions as a torch dataset, i.e., it implements `__len__` and `__getitem__`.
+    Pytorch data loaders can be used to sample from or iterate over the buffer.
+
+    Data can be added to the buffer via `buffer.update(dataset, metadata)`. `dataset` is a
+    pytorch dataset expected to return an arbitrary nested `tuple`/`dict` structure containing
+    `torch.Tensor`s of _fixed_ size and data type. `metadata` is a dictionary mapping strings to
+    tensors for associated metadata. The logic to decide which data points remain in the buffer is
+    implemented by different subclasses.
+
+    Extracting an element from the buffer will return a nested tuple of the form
+    `data_point, metadata = buffer[i]`, where `data_point` is the raw data point  and `metadata` is
+    a dictionary containing associated metadata as well as field `idx` containing the index of the
+    data point in the buffer. Additional fields of metadata might be added by some buffering
+    methods, e.g., instance weights in coreset methods.
+
+    In addition to passing metadata to the `update` method, one also access and replace the metadata
+    in the buffer via the `get_metadata` and `set_metadata` methods.
+
+    Note that, in order to apply transformations, the buffer assumes that the data points are tuples
+    of the form `(x, y)`. We apply `transform` to `inputs` and `target_transform` to `y`. Ensure
+    that the transforms accept the correct type, e.g., if `x` is a dictionary, `transform` needs to
+    operate on a dictionary.
     """
 
     def __init__(
         self,
         max_size: Optional[int] = None,
-        storage_mode: defaults.SUPPORTED_BUFFER_STORAGE_MODES = defaults.BUFFER_STORAGE_MODE,
         seed: int = defaults.SEED,
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
     ) -> None:
         self._max_size = max_size
-        self._storage_mode = storage_mode
         self._seed = seed
+        self._transform = transform
+        self._target_transform = target_transform
 
         self._rng = get_generator(self._seed)
 
         self._count = 0
-
-        self._data_points: DataDict = {}
-        self.metadata: DataDict = {}
-        self._size = 0
-
-        self._transform = transform
-        self._target_transform = target_transform
+        self._datasets = []
+        self._indices = {}
+        self._data_point_prototype = None
+        self._metadata = {}
 
     def __len__(self) -> int:
-        """Returns the number of data points in the buffer."""
-        return self._size
+        """Returns the current length of the buffer."""
+        return len(self._indices)
 
-    def __getitem__(self, idx: int) -> Tuple[DataTuple, DataDict]:
-        """Retrieves a data point from the buffer."""
-        metadata = {key: value[idx] for key, value in self.metadata.items()}
-        metadata["idx"] = torch.tensor(idx, dtype=torch.long)
-        data = tuple(self._data_points[f"{i}"][idx] for i in range(len(self._data_points)))
-        if self._transform is not None or self._target_transform is not None:
-            x, y = data
+    def __getitem__(self, idx: int) -> NestedTensors:
+        """Reads the item at index `idx` of the buffer."""
+        i, j = self._indices[idx]
+        data = self._datasets[i][j]
+        metadata = {key: value[idx] for key, value in self._metadata.items()}
+        if self._transform is None and self._target_transform is None:
+            return data, metadata
+        else:
+            inputs, targets = data
             if self._transform is not None:
-                x = self._transform(x)
+                inputs = self._transform(inputs)
             if self._target_transform is not None:
-                y = self._target_transform(y)
-            return (x, y), metadata
-        return data, metadata
-
-    def _verify_metadata(self, metadata: DataDict, expected_length: int) -> None:
-        """Verifies that passed metadata is compatible with internal metadata."""
-        if len(self) == 0:
-            return
-
-        if set(self.metadata.keys()) != set(metadata.keys()):
-            raise KeyError(
-                f"Keys of provided metadata {list(metadata.keys())} do not match those present in ",
-                f"the buffer {list(self.metadata.keys())}.",
-            )
-
-        for key in metadata:
-            if not isinstance(metadata[key], torch.Tensor):
-                raise TypeError(
-                    f"Metadata needs to map to `torch.Tensor`, found {type(metadata[key])} at ",
-                    f"key {key}.",
-                )
-            if metadata[key].dtype != self.metadata[key].dtype:
-                raise TypeError(
-                    f"Provided metadata at key {key} is of type {metadata[key].dtype}. This does "
-                    f"not match type {self.metadata[key].dtype} already present in the buffer."
-                )
-            if metadata[key].size(0) != expected_length:
-                raise ValueError(
-                    f"Tensors in metadata dictionary need to be of size {expected_length} (size ",
-                    f"of the associated dataset) in dimension 0. Found size {metadata[key].size()} ",
-                    f"at key {key}.",
-                )
+                targets = self._target_transform(targets)
+            return (inputs, targets), metadata
 
-    def __setitem__(self, idx: int, data_and_metadata: Tuple[DataTuple, DataDict]) -> None:
-        """Replaces a data point in the buffer."""
-        data, metadata = data_and_metadata
-        for i, d in enumerate(data):
-            self._data_points[f"{i}"][idx] = d
-        for key in metadata:
-            self.metadata[key][idx] = metadata[key]
-
-    def _append(self, data: DataTuple, metadata: DataDict) -> None:
-        """Appends a data point to the internal storage."""
-        for i, d in enumerate(data):
-            key = f"{i}"  # FIXME: choose a better naming for the keys of the data points coming from the dataset
-            if key not in self._data_points:
-                self._data_points[key] = torch.empty(
-                    (self._max_size, *d.shape), dtype=d.dtype, device=d.device
-                )
+    def update(self, dataset: Dataset, metadata: Optional[Dict] = None) -> None:
+        """Updates the buffer with a new dataset."""
+        metadata = metadata or {}
+        self._check_metadata_internal_consistency(metadata, expected_length=len(dataset))
+        if not len(self):
+            self._data_point_prototype = copy.deepcopy(dataset[0])
+            self._add_metadata_like(metadata)
+        else:
+            self._check_metadata_compatibility(metadata)
+        assignments = self._update(dataset, metadata)
+        self._check_assignments_are_contiguous(assignments)
+
+        # Perform assignments.
+        d = len(self._datasets)
+        self._datasets.append(dataset)
+        for buffer_idx, dataset_idx in assignments.items():
+            self._indices[buffer_idx] = (d, dataset_idx)
+            for key in self._metadata.keys():
+                self._metadata[key][buffer_idx] = metadata[key][dataset_idx]
 
-        for key in metadata:
-            if key not in self.metadata:
-                self.metadata[key] = torch.empty(
-                    (self._max_size, *metadata[key].shape),
-                    dtype=metadata[key].dtype,
-                    device=metadata[key].device,
-                )
-        self[self._size] = data, metadata
-        self._size += 1
+    def _update(self, dataset: Dataset, metadata: Dict) -> Dict[int, int]:
+        """Returns the updates.
 
-    def update(self, dataset: Dataset, metadata: Optional[DataDict] = None) -> None:
-        """Updates the buffer with a new dataset.
+        This method is used to implement different buffering methods. Given a dataset, it returns a
+        dictionary of `assignments` indicating the updates to be performed to the buffer.
 
         Args:
-            dataset: A dataset containing a new chunk of data.
-            metadata: A dictionary mapping to tensors, which are assumed to
-                have size n in dimension 0, where `n = len(dataset)`.
+            dataset: The dataset used to update the buffer.
+
+        Returns:
+            assignments: A dictionary mapping int to int. The presence of the pair `(i, j)` means
+                that the `i`-th buffer slot will be filled with the `j`-th element of `dataset`.
         """
-        metadata = metadata or {}
-        self._verify_metadata(metadata, expected_length=len(dataset))
-        return self._update(dataset, metadata)
+        raise NotImplementedError()
+
+    def get_metadata(self, key: str) -> Dict[str, torch.Tensor]:
+        return self._metadata[key][: len(self)]
 
-    @abstractmethod
-    def _update(self, dataset: Dataset, metadata: DataDict) -> None:
-        pass
+    def set_metadata(self, key: str, values: torch.Tensor) -> None:
+        if values.size(0) != len(self):
+            raise ValueError()
+        if key not in self._metadata:
+            self._add_metadata_like({key: values})
+        self._metadata[key][: len(self)] = values.cpu()
 
     def set_transforms(
         self, transform: Optional[Callable] = None, target_transform: Optional[Callable] = None
     ) -> None:
         """Update the transformations applied to the data."""
         self._transform = transform
         self._target_transform = target_transform
 
-    def state_dict(self) -> Dict[str, Any]:
-        """Returns the state of the buffer as a dictionary."""
+    def state_dict(self) -> Dict:
         return {
             "buffer_class_name": self.__class__.__name__,
             "max_size": self._max_size,
-            "storage_mode": self._storage_mode,
             "seed": self._seed,
             "count": self._count,
-            "size": self._size,
-            "data_points": self._data_points,
-            "metadata": self.metadata,
+            "indices": self._indices,
+            "data_point_prototype": self._data_point_prototype,
+            "metadata": self._metadata,
         }
 
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        """Assigns the values from `state_dict` into their respective attributes."""
+    def load_state_dict(self, state_dict: Dict) -> None:
         if self.__class__.__name__ != state_dict["buffer_class_name"]:
             raise RuntimeError(
                 f"Buffer of class {self.__class__} was used to load a state dict created by class "
                 f"{state_dict['buffer_class_name']}."
             )
         self._max_size = state_dict["max_size"]
-        self._storage_mode = state_dict["storage_mode"]
         self._seed = state_dict["seed"]
         self._count = state_dict["count"]
-        self._size = state_dict["size"]
-        self._data_points = state_dict["data_points"]
-        self.metadata = state_dict["metadata"]
-
+        self._indices = state_dict["indices"]
+        self._data_point_prototype = state_dict["data_point_prototype"]
+        self._metadata = state_dict["metadata"]
         self._rng = get_generator(self._seed)
 
-        for key in ["count", "size"]:
-            if not isinstance(state_dict[key], int):
-                raise TypeError(f"Invalid type for: {key}, should be int.")
-
-        if not isinstance(state_dict["storage_mode"], str):
-            raise TypeError("Invalid type for storage_mode, should be str.")
-
-        if not isinstance(state_dict["data_points"], dict):
-            raise TypeError("Invalid container for data points, should be a dictionary.")
-
-        if not isinstance(state_dict["metadata"], dict):
-            raise TypeError("Invalid container for metadata, should be a dictionary.")
-
+    def save(self, target_dir: str) -> None:
+        if not len(self):
+            return
 
-class InfiniteBuffer(DataBuffer):
-    """A data buffer that supports infinite size.
+        transforms = self._transform, self._target_transform
+        self._transform, self._target_transform = None, None
+        storage = MemoryMappedTensorStorage(
+            target_dir,
+            data_point=self._data_point_prototype,
+            length=len(self),
+        )
+        for i in range(len(self)):
+            storage[i] = self[i][0]  # Drop metadata.
+        self._datasets = [storage]
+        self._indices = {i: (0, i) for i in range(len(self))}
+        self.set_transforms(*transforms)
 
-    Args:
-        storage_mode: How to store the data in the buffer. Currently, we only
-           support `in_memory`.
-        transform: The transformation to be applied to the memory buffer data samples.
-        target_transform: The target transformation to be applied to the memory buffer target samples.
-    """
+    def load(self, source_dir: str) -> None:
+        if not len(self):
+            return
 
-    def __init__(
-        self,
-        storage_mode: defaults.SUPPORTED_BUFFER_STORAGE_MODES = defaults.BUFFER_STORAGE_MODE,
-        transform: Optional[Callable] = None,
-        target_transform: Optional[Callable] = None,
-    ) -> None:
-        super().__init__(
-            storage_mode=storage_mode, transform=transform, target_transform=target_transform
+        storage = MemoryMappedTensorStorage(
+            source_dir,
+            data_point=self._data_point_prototype,
+            length=len(self),
         )
-        self._max_size = 1
+        self._datasets = [storage]
 
-    def _update(self, dataset: Dataset, metadata: DataDict) -> None:
-        for i in range(len(dataset)):
-            self._append(dataset[i], {key: value[i] for key, value in metadata.items()})
+    def _add_metadata_like(self, metadata: DataDict):
+        for key, value in metadata.items():
+            self._metadata[key] = torch.empty(
+                (self._max_size, *value.size()[1:]), dtype=value.dtype, device="cpu"
+            )
 
-    def _append(self, data: DataTuple, metadata: DataDict) -> None:
-        """Appends a data point to the internal storage.
+    def _check_assignments_are_contiguous(self, assignments):
+        # The subclass _update method is expected to only return assignments that populate the
+        # buffer contiguously. We check this here. The invariant we expect to hold is that, at any
+        # time, the indices 0:len(buffer) are filled.
+        current_length = len(self)
+        new_idx = [i for i in assignments.keys() if i > current_length]
+        if new_idx:
+            assert max(new_idx) == current_length + len(new_idx)
+
+    @staticmethod
+    def _check_metadata_internal_consistency(metadata: DataDict, expected_length: int):
+        """Checks metadata for internal consistency and an expected length."""
+        for key in metadata:
+            if not isinstance(metadata[key], torch.Tensor):
+                raise TypeError(
+                    f"Expected tensors in `metadata`, found {type(metadata[key])} at key {key}."
+                )
+            if not metadata[key].size(0) == expected_length:
+                raise ValueError(
+                    f"Tensors in metadata dictionary need to be of size {expected_length} (size "
+                    f"of the associated dataset) in dimension 0. Found size {metadata[key].size()} "
+                    f"at key {key}."
+                )
 
-        Initializes a new buffer with twice the size if the current one is full.
-        """
-        super()._append(data, metadata)
-        if self._size == self._max_size:
-            data_containers = [self._data_points, metadata]
-            for data_container in data_containers:
-                for key in data_container:
-                    data_container[key] = torch.cat(
-                        [data_container[key], torch.empty_like(data_container[key])], dim=0
-                    )
-            self._max_size *= 2
+    def _check_metadata_compatibility(self, metadata: DataDict) -> None:
+        """Verifies that passed metadata is compatible with internal metadata."""
+        if not len(self):
+            return
+        if set(self._metadata.keys()) != set(metadata.keys()):
+            raise KeyError(
+                f"Keys of provided metadata {list(metadata.keys())} do not match those present in ",
+                f"the buffer {list(self._metadata.keys())}.",
+            )
+        for key in metadata:
+            if metadata[key].size()[1:] != self._metadata[key].size()[1:]:
+                raise ValueError()
+            if metadata[key].dtype != self._metadata[key].dtype:
+                raise TypeError(
+                    f"Provided metadata at key {key} is of type {metadata[key].dtype}. This does "
+                    f"not match type {self._metadata[key].dtype} already present in the buffer."
+                )
 
 
 class ReservoirBuffer(DataBuffer):
-    """A buffer implementing reservoir sampling.
+    """A buffer implementing reservoir sampling."""
 
-    Reservoir sampling maintains a uniform subset of the data seen so far.
-
-    TODO: Adjust citation once we've agreed on a format.
-    Jeffrey S. Vitter. 1985. Random sampling with a reservoir. ACM Trans.
-    Math. Softw. 11, 1 (March 1985), 37–57. https://doi.org/10.1145/3147.3165
-    """
-
-    def _update(self, dataset: Dataset, metadata: DataDict) -> None:
+    def _update(self, dataset: Dataset, metadata: Dict) -> Dict[int, int]:
+        assignments = {}
         for i in range(len(dataset)):
-            if len(self) < self._max_size:
-                self._append(dataset[i], {key: value[i] for key, value in metadata.items()})
+            if self._count < self._max_size:
+                assignments[self._count] = i
             else:
                 rand = torch.randint(low=0, high=self._count, size=(), generator=self._rng).item()
                 if rand < self._max_size:
-                    self[rand] = (dataset[i], {key: value[i] for key, value in metadata.items()})
+                    assignments[rand] = i
             self._count += 1
+        return assignments
 
 
 class SlidingWindowBuffer(DataBuffer):
-    """A sliding window buffer, retaining the most recent data points."""
+    """A buffer implementing a sliding window."""
 
-    def _update(self, dataset: Dataset, metadata: DataDict) -> None:
+    def _update(self, dataset: Dataset, metadata) -> Dict[int, int]:
+        assignments = {}
         for i in range(len(dataset)):
-            if len(self) < self._max_size:
-                self._append(dataset[i], {key: value[i] for key, value in metadata.items()})
-            else:
-                self[self._count % self._max_size] = (
-                    dataset[i],
-                    {key: value[i] for key, value in metadata.items()},
-                )
+            assignments[self._count % self._max_size] = i
             self._count += 1
+        return assignments
 
 
 class GreedyClassBalancingBuffer(DataBuffer):
-    """A greedy class balancing buffer as proposed in:
+    """A buffer implementing a greedy class-balancing approach."""
+
+    def __init__(
+        self,
+        max_size: Optional[int] = None,
+        seed: int = defaults.SEED,
+        transform: Optional[Callable] = None,
+        target_transform: Optional[Callable] = None,
+    ) -> None:
+        super().__init__(max_size, seed, transform, target_transform)
+        self._indices_by_class = defaultdict(list)
 
-    Prabhu, Ameya, Philip HS Torr, and Puneet K. Dokania. "GDumb: A simple
-    approach that questions our progress in continual learning." ECCV, 2020.
+    def state_dict(self) -> Dict:
+        state_dict = super().state_dict()
+        state_dict["indices_by_class"] = self._indices_by_class
+        return state_dict
 
-    Note that, this implementation works only with respect to classification problems
-    and datasets, where we expect the data coming from the dataset to be organised
-    as `x,y` tuples where `x` is the input and `y` is an integer class index.
-    """
+    def load_state_dict(self, state_dict: Dict) -> None:
+        super().load_state_dict(state_dict)
+        self._indices_by_class = defaultdict(list)
+        self._indices_by_class.update(state_dict["indices_by_class"])
 
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs)
-        self._class_to_index_map = defaultdict(list)
+    def _get_largest_class(self):
+        largest_classes = []
+        max_length = 0
+        for y, indices in self._indices_by_class.items():
+            if len(indices) > max_length:
+                largest_classes = [y]
+                max_length = len(indices)
+            if len(indices) == max_length:
+                largest_classes.append(y)
+        rand = torch.randint(low=0, high=len(largest_classes), size=(1,), generator=self._rng)
+        largest_class = largest_classes[rand.item()]
+        return largest_class, max_length
 
-    def _update(self, dataset: Dataset, metadata: DataDict) -> None:
+    def _update(self, dataset: Dataset, metadata: Dict) -> Dict[int, int]:
+        assignments = {}
         for i in range(len(dataset)):
-            if len(self) < self._max_size:
-                self._append(dataset[i], {key: value[i] for key, value in metadata.items()})
-                self._record_class_index(dataset[i], len(self) - 1)
+            y = int(dataset[i][1])
+            if self._count < self._max_size:
+                assignments[self._count] = i
+                self._indices_by_class[y].append(self._count)
             else:
-                class_counts_max_value = max(
-                    [len(self._class_to_index_map[key]) for key in self._class_to_index_map.keys()]
-                )
-                largest_classes = [
-                    k
-                    for k, v in self._class_to_index_map.items()
-                    if len(v) == class_counts_max_value
-                ]
-                largest_class = largest_classes[
-                    torch.randint(
-                        low=0, high=len(largest_classes), size=(1,), generator=self._rng
-                    ).item()
-                ]
-                memory_idx_to_replace = self._class_to_index_map[largest_class][
-                    torch.randint(
-                        low=0,
-                        high=len(self._class_to_index_map[largest_class]),
-                        size=(1,),
-                        generator=self._rng,
-                    ).item()
-                ]
-                self[memory_idx_to_replace] = (
-                    dataset[i],
-                    {key: value[i] for key, value in metadata.items()},
-                )
-                self._class_to_index_map[largest_class].remove(memory_idx_to_replace)
-                self._record_class_index(dataset[i], memory_idx_to_replace)
-
+                largest_class, max_length = self._get_largest_class()
+                rand = torch.randint(low=0, high=max_length, size=(1,), generator=self._rng).item()
+                idx_to_replace = self._indices_by_class[largest_class].pop(rand)
+                assignments[idx_to_replace] = i
+                self._indices_by_class[y].append(idx_to_replace)
             self._count += 1
+        return assignments
 
-    def _record_class_index(self, data: DataTuple, target_index: int) -> None:
-        """Helper function to record the class membership in the mapping."""
-        _, y = data
-        if isinstance(y, torch.Tensor):
-            y = y.item()
-        self._class_to_index_map[y].append(target_index)
 
-    def state_dict(self) -> Dict[str, Any]:
-        """Returns the state of the buffer as a dictionary."""
-        state_dict = super().state_dict()
-        state_dict["class_to_index_map"] = self._class_to_index_map
-        return state_dict
+class InfiniteBuffer(DataBuffer):
+    """A data buffer that stores _all_ incoming data."""
 
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        super().load_state_dict(state_dict)
-        self._class_to_index_map = state_dict["class_to_index_map"]
+    def __init__(
+        self,
+        transform: Optional[Callable] = None,
+        target_transform: Optional[Callable] = None,
+    ) -> None:
+        super().__init__(max_size=1, transform=transform, target_transform=target_transform)
+
+    def _update(self, dataset: Dataset, metadata: Dict) -> Dict[int, int]:
+        # Resize metadata dictionary.
+        if self._count + len(dataset) > self._max_size:
+            while self._count + len(dataset) > self._max_size:
+                self._max_size *= 2
+            current_metadata = {key: self.get_metadata(key).clone() for key in self._metadata}
+            self._add_metadata_like(current_metadata)
+            for key, values in current_metadata.items():
+                self.set_metadata(key, values)
+
+        assignments = {self._count + i: i for i in range(len(dataset))}
+        self._count += len(dataset)
+        return assignments
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Renate-0.1.0/src/renate/models/layers/cn.py` & `Renate-0.2.0/src/renate/models/layers/cn.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class ContinualNorm(_BatchNorm):
     """Continual Normalization as a replacement for Batch Normalization.
 
     Pham, Quang, Chenghao Liu, and Steven Hoi.
     "Continual normalization: Rethinking batch normalization for online continual learning."
     International Conference on Learning Representations (2022).
 
-    It combines Group Normalization with respect to a user-defined `num_groups` parameter, the number of groups in Group Normalization,
-    followed by Batch Normalization.
+    It combines Group Normalization with respect to a user-defined `num_groups` parameter, the
+    number of groups in Group Normalization, followed by Batch Normalization.
 
     Args:
         num_features: The number of input features in the channel dimension.
         eps:  A value added to the denominator for numerical stability.
         momentum: the value used for the running_mean and running_var computation.
                   Can be set to ``None`` for cumulative moving average.
         affine: Whether learnable affine parameters are going to be used in Batch Normalization.
```

### Comparing `Renate-0.1.0/src/renate/models/renate_module.py` & `Renate-0.2.0/src/renate/models/renate_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import copy
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List, Optional, Set
 
 import torch
 
 from renate.models.layers import ContinualNorm
+from renate.types import NestedTensors
 
 
 class RenateModule(torch.nn.Module, ABC):
     """A class for torch models with some additional functionality for continual learning.
 
     ``RenateModule`` derives from ``torch.nn.Module`` and provides some additional functionality
     relevant to continual learning. In particular, this concerns saving and reloading the model
@@ -87,23 +88,26 @@
     def set_extra_state(self, state: Any):
         """Extract the content of the ``_extra_state`` and set the related values in the module."""
         self._constructor_arguments = state["constructor_arguments"]
         self._tasks_params_ids = state["tasks_params_ids"]
         self.loss_fn = state["loss_fn"]
 
     @abstractmethod
-    def forward(self, x: torch.Tensor, task_id: Optional[str] = None) -> torch.Tensor:
+    def forward(self, x: NestedTensors, task_id: Optional[str] = None) -> torch.Tensor:
         """Performs a forward pass on the inputs and returns the predictions.
 
         This method accepts a task ID, which may be provided by some continual learning scenarios.
-        As an examle, the task id may be used to switch between multiple output heads.
+        As an example, the task id may be used to switch between multiple output heads.
 
         Args:
-            x: The input tensor.
+            x: Input(s) to the model. Can be a single tensor, a tuple of tensor, or a dictionary
+                mapping strings to tensors.
             task_id: The identifier of the task for which predictions are made.
+        Returns:
+            The model's predictions.
         """
         pass
 
     def get_params(self, task_id: Optional[str] = None) -> List[torch.nn.Parameter]:
         """User-facing function which returns the list of parameters.
 
         If a ``task_id`` is given, this should return only parameters used for the specific task.
@@ -134,22 +138,23 @@
             task_id: The task id for which the new parameters are added.
         """
         if task_id in self._tasks_params_ids:
             return
         self._add_task_params(task_id)
         self._tasks_params_ids.add(task_id)
 
-    def get_logits(self, x: torch.Tensor, task_id: Optional[str] = None) -> torch.Tensor:
+    def get_logits(self, x: NestedTensors, task_id: Optional[str] = None) -> torch.Tensor:
         """Returns the logits for a given pair of input and task id.
 
         By default, this method returns the output of the forward pass. This may be overwritten
         with custom behavior, if necessary.
 
         Args:
-            x: The input tensor.
+            x: Input(s) to the model. Can be a single tensor, a tuple of tensor, or a dictionary
+                mapping strings to tensors.
             task_id: The task id.
         """
         return self.forward(x, task_id)
 
     def get_intermediate_representation(self) -> List[torch.Tensor]:
         """Returns the cached intermediate representation."""
         return self._intermediate_representation_cache
@@ -158,15 +163,15 @@
         """Replaces every occurence of batch normalization with continual normalization.
 
         Pham, Q., Liu, C., & Hoi, S. (2022). Continual normalization: Rethinking batch
         normalization for online continual learning. arXiv preprint arXiv:2203.16102.
 
         Args:
             num_groups: Number of groups when considering the group normalization in continual
-                normalizeion
+                normalization.
         """
 
         def _replace(module):
             for name, child in module.named_children():
                 if not list(module.children()):
                     _replace(child)
                 if isinstance(
@@ -220,15 +225,17 @@
 
 
 class RenateWrapper(RenateModule):
     """A simple wrapper around a torch model.
 
     If you are using a torch model with fixed hyperparameters, you can use this wrapper to expose
     it as a ``RenateModule``. In this case, do _not_ use the ``from_state_dict`` method but
-    reinstantiate the model, wrap it, and call ``load_state_dict``.
+    reinstantiate the model, wrap it, and call ``load_state_dict``. If a tuple or a dictionary of
+    tensors is passed to the `RenateWrapper`'s forward function, it is unpacked before passing it
+    to the torch model's forward function.
 
     Example::
 
         my_torch_model = torch.nn.Linear(28*28, 10)  # Instantiate your torch model.
         model = RenateWrapper(my_torch_model)
         state_dict = torch.load("my_state_dict.pt")
         model.load_state_dict(state_dict)
@@ -238,16 +245,28 @@
         loss_fn: The loss function to be optimized during the training.
     """
 
     def __init__(self, model: torch.nn.Module, loss_fn: torch.nn.Module) -> None:
         super().__init__(constructor_arguments={}, loss_fn=loss_fn)
         self._model = model
 
-    def forward(self, x: torch.Tensor, task_id: Optional[str] = None) -> torch.Tensor:
-        return self._model(x)
+    def forward(self, x: NestedTensors, task_id: Optional[str] = None) -> torch.Tensor:
+        if isinstance(x, torch.Tensor):
+            outputs = self._model(x)
+        elif isinstance(x, tuple):
+            outputs = self._model(*x)
+        elif isinstance(x, dict):
+            outputs = self._model(**x)
+        else:
+            raise TypeError(f"Expected tensor or tuple/dict of tensors; found {type(x)}.")
+
+        if isinstance(outputs, tuple) and len(outputs) == 1:
+            return outputs[0]
+        else:
+            return outputs
 
     @classmethod
     def from_state_dict(cls, state_dict):
         raise NotImplementedError(
             "RenateWrapper does not support `from_state_dict`. Instantiate the object using the "
             "standard constructor, then call `load_state_dict`."
         )
```

### Comparing `Renate-0.1.0/src/renate/tuning/config_spaces.py` & `Renate-0.2.0/src/renate/utils/config_spaces.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/src/renate/tuning/tuning.py` & `Renate-0.2.0/src/renate/training/training.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from syne_tune.stopping_criterion import StoppingCriterion
 from syne_tune.tuner import Tuner
 from syne_tune.tuner_callback import StoreResultsCallback
 from syne_tune.util import experiment_path
 
 import renate
 from renate import defaults
-from renate.cli.parsing_functions import get_data_module_fn_args
+from renate.cli.parsing_functions import to_dense_str, get_data_module_fn_kwargs
 from renate.utils.file import move_to_uri
 from renate.utils.module import get_and_prepare_data_module, import_module
 from renate.utils.syne_tune import (
     TrainingLoggerCallback,
     TuningLoggerCallback,
     best_hyperparameters,
     config_space_to_dict,
@@ -52,29 +52,29 @@
     "task_id",
     "working_directory",
     "seed",
     "accelerator",
     "devices",
     "metric",
     "mode",
-    "state_url",
+    "input_state_url",
 ]
 
 
-def execute_tuning_job(
+def run_training_job(
     mode: defaults.SUPPORTED_TUNING_MODE_TYPE,
     config_space: Dict[str, Any],
     metric: str,
     backend: defaults.SUPPORTED_BACKEND_TYPE,
     updater: str = defaults.LEARNER,
     max_epochs: int = defaults.MAX_EPOCHS,
     task_id: str = defaults.TASK_ID,
     chunk_id: int = defaults.CHUNK_ID,
-    state_url: Optional[str] = None,
-    next_state_url: Optional[str] = None,
+    input_state_url: Optional[str] = None,
+    output_state_url: Optional[str] = None,
     working_directory: Optional[str] = defaults.WORKING_DIRECTORY,
     source_dir: Optional[str] = None,
     config_file: Optional[str] = None,
     requirements_file: Optional[str] = None,
     role: Optional[str] = None,
     instance_type: str = defaults.INSTANCE_TYPE,
     instance_count: int = defaults.INSTANCE_COUNT,
@@ -86,63 +86,72 @@
     max_cost: Optional[float] = None,
     n_workers: int = defaults.N_WORKERS,
     scheduler: Optional[Union[str, Type[TrialScheduler]]] = None,
     scheduler_kwargs: Optional[Dict] = None,
     seed: int = defaults.SEED,
     accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
     devices: int = defaults.DEVICES,
+    deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     job_name: str = defaults.JOB_NAME,
 ) -> Optional[Tuner]:
     """Starts updating the model including hyperparameter optimization.
 
     Args:
         mode: Declares the type of optimization problem: `min` or `max`.
         config_space: Details for defining your own search space is provided in the
-            `Syne Tune Documentation <https://github.com/awslabs/syne-tune/blob/main/docs/search_space.md>`_.
+            `Syne Tune Documentation
+            <https://syne-tune.readthedocs.io/en/latest/search_space.html>`_.
         metric: Name of metric to optimize.
         backend: Whether to run jobs locally (`local`) or on SageMaker (`sagemaker`).
         updater: Updater used for model update.
         max_epochs: Maximum number of epochs the model is trained.
         task_id: Unique identifier for the current task.
         chunk_id: Unique identifier for the current data chunk.
-        state_url: Path to the Renate model state.
-        next_state_url: Path where Renate model state will be stored.
+        input_state_url: Path to the Renate model state.
+        output_state_url: Path where Renate model state will be stored.
         working_directory: Path to the working directory.
         source_dir: (SageMaker backend only) Root directory which will be moved to SageMaker.
         config_file: File containing the definition of `model_fn` and `data_module_fn`.
-        requirements_file: (SageMaker backend only) Path to requirements.txt containing environment dependencies.
+        requirements_file: (SageMaker backend only) Path to requirements.txt containing environment
+            dependencies.
         role: (SageMaker backend only) An AWS IAM role (either name or full ARN).
         instance_type: (SageMaker backend only) Sagemaker instance type for each worker.
         instance_count: (SageMaker backend only) Number of instances for each worker.
-        instance_max_time: (SageMaker backend only) Requested maximum wall_clock time for each worker.
+        instance_max_time: (SageMaker backend only) Requested maximum wall_clock time for each
+            worker.
         max_time: Stopping criterion: wall clock time.
         max_num_trials_started: Stopping criterion: trials started.
         max_num_trials_completed: Stopping criterion: trials completed.
         max_num_trials_finished: Stopping criterion: trials finished.
         max_cost: (SageMaker backend only) Stopping criterion: SageMaker cost.
         n_workers: Number of workers running in parallel.
-        scheduler: Default is random search, you can change it by providing a either a string (`random`, `bo`, `asha` or
-            `rush`) or scheduler class and its corresponding scheduler_kwargs if required. For latter option,
+        scheduler: Default is random search, you can change it by providing a either a string
+            (`random`, `bo`, `asha` or `rush`) or scheduler class and its corresponding
+            `scheduler_kwargs` if required. For latter option,
             `see details at <https://github.com/awslabs/syne-tune/blob/main/docs/schedulers.md>`_ .
         scheduler_kwargs: Only required if custom scheduler is provided.
         seed: Seed used for ensuring reproducibility.
         accelerator: Type of accelerator to use.
         devices: Number of devices to use.
-        job_name: Name of the tuning job.
+        deterministic_trainer: When true the Trainer adopts a deterministic behaviour also on GPU.
+        job_name: Prefix for the name of the SageMaker training job.
     """
     assert (
         mode in defaults.SUPPORTED_TUNING_MODE
     ), f"Mode {mode} is not in {defaults.SUPPORTED_TUNING_MODE}."
     assert (
         backend in defaults.SUPPORTED_BACKEND
     ), f"Backend {backend} is not in {defaults.SUPPORTED_BACKEND}."
+    for key, value in config_space.items():
+        if isinstance(value, (bool, list, tuple)):
+            config_space[key] = to_dense_str(value)
     if backend == "local":
-        return _execute_tuning_job_locally(
-            state_url=state_url,
-            next_state_url=next_state_url,
+        return _execute_training_and_tuning_job_locally(
+            input_state_url=input_state_url,
+            output_state_url=output_state_url,
             working_directory=working_directory,
             config_file=config_file,
             mode=mode,
             config_space=config_space,
             metric=metric,
             updater=updater,
             max_epochs=max_epochs,
@@ -155,18 +164,19 @@
             max_cost=max_cost,
             n_workers=n_workers,
             scheduler=scheduler,
             scheduler_kwargs=scheduler_kwargs,
             seed=seed,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
     submit_remote_job(
-        state_url=state_url,
-        next_state_url=next_state_url,
+        input_state_url=input_state_url,
+        output_state_url=output_state_url,
         working_directory=working_directory,
         config_file=config_file,
         mode=mode,
         config_space=config_space,
         metric=metric,
         updater=updater,
         max_epochs=max_epochs,
@@ -185,26 +195,27 @@
         max_cost=max_cost,
         n_workers=n_workers,
         scheduler=scheduler,
         scheduler_kwargs=scheduler_kwargs,
         seed=seed,
         accelerator=accelerator,
         devices=devices,
+        deterministic_trainer=deterministic_trainer,
         job_name=job_name,
     )
 
 
 def _prepare_remote_job(
     tmp_dir: str, requirements_file: Optional[str], **job_kwargs: Any
 ) -> List[str]:
-    """Prepares a SageMaker tuning job."""
+    """Prepares a SageMaker job."""
     dependencies = list(renate.__path__ + [job_kwargs["config_file"]])
 
-    if "state_url" in job_kwargs and job_kwargs["state_url"] is None:
-        del job_kwargs["state_url"]
+    if "input_state_url" in job_kwargs and job_kwargs["input_state_url"] is None:
+        del job_kwargs["input_state_url"]
     job_kwargs["config_file"] = os.path.basename(job_kwargs["config_file"])
     job_kwargs["config_space"] = config_space_to_dict(job_kwargs["config_space"])
 
     jobs_kwargs_file = os.path.join(tmp_dir, defaults.JOB_KWARGS_FILE)
     with open(jobs_kwargs_file, "w") as f:
         json.dump(job_kwargs, f)
     dependencies.append(jobs_kwargs_file)
@@ -219,25 +230,28 @@
 
 def _get_transfer_learning_task_evaluations(
     tuning_results: pd.DataFrame,
     config_space: Dict[str, Any],
     metric: str,
     max_epochs: int,
 ) -> Optional[TransferLearningTaskEvaluations]:
-    """Converts data frame with tuning results of a single update step into `TransferLearningTaskEvaluations`.
+    """Converts data frame with training results of a single update step into
+    `TransferLearningTaskEvaluations`.
 
     Args:
         tuning_results: Results of previous hyperparameter optimization runs.
         config_space: Configuration space used.
-        metric: The metric to be optimized. This will be the only metric added to `TransferLearningTaskEvaluations`.
-        max_epochs: Length of the learning curve. Learning curves will be padded with `np.nan` to this length.
+        metric: The metric to be optimized. This will be the only metric added to
+            `TransferLearningTaskEvaluations`.
+        max_epochs: Length of the learning curve. Learning curves will be padded with `np.nan`
+            to this length.
     Returns:
-        `TransferLearningTaskEvaluations` contains a `pd.DataFrame` of hyperparameters, a `np.array` of shape
-        `(num_hyperparameters, 1, max_epochs, 1)` which contains the learning curves for `metric` for each
-        hyperparameter.
+        `TransferLearningTaskEvaluations` contains a `pd.DataFrame` of hyperparameters, a `np.array`
+        of shape `(num_hyperparameters, 1, max_epochs, 1)` which contains the learning curves for
+        `metric` for each hyperparameter.
     """
     for config in RENATE_CONFIG_COLUMNS:
         config_with_prefix = f"config_{config}"
         if config in config_space:
             tuning_results[config_with_prefix] = config_space[config]
         elif config_with_prefix in tuning_results:
             del tuning_results[config_with_prefix]
@@ -283,29 +297,31 @@
         hyperparameters=hyperparameters,
         objectives_names=[metric],
         objectives_evaluations=objectives_evaluations,
     )
 
 
 def _load_tuning_history(
-    state_url: str, config_space: Dict[str, Any], metric: str
+    input_state_url: str, config_space: Dict[str, Any], metric: str
 ) -> Dict[str, TransferLearningTaskEvaluations]:
-    """Loads the tuning history in a list where each entry of the list is the tuning history of one update.
+    """Loads the tuning history in a list where each entry of the list is the tuning history of one
+    update.
 
     Args:
-        state_url: Location of state. Will check at this location of a tuning history exists.
+        input_state_url: Location of state. Will check at this location of a tuning history exists.
         config_space: The configuration space defines which parts of the tuning history to load.
         metric: Only the defined metric of the tuning history will be loaded.
     Returns:
-        Returns an empty list if no previous tuning history exists or it does not match the current `config_space`.
-        The list contains an instance of `TransferLearningTaskEvaluations` for each update that contains matching data.
+        Returns an empty list if no previous tuning history exists or it does not match the current
+        `config_space`. The list contains an instance of `TransferLearningTaskEvaluations` for each
+        update that contains matching data.
     """
-    if state_url is None or not Path(defaults.hpo_file(state_url)).exists():
+    if input_state_url is None or not Path(defaults.hpo_file(input_state_url)).exists():
         return {}
-    tuning_results = pd.read_csv(defaults.hpo_file(state_url))
+    tuning_results = pd.read_csv(defaults.hpo_file(input_state_url))
     hyperparameter_names = [
         hyperparameter for hyperparameter in tuning_results if hyperparameter.startswith("config_")
     ]
     agg_dict = {
         hyperparameter_name: lambda x: x.iloc[0] for hyperparameter_name in hyperparameter_names
     }
     agg_dict[metric] = list
@@ -324,94 +340,96 @@
             task_evaluations[f"update_id_{update_id}"] = task_evaluation
     return task_evaluations
 
 
 def _merge_tuning_history(
     new_tuning_results: pd.DataFrame, old_tuning_results: Optional[pd.DataFrame] = None
 ) -> pd.DataFrame:
-    """Merges old tuning history with tuning results from current chunk.
+    """Merges old tuning history with training results from current chunk.
 
-    `update_id` identifies the update step in the csv file. This allows creating the metadata required for transfer
-        hyperparameter optimization.
+    `update_id` identifies the update step in the csv file. This allows creating the metadata
+        required for transfer hyperparameter optimization.
     """
     update_id = 0 if old_tuning_results is None else old_tuning_results["update_id"].max() + 1
     new_tuning_results.insert(0, "update_id", update_id)
     if old_tuning_results is not None:
         return pd.concat([old_tuning_results, new_tuning_results], axis=0, ignore_index=True)
     return new_tuning_results
 
 
 def _teardown_tuning_job(
     backend: LocalBackend,
     config_space: Dict[str, Union[Domain, int, float, str]],
     job_name: str,
-    state_url: Optional[str] = None,
-    next_state_url: Optional[str] = None,
+    input_state_url: Optional[str] = None,
+    output_state_url: Optional[str] = None,
 ) -> None:
     """Update lifelong hyperparameter optimization results, save state and clean up disk."""
     experiment_folder = redirect_to_tmp(str(experiment_path(job_name)))
-    if next_state_url is not None:
+    if output_state_url is not None:
         experiment = load_experiment(job_name)
         try:
             best_trial_id = experiment.best_config()["trial_id"]
             if is_syne_tune_config_space(config_space):
                 logger.info(
-                    f"Best hyperparameter settings: {best_hyperparameters(experiment, config_space)}"
+                    "Best hyperparameter settings: "
+                    f"{best_hyperparameters(experiment, config_space)}"
                 )
         except AttributeError:
             raise RuntimeError(
                 "Not a single training run finished. This may have two reasons:\n"
                 "1) The provided tuning time is too short.\n"
                 "2) There is a bug in the training script."
                 + "\n\nLogs (stdout):\n\n{}".format("".join(backend.stdout(0)))
                 + "\n\nLogs (stderr):\n\n{}".format("".join(backend.stderr(0)))
             )
-        next_state_folder = defaults.next_state_folder(
+        output_state_folder = defaults.output_state_folder(
             f"{experiment_folder}/{best_trial_id}/checkpoints"
         )
         old_tuning_results = (
-            pd.read_csv(defaults.hpo_file(state_url))
-            if state_url is not None and os.path.exists(defaults.hpo_file(state_url))
+            pd.read_csv(defaults.hpo_file(input_state_url))
+            if input_state_url is not None and os.path.exists(defaults.hpo_file(input_state_url))
             else None
         )
         tuning_results = _merge_tuning_history(experiment.results, old_tuning_results)
-        tuning_results.to_csv(defaults.hpo_file(next_state_folder), index=False)
-        move_to_uri(next_state_folder, next_state_url)
-        logger.info(f"Renate state is available at {next_state_url}.")
+        tuning_results.to_csv(defaults.hpo_file(output_state_folder), index=False)
+        move_to_uri(output_state_folder, output_state_url)
+        logger.info(f"Renate state is available at {output_state_url}.")
     shutil.rmtree(experiment_folder, ignore_errors=True)
     shutil.rmtree(experiment_path(job_name), ignore_errors=True)
 
 
 def _verify_validation_set_for_hpo_and_checkpointing(
     config_space: Dict[str, Any],
     config_file: str,
     tune_hyperparameters: bool,
     metric: str,
     mode: defaults.SUPPORTED_TUNING_MODE_TYPE,
     working_directory: str,
     chunk_id: int,
     seed: int,
 ) -> Tuple[str, defaults.SUPPORTED_TUNING_MODE_TYPE]:
-    """Checks if validation set is provided when needed and updates config_space such that checkpointing works.
+    """Checks if validation set is provided when needed and updates config_space such that
+    checkpointing works.
 
-    If a validation set exists, the metric is forwarded such that we store the checkpoint which performs best on
-    validation. This is a side effect changing `config_space`. Otherwise, the checkpoint of the last epoch is used.
+    If a validation set exists, the metric is forwarded such that we store the checkpoint which
+    performs best on validation. This is a side effect changing `config_space`. Otherwise, the
+    checkpoint of the last epoch is used.
 
     Returns:
-        Metric and mode used by the Syne Tune tuner. If there is no validation set, returns `("train_loss", "min")`.
+        Metric and mode used by the Syne Tune tuner. If there is no validation set, returns
+        `("train_loss", "min")`.
     Raises:
         AssertionError: If `tune_hyperparameters` is True but no validation set is provided.
     """
     config_module = import_module("config_module", config_file)
     data_module = get_and_prepare_data_module(
         config_module,
         data_path=defaults.data_folder(working_directory),
-        chunk_id=chunk_id,
-        seed=seed,
-        **get_data_module_fn_args(config_space),
+        **get_data_module_fn_kwargs(config_module, config_space, cast_arguments=True),
     )
     data_module.setup()
     val_exists = data_module.val_data() is not None
     assert (
         val_exists or not tune_hyperparameters
     ), "Provide a validation set to optimize hyperparameters."
     if val_exists:
@@ -424,54 +442,53 @@
 
 
 def _create_scheduler(
     scheduler: Union[str, Type[TrialScheduler]],
     config_space: Dict[str, Any],
     metric: str,
     mode: defaults.SUPPORTED_TUNING_MODE_TYPE,
-    max_epochs: int,
     seed: int,
     scheduler_kwargs: Optional[Dict[str, Any]] = None,
-    state_url: Optional[str] = None,
+    input_state_url: Optional[str] = None,
 ) -> TrialScheduler:
     scheduler_kwargs = scheduler_kwargs or {}
     if isinstance(scheduler, str):
-        hyperband_scheduler_kwargs = {"max_t": max_epochs, "resource_attr": "epoch"}
+        hyperband_scheduler_kwargs = {"max_resource_attr": "max_epochs", "resource_attr": "epoch"}
         scheduler_classes = {
             "asha": {"scheduler": ASHA, "scheduler_kwargs": hyperband_scheduler_kwargs},
             "bo": {"scheduler": FIFOScheduler, "scheduler_kwargs": {"searcher": "bayesopt"}},
             "rush": {"scheduler": RUSHScheduler, "scheduler_kwargs": hyperband_scheduler_kwargs},
             "random": {"scheduler": FIFOScheduler, "scheduler_kwargs": {"searcher": "random"}},
         }
         assert (
             scheduler in scheduler_classes
         ), f"Unknown scheduler {scheduler}. Options: {list(scheduler_classes)}."
         scheduler_kwargs.update(scheduler_classes[scheduler]["scheduler_kwargs"])
         scheduler = scheduler_classes[scheduler]["scheduler"]
     if "transfer_learning_evaluations" in inspect.getfullargspec(scheduler.__init__).args:
         scheduler_kwargs["transfer_learning_evaluations"] = _load_tuning_history(
-            state_url=state_url, config_space=config_space, metric=metric
+            input_state_url=input_state_url, config_space=config_space, metric=metric
         )
         if scheduler_kwargs["transfer_learning_evaluations"]:
             logger.info(
-                f"Using information of {len(scheduler_kwargs['transfer_learning_evaluations'])} previous tuning "
-                "jobs to accelerate this job."
+                f"Using information of {len(scheduler_kwargs['transfer_learning_evaluations'])} "
+                "previous tuning jobs to accelerate this job."
             )
     return scheduler(
         config_space=config_space,
         mode=mode,
         metric=metric,
         random_seed=seed,
         **scheduler_kwargs,
     )
 
 
-def _execute_tuning_job_locally(
-    state_url: Optional[str],
-    next_state_url: Optional[str],
+def _execute_training_and_tuning_job_locally(
+    input_state_url: Optional[str],
+    output_state_url: Optional[str],
     working_directory: Optional[str],
     config_file: str,
     mode: defaults.SUPPORTED_TUNING_MODE_TYPE,
     config_space: Dict[str, Any],
     metric: str,
     updater: str,
     max_epochs: int,
@@ -484,32 +501,34 @@
     max_cost: float,
     n_workers: int,
     scheduler: Union[str, Type[TrialScheduler]],
     scheduler_kwargs: Dict[str, Any],
     seed: int,
     accelerator: str,
     devices: int,
+    deterministic_trainer: bool,
 ):
-    """Executes the tuning job locally.
+    """Executes the training job locally.
 
-    See renate.tuning.execute_tuning_job for a description of arguments.
+    See renate.train.run_training_job for a description of arguments.
     """
     tune_hyperparameters = is_syne_tune_config_space(config_space)
     config_space["updater"] = updater
     config_space["max_epochs"] = max_epochs
     config_space["config_file"] = config_file
-    config_space["prepare_data"] = 0
+    config_space["prepare_data"] = False
     config_space["chunk_id"] = chunk_id
     config_space["task_id"] = task_id
     config_space["working_directory"] = working_directory
     config_space["seed"] = seed
     config_space["accelerator"] = accelerator
     config_space["devices"] = devices
-    if state_url is not None:
-        config_space["state_url"] = state_url
+    config_space["deterministic_trainer"] = deterministic_trainer
+    if input_state_url is not None:
+        config_space["input_state_url"] = input_state_url
 
     metric, mode = _verify_validation_set_for_hpo_and_checkpointing(
         config_space=config_space,
         config_file=config_file,
         tune_hyperparameters=tune_hyperparameters,
         metric=metric,
         mode=mode,
@@ -519,33 +538,34 @@
     )
 
     training_script = str(Path(renate.__path__[0]) / "cli" / "run_training.py")
     assert Path(training_script).is_file(), f"Could not find training script {training_script}."
     logger.info("Start updating the model.")
     if tune_hyperparameters:
         logger.info(
-            f"Tuning hyperparameters with respect to {metric} ({mode}) for {max_time} seconds on {n_workers} worker(s)."
+            f"Tuning hyperparameters with respect to {metric} ({mode}) for {max_time} seconds on "
+            f"{n_workers} worker(s)."
         )
     backend = LocalBackend(entry_point=training_script)
     if scheduler is None or not tune_hyperparameters:
         if scheduler is not None:
             warnings.warn(
-                "Configuration space contains exactly one configuration, custom scheduler is ignored."
+                "Configuration space contains exactly one configuration, custom scheduler is "
+                "ignored."
             )
         scheduler = defaults.scheduler(config_space=config_space, mode=mode, metric=metric)
     else:
         scheduler = _create_scheduler(
             scheduler=scheduler,
             config_space=config_space,
             metric=metric,
             mode=mode,
-            max_epochs=max_epochs,
             seed=seed,
             scheduler_kwargs=scheduler_kwargs,
-            state_url=state_url,
+            input_state_url=input_state_url,
         )
     logging_callback = (
         TuningLoggerCallback(mode=mode, metric=metric)
         if tune_hyperparameters
         else TrainingLoggerCallback()
     )
     tuner = Tuner(
@@ -573,35 +593,35 @@
 
     logger.info("All training is completed. Saving state...")
 
     _teardown_tuning_job(
         backend=backend,
         config_space=config_space,
         job_name=tuner.name,
-        state_url=state_url,
-        next_state_url=next_state_url,
+        input_state_url=input_state_url,
+        output_state_url=output_state_url,
     )
 
     logger.info("Renate update completed successfully.")
 
     return tuner
 
 
 def submit_remote_job(
-    source_dir: str,
+    source_dir: Union[str, None],
     role: str,
     instance_type: str,
     instance_count: int,
     instance_max_time: float,
     job_name: str,
     **job_kwargs: Any,
 ) -> str:
-    """Executes the tuning job on SageMaker.
+    """Executes the training job on SageMaker.
 
-    See renate.tuning.execute_tuning_job for a description of arguments."""
+    See renate.train.run_training_job for a description of arguments."""
     tuning_script = str(Path(renate.__path__[0]) / "cli" / "run_remote_job.py")
     job_timestamp = defaults.current_timestamp()
     job_name = f"{job_name}-{job_timestamp}"
     tmp_dir = tempfile.mkdtemp()
     dependencies = _prepare_remote_job(tmp_dir=tmp_dir, **job_kwargs)
     PyTorch(
         entry_point=tuning_script,
```

### Comparing `Renate-0.1.0/src/renate/updaters/experimental/er.py` & `Renate-0.2.0/src/renate/updaters/experimental/er.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import abc
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
-from torch.utils.data import DataLoader, Dataset, Subset
 import torchmetrics
 from pytorch_lightning.loggers.logger import Logger
 from pytorch_lightning.utilities.types import STEP_OUTPUT
+from torch.utils.data import DataLoader, Dataset, Subset
 
 from renate import defaults
-from renate.data.datasets import _EnumeratedDataset
-from renate.memory.buffer import DataTuple, DataDict
+from renate.data.datasets import _EnumeratedDataset, _TransformedDataset
+from renate.memory.buffer import DataDict
 from renate.models import RenateModule
+from renate.types import NestedTensors
 from renate.updaters.learner import ReplayLearner
 from renate.updaters.learner_components.losses import (
     WeightedCLSLossComponent,
     WeightedCustomLossComponent,
     WeightedMeanSquaredErrorLossComponent,
     WeightedPooledOutputDistillationLossComponent,
 )
 from renate.updaters.learner_components.reinitialization import (
     ShrinkAndPerturbReinitializationComponent,
 )
-from renate.updaters.model_updater import SimpleModelUpdater
+from renate.updaters.model_updater import SingleTrainingLoopUpdater
+from renate.utils.pytorch import move_tensors_to_device
 
 
 class BaseExperienceReplayLearner(ReplayLearner, abc.ABC):
     """A base implementation of experience replay.
 
     It is designed for the online CL setting, where only one pass over each new chunk of data is
     allowed. The Learner maintains a Reservoir buffer. In the training step, it samples a batch of
     data from the memory and appends it to the batch of current-task data. At the end of the
     training step, the memory is updated.
 
     Args:
-        components: An ordered dictionary of components that are part of the experience replay learner.
+        components: An ordered dictionary of components that are part of the experience replay
+            learner.
         loss_weight: A scalar weight factor for the base loss function to trade it off with other
             loss functions added by `components`.
-        ema_memory_update_gamma: The gamma used for exponential moving average to update the meta data with respect to
-            the logits and intermediate representation, if there is some.
+        ema_memory_update_gamma: The gamma used for exponential moving average to update the meta
+            data with respect to the logits and intermediate representation, if there is some.
         loss_normalization: Whether to normalize the loss by the weights of all the components.
     """
 
     def __init__(
         self,
         components: nn.ModuleDict,
         loss_weight: float = defaults.LOSS_WEIGHT,
@@ -66,35 +69,41 @@
     def _create_metrics_collections(
         self, logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None
     ) -> None:
         super()._create_metrics_collections(logged_metrics)
         for name in self._components_names:
             if name in self._loss_collections:
                 raise ValueError(
-                    f"Component name {name} is already used as a loss name. Please pick a different name."
+                    f"Component name {name} is already used as a loss name. Please pick a "
+                    "different name."
                 )
             self._loss_collections["train_losses"].update({name: torchmetrics.MeanMetric()})
 
     def on_model_update_start(
         self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[str] = None
-    ) -> Tuple[DataLoader, DataLoader]:
+    ) -> None:
         """Called before a model update starts."""
+        super().on_model_update_start(train_dataset, val_dataset, task_id)
         self._set_memory_loader()
-        self._current_train_dataset = train_dataset
-        train_loader, val_loader = super().on_model_update_start(
-            train_dataset, val_dataset, task_id
+
+    def train_dataloader(self) -> DataLoader:
+        train_dataset = _EnumeratedDataset(
+            _TransformedDataset(
+                self._train_dataset,
+                transform=self._train_transform,
+                target_transform=self._train_target_transform,
+            )
         )
-        train_loader = DataLoader(
-            _EnumeratedDataset(train_loader.dataset),
+        return DataLoader(
+            train_dataset,
             batch_size=self._batch_size,
             shuffle=True,
             generator=self._rng,
             pin_memory=True,
         )
-        return train_loader, val_loader
 
     def on_train_start(self) -> None:
         """PyTorch Lightning function to be run at the start of the training."""
         super().on_train_start()
         for component in self._components.values():
             component.on_train_start(model=self._model)
 
@@ -129,34 +138,34 @@
             self._loss_weight = args["loss_weight"]
         if "ema_memory_update_gamma" in args:
             self._ema_memory_update_gamma = args["ema_memory_update_gamma"]
         if "loss_normalization" in args:
             self._use_loss_normalization = args["loss_normalization"]
 
     def training_step(
-        self, batch: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], batch_idx: int
+        self, batch: Tuple[torch.Tensor, Tuple[NestedTensors, torch.Tensor]], batch_idx: int
     ) -> STEP_OUTPUT:
         """PyTorch Lightning function to return the training loss."""
-        idx, (X, y) = batch
-        step_output = super().training_step(batch=(X, y), batch_idx=batch_idx)
+        idx, (inputs, targets) = batch
+        step_output = super().training_step(batch=(inputs, targets), batch_idx=batch_idx)
         step_output["train_data_idx"] = idx
         step_output["loss"] *= self._loss_weight
 
         batch_memory: Optional[torch.Tensor] = None
         metadata_memory: Optional[torch.Tensor] = None
         outputs_memory: Optional[torch.Tensor] = None
         intermediate_representation_memory: Optional[List[torch.Tensor]] = None
         loss_normalization = self._loss_weight
         if self._memory_loader is not None:
             for name, component in self._components.items():
                 memory_sampled = False
                 if component.sample_new_memory_batch or batch_memory is None:
                     batch_memory = self._sample_from_buffer(device=step_output["loss"].device)
-                    (x_memory, _), metadata_memory = batch_memory
-                    outputs_memory = self(x_memory)
+                    (inputs_memory, _), metadata_memory = batch_memory
+                    outputs_memory = self(inputs_memory)
                     intermediate_representation_memory = (
                         self._model.get_intermediate_representation()
                     )
                     self._model.reset_intermediate_representation_cache()
                     memory_sampled = True
 
                 component_loss = component.loss(
@@ -177,24 +186,19 @@
                         1.0 - self._ema_memory_update_gamma
                     )
             if self._use_loss_normalization:
                 step_output["loss"] /= loss_normalization
 
         return step_output
 
-    def _sample_from_buffer(self, device: torch.device) -> Optional[Tuple[DataTuple, DataDict]]:
+    def _sample_from_buffer(self, device: torch.device) -> Optional[Tuple[NestedTensors, DataDict]]:
         """Function to sample from the buffer, if buffer is populated."""
         if self._memory_loader is not None and len(self._memory_buffer) >= self._memory_batch_size:
             memory_batch = next(iter(self._memory_loader))
-            (x_memory, y_memory), metadata = memory_batch
-            x_memory, y_memory = x_memory.to(device), y_memory.to(device)
-            for key, value in metadata.items():
-                if isinstance(value, torch.Tensor):
-                    metadata[key] = value.to(device)
-            return (x_memory, y_memory), metadata
+            return move_tensors_to_device(memory_batch, device)
         else:
             return None
 
     def training_step_end(self, step_output: STEP_OUTPUT) -> STEP_OUTPUT:
         """PyTorch Lightning function to perform after the training step."""
         super().training_step_end(step_output)
         self._update_memory_buffer(step_output)
@@ -203,15 +207,17 @@
     def _update_memory_buffer(self, step_output: STEP_OUTPUT) -> None:
         outputs = step_output["outputs"]
         metadata = {"outputs": outputs.detach().cpu()}
         for i, intermediate_representation in enumerate(step_output["intermediate_representation"]):
             metadata[
                 f"intermediate_representation_{i}"
             ] = intermediate_representation.detach().cpu()
-        dataset = Subset(self._current_train_dataset, step_output["train_data_idx"])
+        # Some datasets have problems using tensors as subset indices, convert to list of ints.
+        train_data_idx = [int(idx) for idx in step_output["train_data_idx"]]
+        dataset = Subset(self._train_dataset, train_data_idx)
         self._memory_buffer.update(dataset, metadata)
         self._set_memory_loader()
 
     def _set_memory_loader(self) -> None:
         """Create a memory loader from a memory buffer."""
         if self._memory_loader is None and len(self._memory_buffer) >= self._memory_batch_size:
             self._memory_loader = DataLoader(
@@ -271,18 +277,18 @@
 class DarkExperienceReplayLearner(ExperienceReplayLearner):
     """A Learner that implements Dark Experience Replay.
 
     Pietro Buzzega, Matteo Boschini, Angelo Porrello, Davide Abati, Simone Calderara:
     Dark Experience for General Continual Learning: a Strong, Simple Baseline. NeurIPS 2020
 
     Args:
-        alpha: The weight of the mean squared error loss component between memorised logits and the current logits
-               on the memory data.
-        beta: The weight of the cross-entropy loss component between memorised targets and the current logits
-              on the memory data.
+        alpha: The weight of the mean squared error loss component between memorised logits and the
+            current logits on the memory data.
+        beta: The weight of the cross-entropy loss component between memorised targets and the
+            current logits on the memory data.
     """
 
     def __init__(
         self, alpha: float = defaults.DER_ALPHA, beta: float = defaults.DER_BETA, **kwargs
     ) -> None:
         super().__init__(alpha=beta, **kwargs)
         self._components = self.components(model=kwargs["model"], alpha=alpha, beta=beta)
@@ -310,21 +316,24 @@
         if "beta" in args:
             self._components["memory_loss"].set_weight(args["beta"])
 
 
 class PooledOutputDistillationExperienceReplayLearner(BaseExperienceReplayLearner):
     """A Learner that implements Pooled Output Distillation.
 
-    Douillard, Arthur, et al. "Podnet: Pooled outputs distillation for small-tasks incremental learning."
+    Douillard, Arthur, et al. "Podnet: Pooled outputs distillation for small-tasks incremental
+    learning."
     European Conference on Computer Vision. Springer, Cham, 2020.
 
     Args:
         alpha: Scaling value which scales the loss with respect to all intermediate representations.
-        distillation_type: Which distillation type to apply with respect to the intermediate representation.
-        normalize: Whether to normalize both the current and cached features before computing the Frobenius norm.
+        distillation_type: Which distillation type to apply with respect to the intermediate
+            representation.
+        normalize: Whether to normalize both the current and cached features before computing the
+            Frobenius norm.
     """
 
     def __init__(
         self,
         alpha: float = defaults.POD_ALPHA,
         distillation_type: str = defaults.POD_DISTILLATION_TYPE,
         normalize: bool = defaults.POD_NORMALIZE,
@@ -365,24 +374,25 @@
             component.set_normalize(args["normalize"])
 
 
 class CLSExperienceReplayLearner(BaseExperienceReplayLearner):
     """A learner that implements a Complementary Learning Systems Based Experience Replay.
 
     Arani, Elahe, Fahad Sarfraz, and Bahram Zonooz.
-    "Learning fast, learning slow: A general continual learning method based on complementary learning system."
+    "Learning fast, learning slow: A general continual learning method based on complementary
+    learning system."
     arXiv preprint arXiv:2201.12604 (2022).
 
     Args:
         alpha: Scaling value for the cross-entropy loss.
         beta: Scaling value for the consistency loss.
-        stable_model_update_weight: The starting weight for the exponential moving average to update the stable model
-            copy.
-        plastic_model_update_weight: The starting weight for the exponential moving average to update the plastic model
-            copy.
+        stable_model_update_weight: The starting weight for the exponential moving average to update
+            the stable model copy.
+        plastic_model_update_weight: The starting weight for the exponential moving average to
+            update the plastic model copy.
         stable_model_update_probability: The probability to update the stable model copy.
         plastic_model_update_probability: The probability to update the plastic model copy.
     """
 
     def __init__(
         self,
         alpha: float = defaults.CLS_ALPHA,
@@ -454,45 +464,48 @@
             )
 
 
 class SuperExperienceReplayLearner(BaseExperienceReplayLearner):
     """A learner that implements a selected combination of methods.
 
     Args:
-        der_alpha: The weight of the mean squared error loss component between memorised logits and the current logits
-                   on the memory data.
-        der_beta: The weight of the cross-entropy loss component between memorised targets and the current logits
-                  on the memory data.
+        der_alpha: The weight of the mean squared error loss component between memorised logits and
+            the current logits on the memory data.
+        der_beta: The weight of the cross-entropy loss component between memorised targets and the
+            current logits on the memory data.
         sp_shrink_factor: Shrinking value applied with respect to shrink and perturbation.
         sp_sigma: Standard deviation applied with respect to shrink and perturbation.
         cls_alpha: Scaling value for the consistency loss added to the base cross-entropy loss.
-        cls_stable_model_update_weight: The starting weight for the exponential moving average to update the stable
-            model copy.
-        cls_plastic_model_update_weight: The starting weight for the exponential moving average to update the plastic
-            model copy.
+        cls_stable_model_update_weight: The starting weight for the exponential moving average to
+            update the stable model copy.
+        cls_plastic_model_update_weight: The starting weight for the exponential moving average to
+            update the plastic model copy.
         cls_stable_model_update_probability: The probability to update the stable model copy.
         cls_plastic_model_update_probability: The probability to update the plastic model copy.
-        pod_alpha: Scaling value which scales the loss with respect to all intermediate representations.
-        pod_distillation_type: Which distillation type to apply with respect to the intermediate representation.
-        pod_normalize: Whether to normalize both the current and cached features before computing the Frobenius norm.
-        ema_memory_update_gamma: The gamma used for exponential moving average to update the meta data with respect to
-            the logits and intermediate representation, if there is some.
+        pod_alpha: Scaling value which scales the loss with respect to all intermediate
+            representations.
+        pod_distillation_type: Which distillation type to apply with respect to the intermediate
+            representation.
+        pod_normalize: Whether to normalize both the current and cached features before computing
+            the Frobenius norm.
+        ema_memory_update_gamma: The gamma used for exponential moving average to update the meta
+            data with respect to the logits and intermediate representation, if there is some.
     """
 
     def __init__(
         self,
         der_alpha: float = defaults.SER_DER_ALPHA,
         der_beta: float = defaults.SER_DER_BETA,
         sp_shrink_factor: float = defaults.SER_SP_SHRINK_FACTOR,
         sp_sigma: float = defaults.SER_SP_SIGMA,
         cls_alpha: float = defaults.SER_CLS_ALPHA,
         cls_stable_model_update_weight: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_WEIGHT,
         cls_plastic_model_update_weight: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_WEIGHT,
-        cls_stable_model_update_probability: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_PROBABILITY,
-        cls_plastic_model_update_probability: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_PROBABILITY,
+        cls_stable_model_update_probability: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_PROBABILITY,  # noqa: E501
+        cls_plastic_model_update_probability: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_PROBABILITY,  # noqa: E501
         pod_alpha: float = defaults.SER_POD_ALPHA,
         pod_distillation_type: str = defaults.SER_POD_DISTILLATION_TYPE,
         pod_normalize: bool = defaults.SER_POD_NORMALIZE,
         ema_memory_update_gamma: float = defaults.EMA_MEMORY_UPDATE_GAMMA,
         **kwargs,
     ) -> None:
         components = self.components(
@@ -522,16 +535,16 @@
         der_alpha: float = defaults.SER_DER_ALPHA,
         der_beta: float = defaults.SER_DER_BETA,
         sp_shrink_factor: float = defaults.SER_SP_SHRINK_FACTOR,
         sp_sigma: float = defaults.SER_SP_SIGMA,
         cls_alpha: float = defaults.SER_CLS_ALPHA,
         cls_stable_model_update_weight: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_WEIGHT,
         cls_plastic_model_update_weight: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_WEIGHT,
-        cls_stable_model_update_probability: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_PROBABILITY,
-        cls_plastic_model_update_probability: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_PROBABILITY,
+        cls_stable_model_update_probability: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_PROBABILITY,  # noqa: E501
+        cls_plastic_model_update_probability: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_PROBABILITY,  # noqa: E501
         pod_alpha: float = defaults.SER_POD_ALPHA,
         pod_distillation_type: str = defaults.SER_POD_DISTILLATION_TYPE,
         pod_normalize: bool = defaults.SER_POD_NORMALIZE,
     ) -> nn.ModuleDict:
         return nn.ModuleDict(
             {
                 "mse_loss": WeightedMeanSquaredErrorLossComponent(
@@ -593,34 +606,34 @@
             )
         if "cls_plastic_model_update_probability" in args:
             self._components["cls_loss"].set_plastic_model_update_probability(
                 args["cls_plastic_model_update_probability"]
             )
 
 
-class ExperienceReplayModelUpdater(SimpleModelUpdater):
+class ExperienceReplayModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
         loss_weight: float = defaults.LOSS_WEIGHT,
         ema_memory_update_gamma: float = defaults.EMA_MEMORY_UPDATE_GAMMA,
         loss_normalization: int = defaults.LOSS_NORMALIZATION,
         alpha: float = defaults.ER_ALPHA,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
@@ -628,14 +641,15 @@
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "memory_batch_size": memory_batch_size,
             "loss_weight": loss_weight,
             "ema_memory_update_gamma": ema_memory_update_gamma,
             "loss_normalization": loss_normalization,
@@ -650,54 +664,55 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=ExperienceReplayLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
 
 
-class DarkExperienceReplayModelUpdater(SimpleModelUpdater):
+class DarkExperienceReplayModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
         loss_weight: float = defaults.LOSS_WEIGHT,
         ema_memory_update_gamma: float = defaults.EMA_MEMORY_UPDATE_GAMMA,
         loss_normalization: int = defaults.LOSS_NORMALIZATION,
         alpha: float = defaults.DER_ALPHA,
         beta: float = defaults.DER_BETA,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
@@ -705,14 +720,15 @@
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "memory_batch_size": memory_batch_size,
             "loss_weight": loss_weight,
             "ema_memory_update_gamma": ema_memory_update_gamma,
             "loss_normalization": loss_normalization,
@@ -728,55 +744,56 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=DarkExperienceReplayLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
 
 
-class PooledOutputDistillationExperienceReplayModelUpdater(SimpleModelUpdater):
+class PooledOutputDistillationExperienceReplayModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
         loss_weight: float = defaults.LOSS_WEIGHT,
         ema_memory_update_gamma: float = defaults.EMA_MEMORY_UPDATE_GAMMA,
         loss_normalization: int = defaults.LOSS_NORMALIZATION,
         alpha: float = defaults.POD_ALPHA,
         distillation_type: str = defaults.POD_DISTILLATION_TYPE,
         normalize: bool = defaults.POD_NORMALIZE,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
@@ -784,14 +801,15 @@
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "memory_batch_size": memory_batch_size,
             "loss_weight": loss_weight,
             "ema_memory_update_gamma": ema_memory_update_gamma,
             "loss_normalization": loss_normalization,
@@ -808,34 +826,35 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=PooledOutputDistillationExperienceReplayLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
 
 
-class CLSExperienceReplayModelUpdater(SimpleModelUpdater):
+class CLSExperienceReplayModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
         loss_weight: float = defaults.LOSS_WEIGHT,
         ema_memory_update_gamma: float = defaults.EMA_MEMORY_UPDATE_GAMMA,
@@ -844,22 +863,22 @@
         beta: float = defaults.CLS_BETA,
         stable_model_update_weight: float = defaults.CLS_STABLE_MODEL_UPDATE_WEIGHT,
         plastic_model_update_weight: float = defaults.CLS_PLASTIC_MODEL_UPDATE_WEIGHT,
         stable_model_update_probability: float = defaults.CLS_STABLE_MODEL_UPDATE_PROBABILITY,
         plastic_model_update_probability: float = defaults.CLS_PLASTIC_MODEL_UPDATE_PROBABILITY,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
@@ -867,14 +886,15 @@
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "memory_batch_size": memory_batch_size,
             "loss_weight": loss_weight,
             "ema_memory_update_gamma": ema_memory_update_gamma,
             "loss_normalization": loss_normalization,
@@ -894,34 +914,35 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=CLSExperienceReplayLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
 
 
-class SuperExperienceReplayModelUpdater(SimpleModelUpdater):
+class SuperExperienceReplayModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
         loss_weight: float = defaults.LOSS_WEIGHT,
         ema_memory_update_gamma: float = defaults.EMA_MEMORY_UPDATE_GAMMA,
@@ -929,29 +950,29 @@
         der_alpha: float = defaults.SER_DER_ALPHA,
         der_beta: float = defaults.SER_DER_BETA,
         sp_shrink_factor: float = defaults.SER_SP_SHRINK_FACTOR,
         sp_sigma: float = defaults.SER_SP_SIGMA,
         cls_alpha: float = defaults.SER_CLS_ALPHA,
         cls_stable_model_update_weight: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_WEIGHT,
         cls_plastic_model_update_weight: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_WEIGHT,
-        cls_stable_model_update_probability: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_PROBABILITY,
-        cls_plastic_model_update_probability: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_PROBABILITY,
+        cls_stable_model_update_probability: float = defaults.SER_CLS_STABLE_MODEL_UPDATE_PROBABILITY,  # noqa: E501
+        cls_plastic_model_update_probability: float = defaults.SER_CLS_PLASTIC_MODEL_UPDATE_PROBABILITY,  # noqa: E501
         pod_alpha: float = defaults.SER_POD_ALPHA,
         pod_distillation_type: str = defaults.SER_POD_DISTILLATION_TYPE,
         pod_normalize: bool = defaults.SER_POD_NORMALIZE,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
@@ -959,14 +980,15 @@
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "memory_batch_size": memory_batch_size,
             "loss_weight": loss_weight,
             "ema_memory_update_gamma": ema_memory_update_gamma,
             "loss_normalization": loss_normalization,
@@ -992,24 +1014,25 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=SuperExperienceReplayLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
```

### Comparing `Renate-0.1.0/src/renate/updaters/experimental/gdumb.py` & `Renate-0.2.0/src/renate/updaters/experimental/gdumb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, Optional, Tuple
 
 import torch
 import torchmetrics
 from pytorch_lightning.loggers.logger import Logger
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch.utils.data import DataLoader, Dataset
 
 from renate import defaults
 from renate.memory import GreedyClassBalancingBuffer
-from renate.models.renate_module import RenateModule
+from renate.models import RenateModule
+from renate.types import NestedTensors
 from renate.updaters.learner import Learner, ReplayLearner
-from renate.updaters.model_updater import SimpleModelUpdater
+from renate.updaters.model_updater import SingleTrainingLoopUpdater
 from renate.utils.pytorch import reinitialize_model_parameters
 
 
 class GDumbLearner(ReplayLearner):
     """A Learner that implements the GDumb strategy.
 
     Prabhu, Ameya, Philip HS Torr, and Puneet K. Dokania. "GDumb: A simple
@@ -51,57 +52,63 @@
             seed=seed,
             transform=buffer_transform,
             target_transform=buffer_target_transform,
         )
 
     def load_state_dict(self, model: RenateModule, state_dict: Dict[str, Any], **kwargs) -> None:
         """Restores the state of the learner."""
+        if not hasattr(self, "_memory_buffer"):
+            self._memory_buffer = GreedyClassBalancingBuffer()
         Learner.load_state_dict(self, model, state_dict, **kwargs)
         self._memory_batch_size = state_dict["memory_batch_size"]
-        self._memory_buffer = GreedyClassBalancingBuffer()
         self._memory_buffer.load_state_dict(state_dict["memory_buffer"])
 
     def on_model_update_start(
         self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[str] = None
-    ) -> Tuple[DataLoader, DataLoader]:
+    ) -> None:
         """Called before a model update starts."""
+        super().on_model_update_start(train_dataset, val_dataset, task_id)
         self._memory_buffer.update(train_dataset)
-        _, val_loader = super().on_model_update_start(train_dataset, val_dataset, task_id)
-        train_loader = DataLoader(
+        reinitialize_model_parameters(self._model)
+
+    def train_dataloader(self) -> DataLoader:
+        return DataLoader(
             self._memory_buffer,
             batch_size=self._batch_size,
             shuffle=True,
             generator=self._rng,
             pin_memory=True,
         )
-        reinitialize_model_parameters(self._model)
-        return train_loader, val_loader
 
-    def training_step(self, batch: List[torch.Tensor], batch_idx: int) -> STEP_OUTPUT:
+    def training_step(
+        self,
+        batch: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
+        batch_idx: int,
+    ) -> STEP_OUTPUT:
         """PyTorch Lightning function to return the training loss."""
         batch, _ = batch
         return super().training_step(batch=batch, batch_idx=batch_idx)
 
 
-class GDumbModelUpdater(SimpleModelUpdater):
+class GDumbModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
@@ -109,14 +116,15 @@
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "memory_batch_size": memory_batch_size,
             "optimizer": optimizer,
             "learning_rate": learning_rate,
             "learning_rate_scheduler": learning_rate_scheduler,
@@ -127,24 +135,25 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=GDumbLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
```

### Comparing `Renate-0.1.0/src/renate/updaters/experimental/joint.py` & `Renate-0.2.0/src/renate/updaters/experimental/joint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from typing import Any, Callable, Dict, List, Optional, Tuple
+import os
+from typing import Any, Callable, Dict, Optional, Tuple
 
 import torch
 import torchmetrics
 from pytorch_lightning.loggers.logger import Logger
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch.utils.data import DataLoader, Dataset
 
 from renate import defaults
 from renate.memory import InfiniteBuffer
 from renate.models import RenateModule
+from renate.types import NestedTensors
 from renate.updaters.learner import Learner
-from renate.updaters.model_updater import SimpleModelUpdater
+from renate.updaters.model_updater import SingleTrainingLoopUpdater
 from renate.utils.pytorch import reinitialize_model_parameters
 
 
 class JointLearner(Learner):
     """A Learner that implements the Joint strategy.
 
     This is a simple strategy that trains the model on all previously observed data.
@@ -36,18 +38,29 @@
         """Returns the state of the learner."""
         state_dict = super().state_dict(**kwargs)
         state_dict["memory_buffer"] = self._memory_buffer.state_dict()
         return state_dict
 
     def load_state_dict(self, model: RenateModule, state_dict: Dict[str, Any], **kwargs) -> None:
         """Restores the state of the learner."""
+        if not hasattr(self, "_memory_buffer"):
+            self._memory_buffer = InfiniteBuffer()
         super().load_state_dict(model, state_dict, **kwargs)
-        self._memory_buffer = InfiniteBuffer()
         self._memory_buffer.load_state_dict(state_dict["memory_buffer"])
 
+    def save(self, output_state_dir: str) -> None:
+        super().save(output_state_dir)
+        buffer_dir = os.path.join(output_state_dir, "memory_buffer")
+        os.makedirs(buffer_dir, exist_ok=True)
+        self._memory_buffer.save(buffer_dir)
+
+    def load(self, input_state_dir: str) -> None:
+        super().load(input_state_dir)
+        self._memory_buffer.load(os.path.join(input_state_dir, "memory_buffer"))
+
     def set_transforms(
         self,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
     ) -> None:
@@ -55,61 +68,67 @@
         super().set_transforms(
             train_transform, train_target_transform, test_transform, test_target_transform
         )
         self._memory_buffer.set_transforms(train_transform, train_target_transform)
 
     def on_model_update_start(
         self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[str] = None
-    ) -> Tuple[DataLoader, DataLoader]:
+    ) -> None:
         """Called before a model update starts."""
-        _, val_loader = super().on_model_update_start(train_dataset, val_dataset, task_id)
+        super().on_model_update_start(train_dataset, val_dataset, task_id)
         self._memory_buffer.update(train_dataset)
-        train_loader = DataLoader(
+        reinitialize_model_parameters(self._model)
+
+    def train_dataloader(self) -> DataLoader:
+        return DataLoader(
             self._memory_buffer,
             batch_size=self._batch_size,
             shuffle=True,
             generator=self._rng,
             pin_memory=True,
         )
-        reinitialize_model_parameters(self._model)
-        return train_loader, val_loader
 
-    def training_step(self, batch: List[torch.Tensor], batch_idx: int) -> STEP_OUTPUT:
+    def training_step(
+        self,
+        batch: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
+        batch_idx: int,
+    ) -> STEP_OUTPUT:
         """PyTorch Lightning function to return the training loss."""
         batch, _ = batch
         return super().training_step(batch=batch, batch_idx=batch_idx)
 
 
-class JointModelUpdater(SimpleModelUpdater):
+class JointModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         metric: Optional[str] = None,
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "optimizer": optimizer,
             "learning_rate": learning_rate,
             "learning_rate_scheduler": learning_rate_scheduler,
             "learning_rate_scheduler_gamma": learning_rate_scheduler_gamma,
             "learning_rate_scheduler_step_size": learning_rate_scheduler_step_size,
@@ -118,22 +137,23 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=JointLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
```

### Comparing `Renate-0.1.0/src/renate/updaters/experimental/offline_er.py` & `Renate-0.2.0/src/renate/updaters/experimental/offline_er.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, Optional, Tuple
 
 import torch
 import torchmetrics
 from pytorch_lightning.loggers.logger import Logger
 from pytorch_lightning.trainer.supporters import CombinedLoader
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch.utils.data import DataLoader, Dataset
 
 from renate import defaults
 from renate.models import RenateModule
+from renate.types import NestedTensors
 from renate.updaters.learner import ReplayLearner
-from renate.updaters.model_updater import SimpleModelUpdater
+from renate.updaters.model_updater import SingleTrainingLoopUpdater
 
 
 class OfflineExperienceReplayLearner(ReplayLearner):
     """Experience Replay in the offline version.
 
     The model will be trained on weighted mixture of losses computed on the new data and a replay
     buffer. In contrast to the online version, the buffer will only be updated after training has
@@ -55,58 +56,58 @@
         self, logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None
     ) -> None:
         super()._create_metrics_collections(logged_metrics)
         self._loss_collections["train_losses"]["memory_loss"] = torchmetrics.MeanMetric()
 
     def on_model_update_start(
         self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[str] = None
-    ) -> Tuple[DataLoader, DataLoader]:
+    ) -> None:
         """Called before a model update starts."""
+        super().on_model_update_start(train_dataset, val_dataset, task_id)
         self._num_points_current_task = len(train_dataset)
-        train_loader, val_loader = super().on_model_update_start(
-            train_dataset, val_dataset, task_id
-        )
+
+    def train_dataloader(self) -> DataLoader:
+        train_loader = super().train_dataloader()
         loaders = {"current_task": train_loader}
         if len(self._memory_buffer) > self._memory_batch_size:
             loaders["memory"] = DataLoader(
                 dataset=self._memory_buffer,
                 batch_size=self._memory_batch_size,
                 drop_last=True,
                 shuffle=True,
                 generator=self._rng,
                 pin_memory=True,
             )
-        return CombinedLoader(loaders, mode="max_size_cycle"), val_loader
+        return CombinedLoader(loaders, mode="max_size_cycle")
 
-    def on_model_update_end(
-        self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[str] = None
-    ) -> RenateModule:
+    def on_model_update_end(self) -> None:
         """Called right before a model update terminates."""
-        self._memory_buffer.update(train_dataset)
+        self._memory_buffer.update(self._train_dataset)
         self._num_points_previous_tasks += self._num_points_current_task
         self._num_points_current_task = -1
-        return super().on_model_update_end(train_dataset, val_dataset, task_id)
 
-    def training_step(self, batch: Dict[str, List[torch.Tensor]], batch_idx: int) -> STEP_OUTPUT:
+    def training_step(
+        self, batch: Dict[str, Tuple[NestedTensors, torch.Tensor]], batch_idx: int
+    ) -> STEP_OUTPUT:
         """PyTorch Lightning function to return the training loss."""
         if self._loss_weight_new_data is None:
             alpha = self._num_points_current_task / (
                 self._num_points_current_task + self._num_points_previous_tasks
             )
         else:
             alpha = self._loss_weight_new_data
-        x, y = batch["current_task"]
-        outputs = self(x)
-        loss = self._model.loss_fn(outputs, y)
+        inputs, targets = batch["current_task"]
+        outputs = self(inputs)
+        loss = self._model.loss_fn(outputs, targets)
         self._loss_collections["train_losses"]["base_loss"](loss)
-        self._update_metrics(outputs, y, "train")
+        self._update_metrics(outputs, targets, "train")
         if "memory" in batch:
-            x_mem, y_mem = batch["memory"]
-            outputs_mem = self(x_mem)
-            loss_mem = self._model.loss_fn(outputs_mem, y_mem)
+            (inputs_mem, targets_mem), _ = batch["memory"]
+            outputs_mem = self(inputs_mem)
+            loss_mem = self._model.loss_fn(outputs_mem, targets_mem)
             self._loss_collections["train_losses"]["memory_loss"](loss_mem)
             loss = alpha * loss + (1.0 - alpha) * loss_mem
         return {"loss": loss}
 
     def state_dict(self, **kwargs) -> Dict[str, Any]:
         """Returns the state of the learner."""
         state_dict = super().state_dict(**kwargs)
@@ -117,31 +118,31 @@
     def load_state_dict(self, model: RenateModule, state_dict: Dict[str, Any], **kwargs) -> None:
         """Restores the state of the learner."""
         super().load_state_dict(model, state_dict, **kwargs)
         self._loss_weight_new_data = state_dict["loss_weight_new_data"]
         self._num_points_previous_tasks = state_dict["num_points_previous_tasks"]
 
 
-class OfflineExperienceReplayModelUpdater(SimpleModelUpdater):
+class OfflineExperienceReplayModelUpdater(SingleTrainingLoopUpdater):
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
         loss_weight_new_data: Optional[float] = None,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
@@ -149,14 +150,15 @@
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         seed: int = defaults.SEED,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "memory_batch_size": memory_batch_size,
             "loss_weight_new_data": loss_weight_new_data,
             "optimizer": optimizer,
             "learning_rate": learning_rate,
@@ -168,24 +170,25 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model,
             learner_class=OfflineExperienceReplayLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logged_metrics=logged_metrics,
             early_stopping_enabled=early_stopping_enabled,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
+            deterministic_trainer=deterministic_trainer,
         )
```

### Comparing `Renate-0.1.0/src/renate/updaters/experimental/repeated_distill.py` & `Renate-0.2.0/src/renate/updaters/experimental/repeated_distill.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import copy
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Callable, Dict, Optional, Tuple
 
 import torch
 import torchmetrics
 from pytorch_lightning.loggers.logger import Logger
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch.utils.data import DataLoader, Dataset
 
 from renate import defaults
 from renate.memory import DataBuffer
 from renate.models import RenateModule
+from renate.types import NestedTensors
 from renate.updaters.learner import Learner, ReplayLearner
 from renate.updaters.model_updater import ModelUpdater
-from renate.utils.pytorch import reinitialize_model_parameters
+from renate.utils.pytorch import move_tensors_to_device, reinitialize_model_parameters
 
 
 def double_distillation_loss(
     predicted_logits: torch.Tensor, target_logits: torch.Tensor
 ) -> torch.Tensor:
     """Double distillation loss, where target logits are normalized across the class-dimension.
 
@@ -58,71 +59,72 @@
     Returns:
         A tensor `logits` of shape `(N, C)` where `N` is the length of the dataset and `C` is
         the output dimension of `model`, i.e., the number of classes.
     """
     logits = []
     loader = DataLoader(dataset, batch_size, shuffle=False, drop_last=False, pin_memory=True)
     for batch in loader:
-        if isinstance(dataset, DataBuffer):
-            X = batch[0][0].to(next(model.parameters()).device)
-        else:
-            X = batch[0].to(next(model.parameters()).device)
-        logits.append(model.get_logits(X, task_id))
+        inputs = batch[0][0] if isinstance(dataset, DataBuffer) else batch[0]
+        device = next(model.parameters()).device
+        inputs = move_tensors_to_device(inputs, device)
+        logits.append(model.get_logits(inputs, task_id))
     return torch.cat(logits, dim=0)
 
 
 class RepeatedDistillationModelUpdater(ModelUpdater):
-    """Repeated Distillation (RD) is inspired by Deep Model Consolidation (DMC), which was proposed in
+    """Repeated Distillation (RD) is inspired by Deep Model Consolidation (DMC), which was proposed
+    in
 
         TODO: Fix citation once we agreed on a format.
         Zhang, Junting, et al. "Class-incremental learning via deep model consolidation."
         Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision. 2020.
 
     The idea underlying RD is the following: Given a new task/batch, a new model copy is trained
     from scratch on that data. Subsequently, this expert model is consolidated with the previous
     model state via knowledge distillation. The resulting consolidated model state is maintained,
     whereas the expert model is discarded.
 
     Our variant differs from the original algorithm in two ways:
         - The original algorithm is designed specifically for the class-incremental setting, where
           each new task introduces one or more novel classes. This variant is designed for the
           general continual learning setting with a pre-determined number of classes.
-        - The original method is supposed to be memory-free and uses auxilliary data for the model
+        - The original method is supposed to be memory-free and uses auxiliary data for the model
           consolidation phase. Our variant performs knowledge distillation over a memory
     """
 
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         optimizer: str = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: float = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         metric: Optional[str] = None,
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         seed: Optional[int] = None,
         early_stopping_enabled=False,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         learner_kwargs = {
             "memory_size": memory_size,
             "optimizer": optimizer,
             "learning_rate": learning_rate,
             "learning_rate_scheduler": learning_rate_scheduler,
             "learning_rate_scheduler_gamma": learning_rate_scheduler_gamma,
@@ -132,30 +134,31 @@
             "batch_size": batch_size,
             "seed": seed,
         }
         super().__init__(
             model=model,
             learner_class=RepeatedDistillationLearner,
             learner_kwargs=learner_kwargs,
-            current_state_folder=current_state_folder,
-            next_state_folder=next_state_folder,
+            input_state_folder=input_state_folder,
+            output_state_folder=output_state_folder,
             max_epochs=max_epochs,
             train_transform=train_transform,
             train_target_transform=train_target_transform,
             test_transform=test_transform,
             test_target_transform=test_target_transform,
             buffer_transform=buffer_transform,
             buffer_target_transform=buffer_target_transform,
             metric=metric,
             mode=mode,
             logger=logger,
             accelerator=accelerator,
             devices=devices,
             early_stopping_enabled=early_stopping_enabled,
             logged_metrics=logged_metrics,
+            deterministic_trainer=deterministic_trainer,
         )
 
     def update(
         self,
         train_dataset: Dataset,
         val_dataset: Optional[Dataset] = None,
         task_id: Optional[str] = None,
@@ -174,56 +177,45 @@
         reinitialize_model_parameters(expert_model)
         expert_learner = Learner(
             model=expert_model,
             train_transform=self._train_transform,
             train_target_transform=self._train_target_transform,
             **{key: value for key, value in self._learner_kwargs.items() if key != "memory_size"},
         )
-
-        train_loader, val_loader = expert_learner.on_model_update_start(
-            train_dataset, val_dataset, task_id
-        )
-        self._fit_learner(
-            expert_learner,
-            train_loader,
-            val_loader,
-            use_syne_tune_callback=False,
-        )
-        expert_model = expert_learner.on_model_update_end(train_dataset, val_dataset, task_id)
+        expert_learner.on_model_update_start(train_dataset, val_dataset, task_id)
+        self._fit_learner(expert_learner)
 
         # Extract logits from the expert model and register them with the consolidation learner.
         expert_logits = extract_logits(
             expert_model,
             train_dataset,
             batch_size=self._learner_kwargs["batch_size"],
             task_id=task_id,
         )
 
         self._learner.update_expert_logits(expert_logits)
         del expert_model
         del expert_learner
 
         # Run consolidation.
-        train_loader, val_loader = self._learner.on_model_update_start(
-            train_dataset, val_dataset, task_id
-        )
-        self._fit_learner(self._learner, train_loader, val_loader)
-        return self._learner.on_model_update_end(train_dataset, val_dataset, task_id)
+        self._learner.on_model_update_start(train_dataset, val_dataset, task_id)
+        self._fit_learner(self._learner)
+        return self._model
 
 
 class RepeatedDistillationLearner(ReplayLearner):
     """A learner performing distillation."""
 
     def __init__(
         self,
         model: RenateModule,
         memory_size: int,
         optimizer: str = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: float = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
@@ -259,40 +251,41 @@
 
     def update_expert_logits(self, new_expert_logits: torch.Tensor) -> None:
         """Update expert logits."""
         self._expert_logits = new_expert_logits
 
     def on_model_update_start(
         self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[int] = None
-    ) -> Tuple[DataLoader, DataLoader]:
+    ) -> None:
         """Called before a model update starts."""
-        reinitialize_model_parameters(self._model)
+        super().on_model_update_start(train_dataset, val_dataset, task_id)
         self._memory_buffer.update(train_dataset, metadata={"logits": self._expert_logits})
+        reinitialize_model_parameters(self._model)
         self._expert_logits = None
 
-        _, val_loader = super().on_model_update_start(train_dataset, val_dataset, task_id)
-        train_loader = DataLoader(
+    def train_dataloader(self) -> DataLoader:
+        return DataLoader(
             self._memory_buffer,
             batch_size=self._batch_size,
             shuffle=True,
             generator=self._rng,
             pin_memory=True,
         )
-        return train_loader, val_loader
 
-    def on_model_update_end(
-        self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[int] = None
-    ) -> RenateModule:
+    def on_model_update_end(self) -> None:
         """Called right before a model update terminates."""
         # Update the logits in memory using the newly consolidated model.
         logits = extract_logits(self._model, self._memory_buffer, self._batch_size)
-        self._memory_buffer.metadata["logits"][: len(self._memory_buffer)] = logits
-        return super().on_model_update_end(train_dataset, val_dataset, task_id)
+        self._memory_buffer.set_metadata("logits", logits)
 
-    def training_step(self, batch: List[torch.Tensor], batch_idx: int) -> STEP_OUTPUT:
+    def training_step(
+        self,
+        batch: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
+        batch_idx: int,
+    ) -> STEP_OUTPUT:
         """PyTorch Lightning function to return the training loss."""
-        (X, y), metadata = batch
-        outputs = self._model(X)
+        (inputs, targets), metadata = batch
+        outputs = self(inputs)
         loss = double_distillation_loss(outputs, metadata["logits"]).mean()
-        self._update_metrics(outputs, y, prefix="train")
+        self._update_metrics(outputs, targets, prefix="train")
         self._loss_collections["train_losses"]["base_loss"](loss)
         return {"loss": loss, "outputs": outputs}
```

### Comparing `Renate-0.1.0/src/renate/updaters/learner.py` & `Renate-0.2.0/src/renate/updaters/learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import abc
+import os
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torchmetrics
 from pytorch_lightning import LightningModule
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch import Tensor
 from torch.utils.data import DataLoader, Dataset
 
 from renate import defaults
 from renate.data.datasets import _TransformedDataset
 from renate.evaluation.metrics.utils import create_metrics
-from renate.memory.buffer import DataBuffer, InfiniteBuffer, ReservoirBuffer
+from renate.memory import DataBuffer, InfiniteBuffer, ReservoirBuffer
 from renate.models import RenateModule
+from renate.types import NestedTensors
 from renate.utils.optimizer import create_optimizer, create_scheduler
 from renate.utils.pytorch import get_generator
 
 
 class Learner(LightningModule, abc.ABC):
     """Base class for Learners, which encapsulate the core CL methodologies.
 
@@ -53,15 +55,15 @@
     """
 
     def __init__(
         self,
         model: RenateModule,
         optimizer: defaults.SUPPORTED_OPTIMIZERS_TYPE = defaults.OPTIMIZER,
         learning_rate: float = defaults.LEARNING_RATE,
-        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,
+        learning_rate_scheduler: defaults.SUPPORTED_LEARNING_RATE_SCHEDULERS_TYPE = defaults.LEARNING_RATE_SCHEDULER,  # noqa: E501
         learning_rate_scheduler_gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
         learning_rate_scheduler_step_size: int = defaults.LEARNING_RATE_SCHEDULER_STEP_SIZE,
         momentum: float = defaults.MOMENTUM,
         weight_decay: float = defaults.WEIGHT_DECAY,
         batch_size: int = defaults.BATCH_SIZE,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
@@ -89,15 +91,14 @@
 
         self._val_memory_buffer: DataBuffer = InfiniteBuffer()
         self._create_metrics_collections(logged_metrics)
         self._post_init()
 
     def _post_init(self) -> None:
         self._rng = get_generator(self._seed)
-        self._val_enabled = False
 
     def _create_metrics_collections(
         self, logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None
     ) -> None:
         """Creates all logged metrics."""
         metrics = create_metrics(task="classification", additional_metrics=logged_metrics)
         train_metrics = metrics.clone(prefix="train_")
@@ -163,18 +164,27 @@
         self._learning_rate_scheduler_gamma = state_dict["learning_rate_scheduler_gamma"]
         self._learning_rate_scheduler_step_size = state_dict["learning_rate_scheduler_step_size"]
         self._momentum = state_dict["momentum"]
         self._weight_decay = state_dict["weight_decay"]
         self._batch_size = state_dict["batch_size"]
         self._seed = state_dict["seed"]
         self._task_id = state_dict["task_id"]
-        self._val_memory_buffer = InfiniteBuffer()
+        if not hasattr(self, "_val_memory_buffer"):
+            self._val_memory_buffer = InfiniteBuffer()
         self._val_memory_buffer.load_state_dict(state_dict["val_memory_buffer"])
         self._post_init()
 
+    def save(self, output_state_dir: str) -> None:
+        val_buffer_dir = os.path.join(output_state_dir, "val_memory_buffer")
+        os.makedirs(val_buffer_dir, exist_ok=True)
+        self._val_memory_buffer.save(val_buffer_dir)
+
+    def load(self, input_state_dir: str) -> None:
+        self._val_memory_buffer.load(os.path.join(input_state_dir, "val_memory_buffer"))
+
     def set_transforms(
         self,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
     ) -> None:
@@ -224,72 +234,76 @@
         if "weight_decay" in args:
             self._weight_decay = args["weight_decay"]
         if "batch_size" in args:
             self._batch_size = args["batch_size"]
 
     def on_model_update_start(
         self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[str] = None
-    ) -> Tuple[DataLoader, DataLoader]:
-        """Called before a model update starts."""
+    ) -> None:
+        self._train_dataset = train_dataset
+        self._val_dataset = val_dataset
+        self.val_enabled = val_dataset is not None and len(val_dataset)
+        self._task_id = task_id
+        self._model.add_task_params(task_id=self._task_id)
+
+    def train_dataloader(self) -> DataLoader:
+        """Returns the dataloader for training the model."""
         train_dataset = _TransformedDataset(
-            train_dataset,
+            self._train_dataset,
             transform=self._train_transform,
             target_transform=self._train_target_transform,
         )
-        self._task_id = task_id
-        self._model.add_task_params(task_id=task_id)
-        train_loader = DataLoader(
+        return DataLoader(
             train_dataset,
             batch_size=self._batch_size,
             shuffle=True,
             generator=self._rng,
             pin_memory=True,
         )
-        if val_dataset is not None:
+
+    def val_dataloader(self) -> DataLoader:
+        if self._val_dataset is not None:
             val_dataset = _TransformedDataset(
-                val_dataset,
+                self._val_dataset,
                 transform=self._test_transform,
                 target_transform=self._test_target_transform,
             )
             self._val_memory_buffer.update(val_dataset)
 
-        val_loader = None
         if len(self._val_memory_buffer):
-            val_loader = DataLoader(
+            return DataLoader(
                 self._val_memory_buffer,
                 batch_size=self._batch_size,
                 shuffle=False,
                 generator=self._rng,
                 pin_memory=True,
             )
-            self._val_enabled = True
-
-        return train_loader, val_loader
+        else:
+            return None
 
-    def on_model_update_end(
-        self, train_dataset: Dataset, val_dataset: Dataset, task_id: Optional[str] = None
-    ) -> RenateModule:
+    def on_model_update_end(self) -> None:
         """Called right before a model update terminates."""
-        return self._model
+        pass
 
-    def forward(self, x, task_id: Optional[str] = None) -> torch.Tensor:
+    def forward(self, inputs: NestedTensors, task_id: Optional[str] = None) -> torch.Tensor:
         """Forward pass of the model."""
         if task_id is None:
             task_id = self._task_id
-        return self._model(x, task_id=task_id)
+        return self._model(inputs, task_id=task_id)
 
-    def training_step(self, batch: List[torch.Tensor], batch_idx: int) -> STEP_OUTPUT:
+    def training_step(
+        self, batch: Tuple[NestedTensors, torch.Tensor], batch_idx: int
+    ) -> STEP_OUTPUT:
         """PyTorch Lightning function to return the training loss."""
-        x, y = batch
-        outputs = self(x)
+        inputs, targets = batch
+        outputs = self(inputs)
         intermediate_representation = self._model.get_intermediate_representation()
         self._model.reset_intermediate_representation_cache()
-        loss = self._model.loss_fn(outputs, y)
-
-        self._update_metrics(outputs, y, "train")
+        loss = self._model.loss_fn(outputs, targets)
+        self._update_metrics(outputs, targets, "train")
         self._loss_collections["train_losses"]["base_loss"](loss)
         return {
             "loss": loss,
             "outputs": outputs,
             "intermediate_representation": intermediate_representation,
         }
 
@@ -298,23 +312,23 @@
         super().training_step_end(step_output)
         self._loss_collections["train_losses"]["loss"](step_output["loss"])
         return step_output
 
     def training_epoch_end(self, outputs: List[Union[Tensor, Dict[str, Any]]]) -> None:
         """PyTorch Lightning function to run at the end of training epoch."""
         super().training_epoch_end(outputs)
-        if not self._val_enabled:
+        if not self.val_enabled:
             self._log_metrics()
 
-    def validation_step(self, batch: List[torch.Tensor], batch_idx: int) -> None:
+    def validation_step(self, batch: Tuple[NestedTensors, torch.Tensor], batch_idx: int) -> None:
         """PyTorch Lightning function to estimate validation metrics."""
-        (x, y), _ = batch
-        outputs = self(x)
-        loss = self._model.loss_fn(outputs, y)
-        self._update_metrics(outputs, y, "val")
+        (inputs, targets), _ = batch
+        outputs = self(inputs)
+        loss = self._model.loss_fn(outputs, targets)
+        self._update_metrics(outputs, targets, "val")
         self._loss_collections["val_losses"]["loss"](loss)
 
     def validation_epoch_end(self, outputs: List[Union[Tensor, Dict[str, Any]]]) -> None:
         """PyTorch Lightning function to run at the end of validation epoch."""
         super().validation_epoch_end(outputs)
         self._log_metrics()
 
@@ -348,15 +362,15 @@
 
     def _log_metrics(
         self,
     ) -> None:
         """Shared logic for logging metrics, including the loss."""
         if self.trainer.sanity_checking:
             return
-        prefixes = ["train", "val"] if self._val_enabled else ["train"]
+        prefixes = ["train", "val"] if self.val_enabled else ["train"]
         for prefix in prefixes:
             self.log_dict(
                 self._metric_collections[f"{prefix}_metrics"].compute(),
                 on_step=False,
                 on_epoch=True,
                 logger=True,
             )
@@ -378,15 +392,16 @@
 
     Args:
         memory_size: The maximum size of the memory.
         memory_batch_size: Size of batches sampled from the memory. The memory batch will be
             appended to the batch sampled from the current dataset, leading to an effective batch
             size of `memory_batch_size + batch_size`.
         buffer_transform: The transformation to be applied to the memory buffer data samples.
-        buffer_target_transform: The target transformation to be applied to the memory buffer target samples.
+        buffer_target_transform: The target transformation to be applied to the memory buffer target
+            samples.
         seed: See :func:`renate.models.utils.get_generator`.
     """
 
     def __init__(
         self,
         memory_size: int,
         memory_batch_size: int = defaults.BATCH_SIZE,
@@ -415,17 +430,28 @@
         )
         return state_dict
 
     def load_state_dict(self, model: RenateModule, state_dict: Dict[str, Any], **kwargs) -> None:
         """Restores the state of the learner."""
         super().load_state_dict(model, state_dict, **kwargs)
         self._memory_batch_size = state_dict["memory_batch_size"]
-        self._memory_buffer = ReservoirBuffer()
+        if not hasattr(self, "_memory_buffer"):
+            self._memory_buffer = ReservoirBuffer()
         self._memory_buffer.load_state_dict(state_dict["memory_buffer"])
 
+    def save(self, output_state_dir: str) -> None:
+        super().save(output_state_dir)
+        buffer_dir = os.path.join(output_state_dir, "memory_buffer")
+        os.makedirs(buffer_dir, exist_ok=True)
+        self._memory_buffer.save(buffer_dir)
+
+    def load(self, input_state_dir: str) -> None:
+        super().load(input_state_dir)
+        self._memory_buffer.load(os.path.join(input_state_dir, "memory_buffer"))
+
     def set_transforms(
         self,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
```

### Comparing `Renate-0.1.0/src/renate/updaters/learner_components/component.py` & `Renate-0.2.0/src/renate/updaters/learner_components/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import abc
-from typing import Any, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import torch
 import torch.nn as nn
 
-from renate.memory.buffer import DataDict, DataTuple
-from renate.models.renate_module import RenateModule
+from renate.models import RenateModule
+from renate.types import NestedTensors
 
 
 class Component(nn.Module, abc.ABC):
     """The abstract class implementing a Component, usable in the BaseExperienceReplayLearner.
 
     This is an abstract class from which each other component e.g. additional
     regularising loss or a module updater should inherit from.
@@ -23,23 +23,25 @@
         super().__init__()
         self._register_parameters(**kwargs)
         self._verify_attributes()
 
     def loss(
         self,
         outputs_memory: torch.Tensor,
-        batch_memory: Tuple[DataTuple, DataDict],
+        batch_memory: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
         intermediate_representation_memory: Optional[List[torch.Tensor]],
     ) -> torch.Tensor:
-        """Computes some user-defined loss which is added to the main training loss in the training step.
+        """Computes some user-defined loss which is added to the main training loss in the training
+        step.
 
         Args:
             outputs_memory: The outputs of the model with respect to memory data (batch_memory).
             batch_memory: The batch of data sampled from the memory buffer, including the meta data.
-            intermediate_representation_memory: Intermediate feature representations of the network upon passing the input through the network.
+            intermediate_representation_memory: Intermediate feature representations of the network
+                upon passing the input through the network.
         """
         return torch.tensor(0.0)
 
     def on_train_start(self, model: RenateModule) -> None:
         """Updates the model parameters.
 
         Args:
```

### Comparing `Renate-0.1.0/src/renate/updaters/learner_components/losses.py` & `Renate-0.2.0/src/renate/updaters/learner_components/losses.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import copy
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 
-from renate.memory.buffer import DataDict, DataTuple
-from renate.models.renate_module import RenateModule
+from renate.models import RenateModule
+from renate.types import NestedTensors
 from renate.updaters.learner_components.component import Component
 
 
 class WeightedLossComponent(Component, ABC):
     """The abstract class implementing a weighted loss function.
 
     This is an abstract class from which each other loss should inherit from.
 
     Args:
         weight: A scaling coefficient which should scale the loss which gets returned.
-        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory buffer when the loss is calculated.
+        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory
+            buffer when the loss is calculated.
     """
 
     def __init__(self, weight: float, sample_new_memory_batch: bool, **kwargs: Any) -> None:
         super().__init__(weight=weight, sample_new_memory_batch=sample_new_memory_batch, **kwargs)
 
     def _verify_attributes(self) -> None:
         """Verify if attributes have valid values."""
@@ -43,98 +44,101 @@
             weight, dtype=self._weight.dtype, device=self._weight.device
         )
         self._verify_attributes()
 
     def loss(
         self,
         outputs_memory: torch.Tensor,
-        batch_memory: Tuple[DataTuple, DataDict],
+        batch_memory: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
         intermediate_representation_memory: Optional[List[torch.Tensor]],
     ) -> torch.Tensor:
         if self.weight == 0:
             return torch.tensor(0.0)
         return self._loss(
             outputs_memory=outputs_memory,
             batch_memory=batch_memory,
             intermediate_representation_memory=intermediate_representation_memory,
         )
 
     @abstractmethod
     def _loss(
         self,
         outputs_memory: torch.Tensor,
-        batch_memory: Tuple[DataTuple, DataDict],
+        batch_memory: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
         intermediate_representation_memory: Optional[List[torch.Tensor]],
     ) -> torch.Tensor:
         pass
 
 
 class WeightedCustomLossComponent(WeightedLossComponent):
     """Adds a (weighted) user-provided custom loss contribution.
 
     Args:
         loss_fn: The loss function to apply.
         weight: A scaling coefficient which should scale the loss which gets returned.
-        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory buffer when the loss is calculated.
+        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory
+            buffer when the loss is calculated.
     """
 
     def __init__(
         self, loss_fn: Callable, weight: float, sample_new_memory_batch: bool, **kwargs: Any
     ) -> None:
         super().__init__(weight=weight, sample_new_memory_batch=sample_new_memory_batch, **kwargs)
         self._loss_fn = loss_fn
 
     def _loss(
         self,
         outputs_memory: torch.Tensor,
-        batch_memory: Tuple[DataTuple, DataDict],
+        batch_memory: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
         intermediate_representation_memory: Optional[List[torch.Tensor]],
     ) -> torch.Tensor:
         """Returns user-provided loss evaluated on memory batch."""
-        (_, y_memory), _ = batch_memory
-        return self.weight * self._loss_fn(outputs_memory, y_memory)
+        (_, targets_memory), _ = batch_memory
+        return self.weight * self._loss_fn(outputs_memory, targets_memory)
 
 
 class WeightedMeanSquaredErrorLossComponent(WeightedLossComponent):
-    """Mean squared error between the current and previous logits computed with respect to the memory sample.
-
-    Args:
-        weight: A scaling coefficient which should scale the loss which gets returned.
-        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory buffer when the loss is calculated.
+    """Mean squared error between the current and previous logits computed with respect to the
+    memory sample.
     """
 
     def _loss(
         self,
         outputs_memory: torch.Tensor,
-        batch_memory: Tuple[DataTuple, DataDict],
+        batch_memory: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
         intermediate_representation_memory: Optional[List[torch.Tensor]],
     ) -> torch.Tensor:
         """Mean-squared error between current and previous logits on memory."""
         logits = outputs_memory
-        (_, _), meta_data = batch_memory
+        _, meta_data = batch_memory
         previous_logits = meta_data["outputs"]
         return self.weight * F.mse_loss(logits, previous_logits, reduction="mean")
 
 
 class WeightedPooledOutputDistillationLossComponent(WeightedLossComponent):
     """Pooled output feature distillation with respect to intermediate network features.
 
-    As described in: Douillard, Arthur, et al. "Podnet: Pooled outputs distillation for small-tasks incremental learning."
-    European Conference on Computer Vision. Springer, Cham, 2020.
+    As described in: Douillard, Arthur, et al. "Podnet: Pooled outputs distillation for small-tasks
+    incremental learning." European Conference on Computer Vision. Springer, Cham, 2020.
 
-    Given the intermediate representations collected at different parts of the network, minimise their Euclidean distance
-    with respect to the cached representation. There are different `distillation_type`s trading-off plasticity and stability
-    of the resultant representations. `normalize` enables the user to normalize the resultant feature representations
-    to ensure that they are less affected by their magnitude.
+    Given the intermediate representations collected at different parts of the network, minimise
+    their Euclidean distance with respect to the cached representation. There are different
+    `distillation_type`s trading-off plasticity and stability of the resultant representations.
+    `normalize` enables the user to normalize the resultant feature representations to ensure that
+    they are less affected by their magnitude.
 
     Args:
-        weight: Scaling coefficient which scales the loss with respect to all intermediate representations.
-        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory buffer when the loss is calculated.
-        distillation_type: Which distillation type to apply with respect to all intermediate representations.
-        normalize: Whether to normalize both the current and cached features before computing the Frobenius norm.
+        weight: Scaling coefficient which scales the loss with respect to all intermediate
+            representations.
+        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory
+            buffer when the loss is calculated.
+        distillation_type: Which distillation type to apply with respect to all intermediate
+            representations.
+        normalize: Whether to normalize both the current and cached features before computing the
+            Frobenius norm.
     """
 
     def __init__(
         self,
         weight: float,
         sample_new_memory_batch: bool,
         distillation_type: str = "spatial",
@@ -193,15 +197,16 @@
 
         Args:
             features: Current intermediate features.
             features_memory: Cached intermediate features.
         """
         if features.shape != features_memory.shape:
             raise ValueError(
-                f"The shape of the features and the cached features should be the same: {features.shape}, and: {features_memory.shape}"
+                "The shape of the features and the cached features should be the same: "
+                f"{features.shape}, and: {features_memory.shape}"
             )
 
         features = features.pow(2)
         features_memory = features_memory.pow(2)
 
         if self._distillation_type == "channels":
             features, features_memory = self._sum_reshape(features, 1), self._sum_reshape(
@@ -241,45 +246,50 @@
     def set_normalize(self, normalize: bool) -> None:
         self._normalize = torch.tensor(normalize, dtype=torch.bool, device=self._normalize.device)
         self._verify_attributes()
 
     def _loss(
         self,
         outputs_memory: torch.Tensor,
-        batch_memory: Tuple[DataTuple, DataDict],
+        batch_memory: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
         intermediate_representation_memory: List[torch.Tensor],
     ) -> torch.Tensor:
-        """Compute the pooled output with respect to current and cached intermediate outputs from memory."""
+        """Compute the pooled output with respect to current and cached intermediate outputs from
+        memory.
+        """
         loss = 0.0
-        (_, _), meta_data = batch_memory
+        _, meta_data = batch_memory
         for n in range(len(intermediate_representation_memory)):
             features = intermediate_representation_memory[n]
             features_memory = meta_data[f"intermediate_representation_{n}"]
             loss += self._pod(features, features_memory)
         return (self.weight * loss) / len(intermediate_representation_memory)
 
 
 class WeightedCLSLossComponent(WeightedLossComponent):
     """Complementary Learning Systems Based Experience Replay.
 
     Arani, Elahe, Fahad Sarfraz, and Bahram Zonooz.
-    "Learning fast, learning slow: A general continual learning method based on complementary learning system."
-    arXiv preprint arXiv:2201.12604 (2022).
+    "Learning fast, learning slow: A general continual learning method based on complementary
+    learning system." arXiv preprint arXiv:2201.12604 (2022).
 
     The implementation follows the Algorithm 1 in the respective paper. The complete `Learner`
     implementing this loss, is the `CLSExperienceReplayLearner`.
 
     Args:
         weight: A scaling coefficient which should scale the loss which gets returned.
-        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory buffer when the loss is calculated.
+        sample_new_memory_batch: Whether a new batch of data should be sampled from the memory
+            buffer when the loss is calculated.
         model: The model that is being trained.
         stable_model_update_weight: The weight used in the update of the stable model.
         plastic_model_update_weight:  The weight used in the update of the plastic model.
-        stable_model_update_probability:  The probability of updating the stable model at each training step.
-        plastic_model_update_probability:  The probability of updating the plastic model at each training step.
+        stable_model_update_probability:  The probability of updating the stable model at each
+            training step.
+        plastic_model_update_probability:  The probability of updating the plastic model at each
+            training step.
     """
 
     def __init__(
         self,
         weight: float,
         sample_new_memory_batch: bool,
         model: RenateModule,
@@ -344,36 +354,27 @@
         assert 0.0 <= self._plastic_model_update_probability <= 1.0
         assert self._plastic_model_update_probability > self._stable_model_update_probability
         assert self._plastic_model_update_weight <= self._stable_model_update_weight
 
     def _loss(
         self,
         outputs_memory: torch.Tensor,
-        batch_memory: Tuple[DataTuple, DataDict],
+        batch_memory: Tuple[Tuple[NestedTensors, torch.Tensor], Dict[str, torch.Tensor]],
         intermediate_representation_memory: Optional[List[torch.Tensor]],
     ) -> torch.Tensor:
         """Computes the consistency loss with respect to averaged plastic and stable models."""
-        (x_memory, y_memory), _ = batch_memory
+        (inputs_memory, targets_memory), _ = batch_memory
         with torch.no_grad():
-
-            outputs_plastic = self._plastic_model(x_memory)
-            outputs_stable = self._stable_model(x_memory)
-
+            outputs_plastic = self._plastic_model(inputs_memory)
+            outputs_stable = self._plastic_model(inputs_memory)
             probs_plastic = F.softmax(outputs_plastic, dim=-1)
             probs_stable = F.softmax(outputs_stable, dim=-1)
-
-            label_mask = F.one_hot(y_memory, num_classes=outputs_stable.shape[-1]) > 0
+            label_mask = F.one_hot(targets_memory, num_classes=outputs_stable.shape[-1]) > 0
             idx = (probs_stable[label_mask] > probs_plastic[label_mask]).unsqueeze(1)
-
-            outputs = torch.where(
-                idx,
-                outputs_stable,
-                outputs_plastic,
-            )
-
+            outputs = torch.where(idx, outputs_stable, outputs_plastic)
         consistency_loss = F.mse_loss(outputs_memory, outputs.detach(), reduction="mean")
         return self.weight * consistency_loss
 
     @torch.no_grad()
     def _update_model_variables(
         self, model: RenateModule, original_model: RenateModule, weight: torch.Tensor
     ) -> None:
```

### Comparing `Renate-0.1.0/src/renate/updaters/learner_components/reinitialization.py` & `Renate-0.2.0/src/renate/updaters/learner_components/reinitialization.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/src/renate/updaters/model_updater.py` & `Renate-0.2.0/src/renate/updaters/model_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import torch
 import torchmetrics
 from pytorch_lightning import Callback, LightningModule, Trainer
 from pytorch_lightning.callbacks import EarlyStopping, ModelCheckpoint
 from pytorch_lightning.loggers.logger import Logger
 from syne_tune import Reporter
-from torch.utils.data import DataLoader, Dataset
+from torch.utils.data import Dataset
 
 from renate import defaults
 from .learner import Learner, ReplayLearner
 from ..models import RenateModule
 
 logging_logger = logging.getLogger(__name__)
 
@@ -56,55 +56,55 @@
 
 
 class RenateModelCheckpoint(ModelCheckpoint):
     """Callback to save Renate state after each epoch.
 
     Args:
         model: Model to be saved when creating a checkpoint.
-        state_folder: Checkpoint folder location.
+        output_state_folder: Checkpoint folder location.
         val_enabled: Whether validation was enabled in the Learner. Forwarded to `SyneTuneCallback`.
-        metric: Monitored metric to decide when to write a new checkpoint. If no metric is provided or validation is not
-            enabled, the latest model will be stored.
+        metric: Monitored metric to decide when to write a new checkpoint. If no metric is provided
+            or validation is not enabled, the latest model will be stored.
         mode: `min` or `max`. Whether to minimize or maximize the monitored `metric`.
         use_syne_tune_callback: Whether to use `SyneTuneCallback`.
     """
 
     def __init__(
         self,
         model: RenateModule,
-        state_folder: str,
+        output_state_folder: str,
         val_enabled: bool,
         metric: Optional[str] = None,
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         use_syne_tune_callback: bool = True,
     ) -> None:
         every_n_epochs = 1
         save_last = False
         if metric is None or not val_enabled:
             every_n_epochs = 0
             save_last = True
         learner_checkpoint_filename = Path(defaults.learner_state_file("")).stem
         super().__init__(
-            dirpath=state_folder,
+            dirpath=output_state_folder,
             filename=learner_checkpoint_filename,
             every_n_epochs=every_n_epochs,
             monitor=metric,
             mode=mode,
             save_last=save_last,
             save_weights_only=True,
         )
         self._model = model
-        self._state_folder = state_folder
+        self._output_state_folder = output_state_folder
         self.CHECKPOINT_NAME_LAST = learner_checkpoint_filename
         # Delete old checkpoint if exists
-        Path(defaults.learner_state_file(self._state_folder)).unlink(missing_ok=True)
+        Path(defaults.learner_state_file(self._output_state_folder)).unlink(missing_ok=True)
         # FIXME: Hack to make sure Syne Tune is called after checkpointing.
         # Details: https://github.com/Lightning-AI/lightning/issues/15026
-        # If fixed, remove on_train_epoch_end, on_validation_epoch_end, val_enabled, remove line below,
-        # and add in ModelUpdaterSyneTune callback.
+        # If fixed, remove on_train_epoch_end, on_validation_epoch_end, val_enabled, remove line
+        # below, and add in ModelUpdaterSyneTune callback.
         if use_syne_tune_callback:
             self._syne_tune_callback = SyneTuneCallback(val_enabled)
         else:
             self._syne_tune_callback = None
 
     def _save_checkpoint(self, trainer: Trainer, filepath: str) -> None:
         Path(self.dirpath).mkdir(parents=True, exist_ok=True)
@@ -117,91 +117,122 @@
             self._syne_tune_callback.on_train_epoch_end(trainer=trainer, pl_module=pl_module)
 
     def on_validation_epoch_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
         super().on_validation_epoch_end(trainer=trainer, pl_module=pl_module)
         if self._syne_tune_callback is not None:
             self._syne_tune_callback.on_validation_epoch_end(trainer=trainer, pl_module=pl_module)
 
+    def _load_best_checkpoint_and_save(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        # Reload best state.
+        learner_state_path = Path(defaults.learner_state_file(self._output_state_folder))
+        if learner_state_path.exists():
+            self._model.load_state_dict(torch.load(defaults.model_file(self.dirpath)))
+            pl_module.load_state_dict(self._model, torch.load(learner_state_path)["state_dict"])
+        # Finalize model update.
+        pl_module.on_model_update_end()
+        # Save permanently.
+        pl_module.save(self._output_state_folder)
+        # Overwrite checkpoint.
+        self._save_checkpoint(trainer, learner_state_path)
+
+    def on_exception(
+        self, trainer: Trainer, pl_module: LightningModule, exception: BaseException
+    ) -> None:
+        super().on_exception(trainer, pl_module, exception)
+        self._load_best_checkpoint_and_save(trainer, pl_module)
+
+    def on_fit_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        super().on_fit_end(trainer, pl_module)
+        self._load_best_checkpoint_and_save(trainer, pl_module)
+
 
 class ModelUpdater(abc.ABC):
     """Updates a learner using the data provided.
 
     Args:
         model: The potentially pretrained model to be updated with new data.
         learner_class: Class of the learner to be used for model update.
         learner_kwargs: Arguments either used for creating a new learner (no previous
             state available) or replace current arguments of the learner.
-        current_state_folder: Folder used by Renate to store files for current state.
-        next_state_folder: Folder used by Renate to store files for next state.
+        input_state_folder: Folder used by Renate to store files for current state.
+        output_state_folder: Folder used by Renate to store files for next state.
         max_epochs: The maximum number of epochs used to train the model.
         train_transform: The transformation applied during training.
         train_target_transform: The target transformation applied during testing.
         test_transform: The transformation at test time.
         test_target_transform: The target transformation at test time.
-        buffer_transform: Augmentations applied to the input data coming from the memory. Not all updaters require this.
-            If required but not passed, `transform` will be used.
-        buffer_target_transform: Transformations applied to the target. Not all updaters require this.
-            If required but not passed, `target_transform` will be used.
-        metric: Monitored metric to decide when to write a new checkpoint or early-stop the optimization.
-            If no metric is provided, the latest model will be stored.
+        buffer_transform: Augmentations applied to the input data coming from the memory. Not all
+            updaters require this. If required but not passed, `transform` will be used.
+        buffer_target_transform: Transformations applied to the target. Not all updaters require
+            this. If required but not passed, `target_transform` will be used.
+        metric: Monitored metric to decide when to write a new checkpoint or early-stop the
+            optimization. If no metric is provided, the latest model will be stored.
         mode: `min` or `max`. Whether to minimize or maximize the monitored `metric`.
         logged_metrics: Metrics logged additional to the default ones.
         early_stopping_enabled: Enables the early stopping of the optimization.
         logger: Logger used by PyTorch Lightning to log intermediate results.
         accelerator: Accelerator used by PyTorch Lightning to train the model.
-        devices: Devices used by PyTorch Lightning to train the model. If the devices flag is not defined,
-            it will assume devices to be "auto" and fetch the `auto_device_count` from the `accelerator`.
+        devices: Devices used by PyTorch Lightning to train the model. If the devices flag is not
+            defined, it will assume devices to be "auto" and fetch the `auto_device_count` from the
+            `accelerator`.
+        deterministic_trainer: When set to True makes the output of the training deterministic.
+            The value is passed to the trainer as described
+            `here <https://pytorch-lightning.readthedocs.io/en/stable/common\
+            /trainer.html#reproducibility>`_.
     """
 
     def __init__(
         self,
         model: RenateModule,
         learner_class: Type[Learner],
         learner_kwargs: Optional[Dict[str, Any]] = None,
-        current_state_folder: Optional[str] = None,
-        next_state_folder: Optional[str] = None,
+        input_state_folder: Optional[str] = None,
+        output_state_folder: Optional[str] = None,
         max_epochs: int = defaults.MAX_EPOCHS,
         train_transform: Optional[Callable] = None,
         train_target_transform: Optional[Callable] = None,
         test_transform: Optional[Callable] = None,
         test_target_transform: Optional[Callable] = None,
         buffer_transform: Optional[Callable] = None,
         buffer_target_transform: Optional[Callable] = None,
         metric: Optional[str] = None,
         mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "min",
         logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
         early_stopping_enabled: bool = False,
         logger: Logger = defaults.LOGGER(**defaults.LOGGER_KWARGS),
         accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
         devices: Optional[int] = None,
+        deterministic_trainer: bool = defaults.DETERMINISTIC_TRAINER,
     ):
         self._learner_kwargs = learner_kwargs or {}
         self._model = model
         self._learner_state_file: Optional[str] = None
-        if current_state_folder is not None:
-            self._learner_state_file = defaults.learner_state_file(current_state_folder)
+        if input_state_folder is not None:
+            self._learner_state_file = defaults.learner_state_file(input_state_folder)
         else:
             logging_logger.info(
                 "No location for current updater state provided. Updating will start from scratch."
             )
-        if next_state_folder is None:
+        if output_state_folder is None:
             logging_logger.info(
                 "No location for next updater state provided. No state will be stored."
             )
         elif metric is None:
             logging_logger.info(
                 "Metric or mode is not provided. Checkpoint is saved only after training."
             )
         if metric is None and early_stopping_enabled:
             warnings.warn(
-                "Early stopping is enabled but no metric is specified. Early stopping will be ignored."
+                "Early stopping is enabled but no metric is specified. Early stopping will be "
+                "ignored."
             )
             early_stopping_enabled = False
 
-        self._next_state_folder = next_state_folder
+        self._input_state_folder = input_state_folder
+        self._output_state_folder = output_state_folder
         self._metric = metric
         self._mode = mode
         self._logged_metrics = logged_metrics
         self._early_stopping_enabled = early_stopping_enabled
         self._train_transform = train_transform
         self._train_target_transform = train_target_transform
         self._test_transform = test_transform
@@ -213,34 +244,35 @@
             "train_target_transform": self._train_target_transform,
             "test_transform": self._test_transform,
             "test_target_transform": self._test_target_transform,
         }
         if issubclass(learner_class, ReplayLearner):
             self._transforms_kwargs["buffer_transform"] = self._buffer_transform
             self._transforms_kwargs["buffer_target_transform"] = self._buffer_target_transform
-        self._learner = self._load_learner(learner_class, self._learner_kwargs)
-        assert self._learner.is_logged_metric(metric), f"Target metric `{metric}` is not logged."
         self._max_epochs = max_epochs
-        self._logger = logger
-        self._num_epochs_trained = 0
         if accelerator not in defaults.SUPPORTED_ACCELERATORS:
             raise ValueError(
                 f"Accelerator {accelerator} not supported. "
                 f"Supported accelerators are {defaults.SUPPORTED_ACCELERATORS}."
             )
         self._accelerator = accelerator
         self._devices = devices
+        self._learner = self._load_learner(learner_class, self._learner_kwargs)
+        assert self._learner.is_logged_metric(metric), f"Target metric `{metric}` is not logged."
+        self._logger = logger
+        self._num_epochs_trained = 0
+        self._deterministic_trainer = deterministic_trainer
 
     @abc.abstractmethod
     def update(
         self,
         train_dataset: Dataset,
         val_dataset: Optional[Dataset] = None,
         task_id: Optional[str] = None,
-    ) -> RenateModule:
+    ) -> None:
         """Updates the model using the data passed as input.
 
         Args:
             train_dataset: The training data.
             val_dataset: The validation data.
             task_id: The task id.
         """
@@ -256,67 +288,62 @@
                 model=self._model,
                 **learner_kwargs,
                 logged_metrics=self._logged_metrics,
                 **self._transforms_kwargs,
             )
         learner = learner_class.__new__(learner_class)
         learner.load_state_dict(self._model, torch.load(self._learner_state_file)["state_dict"])
+        learner.load(self._input_state_folder)
         learner.set_transforms(**self._transforms_kwargs)
         learner.set_logged_metrics(self._logged_metrics)
         learner.update_hyperparameters(learner_kwargs)
         return learner
 
     def _fit_learner(
         self,
         learner: Learner,
-        train_loader: DataLoader,
-        val_loader: DataLoader,
         use_syne_tune_callback: bool = True,
     ) -> None:
         callbacks: List[Callback] = []
         if use_syne_tune_callback:
-            callbacks.append(SyneTuneCallback(val_loader is not None))
-        if self._next_state_folder is not None:
+            callbacks.append(SyneTuneCallback(learner.val_enabled))
+        if self._output_state_folder is not None:
             model_checkpoint_callback = RenateModelCheckpoint(
                 model=self._model,
-                state_folder=self._next_state_folder,
+                output_state_folder=self._output_state_folder,
                 metric=self._metric,
                 mode=self._mode,
-                val_enabled=val_loader is not None,
+                val_enabled=learner.val_enabled,
                 use_syne_tune_callback=use_syne_tune_callback,
             )
             callbacks = [model_checkpoint_callback]  # FIXME: insert at 0 as soon as PTL is fixed.
 
         if self._early_stopping_enabled:
-            if val_loader is not None:
-                callbacks.insert(
-                    0,
-                    EarlyStopping(
-                        monitor=self._metric,
-                        mode=self._mode,
-                    ),
-                )
+            if learner.val_enabled:
+                callbacks.insert(0, EarlyStopping(monitor=self._metric, mode=self._mode))
             else:
                 warnings.warn(
-                    "Early stopping is currently not supported without a validation set. It will be ignored."
+                    "Early stopping is currently not supported without a validation set. It will "
+                    "be ignored."
                 )
 
         trainer = Trainer(
             accelerator=self._accelerator,
             devices=self._devices,
             max_epochs=self._max_epochs,
             callbacks=callbacks,
             logger=self._logger,
             enable_progress_bar=False,
+            deterministic=self._deterministic_trainer,
         )
-        trainer.fit(learner, train_loader, val_loader)
+        trainer.fit(learner)
         self._num_epochs_trained = trainer.current_epoch
 
 
-class SimpleModelUpdater(ModelUpdater):
+class SingleTrainingLoopUpdater(ModelUpdater):
     """Simple ModelUpdater which requires a single learner only to update the model."""
 
     def update(
         self,
         train_dataset: Dataset,
         val_dataset: Optional[Dataset] = None,
         task_id: Optional[str] = None,
@@ -324,14 +351,10 @@
         """Updates the model using the data passed as input.
 
         Args:
             train_dataset: The training data.
             val_dataset: The validation data.
             task_id: The task id.
         """
-        train_loader, val_loader = self._learner.on_model_update_start(
-            train_dataset, val_dataset, task_id
-        )
-
-        self._fit_learner(self._learner, train_loader, val_loader)
-
-        return self._learner.on_model_update_end(train_dataset, val_dataset, task_id)
+        self._learner.on_model_update_start(train_dataset, val_dataset, task_id)
+        self._fit_learner(self._learner)
+        return self._model
```

### Comparing `Renate-0.1.0/src/renate/utils/file.py` & `Renate-0.2.0/src/renate/utils/file.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/src/renate/utils/module.py` & `Renate-0.2.0/src/renate/utils/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,31 @@
     task_id: str = defaults.TASK_ID,
     logged_metrics: Optional[Dict[str, torchmetrics.Metric]] = None,
     metric_postfix: str = "",
     batch_size: int = defaults.BATCH_SIZE,
     accelerator: defaults.SUPPORTED_ACCELERATORS_TYPE = defaults.ACCELERATOR,
     devices: Optional[int] = None,
 ) -> Dict[str, List[List[float]]]:
-    """A helper function that performs the evaluation on test data and records quantitative metrics in a dictionary.
+    """A helper function that performs the evaluation on test data and records quantitative metrics
+    in a dictionary.
 
     Args:
         results: The results dictionary to which the results should be saved.
         model: A RenateModule to be evaluated.
         data_module: A Scenario or RenateDataModule from which the test data is queried.
         transform: The transformation applied for evaluation.
         target_transform: The target transformation applied for evaluation.
         task_id: The task ID for which the evaluation should be performed.
         logged_metrics: Metrics logged additional to the default ones.
         metric_postfix: The postfix for the metric names.
         batch_size: A batch size for the test loader.
         accelerator: Accelerator used by PyTorch Lightning to train the model.
-        devices: Devices used by PyTorch Lightning to train the model. If the devices flag is not defined,
-                 it will assume devices to be "auto" and fetch the `auto_device_count` from the `accelerator`.
+        devices: Devices used by PyTorch Lightning to train the model. If the devices flag is not
+            defined, it will assume devices to be "auto" and fetch the `auto_device_count` from the
+            `accelerator`.
     """
 
     data_module.setup()
 
     update_results = evaluate(
         model=model,
         test_dataset=data_module.test_data(),
@@ -86,15 +88,15 @@
     data_module = get_data_module(config_module, **kwargs)
     data_module.prepare_data()
     return data_module
 
 
 def get_and_setup_data_module(
     config_module: ModuleType,
-    prepare_data: int,
+    prepare_data: bool,
     **kwargs: Any,
 ) -> RenateDataModule:
     """Creates data module and possibly calls the prepare_data function needed for setup"""
     data_module = get_data_module(config_module, **kwargs)
     if prepare_data:
         data_module.prepare_data()
     data_module.setup()
```

### Comparing `Renate-0.1.0/src/renate/utils/optimizer.py` & `Renate-0.2.0/src/renate/utils/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     gamma: float = defaults.LEARNING_RATE_SCHEDULER_GAMMA,
 ) -> torch.optim.lr_scheduler._LRScheduler:
     """Creates a learning rate scheduler used to train the model.
 
     Args:
         optimizer: The optimizer to be used.
         scheduler: The name of the scheduler to be used.
+        step_size: Period of learning rate decay.
         gamma: Value for the gamma hyperparameter (if relevant).
     """
 
     if scheduler == "ConstantLR":
         return torch.optim.lr_scheduler.ConstantLR(optimizer, factor=1.0)
     elif scheduler == "ExponentialLR":
         return torch.optim.lr_scheduler.ExponentialLR(optimizer, gamma=gamma)
```

### Comparing `Renate-0.1.0/src/renate/utils/syne_tune.py` & `Renate-0.2.0/src/renate/utils/syne_tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 logger = logging.getLogger(__name__)
 
 
 class TuningLoggerCallback(TunerCallback):
     """Syne Tune Logging Callback when running hyperparameter optimization.
 
-    Will report whenever improved results are obtained. If no better configuration is received within the last ten
-    minutes, it will send a message to indicate it is still running."""
+    Will report whenever improved results are obtained. If no better configuration is received
+    within the last ten minutes, it will send a message to indicate it is still running.
+    """
 
     def __init__(self, mode: str, metric: str):
         self._mode = mode
         self._metric = metric
         self._best_score = float("inf") * (1 if self._mode == "min" else -1)
         self._last_log = time.time()
 
@@ -57,16 +58,17 @@
         )
         logger.info(f"Epoch {result['epoch']}/{trial.config['max_epochs']}\n{result_table}")
 
 
 def redirect_to_tmp(uri: str) -> str:
     """Changes uri in /opt/ml to /tmp.
 
-    Syne Tune stores checkpoints by default in /opt/ml when running on SageMaker. While we want to store checkpoints,
-    we have no interest in uploading them to S3. Therefore, this function changes the location to /tmp instead.
+    Syne Tune stores checkpoints by default in /opt/ml when running on SageMaker. While we want to
+    store checkpoints, we have no interest in uploading them to S3. Therefore, this function changes
+    the location to /tmp instead.
     """
     if "SM_MODEL_DIR" in os.environ:  # If running on sagemaker, redirect checkpoints to /tmp
         assert uri.startswith("/opt/ml")
         uri = "/tmp" + uri[7:]
     return uri
 
 
@@ -85,15 +87,16 @@
     # TODO: remove with Syne Tune 0.3.3
     return {k: from_dict(v) if isinstance(v, dict) else v for k, v in config_space_dict.items()}
 
 
 def best_hyperparameters(
     experiment: ExperimentResult, config_space: Dict[str, Union[Domain, int, float, str]]
 ) -> Dict[str, Union[int, float, str]]:
-    """Returns the values of all keys in the `config_space` that belong to a Syne Tune search space."""
+    """Returns the values of all keys in the `config_space` that belong to a Syne Tune search
+    space."""
     return {
         k[7:]: v
         for k, v in experiment.best_config().items()
         if k.startswith("config_") and isinstance(config_space[k[7:]], Domain)
     }
```

### Comparing `Renate-0.1.0/test/conftest.py` & `Renate-0.2.0/test/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,39 +4,46 @@
 import shutil
 from typing import Callable, Dict
 
 import pytest
 import torch
 from pytorch_lightning.loggers import TensorBoardLogger
 
-from renate.benchmark.models.mlp import MultiLayerPerceptron
-from renate.benchmark.models.resnet import (
+from renate.benchmark.models import (
+    MultiLayerPerceptron,
     ResNet18,
     ResNet18CIFAR,
     ResNet34,
     ResNet34CIFAR,
     ResNet50,
     ResNet50CIFAR,
-)
-from renate.benchmark.models.vision_transformer import (
     VisionTransformerB16,
     VisionTransformerB32,
     VisionTransformerCIFAR,
     VisionTransformerH14,
     VisionTransformerL16,
     VisionTransformerL32,
 )
 from renate.models.renate_module import RenateModule
-from renate.updaters.experimental.repeated_distill import RepeatedDistillationLearner
+from renate.updaters.avalanche.learner import (
+    AvalancheEWCLearner,
+    AvalancheICaRLLearner,
+    AvalancheLwFLearner,
+    AvalancheReplayLearner,
+)
+from renate.updaters.avalanche.model_updater import (
+    AvalancheModelUpdater,
+)
 from renate.updaters.experimental.er import ExperienceReplayLearner
 from renate.updaters.experimental.gdumb import GDumbLearner
 from renate.updaters.experimental.joint import JointLearner
 from renate.updaters.experimental.offline_er import OfflineExperienceReplayLearner
+from renate.updaters.experimental.repeated_distill import RepeatedDistillationLearner
 from renate.updaters.learner import Learner, ReplayLearner
-from renate.updaters.model_updater import SimpleModelUpdater
+from renate.updaters.model_updater import SingleTrainingLoopUpdater
 
 pytest_plugins = ["helpers_namespace"]
 
 
 def pytest_addoption(parser):
     parser.addoption(
         "--runslow",
@@ -112,14 +119,55 @@
         "learning_rate": 2.5,
         "momentum": 1.3,
         "weight_decay": 0.5,
         "batch_size": 50,
         "seed": 1,
     },
 }
+AVALANCHE_LEARNER_KWARGS = {
+    AvalancheReplayLearner: {
+        "memory_size": 30,
+        "memory_batch_size": 20,
+        "optimizer": "SGD",
+        "learning_rate": 2.5,
+        "momentum": 1.3,
+        "weight_decay": 0.5,
+        "batch_size": 50,
+        "seed": 1,
+    },
+    AvalancheEWCLearner: {
+        "ewc_lambda": 0.1,
+        "optimizer": "SGD",
+        "learning_rate": 2.5,
+        "momentum": 1.3,
+        "weight_decay": 0.5,
+        "batch_size": 50,
+        "seed": 1,
+    },
+    AvalancheLwFLearner: {
+        "alpha": 0.1,
+        "temperature": 2,
+        "optimizer": "SGD",
+        "learning_rate": 2.5,
+        "momentum": 1.3,
+        "weight_decay": 0.5,
+        "batch_size": 50,
+        "seed": 1,
+    },
+    AvalancheICaRLLearner: {
+        "memory_size": 30,
+        "memory_batch_size": 20,
+        "optimizer": "SGD",
+        "learning_rate": 2.5,
+        "momentum": 1.3,
+        "weight_decay": 0.5,
+        "batch_size": 50,
+        "seed": 1,
+    },
+}
 LEARNER_HYPERPARAMETER_UPDATES = {
     ExperienceReplayLearner: {
         "optimizer": "Adam",
         "learning_rate": 3.0,
         "momentum": 0.5,
         "weight_decay": 0.01,
         "batch_size": 128,
@@ -154,15 +202,27 @@
         "optimizer": "Adam",
         "learning_rate": 3.0,
         "momentum": 0.5,
         "weight_decay": 0.01,
         "batch_size": 128,
     },
 }
+AVALANCHE_LEARNER_HYPERPARAMETER_UPDATES = {
+    AvalancheEWCLearner: {
+        "ewc_lambda": 0.3,
+    },
+    AvalancheLwFLearner: {
+        "alpha": 0.2,
+        "temperature": 3,
+    },
+    AvalancheICaRLLearner: {},
+    AvalancheReplayLearner: {},
+}
 LEARNERS = list(LEARNER_KWARGS)
+AVALANCHE_LEARNERS = list(AVALANCHE_LEARNER_KWARGS)
 LEARNERS_USING_SIMPLE_UPDATER = [
     ExperienceReplayLearner,
     Learner,
     GDumbLearner,
     JointLearner,
     OfflineExperienceReplayLearner,
 ]
@@ -178,20 +238,29 @@
 
 TEST_WORKING_DIRECTORY = "./test_renate_working_dir/"
 TEST_LOGGER = TensorBoardLogger
 TEST_LOGGER_KWARGS = {"save_dir": TEST_WORKING_DIRECTORY, "version": 1, "name": "lightning_logs"}
 
 
 @pytest.helpers.register
-def get_renate_module_mlp(num_inputs, num_outputs, num_hidden_layers, hidden_size) -> RenateModule:
-    return MultiLayerPerceptron(num_inputs, num_outputs, num_hidden_layers, hidden_size)
+def get_renate_module_mlp(
+    num_inputs, num_outputs, num_hidden_layers, hidden_size, add_icarl_class_means=False
+) -> RenateModule:
+    return MultiLayerPerceptron(
+        num_inputs,
+        num_outputs,
+        num_hidden_layers,
+        hidden_size,
+        add_icarl_class_means=add_icarl_class_means,
+    )
 
 
 @pytest.helpers.register
 def get_renate_module_resnet(sub_class="resnet18cifar", **kwargs) -> RenateModule:
+    kwargs["add_icarl_class_means"] = False
     if sub_class == "resnet18cifar":
         return ResNet18CIFAR(**kwargs)
     elif sub_class == "resnet34cifar":
         return ResNet34CIFAR(**kwargs)
     elif sub_class == "resnet50cifar":
         return ResNet50CIFAR(**kwargs)
     elif sub_class == "resnet18":
@@ -204,14 +273,15 @@
         raise ValueError("Invalid ResNet called.")
 
 
 @pytest.helpers.register
 def get_renate_module_vision_transformer(
     sub_class="visiontransformerb16", **kwargs
 ) -> RenateModule:
+    kwargs["add_icarl_class_means"] = False
     if sub_class == "visiontransformercifar":
         return VisionTransformerCIFAR(**kwargs)
     elif sub_class == "visiontransformerb16":
         return VisionTransformerB16(**kwargs)
     elif sub_class == "visiontransformerb32":
         return VisionTransformerB32(**kwargs)
     elif sub_class == "visiontransformerl16":
@@ -239,20 +309,22 @@
     num_inputs,
     num_outputs,
     num_hidden_layers,
     hidden_size,
     train_num_samples,
     test_num_samples,
     val_num_samples=0,
+    add_icarl_class_means=False,
 ):
     model = get_renate_module_mlp(
         num_inputs=num_inputs,
         num_outputs=num_outputs,
         hidden_size=hidden_size,
         num_hidden_layers=num_hidden_layers,
+        add_icarl_class_means=add_icarl_class_means,
     )
     train_dataset = torch.utils.data.TensorDataset(
         torch.rand(train_num_samples, num_inputs),
         torch.randint(num_outputs, (train_num_samples,)),
     )
     test_data = torch.rand(test_num_samples, num_inputs)
 
@@ -284,60 +356,97 @@
     test_data = torch.rand(test_num_samples, *input_size)
     return model, train_dataset, test_data
 
 
 @pytest.helpers.register
 def get_simple_updater(
     model,
-    current_state_folder=None,
-    next_state_folder=None,
+    input_state_folder=None,
+    output_state_folder=None,
     learner_class=ExperienceReplayLearner,
     learner_kwargs={"memory_size": 10},
     max_epochs=5,
     train_transform=None,
     train_target_transform=None,
     test_transform=None,
     test_target_transform=None,
     buffer_transform=None,
     buffer_target_transform=None,
     early_stopping_enabled=False,
     metric=None,
+    deterministic_trainer=False,
 ):
     transforms_kwargs = {
         "train_transform": train_transform,
         "train_target_transform": train_target_transform,
         "test_transform": test_transform,
         "test_target_transform": test_target_transform,
     }
     if issubclass(learner_class, ReplayLearner):
         transforms_kwargs["buffer_transform"] = buffer_transform
         transforms_kwargs["buffer_target_transform"] = buffer_target_transform
-    return SimpleModelUpdater(
+    return SingleTrainingLoopUpdater(
         model=model,
         learner_class=learner_class,
         learner_kwargs=learner_kwargs,
-        current_state_folder=current_state_folder,
-        next_state_folder=next_state_folder,
+        input_state_folder=input_state_folder,
+        output_state_folder=output_state_folder,
         max_epochs=max_epochs,
         accelerator="cpu",
         logger=TEST_LOGGER(**TEST_LOGGER_KWARGS),
         early_stopping_enabled=early_stopping_enabled,
         metric=metric,
+        deterministic_trainer=deterministic_trainer,
+        **transforms_kwargs,
+    )
+
+
+@pytest.helpers.register
+def get_avalanche_updater(
+    model,
+    input_state_folder=None,
+    output_state_folder=None,
+    learner_class=AvalancheReplayLearner,
+    learner_kwargs={"memory_size": 10},
+    max_epochs=5,
+    train_transform=None,
+    train_target_transform=None,
+    test_transform=None,
+    test_target_transform=None,
+    early_stopping_enabled=False,
+    metric=None,
+):
+    transforms_kwargs = {
+        "train_transform": train_transform,
+        "train_target_transform": train_target_transform,
+        "test_transform": test_transform,
+        "test_target_transform": test_target_transform,
+    }
+    return AvalancheModelUpdater(
+        model=model,
+        learner_class=learner_class,
+        learner_kwargs=learner_kwargs,
+        input_state_folder=input_state_folder,
+        output_state_folder=output_state_folder,
+        max_epochs=max_epochs,
+        accelerator="cpu",
+        early_stopping_enabled=early_stopping_enabled,
+        metric=metric,
         **transforms_kwargs,
     )
 
 
 @pytest.helpers.register
 def check_learner_transforms(learner: Learner, expected_transforms: Dict[str, Callable]):
     """Checks if the learner transforms match to expected ones.
 
     Args:
         learner: The learner which transforms will be checked.
-        expected_transforms: Dictionairy mapping from transform name to transform. These are the expected transforms
-            for the learner.
+        expected_transforms: Dictionairy mapping from transform name to transform. These are the
+            expected transforms for the learner.
     """
     assert learner._train_transform is expected_transforms.get(
         "train_transform"
     ) and learner._train_target_transform is expected_transforms.get("train_target_transform")
     if isinstance(learner, ReplayLearner):
         assert learner._memory_buffer._transform is expected_transforms.get(
             "buffer_transform"
```

### Comparing `Renate-0.1.0/test/datasets.py` & `Renate-0.2.0/test/dummy_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     def __len__(self):
         return len(self.data)
 
 
 class DummyTorchVisionDataModule(RenateDataModule):
     """
-    A simple data module similar to `TorchVisionDataModule` with 100 training instances and 100 test instances with
-    shape (1, 5, 5) and 5 classes.
+    A simple data module similar to `TorchVisionDataModule` with 100 training instances and 100 test
+    instances with shape (1, 5, 5) and 5 classes.
     """
 
     def __init__(
         self,
         transform: Optional[Callable] = None,
         val_size: float = defaults.VALIDATION_SIZE,
         seed: int = defaults.SEED,
```

### Comparing `Renate-0.1.0/test/renate/benchmark/models/test_mlp.py` & `Renate-0.2.0/test/renate/benchmark/models/test_mlp.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/test/renate/benchmark/models/test_resnet.py` & `Renate-0.2.0/test/renate/benchmark/models/test_resnet.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/test/renate/benchmark/models/test_vision_transformer.py` & `Renate-0.2.0/test/renate/benchmark/models/test_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/test/renate/benchmark/test_experimentation.py` & `Renate-0.2.0/test/renate/benchmark/test_experimentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 from pathlib import Path
 
 import pandas as pd
 import pytest
-from pandas.testing import assert_frame_equal
 
 from renate.benchmark.experimentation import execute_experiment_job
 
 
 @pytest.fixture
 def experiment_job_kwargs():
     return {
         "backend": "local",
         "config_file": str(Path(__file__).parent.parent / "renate_config_files" / "config.py"),
-        "config_space": {"updater": "ER", "data_module_fn_use_scenario": "True", "max_epochs": 5},
+        "config_space": {"updater": "ER", "use_scenario": True, "max_epochs": 5},
         "mode": "max",
         "metric": "val_accuracy",
         "num_updates": 2,
         "max_time": 15,
         "seed": 0,
     }
 
 
 def test_execute_experiment_job(tmpdir, experiment_job_kwargs):
     """Only checking if things run, not testing anything besides that."""
-    expected_results = pd.DataFrame([[1, 0.15, 0.0, 0.0, 0.0], [2, 0.175, -0.15, 0.0, 0.15]])
     expected_columns = [
         "Task ID",
         "Average Accuracy",
         "Forgetting",
         "Forward Transfer",
         "Backward Transfer",
     ]
     expected_num_updates = experiment_job_kwargs["num_updates"]
-    expected_results.columns = expected_columns
     execute_experiment_job(experiment_outputs_url=tmpdir, **experiment_job_kwargs)
     results_df = pd.read_csv(str(Path(tmpdir) / "logs" / "metrics_summary.csv"))
     assert all(results_df.columns == expected_columns)
-    assert_frame_equal(results_df, expected_results)
     for update_id in range(expected_num_updates):
         assert (Path(tmpdir) / f"update_{update_id}" / "learner.ckpt").is_file()
         assert (Path(tmpdir) / f"update_{update_id}" / "model.ckpt").is_file()
     assert (
         len(
-            pd.read_csv(str(Path(tmpdir) / f"update_{expected_num_updates-1}" / "hpo.csv"))[
+            pd.read_csv(str(Path(tmpdir) / f"update_{expected_num_updates - 1}" / "hpo.csv"))[
                 "update_id"
             ].unique()
         )
         == expected_num_updates
     )
```

### Comparing `Renate-0.1.0/test/renate/benchmark/test_experimentation_config.py` & `Renate-0.2.0/test/renate/benchmark/test_experimentation_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,39 +12,42 @@
     model_fn,
     models,
     train_transform,
 )
 from renate.benchmark.scenarios import (
     BenchmarkScenario,
     ClassIncrementalScenario,
+    FeatureSortingScenario,
+    HueShiftScenario,
+    IIDScenario,
     ImageRotationScenario,
     PermutationScenario,
 )
 
 
 @pytest.mark.parametrize(
     "model_name,expected_model_class",
     [(model_name, model_class) for model_name, model_class in zip(models.keys(), models.values())],
 )
 def test_model_fn(model_name, expected_model_class):
     model = model_fn(
         model_state_url=None,
-        model_fn_model_name=model_name,
-        model_fn_num_inputs=1 if model_name == "MultiLayerPerceptron" else None,
-        model_fn_num_outputs=1 if model_name == "MultiLayerPerceptron" else None,
-        model_fn_num_hidden_layers=1 if model_name == "MultiLayerPerceptron" else None,
-        model_fn_hidden_size="1" if model_name == "MultiLayerPerceptron" else None,
+        model_name=model_name,
+        num_inputs=1 if model_name == "MultiLayerPerceptron" else None,
+        num_outputs=1 if model_name == "MultiLayerPerceptron" else None,
+        num_hidden_layers=1 if model_name == "MultiLayerPerceptron" else None,
+        hidden_size=1 if model_name == "MultiLayerPerceptron" else None,
     )
     assert isinstance(model, expected_model_class)
 
 
 def test_model_fn_fails_for_unknown_model():
     unknown_model_name = "UNKNOWN_MODEL_NAME"
     with pytest.raises(ValueError, match=f"Unknown model `{unknown_model_name}`"):
-        model_fn(model_fn_model_name=unknown_model_name)
+        model_fn(model_name=unknown_model_name)
 
 
 @pytest.mark.parametrize(
     "dataset_name,data_module_class",
     (("CIFAR10", TorchVisionDataModule), ("CLEAR10", CLEARDataModule)),
 )
 def test_get_data_module(tmpdir, dataset_name, data_module_class):
@@ -69,47 +72,67 @@
 
 @pytest.mark.parametrize(
     "scenario_name,dataset_name,scenario_kwargs,expected_scenario_class,expected_num_tasks",
     (
         (
             "ClassIncrementalScenario",
             "CIFAR10",
-            {"data_module_fn_class_groupings": "[[0,1],[2,3,4],[5,6]]"},
+            {"class_groupings": ((0, 1), (2, 3, 4), (5, 6))},
             ClassIncrementalScenario,
             3,
         ),
         (
-            "ClassIncrementalScenario",
-            "AG_NEWS",
-            {"data_module_fn_class_groupings": "[[1,2],[3,4]]"},
-            ClassIncrementalScenario,
-            2,
+            "IIDScenario",
+            "MNIST",
+            {"num_tasks": 3},
+            IIDScenario,
+            3,
         ),
         (
             "ImageRotationScenario",
             "MNIST",
-            {"data_module_fn_degrees": "[0,90,180]"},
+            {"degrees": (0, 90, 180)},
             ImageRotationScenario,
             3,
         ),
-        ("BenchmarkScenario", "CLEAR10", {"data_module_fn_num_tasks": "5"}, BenchmarkScenario, 5),
+        ("BenchmarkScenario", "CLEAR10", {"num_tasks": 5}, BenchmarkScenario, 5),
         (
             "PermutationScenario",
             "MNIST",
-            {"data_module_fn_num_tasks": "3", "data_module_fn_input_dim": "(1,28,28)"},
+            {"num_tasks": 3, "input_dim": (1, 28, 28)},
             PermutationScenario,
             3,
         ),
+        (
+            "FeatureSortingScenario",
+            "MNIST",
+            {
+                "num_tasks": 5,
+                "feature_idx": 0,
+                "randomness": 0.3,
+            },
+            FeatureSortingScenario,
+            5,
+        ),
+        (
+            "HueShiftScenario",
+            "CIFAR10",
+            {"num_tasks": 3, "randomness": 0.5},
+            HueShiftScenario,
+            3,
+        ),
     ),
     ids=[
         "class_incremental_image",
-        "class_incremental_text",
+        "iid",
         "rotation",
         "benchmark",
         "permutation",
+        "feature_sorting",
+        "hue_shift",
     ],
 )
 @pytest.mark.parametrize("val_size", (0, 0.5), ids=["no_val", "val"])
 def test_data_module_fn(
     tmpdir,
     scenario_name,
     dataset_name,
@@ -118,25 +141,27 @@
     expected_num_tasks,
     val_size,
 ):
     scenario = data_module_fn(
         data_path=tmpdir,
         chunk_id=0,
         seed=0,
-        data_module_fn_scenario_name=scenario_name,
-        data_module_fn_dataset_name=dataset_name,
-        data_module_fn_val_size=val_size,
+        scenario_name=scenario_name,
+        dataset_name=dataset_name,
+        val_size=val_size,
         **scenario_kwargs,
     )
     assert isinstance(scenario, expected_scenario_class)
     if expected_scenario_class == ClassIncrementalScenario:
-        assert (
-            str(scenario._class_groupings).replace(" ", "")
-            == scenario_kwargs["data_module_fn_class_groupings"]
-        )
+        assert scenario._class_groupings == scenario_kwargs["class_groupings"]
+    elif expected_scenario_class == FeatureSortingScenario:
+        scenario._feature_idx = scenario_kwargs["feature_idx"]
+        scenario._randomness = scenario_kwargs["randomness"]
+    elif expected_scenario_class == HueShiftScenario:
+        scenario._randomness = scenario_kwargs["randomness"]
     assert scenario._num_tasks == expected_num_tasks
 
 
 @pytest.mark.parametrize(
     "dataset_name,use_transforms",
     (("MNIST", False), ("FashionMNIST", False), ("CIFAR10", True), ("CIFAR100", True)),
 )
```

### Comparing `Renate-0.1.0/test/renate/benchmark/test_scenarios.py` & `Renate-0.2.0/test/renate/benchmark/test_scenarios.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-import copy
 from collections import Counter
 
 import numpy as np
 import pytest
 import torch
 from torchvision.transforms.functional import rotate
 
-from datasets import DummyTorchVisionDataModule, DummyTorchVisionDataModuleWithChunks
+from dummy_datasets import DummyTorchVisionDataModule, DummyTorchVisionDataModuleWithChunks
 from renate.benchmark.datasets.vision_datasets import TorchVisionDataModule
 from renate.benchmark.scenarios import (
     BenchmarkScenario,
     ClassIncrementalScenario,
+    FeatureSortingScenario,
+    IIDScenario,
     ImageRotationScenario,
     PermutationScenario,
 )
 from renate.utils.pytorch import randomly_split_data
 
 
 @pytest.mark.parametrize(
@@ -62,14 +63,26 @@
         val_data = scenario.val_data()
         assert len(train_data) == sum([train_data_class_counts[c] for c in class_groupings[i]])
         assert len(val_data) == sum([val_data_class_counts[c] for c in class_groupings[i]])
         for j, test_data in enumerate(scenario.test_data()):
             assert len(test_data) == sum([test_data_class_counts[c] for c in class_groupings[j]])
 
 
+def test_class_incremental_scenario_class_grouping_error():
+    """Classes selected do not exist in data."""
+    scenario = ClassIncrementalScenario(
+        data_module=DummyTorchVisionDataModule(val_size=0.3, seed=42),
+        class_groupings=[[0, 1, 3], [2, 200]],
+        chunk_id=0,
+    )
+    scenario.prepare_data()
+    with pytest.raises(ValueError, match=r"Chunk 1 does not contain classes \[200\]."):
+        scenario.setup()
+
+
 def test_image_rotation_scenario():
     data_module = DummyTorchVisionDataModule(val_size=0.3)
     degrees = [15, 75]
     for i in range(len(degrees)):
         scenario = ImageRotationScenario(
             data_module=data_module,
             degrees=degrees,
@@ -124,16 +137,94 @@
             assert len(test_data) == len(data_module.test_data())
             for k in range(len(test_data)):
                 a, _ = torch.sort(data_module.test_data()[k][0].flatten())
                 b, _ = torch.sort(test_data[k][0].flatten())
                 assert torch.equal(a, b)
 
 
+@pytest.mark.parametrize(
+    "scenario_class, scenario_kwargs",
+    (
+        (ImageRotationScenario, {"degrees": [0, 90, 180, 270]}),
+        (PermutationScenario, {"num_tasks": 4, "input_dim": (1, 5, 5)}),
+    ),
+)
+def test_transforms_in_transform_scenarios_are_distinct(scenario_class, scenario_kwargs):
+    """Tests if transformations are different.
+
+    Checks two cases: 1) transforms must not be same objects and 2) transforms must not perform
+    identical operations.
+    """
+    data_module = DummyTorchVisionDataModule()
+    scenario = scenario_class(data_module=data_module, **scenario_kwargs, chunk_id=0, seed=0)
+    scenario.prepare_data()
+    scenario.setup()
+    x = data_module.X_train[0]
+    for i, transform in enumerate(scenario._transforms):
+        for j, transform2 in enumerate(scenario._transforms):
+            if i == j:
+                continue
+            assert transform != transform2
+            assert not torch.all(torch.isclose(transform(x), transform2(x)))
+
+
 def test_benchmark_scenario():
     data_module = DummyTorchVisionDataModuleWithChunks(num_chunks=3, val_size=0.2)
     for chunk_id in range(3):
         scenario = BenchmarkScenario(data_module=data_module, num_tasks=3, chunk_id=chunk_id)
         scenario.prepare_data()
         scenario.setup()
         assert scenario.train_data() is not None
         assert scenario.val_data() is not None
         assert len(scenario.test_data()) == 3
+
+
+def test_iid_scenario():
+    """Tests that the IID scenario creates a non-overlapping split."""
+    data_module = DummyTorchVisionDataModule(val_size=0.3)
+    counter = {}
+    for i in range(3):
+        scenario = IIDScenario(
+            data_module=data_module,
+            num_tasks=3,
+            chunk_id=i,
+            seed=data_module._seed,
+        )
+        scenario.prepare_data()
+        scenario.setup()
+        for stage in ["train", "val"]:
+            scenario_data = getattr(scenario, f"{stage}_data")()
+            for j in range(len(scenario_data)):
+                x, y = scenario_data[j]
+                assert x not in counter
+                counter[x] = 1
+        assert len(scenario.test_data()) == 3
+
+
+@pytest.mark.parametrize("feature_idx", (0, 1))
+def test_feature_sorting_scenario(feature_idx):
+    """Tests the FeatureSortingScenario.
+
+    Checks for increasing feature values across chunks.
+    """
+    data_module = DummyTorchVisionDataModule(val_size=0.3)
+    num_tasks = 3
+    max_value = {"train": -float("inf"), "val": -float("inf")}
+    for i in range(3):
+        scenario = FeatureSortingScenario(
+            data_module=data_module,
+            num_tasks=num_tasks,
+            feature_idx=feature_idx,
+            randomness=0,
+            chunk_id=i,
+            seed=data_module._seed,
+        )
+        scenario.prepare_data()
+        scenario.setup()
+        for stage in ["train", "val"]:
+            scenario_data = getattr(scenario, f"{stage}_data")()
+            features = [x[0, feature_idx].mean().item() for x, _ in scenario_data]
+            chunk_min = min(features)
+            chunk_max = max(features)
+            assert max_value[stage] <= chunk_min
+            max_value[stage] = chunk_max
+        assert len(scenario.test_data()) == num_tasks
```

### Comparing `Renate-0.1.0/test/renate/data/test_data_module.py` & `Renate-0.2.0/test/renate/data/test_data_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
+import torch
+import transformers
 from torch.utils.data import Dataset, TensorDataset
 
-from renate.benchmark.datasets.nlp_datasets import TorchTextDataModule
+from renate.benchmark.datasets.nlp_datasets import HuggingfaceTextDataModule
 from renate.benchmark.datasets.vision_datasets import (
     CLEARDataModule,
     TinyImageNetDataModule,
     TorchVisionDataModule,
 )
-from renate.data.data_module import CSVDataModule
+from renate.data import CSVDataModule
 
 
 def test_csv_data_module(tmpdir):
     target_name = "y"
 
     # Create toy data
     features = np.random.randint(10, size=(10, 4))
@@ -83,40 +85,14 @@
     assert len(test_data) == num_te
     assert isinstance(test_data, Dataset)
     assert train_data[0][0].size() == test_data[0][0].size() == x_shape
 
 
 @pytest.mark.slow
 @pytest.mark.parametrize(
-    "dataset_name,num_tr,num_te",
-    [
-        ("AG_NEWS", 120000, 7600),
-        ("AmazonReviewFull", 3000000, 650000),
-        ("DBpedia", 560000, 70000),
-    ],
-)
-def test_torchtext_data_module(tmpdir, dataset_name, num_tr, num_te):
-    """Test loading of torchtext data."""
-    val_size = 0.2
-    data_module = TorchTextDataModule(tmpdir, dataset_name=dataset_name, val_size=val_size)
-    data_module.prepare_data()
-    data_module.setup()
-    train_data = data_module.train_data()
-    val_data = data_module.val_data()
-    test_data = data_module.test_data()
-    assert len(train_data) == round(num_tr * (1 - val_size))
-    assert isinstance(train_data, Dataset)
-    assert len(val_data) == round(num_tr * val_size)
-    assert isinstance(val_data, Dataset)
-    assert len(test_data) == num_te
-    assert isinstance(test_data, Dataset)
-
-
-@pytest.mark.slow
-@pytest.mark.parametrize(
     "dataset_name,chunk_id,num_tr,num_te",
     [
         ("CLEAR10", 0, 2986, 500),
         ("CLEAR100", 0, 9945, 4984),
     ],
 )
 def test_clear_data_module(tmpdir, dataset_name, chunk_id, num_tr, num_te):
@@ -152,7 +128,52 @@
     assert len(train_data) == round(num_tr * (1 - val_size))
     assert isinstance(train_data, Dataset)
     assert len(val_data) == round(num_tr * val_size)
     assert isinstance(val_data, Dataset)
     assert len(test_data) == num_te
     assert isinstance(test_data, Dataset)
     assert train_data[0][0].size() == test_data[0][0].size() == (3, 64, 64)
+
+
+@pytest.mark.parametrize(
+    "dataset_name,input_column,target_column",
+    [
+        ("rotten_tomatoes", "text", "label"),
+    ],
+)
+@pytest.mark.parametrize(
+    "tokenizer", [transformers.DistilBertTokenizer.from_pretrained("distilbert-base-uncased")]
+)
+@pytest.mark.parametrize(
+    "tokenizer_kwargs",
+    [
+        None,
+        dict(padding="longest", max_length=512, truncation=True),
+    ],
+)
+def test_huggingface_data_module(
+    tmpdir, dataset_name, input_column, target_column, tokenizer, tokenizer_kwargs
+):
+    data_module = HuggingfaceTextDataModule(
+        data_path=tmpdir,
+        dataset_name=dataset_name,
+        input_column=input_column,
+        target_column=target_column,
+        tokenizer=tokenizer,
+        tokenizer_kwargs=tokenizer_kwargs,
+        val_size=0.2,
+    )
+    data_module.prepare_data()
+    data_module.setup()
+    train_data = data_module.train_data()
+    val_data = data_module.val_data()
+    test_data = data_module.test_data()
+    assert isinstance(train_data, Dataset)
+    assert isinstance(val_data, Dataset)
+    assert isinstance(test_data, Dataset)
+    for dataset in [train_data, val_data, test_data]:
+        inputs, targets = dataset[0]
+        assert isinstance(targets, torch.Tensor)
+        assert isinstance(inputs, dict)
+        assert set(inputs.keys()) == set(["input_ids", "attention_mask"])
+        assert isinstance(inputs["input_ids"], torch.Tensor)
+        assert isinstance(inputs["attention_mask"], torch.Tensor)
```

### Comparing `Renate-0.1.0/test/renate/data/test_datasets.py` & `Renate-0.2.0/test/renate/data/test_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import os
 
 import numpy as np
-from PIL import Image
 import pytest
 import torch
-from torch.utils.data import TensorDataset
 import torchvision.transforms as transforms
+from PIL import Image
+from torch.utils.data import TensorDataset
 
-from renate.data.datasets import ImageDataset, _EnumeratedDataset, _TransformedDataset
+from renate.data import ImageDataset
+from renate.data.datasets import _EnumeratedDataset, _TransformedDataset
 
 
 class MulTransform:
     def __init__(self, factor=3):
         self.factor = factor
 
     def __call__(self, x):
```

### Comparing `Renate-0.1.0/test/renate/evaluation/metrics/test_classification.py` & `Renate-0.2.0/test/renate/evaluation/metrics/test_classification.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/test/renate/evaluation/metrics/test_regression_metrics.py` & `Renate-0.2.0/test/renate/evaluation/metrics/test_regression_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
     NFR_metric = NegativeFlipRateMetric()
 
     with pytest.raises(AssertionError):
         NFR_metric(new_pred, old_pred, gt)
 
 
 def test_regression_metric_corner_case_unmatch_input():
-
     new_pred = torch.tensor([1, 2])
     old_pred = torch.tensor([1])
     gt = torch.tensor([1])
 
     NFR_metric = NegativeFlipRateMetric()
 
     with pytest.raises(AssertionError):
```

### Comparing `Renate-0.1.0/test/renate/memory/test_buffer.py` & `Renate-0.2.0/test/renate/memory/test_buffer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,65 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
+import copy
 import os
 from collections import defaultdict
 
 import pytest
 import torch
 
-from renate.memory import (
+from renate.data.datasets import NestedTensorDataset
+from renate.memory.buffer import (
     GreedyClassBalancingBuffer,
     InfiniteBuffer,
     ReservoirBuffer,
     SlidingWindowBuffer,
 )
 
 
+def nested_tensors_equal(t1, t2):
+    if type(t1) is not type(t2):
+        print("Type mismatch")
+        return False
+    if isinstance(t1, torch.Tensor):
+        return torch.allclose(t1, t2, rtol=1e-3)
+    if isinstance(t1, tuple):
+        if len(t1) != len(t2):
+            print("Tuple length mismatch")
+            return False
+        return all(nested_tensors_equal(t1_, t2_) for t1_, t2_ in zip(t1, t2))
+    if isinstance(t1, dict):
+        if set(t1.keys()) != set(t2.keys()):
+            print("Dict key mismatch")
+            return False
+        return all(nested_tensors_equal(t1[key], t2[key]) for key in t1.keys())
+
+
 @pytest.mark.parametrize("buffer_cls", [ReservoirBuffer, SlidingWindowBuffer])
 @pytest.mark.parametrize("max_size", [1, 10, 100])
-@pytest.mark.parametrize("num_batches", [1, 10])
-@pytest.mark.parametrize("batch_size", [1, 10, 20])
-def test_buffer_respects_max_size(buffer_cls, max_size, num_batches, batch_size):
+@pytest.mark.parametrize("num_updates", [1, 10])
+@pytest.mark.parametrize(
+    "dataset",
+    [
+        torch.utils.data.TensorDataset(torch.randn(10, 2)),
+        torch.utils.data.TensorDataset(torch.randn(100, 2)),
+        torch.utils.data.TensorDataset(torch.randn(10, 2), torch.arange(10)),
+        torch.utils.data.TensorDataset(torch.randn(100, 2), torch.arange(100)),
+        NestedTensorDataset({"X": torch.randn(10, 2), "y": torch.arange(10)}),
+        NestedTensorDataset({"X": torch.randn(100, 2), "y": torch.arange(100)}),
+        NestedTensorDataset(({"X": torch.randn(10, 2), "z": torch.randn(10)}, torch.arange(10))),
+        NestedTensorDataset(({"X": torch.randn(100, 2), "z": torch.randn(100)}, torch.arange(100))),
+    ],
+)
+def test_buffer_respects_max_size(buffer_cls, max_size, num_updates, dataset):
     buffer = buffer_cls(max_size)
     assert len(buffer) == 0
-    for i in range(num_batches):
-        ds = torch.utils.data.TensorDataset(torch.randn(batch_size))
-        buffer.update(ds)
-        assert len(buffer) == min((i + 1) * batch_size, max_size)
+    for i in range(num_updates):
+        buffer.update(dataset)
+        assert len(buffer) == min((i + 1) * len(dataset), max_size)
 
 
 @pytest.mark.parametrize("buffer", [ReservoirBuffer(30), SlidingWindowBuffer(30)])
 def test_batching_with_metadata(buffer):
     X = torch.randn(100, 3)
     y = torch.randint(0, 10, size=(100,))
     ds = torch.utils.data.TensorDataset(X, y)
@@ -41,87 +72,98 @@
         assert isinstance(metadata_batch, dict)
         assert "foo" in metadata_batch
         assert isinstance(metadata_batch["foo"], torch.Tensor)
         assert torch.all(metadata_batch["foo"] == 1.0)
 
 
 @pytest.mark.parametrize("buffer", [ReservoirBuffer(30), SlidingWindowBuffer(30)])
-def test_get_metadata(buffer):
+def test_get_and_set_metadata(buffer):
     X = torch.randn(100, 3)
     y = torch.randint(0, 10, size=(100,))
     ds = torch.utils.data.TensorDataset(X, y)
     metadata = {"foo": torch.ones(100)}
     buffer.update(ds, metadata)
 
-    metadata_ = buffer.metadata
-    assert isinstance(metadata_, dict)
-    assert "foo" in metadata_
-    assert isinstance(metadata_["foo"], torch.Tensor)
-    assert len(metadata_["foo"]) == len(buffer)
-    assert torch.all(metadata_["foo"] == 1.0)
+    foo_values = buffer.get_metadata("foo")
+    assert isinstance(foo_values, torch.Tensor)
+    assert foo_values.size() == (len(buffer),)
+    assert torch.all(foo_values == 1.0)
+
+    buffer.set_metadata("foo", 2 * torch.ones(len(buffer)))
+    foo_values = buffer.get_metadata("foo")
+    assert isinstance(foo_values, torch.Tensor)
+    assert foo_values.size() == (len(buffer),)
+    assert torch.all(foo_values == 2.0)
 
 
 @pytest.mark.parametrize("buffer", [ReservoirBuffer(30), SlidingWindowBuffer(30)])
 def test_getitem_returns_points_and_metadata(buffer):
     X = torch.randn(100, 3)
     y = torch.randint(0, 10, size=(100,))
     ds = torch.utils.data.TensorDataset(X, y)
     metadata = {"foo": torch.ones(100)}
     buffer.update(ds, metadata)
 
-    for idx in [0, 1, 10, 29, -1, -2, -30]:
+    for idx in [0, 1, 10, 29]:
         datapoint, metadata = buffer[idx]
         assert isinstance(metadata, dict) and ("foo" in metadata)
         assert metadata["foo"] == 1.0
         assert isinstance(datapoint, tuple) and len(datapoint) == 2
         assert datapoint[0].size() == (3,)
         assert datapoint[1].size() == ()
 
     for idx in [30, 31, 50]:
         with pytest.raises(IndexError):
             datapoint[idx]
 
 
 def test_reservoir_is_uniform():
-    # Present buffer with numbers from 1-10k. It should subsample uniformly,
-    # resulting in a mean of 5k with a standard deviation of ~91.
+    """Present buffer with numbers from 1-10k. It should subsample uniformly, resulting in a mean of
+    5k with a standard deviation of ~91.
+    """
     buffer = ReservoirBuffer(max_size=1000)
     for i in range(10):
         x = torch.arange(i * 1000, (i + 1) * 1000, dtype=torch.float) + 1
         ds = torch.utils.data.TensorDataset(x)
         buffer.update(ds)
     xs = torch.stack([buffer[i][0][0] for i in range(len(buffer))], dim=0)
     assert 5000 - 5 * 91 < xs.mean() < 5000 + 5 * 91
 
 
-def test_greedy_is_balanced():
-    # Present buffer with 10 classes with respect to 10000 samples, where each class has 1000 samples.
-    # When inspecting the ._class_counts attribute, it should be uniform.
+def test_greedy_is_balanced(tmpdir):
+    """Present buffer with 10 classes with respect to 10000 samples, where each class has 1000
+    samples. When inspecting the ._class_counts attribute, it should be uniform.
+    """
     buffer = GreedyClassBalancingBuffer(max_size=100)
     X = torch.ones(10000, 1)
     Y = torch.ones(10000, 1, dtype=torch.long)
     for i in range(10):
         Y[i * 1000 : (i + 1) * 1000] = i
     # Randomise the Y such that the classes are not presented in a sequence
     Y = Y[torch.randperm(10000)]
     # Split the data into 10 chunks and perform 10 updates
     for i in range(10):
         ds = torch.utils.data.TensorDataset(
             X[i * 1000 : (i + 1) * 1000], Y[i * 1000 : (i + 1) * 1000]
         )
         buffer.update(ds)
-    counts = torch.tensor(
-        [len(v) for v in buffer._class_to_index_map.values()], dtype=torch.float32
-    )
+        buffer.save(tmpdir)
+        state_dict = buffer.state_dict()
+        del buffer
+        buffer = GreedyClassBalancingBuffer(max_size=100)
+        buffer.load_state_dict(state_dict)
+        buffer.load(tmpdir)
+    counts = torch.tensor([len(v) for v in buffer._indices_by_class.values()], dtype=torch.float32)
     label_counts = defaultdict(int)
-    assert 10 - 1 < counts.mean() < 10 + 1
+    assert torch.all(counts >= 10 - 1)
+    assert torch.all(counts <= 10 + 1)
     for i in range(len(buffer)):
         (_, y), _ = buffer[i]
         label_counts[y.item()] += 1
-    buffer_class_counts = {k: len(v) for k, v in buffer._class_to_index_map.items()}
+    buffer_class_counts = {k: len(v) for k, v in buffer._indices_by_class.items()}
     assert buffer_class_counts == label_counts
 
 
 @pytest.mark.parametrize("max_size", [1, 10, 100])
 @pytest.mark.parametrize("num_batches", [1, 10])
 @pytest.mark.parametrize("batch_size", [1, 10, 20])
 def test_sliding_window_keeps_most_recent(max_size, num_batches, batch_size):
@@ -130,68 +172,14 @@
         ds = torch.utils.data.TensorDataset(torch.arange(i * batch_size, (i + 1) * batch_size))
         buffer.update(ds)
     xs = torch.stack([buffer[i][0][0] for i in range(len(buffer))], dim=0)
     assert xs.max() == num_batches * batch_size - 1
     assert xs.min() == max(num_batches * batch_size - max_size, 0)
 
 
-@pytest.mark.parametrize("max_size", [1, 10, 100])
-def test_buffer_get_state_dict(max_size):
-    buffer = ReservoirBuffer(max_size=max_size)
-    for i in range(20):
-        ds = torch.utils.data.TensorDataset(torch.arange(i * 10, (i + 1) * 10))
-        metadata = {"x": torch.ones(10, 10)}
-        buffer.update(ds, metadata)
-    state_dict = buffer.state_dict()
-    for key, value in state_dict["data_points"].items():
-        assert torch.all(torch.eq(buffer._data_points[key], value))
-
-    assert torch.all(torch.eq(buffer.metadata["x"], state_dict["metadata"]["x"]))
-
-    for key in ["max_size", "storage_mode", "seed", "count", "data_points"]:
-        assert getattr(buffer, "_" + key) == state_dict[key]
-    assert buffer.metadata == state_dict["metadata"]
-    assert state_dict["size"] == max_size
-    assert len(state_dict["data_points"]["0"]) == max_size
-
-
-@pytest.mark.parametrize("buffer_type", [ReservoirBuffer, SlidingWindowBuffer])
-def test_buffer_load_state_dict(buffer_type):
-    buffer = buffer_type(max_size=100)
-
-    state_dict = {
-        "buffer_class_name": buffer_type.__name__,
-        "max_size": 100,
-        "seed": 1,
-        "count": 100,
-        "size": 100,
-        "data_points": {},
-        "metadata": {},
-        "storage_mode": "in_memory",
-    }
-    for i in range(100):
-        x = torch.ones((5,))
-        state_dict["data_points"]["0"] = (
-            x.unsqueeze(0)
-            if i == 0
-            else torch.cat((state_dict["data_points"]["0"], x.unsqueeze(0)), dim=0)
-        )
-    state_dict["metadata"] = {"x": torch.ones(100, 5)}
-
-    buffer.load_state_dict(state_dict)
-    for key, value in state_dict["data_points"].items():
-        assert torch.all(torch.eq(buffer._data_points[key], value))
-
-    assert torch.all(torch.eq(buffer.metadata["x"], state_dict["metadata"]["x"]))
-
-    for key in ["max_size", "storage_mode", "seed", "count", "data_points", "size"]:
-        if not isinstance(getattr(buffer, "_" + key), list):
-            assert getattr(buffer, "_" + key) == state_dict[key]
-
-
 @pytest.mark.parametrize(
     "state_dict",
     [
         {
             "max_size": None,
             "storage_mode": "in_memory",
             "seed": 23,
@@ -253,15 +241,15 @@
     buffer = InfiniteBuffer()
     for i in range(5):
         sample_dataset = torch.utils.data.TensorDataset(torch.ones((10, 3)) * i)
         buffer.update(sample_dataset)
 
     for i in range(5):
         for j in range(10):
-            assert torch.all(torch.eq(buffer[j + i * 10][0][0], torch.ones((3)) * i))
+            assert torch.all(torch.eq(buffer[i * 10 + j][0][0], torch.ones((3)) * i))
 
 
 @pytest.mark.parametrize("max_size", [1, 10, 100])
 @pytest.mark.parametrize("buffer_cls", [ReservoirBuffer, SlidingWindowBuffer])
 def test_buffer_same_size_on_disk_after_updates(tmpdir, max_size, buffer_cls):
     """Test that the buffer size on disk is the same after consequtive updates
     given that the max_size is reached."""
@@ -279,7 +267,79 @@
         buffer.update(ds)
 
     torch.save(buffer.state_dict(), os.path.join(tmpdir, "buffer.pt"))
     if not isinstance(buffer, InfiniteBuffer):
         assert disk_size == os.path.getsize(os.path.join(tmpdir, "buffer.pt"))
     else:
         assert disk_size < os.path.getsize(os.path.join(tmpdir, "buffer.pt"))
+
+
+@pytest.mark.parametrize("buffer_cls", [ReservoirBuffer, SlidingWindowBuffer])
+@pytest.mark.parametrize("max_size", [10, 100])
+@pytest.mark.parametrize("num_updates", [0, 1, 2])
+@pytest.mark.parametrize(
+    "dataset",
+    [
+        torch.utils.data.TensorDataset(torch.randn(10, 2)),
+        torch.utils.data.TensorDataset(torch.randn(10, 2), torch.arange(10)),
+        NestedTensorDataset({"X": torch.randn(10, 2), "y": torch.arange(10)}),
+        NestedTensorDataset(({"X": torch.randn(10, 2), "z": torch.randn(10)}, torch.arange(10))),
+    ],
+)
+@pytest.mark.parametrize("metadata", [None, {"a": torch.arange(10), "b": torch.zeros(10, 2)}])
+def test_load_and_save_buffer(tmpdir, buffer_cls, max_size, num_updates, dataset, metadata):
+    """Tests loading an saving of the buffer state."""
+    buffer = buffer_cls(max_size)
+    for _ in range(2):
+        for _ in range(num_updates):
+            buffer.update(dataset, metadata)
+        elements_before = [copy.deepcopy(buffer[i]) for i in range(len(buffer))]
+        buffer.save(tmpdir)
+        state_dict = buffer.state_dict()
+        del buffer
+        buffer = buffer_cls(max_size)
+        buffer.load_state_dict(state_dict)
+        buffer.load(tmpdir)
+        for j in range(len(buffer)):
+            assert nested_tensors_equal(buffer[j], elements_before[j])
+
+
+@pytest.mark.parametrize("buffer_cls", [ReservoirBuffer, SlidingWindowBuffer])
+@pytest.mark.parametrize("max_size", [10, 100])
+@pytest.mark.parametrize("num_updates", [0, 1, 2])
+@pytest.mark.parametrize(
+    "dataset",
+    [
+        torch.utils.data.TensorDataset(torch.randn(10, 2), torch.arange(10)),
+    ],
+)
+@pytest.mark.parametrize("metadata", [None, {"a": torch.arange(10), "b": torch.zeros(10, 2)}])
+@pytest.mark.parametrize("buffer_transform", [None, lambda x: x * 2])
+@pytest.mark.parametrize("buffer_target_transform", [None, lambda y: y // 5])
+def test_load_and_save_buffer_with_transforms(
+    tmpdir,
+    buffer_cls,
+    max_size,
+    num_updates,
+    dataset,
+    metadata,
+    buffer_transform,
+    buffer_target_transform,
+):
+    """Tests loading an saving of the buffer state."""
+    buffer = buffer_cls(
+        max_size, transform=buffer_transform, target_transform=buffer_target_transform
+    )
+    for _ in range(2):
+        for _ in range(num_updates):
+            buffer.update(dataset, metadata)
+        elements_before = [copy.deepcopy(buffer[i]) for i in range(len(buffer))]
+        buffer.save(tmpdir)
+        state_dict = buffer.state_dict()
+        del buffer
+        buffer = buffer_cls(
+            max_size, transform=buffer_transform, target_transform=buffer_target_transform
+        )
+        buffer.load_state_dict(state_dict)
+        buffer.load(tmpdir)
+        for j in range(len(buffer)):
+            assert nested_tensors_equal(buffer[j], elements_before[j])
```

### Comparing `Renate-0.1.0/test/renate/models/test_renate_module.py` & `Renate-0.2.0/test/renate/models/test_renate_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import pytest
 import torch
 
 from renate.benchmark.models.mlp import MultiLayerPerceptron
 from renate.benchmark.models.resnet import ResNet
 from renate.benchmark.models.vision_transformer import VisionTransformer
 from renate.defaults import TASK_ID
-from renate.models.renate_module import RenateModule, RenateWrapper
+from renate.models import RenateModule
+from renate.models.renate_module import RenateWrapper
 
 
 def test_failing_to_init_abs_class():
     with pytest.raises(TypeError):
         RenateModule({"toy_hyperparam": 1.0}, torch.nn.CrossEntropyLoss())
```

### Comparing `Renate-0.1.0/test/renate/renate_config_files/config.py` & `Renate-0.2.0/test/renate/renate_config_files/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from pathlib import Path
-from typing import Optional, Union
+from typing import Optional, Tuple
 
 import torch
 
-from datasets import DummyTorchVisionDataModule
+from dummy_datasets import DummyTorchVisionDataModule
 from renate.benchmark.models.mlp import MultiLayerPerceptron
 from renate.benchmark.scenarios import ClassIncrementalScenario
 from renate.data.data_module import RenateDataModule
 from renate.models import RenateModule
 
 
-def model_fn(model_state_url: Optional[Union[Path, str]] = None) -> RenateModule:
+def model_fn(model_state_url: Optional[str] = None) -> RenateModule:
     if model_state_url is None:
         return MultiLayerPerceptron(5 * 5, 10, 0, 64)
-    state_dict = torch.load(str(model_state_url))
+    state_dict = torch.load(model_state_url)
     return MultiLayerPerceptron.from_state_dict(state_dict)
 
 
 def data_module_fn(
-    data_path: Union[Path, str],
+    data_path: str,
     chunk_id: Optional[int] = None,
-    data_module_fn_val_size: str = "0.0",
+    val_size: float = 0.0,
     seed: int = 0,
-    data_module_fn_use_scenario: str = "False",
+    use_scenario: bool = False,
+    class_groupings: Tuple[Tuple[int]] = ((0, 1), (2, 3, 4)),
+    optional_tuple: Optional[Tuple[float]] = None,
+    optional_float: Optional[float] = None,
+    list_param: list = [1, 2],
 ) -> RenateDataModule:
-    data_module = DummyTorchVisionDataModule(
-        transform=None, val_size=float(data_module_fn_val_size), seed=seed
-    )
-    if data_module_fn_use_scenario == "True":
+    data_module = DummyTorchVisionDataModule(transform=None, val_size=val_size, seed=seed)
+    if use_scenario:
         return ClassIncrementalScenario(
             data_module=data_module,
             chunk_id=chunk_id,
-            class_groupings=[[0, 1], [2, 3, 4]],
+            class_groupings=class_groupings,
         )
     return data_module
```

### Comparing `Renate-0.1.0/test/renate/tuning/test_tuning.py` & `Renate-0.2.0/test/renate/training/test_run_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,67 +7,70 @@
 import pytest
 from syne_tune.config_space import loguniform, uniform
 from syne_tune.optimizer.baselines import ASHA
 from syne_tune.optimizer.schedulers import FIFOScheduler
 from syne_tune.optimizer.schedulers.transfer_learning import RUSHScheduler
 
 from renate import defaults
-from renate.tuning.tuning import (
+from renate.training.training import (
     RENATE_CONFIG_COLUMNS,
     _create_scheduler,
     _get_transfer_learning_task_evaluations,
     _load_tuning_history,
     _merge_tuning_history,
     _verify_validation_set_for_hpo_and_checkpointing,
-    execute_tuning_job,
+    run_training_job,
 )
 from renate.utils.syne_tune import is_syne_tune_config_space
 
 config_file = str(Path(__file__).parent.parent / "renate_config_files" / "config.py")
 
 
 @pytest.mark.parametrize(
     "num_chunks, val_size, raises, fixed_search_space, scheduler",
     [
         (2, 0.9, False, False, "rush"),
         (1, 0.0, True, False, "rush"),
-        (1, 0.9, False, True, None),
-        (1, 0.0, False, True, None),
+        (2, 0.9, False, True, None),
+        (2, 0.0, False, True, None),
     ],
     ids=[
         "transfer-hpo-with-val",
         "transfer-hpo-without-val-raises-exception",
         "training-single-config-with-val",
         "training-single-config-without-val",
     ],
 )
-def test_execute_tuning_job(tmpdir, num_chunks, val_size, raises, fixed_search_space, scheduler):
+@pytest.mark.parametrize("updater", ("ER", "Avalanche-iCaRL"))
+def test_run_training_job(
+    tmpdir, num_chunks, val_size, raises, fixed_search_space, scheduler, updater
+):
     """Simply running tuning job to check if anything fails.
 
     Case 1: Standard HPO setup with transfer learning in second step.
     Case 2: HPO without validation set fails.
     Case 3: Training of single configuration with validation set.
     Case 4: Training of single configuration without validation set.
     """
     state_url = None
     tmpdir = str(tmpdir)
     for _ in range(num_chunks):
 
         def execute_job():
-            execute_tuning_job(
-                updater="ER",
+            run_training_job(
+                updater=updater,
                 max_epochs=5,
                 config_file=config_file,
-                state_url=state_url,
-                next_state_url=tmpdir,
+                input_state_url=state_url,
+                output_state_url=tmpdir,
                 backend="local",
                 mode="max",
                 config_space={
                     "learning_rate": 0.1 if fixed_search_space else loguniform(10e-5, 0.1),
-                    "data_module_fn_val_size": val_size,
+                    "val_size": val_size,
                 },
                 metric="val_accuracy",
                 max_time=15,
                 scheduler=scheduler,
             )
 
         if raises:
@@ -91,15 +94,15 @@
         ),
         (None, [[0.002, 0.8, 0.02]], [0, 0.002, 0.8, 0.02], None),
     ],
 )
 def test_merge_tuning_history(
     data_old, data_new, expected_data_first_row, expected_data_second_row
 ):
-    """Test whether HPO tuning results are merged correctly.
+    """Test whether HPO results are merged correctly.
 
     Testing two cases:
         1. Old results exist and new ones are added.
         2. No old results exist.
     """
     results_old = None
     if data_old is not None:
@@ -120,19 +123,20 @@
 
 
 @pytest.mark.parametrize("val_size", [0.9, 0.0])
 @pytest.mark.parametrize("tune_hyperparameters", [True, False])
 def test_verify_validation_set_for_hpo_and_checkpointing(tmpdir, val_size, tune_hyperparameters):
     """Check if misconfigurations are spotted and config_space is updated correctly.
 
-    If tune_hyperparameters is `True` (hyperparameter optimization is enabled), a validation set must exist.
-    If a validation set exists, the `config_space` must be changed such that the right metric and mode for checkpointing
-    and hyperparameter optimization is used.
+    If tune_hyperparameters is `True` (hyperparameter optimization is enabled), a validation set
+    must exist.
+    If a validation set exists, the `config_space` must be changed such that the right metric and
+    mode for checkpointing and hyperparameter optimization is used.
     """
-    config_space = {"data_module_fn_val_size": val_size}
+    config_space = {"val_size": val_size}
     expected_metric = "val_accuracy"
     expected_mode: defaults.SUPPORTED_TUNING_MODE_TYPE = "max"
 
     def verify_validation_set():
         return _verify_validation_set_for_hpo_and_checkpointing(
             config_space=config_space,
             config_file=config_file,
@@ -156,15 +160,17 @@
             assert mode == expected_mode
         else:
             assert metric == "train_loss"
             assert mode == "min"
 
 
 def test_is_syne_tune_config_space():
-    """Function should return True if any entry in the `config_space` is a Syne Tune search space."""
+    """Function should return True if any entry in the `config_space` is a Syne Tune search
+    space.
+    """
     assert is_syne_tune_config_space({"a": uniform(0, 1), "b": 1})
     assert not is_syne_tune_config_space({"a": 0.5, "b": 1})
 
 
 def _get_transfer_learning_task_evaluations_input():
     """Helper function which returns the input required for the unit tests below."""
     hyperparameter_names = ["config_lr"]
@@ -195,16 +201,17 @@
         "max_epochs": 3,
     }
 
 
 def test_get_transfer_learning_task_evaluations():
     """Case that should successfully return a result.
 
-    Function must drop duplicate hyperparameters, rows where metric or hyperparameter are missing. Only the relevant
-    metric is kept. Renate configurations are replaced with the current ones (e.g. working space).
+    Function must drop duplicate hyperparameters, rows where metric or hyperparameter are missing.
+    Only the relevant metric is kept. Renate configurations are replaced with the current ones
+    (e.g. working space).
     """
     input_dict = _get_transfer_learning_task_evaluations_input()
     expected_objectives_evaluations = np.array(
         [
             [[[0.33], [0.23], [np.nan]]],
             [[[0.23], [0.13], [0.03]]],
             [[[0.5], [np.nan], [np.nan]]],
@@ -296,18 +303,20 @@
             "config_momentum",
         ],
     )
 
 
 @pytest.mark.parametrize("hyperparameter, num_task_evaluations", [("lr", 2), ("momentum", 1)])
 def test_load_tuning_history(tmpdir, hyperparameter, num_task_evaluations):
-    """Check if tuning results can be successfully converted to a list of TransferLearningTaskEvaluations.
+    """Check if tuning results can be successfully converted to a list of
+    TransferLearningTaskEvaluations.
 
     Case 1: Evaluations for hyperparameter `lr` is available for both updates. Return both.
-    Case 2: Evaluations for hyperparameter `momentum` is only available for the second update. Drop first data.
+    Case 2: Evaluations for hyperparameter `momentum` is only available for the second update.
+        Drop first data.
     """
     tuning_results = _get_tuning_results()
     config_space = {hyperparameter: uniform(0.001, 1)}
     tuning_results.to_csv(defaults.hpo_file(tmpdir), index=False)
     task_evaluations = _load_tuning_history(tmpdir, config_space, "val_loss")
     assert len(task_evaluations) == num_task_evaluations
     assert None not in task_evaluations.values()
@@ -333,16 +342,16 @@
 @pytest.mark.parametrize(
     "scheduler,scheduler_kwargs",
     [
         ("random", None),
         ("asha", None),
         ("rush", None),
         (FIFOScheduler, None),
-        (ASHA, {"max_t": 3, "resource_attr": "epoch"}),
-        (RUSHScheduler, {"max_t": 3, "resource_attr": "epoch"}),
+        (ASHA, {"max_resource_attr": "max_epochs", "resource_attr": "epoch"}),
+        (RUSHScheduler, {"max_resource_attr": "max_epochs", "resource_attr": "epoch"}),
     ],
     ids=["str_random", "str_asha", "str_rush", "class_random", "class_asha", "class_rush"],
 )
 def test_create_scheduler(tmpdir, scheduler, scheduler_kwargs, tuning_results_exist):
     """Test various ways of creating a scheduler with and without previous tuning results.
 
     Cases:
@@ -353,15 +362,14 @@
     tuning_results = _get_tuning_results()
     state_url = None
     if tuning_results_exist:
         state_url = tmpdir
         tuning_results.to_csv(defaults.hpo_file(state_url), index=False)
     _create_scheduler(
         scheduler=scheduler,
-        config_space={"lr": 0.01},
+        config_space={"lr": 0.01, "max_epochs": 3},
         metric="val_loss",
         mode="min",
-        max_epochs=3,
         seed=0,
         scheduler_kwargs=scheduler_kwargs,
-        state_url=state_url,
+        input_state_url=state_url,
     )
```

### Comparing `Renate-0.1.0/test/renate/updaters/experimental/test_er.py` & `Renate-0.2.0/test/renate/updaters/experimental/test_er.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import os
 
 import pytest
 import torch
-from torch.utils.data import TensorDataset
 
 from renate import defaults
-from renate.data.datasets import _EnumeratedDataset, _TransformedDataset
 from renate.updaters.experimental.er import (
     CLSExperienceReplayLearner,
     DarkExperienceReplayLearner,
     ExperienceReplayLearner,
     PooledOutputDistillationExperienceReplayLearner,
     SuperExperienceReplayLearner,
 )
@@ -59,39 +57,38 @@
         hidden_size=32,
         num_hidden_layers=3,
         train_num_samples=10,
         test_num_samples=5,
     )
     datasets_val = []
     state_folder = None
-    next_state_folder = defaults.current_state_folder(tmpdir)
+    next_state_folder = defaults.input_state_folder(tmpdir)
     for i in range(3):
         dataset_val = torch.utils.data.TensorDataset(
             torch.rand((100, 10)),
             torch.randint(10, (100,)),
         )
         model_updater = pytest.helpers.get_simple_updater(
-            model, current_state_folder=state_folder, next_state_folder=next_state_folder
+            model, input_state_folder=state_folder, output_state_folder=next_state_folder
         )
         model_updater.update(
             train_dataset=dataset_train, val_dataset=dataset_val, task_id=defaults.TASK_ID
         )
         datasets_val.append(dataset_val)
         state_folder = next_state_folder
 
     model_updater = pytest.helpers.get_simple_updater(
-        model, current_state_folder=state_folder, next_state_folder=next_state_folder
+        model, input_state_folder=state_folder, output_state_folder=next_state_folder
     )
     for i in range(3):
         for j in range(100):
-            assert torch.all(
-                torch.eq(
-                    datasets_val[i][j][0],
-                    model_updater._learner._val_memory_buffer[i * 100 + j][0][0],
-                )
+            assert torch.allclose(
+                datasets_val[i][j][0],
+                model_updater._learner._val_memory_buffer[i * 100 + j][0][0],
+                rtol=1e-3,
             )
 
 
 @pytest.mark.parametrize(
     "cls,kwargs",
     [
         [ExperienceReplayLearner, {"alpha": 0.2, "memory_size": 10, "memory_batch_size": 10}],
```

### Comparing `Renate-0.1.0/test/renate/updaters/experimental/test_joint.py` & `Renate-0.2.0/test/renate/updaters/experimental/test_joint.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/test/renate/updaters/experimental/test_repeated_distill.py` & `Renate-0.2.0/test/renate/updaters/experimental/test_repeated_distill.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         train_num_samples=10,
         test_num_samples=5,
     )
     model_updater = RepeatedDistillationModelUpdater(
         model,
         memory_size=50,
         max_epochs=1,
-        next_state_folder=defaults.next_state_folder(tmpdir) if provide_folder else None,
+        output_state_folder=defaults.output_state_folder(tmpdir) if provide_folder else None,
     )
     y_hat_before_train = model(test_data, task_id=defaults.TASK_ID)
     model_updater.update(train_dataset, task_id=defaults.TASK_ID)
     y_hat_after_train = model(test_data, task_id=defaults.TASK_ID)
     assert y_hat_before_train.shape[0] == y_hat_after_train.shape[0]
     assert not torch.allclose(y_hat_before_train, y_hat_after_train)
 
@@ -93,21 +93,21 @@
         num_inputs=10,
         num_outputs=10,
         hidden_size=32,
         num_hidden_layers=3,
         train_num_samples=10,
         test_num_samples=5,
     )
-    state_url = defaults.current_state_folder(tmpdir)
+    state_url = defaults.input_state_folder(tmpdir)
     model_updater = RepeatedDistillationModelUpdater(
-        model, memory_size=50, max_epochs=1, next_state_folder=state_url
+        model, memory_size=50, max_epochs=1, output_state_folder=state_url
     )
     model = model_updater.update(train_dataset, task_id=defaults.TASK_ID)
     model_updater = RepeatedDistillationModelUpdater(
-        model, memory_size=50, max_epochs=1, current_state_folder=state_url
+        model, memory_size=50, max_epochs=1, input_state_folder=state_url
     )
     model_updater.update(train_dataset, task_id=defaults.TASK_ID)
 
 
 def test_dmc_loss():
     a = torch.ones(10, 3)
     b = torch.zeros(10, 3)
```

### Comparing `Renate-0.1.0/test/renate/updaters/test_learner.py` & `Renate-0.2.0/test/renate/updaters/test_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 from renate.models import RenateModule
 from renate.updaters.learner import Learner, ReplayLearner
 
 
 def get_model_and_learner_and_learner_kwargs(
     learner_class: Type[Learner],
-) -> Tuple[RenateModule, Dict[str, Any]]:
+) -> Tuple[RenateModule, Learner, Dict[str, Any]]:
     learner_kwargs = LEARNER_KWARGS[learner_class]
     model = pytest.helpers.get_renate_module_mlp(
         num_inputs=1, num_outputs=1, hidden_size=1, num_hidden_layers=1
     )
     learner = learner_class(model=model, **learner_kwargs)
     return model, learner, learner_kwargs
```

### Comparing `Renate-0.1.0/test/renate/updaters/test_model_updater.py` & `Renate-0.2.0/test/renate/updaters/test_model_updater.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import warnings
+from copy import deepcopy
 
 import pytest
 import torch
 from torchvision.transforms import Lambda
 
 from conftest import LEARNERS_USING_SIMPLE_UPDATER, LEARNER_KWARGS, check_learner_transforms
 from renate import defaults
@@ -19,23 +20,56 @@
         num_outputs=10,
         hidden_size=32,
         num_hidden_layers=3,
         train_num_samples=10,
         test_num_samples=5,
     )
     model_updater = pytest.helpers.get_simple_updater(
-        model, next_state_folder=defaults.next_state_folder(tmpdir) if provide_folder else None
+        model, output_state_folder=defaults.output_state_folder(tmpdir) if provide_folder else None
     )
     y_hat_before_train = model(test_data, task_id=defaults.TASK_ID)
-    model_updater.update(train_dataset, task_id=defaults.TASK_ID)
+    model = model_updater.update(train_dataset, task_id=defaults.TASK_ID)
     y_hat_after_train = model(test_data, task_id=defaults.TASK_ID)
     assert y_hat_before_train.shape[0] == y_hat_after_train.shape[0]
     assert not torch.allclose(y_hat_before_train, y_hat_after_train)
 
 
+def test_deterministic_updater():
+    # The behavior is always deterministic on CPU but it can become non-deterministic on GPU
+    # When run on CPU this test never fails so it is only useful when tests are run on GPU
+    model1, train_dataset, test_data = pytest.helpers.get_renate_module_mlp_and_data(
+        num_inputs=10,
+        num_outputs=10,
+        hidden_size=32,
+        num_hidden_layers=3,
+        train_num_samples=10,
+        test_num_samples=5,
+    )
+
+    model2 = deepcopy(model1)
+
+    model_updater1 = pytest.helpers.get_simple_updater(
+        model1,
+        deterministic_trainer=True,
+    )
+
+    model_updater2 = pytest.helpers.get_simple_updater(
+        model2,
+        deterministic_trainer=True,
+    )
+
+    model1 = model_updater1.update(train_dataset, task_id=defaults.TASK_ID)
+    model2 = model_updater2.update(train_dataset, task_id=defaults.TASK_ID)
+
+    y_hat_1 = model1(test_data, task_id=defaults.TASK_ID)
+    y_hat_2 = model2(test_data, task_id=defaults.TASK_ID)
+
+    assert torch.allclose(y_hat_1, y_hat_2)
+
+
 @pytest.mark.parametrize("early_stopping_enabled", [True, False])
 @pytest.mark.parametrize("use_val", [True, False])
 @pytest.mark.parametrize("metric_monitored", [None, "val_accuracy"])
 @pytest.mark.parametrize("updater_type", ["DMC", "SimpleUpdater"])
 def test_model_updater_with_early_stopping(
     use_val, early_stopping_enabled, metric_monitored, updater_type
 ):
@@ -70,15 +104,14 @@
     assert model_updater._num_epochs_trained == 0
     with warnings.catch_warnings(record=True) as warning_update:
         model_updater.update(
             train_dataset, val_dataset=val_dataset if use_val else None, task_id=defaults.TASK_ID
         )
 
     if metric_monitored and use_val and early_stopping_enabled:
-        print(model_updater._num_epochs_trained)
         assert model_updater._num_epochs_trained < max_epochs
     else:
         assert model_updater._num_epochs_trained == max_epochs
 
     is_warning_metric_missing_sent = any(
         [
             str(w.message).startswith("Early stopping is enabled but no metric is specified")
@@ -108,28 +141,28 @@
         num_inputs=10,
         num_outputs=10,
         hidden_size=32,
         num_hidden_layers=1,
         train_num_samples=10,
         test_num_samples=5,
     )
-    state_url = defaults.current_state_folder(tmpdir)
+    state_url = defaults.input_state_folder(tmpdir)
     model_updater = pytest.helpers.get_simple_updater(
         model,
         learner_class=learner_class,
         learner_kwargs=LEARNER_KWARGS[learner_class],
-        next_state_folder=state_url,
+        output_state_folder=state_url,
         max_epochs=2,
     )
     model = model_updater.update(train_dataset, task_id=defaults.TASK_ID)
     model_updater = pytest.helpers.get_simple_updater(
         model,
         learner_class=learner_class,
         learner_kwargs=LEARNER_KWARGS[learner_class],
-        current_state_folder=state_url,
+        input_state_folder=state_url,
         max_epochs=2,
     )
     model_updater.update(train_dataset, task_id=defaults.TASK_ID)
 
 
 @pytest.mark.parametrize("learner_class", LEARNERS_USING_SIMPLE_UPDATER)
 def test_transforms_passed_to_simple_model_updater_will_be_used_by_learner(tmpdir, learner_class):
@@ -147,30 +180,30 @@
         num_inputs=10,
         num_outputs=10,
         hidden_size=32,
         num_hidden_layers=3,
         train_num_samples=10,
         test_num_samples=5,
     )
-    state_url = defaults.current_state_folder(tmpdir)
+    state_url = defaults.input_state_folder(tmpdir)
     transforms_kwargs = {
         "train_transform": identity_transform(),
         "train_target_transform": identity_transform(),
         "test_transform": identity_transform(),
         "test_target_transform": identity_transform(),
     }
     if issubclass(learner_class, ReplayLearner):
         transforms_kwargs["buffer_transform"] = identity_transform()
         transforms_kwargs["buffer_target_transform"] = identity_transform()
     model_updater = pytest.helpers.get_simple_updater(
         model,
-        next_state_folder=state_url,
+        output_state_folder=state_url,
         learner_kwargs=LEARNER_KWARGS[learner_class],
         learner_class=learner_class,
         **transforms_kwargs,
     )
     check_learner_transforms(model_updater._learner, transforms_kwargs)
     model = model_updater.update(train_dataset, task_id=defaults.TASK_ID)
     model_updater = pytest.helpers.get_simple_updater(
-        model, current_state_folder=state_url, learner_class=learner_class, **transforms_kwargs
+        model, input_state_folder=state_url, learner_class=learner_class, **transforms_kwargs
     )
     check_learner_transforms(model_updater._learner, transforms_kwargs)
```

### Comparing `Renate-0.1.0/test/renate/utils/test_file.py` & `Renate-0.2.0/test/renate/utils/test_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 def create_file(path, content):
     os.makedirs(os.path.dirname(path), exist_ok=True)
     with open(path, "w") as f:
         f.write(content)
 
 
 @pytest.mark.parametrize(
-    "file_content1_source_dir, file_content2_source_dir, file_content1_destination_dir, file_content2_destination_dir",
+    "file_content1_source_dir, file_content2_source_dir, file_content1_destination_dir,"
+    "file_content2_destination_dir",
     [["test1_1", "test1_1", "test1_2", "test2_2"]],
 )
 def test_move_to_uri_locally(
     tmpdir,
     file_content1_source_dir,
     file_content2_source_dir,
     file_content1_destination_dir,
     file_content2_destination_dir,
 ):
     """Test for moving files from a local directory to another local directory.
 
-    The files should be moved from the source directory and the destination directory should be created
-    if it does not exist.
+    The files should be moved from the source directory and the destination directory should be
+    created if it does not exist.
 
-    If there are files with the same name in the destination directory as in the source directory they should be overwritten.
+    If there are files with the same name in the destination directory as in the source directory
+    they should be overwritten.
     """
 
     create_file(os.path.join(tmpdir, "source_dir", "file1.txt"), file_content1_source_dir)
     create_file(os.path.join(tmpdir, "source_dir", "file2.txt"), file_content2_source_dir)
 
     create_file(os.path.join(tmpdir, "destination_dir", "file1.txt"), file_content1_destination_dir)
     create_file(os.path.join(tmpdir, "destination_dir", "file3.txt"), file_content2_destination_dir)
@@ -48,30 +50,32 @@
         assert f.read() == file_content2_destination_dir
 
     assert not os.path.exists(os.path.join(tmpdir, "source_dir", "file1.txt"))
     assert not os.path.exists(os.path.join(tmpdir, "source_dir", "file2.txt"))
 
 
 @pytest.mark.parametrize(
-    "file_content1_source_dir, file_content2_source_dir, file_content1_destination_dir, file_content2_destination_dir",
+    "file_content1_source_dir, file_content2_source_dir, file_content1_destination_dir, "
+    "file_content2_destination_dir",
     [["test1_1", "test1_1", "test1_2", "test2_2"]],
 )
 def test_copy_to_uri_locally(
     tmpdir,
     file_content1_source_dir,
     file_content2_source_dir,
     file_content1_destination_dir,
     file_content2_destination_dir,
 ):
     """Test for copying files from a local directory to another local directory.
 
-    The files should be copied from the source directory and the destination directory should be created
-    if it does not exist.
+    The files should be copied from the source directory and the destination directory should be
+    created if it does not exist.
 
-    If there are files with the same name in the destination directory as in the source directory they should be overwritten.
+    If there are files with the same name in the destination directory as in the source directory
+    they should be overwritten.
 
     The source directory should not be changed.
     """
 
     create_file(os.path.join(tmpdir, "source_dir", "file1.txt"), file_content1_source_dir)
     create_file(os.path.join(tmpdir, "source_dir", "file2.txt"), file_content2_source_dir)
```

### Comparing `Renate-0.1.0/test/renate/utils/test_metrics_utils.py` & `Renate-0.2.0/test/renate/utils/test_metrics_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         ),
     ],
     ids=["valid_metric_names", "duplicate_metric_names"],
 )
 def test_given_additional_metrics_create_metrics_adds_them_to_metric_collection(
     additional_metrics, is_duplicate
 ):
-    """Passes if duplicate metric names raise an exception and additional metrics are added to the metric collection.
+    """Passes if duplicate metric names raise an exception and additional metrics are added to the
+    metric collection.
 
     Case 1: Valid case.
     Case 2: Metric name already used as part of the default metric collection.
     """
     if is_duplicate:
         with pytest.raises(AssertionError):
             create_metrics(task="classification", additional_metrics=additional_metrics)
```

### Comparing `Renate-0.1.0/test/renate/utils/test_optimizer.py` & `Renate-0.2.0/test/renate/utils/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/test/renate/utils/test_pytorch.py` & `Renate-0.2.0/test/renate/utils/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `Renate-0.1.0/test/renate/utils/test_syne_tune.py` & `Renate-0.2.0/test/renate/utils/test_syne_tune.py`

 * *Files identical despite different names*

