# Comparing `tmp/mlfoundry-0.7.7.tar.gz` & `tmp/mlfoundry-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.7.7.tar", max compression
+gzip compressed data, was "mlfoundry-0.7.8.tar", max compression
```

## Comparing `mlfoundry-0.7.7.tar` & `mlfoundry-0.7.8.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     3158 2023-04-03 06:04:03.010485 mlfoundry-0.7.7/README.md
--rw-r--r--   0        0        0      991 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0     6975 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      954 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0      731 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      739 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2724 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/constants.py
--rw-r--r--   0        0        0      103 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/__init__.py
--rw-r--r--   0        0        0     7854 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/dataset.py
--rw-r--r--   0        0        0     2255 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/schema.py
--rw-r--r--   0        0        0    13138 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/serde.py
--rw-r--r--   0        0        0     2028 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/serde_utils.py
--rw-r--r--   0        0        0     2078 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/stats.py
--rw-r--r--   0        0        0     1903 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/types.py
--rw-r--r--   0        0        0     2588 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/validation.py
--rw-r--r--   0        0        0       69 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/whylogs_types/__init__.py
--rw-r--r--   0        0        0     4025 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/dataset/whylogs_types/summary.py
--rw-r--r--   0        0        0     1358 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/enums.py
--rw-r--r--   0        0        0      325 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     1906 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-04-03 06:04:03.026484 mlfoundry-0.7.7/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      724 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15215 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22189 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      571 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     7521 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     2871 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    14349 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0     1281 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/dataset_artifact.py
--rw-r--r--   0        0        0      222 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/dataset_schema.py
--rw-r--r--   0        0        0      318 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/dataset_stats.py
--rw-r--r--   0        0        0       50 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7148 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2116 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6908 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6855 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4475 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     4079 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2754 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2287 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    29058 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    46254 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     2031 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6672 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4304 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/run_utils.py
--rw-r--r--   0        0        0      498 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/schema.py
--rw-r--r--   0        0        0     9751 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0      782 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56184 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-04-03 06:04:03.030484 mlfoundry-0.7.7/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3549 2023-04-03 06:04:17.062357 mlfoundry-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-04-24 10:51:50.367933 mlfoundry-0.7.8/README.md
+-rw-r--r--   0        0        0      991 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0     9414 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0      731 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      739 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2724 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/constants.py
+-rw-r--r--   0        0        0      103 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/__init__.py
+-rw-r--r--   0        0        0     7854 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/dataset.py
+-rw-r--r--   0        0        0     2255 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/schema.py
+-rw-r--r--   0        0        0    13138 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/serde.py
+-rw-r--r--   0        0        0     2028 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/serde_utils.py
+-rw-r--r--   0        0        0     2078 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/stats.py
+-rw-r--r--   0        0        0     1903 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/types.py
+-rw-r--r--   0        0        0     2588 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/validation.py
+-rw-r--r--   0        0        0       69 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/whylogs_types/__init__.py
+-rw-r--r--   0        0        0     4025 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/dataset/whylogs_types/summary.py
+-rw-r--r--   0        0        0     1358 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/enums.py
+-rw-r--r--   0        0        0      325 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     1906 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      724 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.387933 mlfoundry-0.7.8/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15215 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22189 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      571 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     7521 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     2871 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    14349 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5983 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0     1281 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/dataset_artifact.py
+-rw-r--r--   0        0        0      222 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/dataset_schema.py
+-rw-r--r--   0        0        0      318 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/dataset_stats.py
+-rw-r--r--   0        0        0       50 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    30890 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    46245 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4304 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0      492 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/schema.py
+-rw-r--r--   0        0        0     9979 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-04-24 10:51:50.391933 mlfoundry-0.7.8/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-04-24 10:51:50.395933 mlfoundry-0.7.8/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3549 2023-04-24 10:52:05.396042 mlfoundry-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.7.8/PKG-INFO
```

### Comparing `mlfoundry-0.7.7/README.md` & `mlfoundry-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/__init__.py` & `mlfoundry-0.7.8/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/__main__.py` & `mlfoundry-0.7.8/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/amplitude.py` & `mlfoundry-0.7.8/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.7.8/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
 import posixpath
+import signal
+import sys
 import typing
 import uuid
+from concurrent.futures import ProcessPoolExecutor, as_completed
+from multiprocessing import active_children
 
 from mlflow.entities import FileInfo, SignedURL
 from mlflow.store.artifact.artifact_repo import ArtifactRepository
 from mlflow.tracking import MlflowClient
 from mlflow.utils.file_utils import (
     download_file_using_http_uri,
     relative_path_to_artifact_path,
@@ -13,16 +17,46 @@
 from mlflow.utils.rest_utils import cloud_storage_http_request
 
 from mlfoundry.exceptions import MlFoundryException
 from mlfoundry.tracking.entities import ArtifactCredential
 from mlfoundry.tracking.truefoundry_rest_store import TruefoundryRestStore
 
 
+def sigterm_handler(sig, frame):
+    print("Handling SIGTERM...")
+    try:
+        active = active_children()
+        # terminate all active children
+        for child in active:
+            child.terminate()
+    finally:
+        # terminate the process
+        sys.exit(0)
+
+
+def sighup_handler(sig, frame):
+    print("Handling SIGHUP...")
+    try:
+        active = active_children()
+        # terminate all active children
+        for child in active:
+            child.terminate()
+    finally:
+        # terminate the process
+        sys.exit(0)
+
+
 class TruefoundryArtifactRepository(ArtifactRepository):
-    def __init__(self, artifact_uri, rest_store: TruefoundryRestStore):
+    def __init__(
+        self,
+        artifact_uri,
+        rest_store: TruefoundryRestStore,
+        credentials=None,
+        storage_integration_id=None,
+    ):
         self.artifact_uri = artifact_uri
         super().__init__(artifact_uri)
 
         self.rest_store: TruefoundryRestStore = rest_store
 
     @staticmethod
     def _extract_run_id(artifact_uri) -> str:
@@ -87,61 +121,107 @@
             run_id=self._extract_run_id(self.artifact_uri), path=remote_file_path
         )
         download_file_using_http_uri(
             http_uri=artifact_credential.signed_uri, download_path=local_path
         )
 
 
+def _signed_uri_upload_file(signed_url: SignedURL, local_file: str):
+    if os.stat(local_file).st_size == 0:
+        with cloud_storage_http_request("put", signed_url.url, data="") as response:
+            response.raise_for_status()
+    else:
+        with open(local_file, "rb") as file:
+            with cloud_storage_http_request(
+                "put", signed_url.url, data=file
+            ) as response:
+                response.raise_for_status()
+
+
 class MlFoundryArtifactsRepository(ArtifactRepository):
     def __init__(self, version_id: uuid.UUID, mlflow_client: MlflowClient):
         self.version_id = version_id
         self._tracking_client = mlflow_client
         super().__init__(artifact_uri=None)
 
     # these methods should be named list_files, log_directory, log_file, etc
 
     def list_artifacts(self, path=None) -> typing.List[FileInfo]:
         return self._tracking_client.list_files_for_artifact_version(
             version_id=self.version_id, path=path
         )
 
+    def get_write_signed_url(self, local_file, artifact_path=None) -> str:
+        dest_path = artifact_path or ""
+        dest_path = dest_path.lstrip(posixpath.sep)
+        dest_path = posixpath.join(dest_path, os.path.basename(local_file))
+
+        return self._tracking_client.get_signed_urls_for_artifact_version_write(
+            version_id=self.version_id, paths=[dest_path]
+        )[0]
+
     def _signed_uri_upload_file(self, signed_url: SignedURL, local_file: str):
-        if os.stat(local_file).st_size == 0:
-            with cloud_storage_http_request("put", signed_url.url, data="") as response:
-                response.raise_for_status()
-        else:
-            with open(local_file, "rb") as file:
-                with cloud_storage_http_request(
-                    "put", signed_url.url, data=file
-                ) as response:
-                    response.raise_for_status()
+        _signed_uri_upload_file(signed_url=signed_url, local_file=local_file)
 
     def log_artifacts(self, local_dir, artifact_path=None):
         dest_path = artifact_path or ""
         dest_path = dest_path.lstrip(posixpath.sep)
+        files = []
+
         for (root, _, file_names) in os.walk(local_dir):
             upload_path = dest_path
             if root != local_dir:
                 rel_path = os.path.relpath(root, local_dir)
                 rel_path = relative_path_to_artifact_path(rel_path)
                 upload_path = posixpath.join(dest_path, rel_path)
             for file_name in file_names:
                 local_file = os.path.join(root, file_name)
-                self.log_artifact(local_file=local_file, artifact_path=upload_path)
+                files.append((upload_path, local_file))
+
+        files.sort(
+            key=lambda x: os.stat(x[1]).st_size
+        )  # sort on the basis of file size
+
+        # finally block doesn't execute when SIGTERM, SIGHUP, SIGKILL are received
+        # Handle SIGTERM, SIGHUP signals to avoid zombie processes
+        signal.signal(signal.SIGTERM, sigterm_handler)
+        signal.signal(signal.SIGHUP, sighup_handler)
+
+        # Log artifacts in parallel using ProcessPoolExecutor
+        with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
+            futures = []
+
+            for upload_path, local_file in files:
+                signed_url = self.get_write_signed_url(
+                    local_file=local_file, artifact_path=upload_path
+                )
+                future = executor.submit(
+                    _signed_uri_upload_file, signed_url, local_file
+                )
+                futures.append(future)
+
+            try:
+                for future in as_completed(futures):
+                    future.result()
+            except Exception as e:
+                raise e
+            finally:
+                [f.cancel() for f in futures]
+                # Accessing protected member of a class here (could fail in future versions)
+                for pid, proc in executor._processes.items():
+                    if proc.is_alive():
+                        proc.terminate()
 
     def log_artifact(self, local_file, artifact_path=None):
-        dest_path = artifact_path or ""
-        dest_path = dest_path.lstrip(posixpath.sep)
-        dest_path = posixpath.join(dest_path, os.path.basename(local_file))
         # TODO (chiragjn): Re-implement log_artifacts to take advantage of getting multiple signed urls at once
         #                  However care also needs to be taken to expose and pass in proper expiry because the user
         #                  user might be on slow connections or downloading many files sequentially might eat up time
-        signed_url = self._tracking_client.get_signed_urls_for_artifact_version_write(
-            version_id=self.version_id, paths=[dest_path]
-        )[0]
+        signed_url = self.get_write_signed_url(
+            local_file=local_file, artifact_path=artifact_path
+        )
         self._signed_uri_upload_file(signed_url, local_file)
 
     def _download_file(self, remote_file_path: str, local_path: str):
         if not remote_file_path:
             raise MlFoundryException(
                 f"remote_file_path cannot be None or empty str {remote_file_path}"
             )
```

### Comparing `mlfoundry-0.7.7/mlfoundry/background/interface.py` & `mlfoundry-0.7.8/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/background/sender.py` & `mlfoundry-0.7.8/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/background/system_metrics.py` & `mlfoundry-0.7.8/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/background/utils.py` & `mlfoundry-0.7.8/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.7.8/mlfoundry/cli/cli_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 
 import click
 
 from mlfoundry.cli.commands import download, login
-from mlfoundry.logger import logger
 from mlfoundry.version import __version__
 
 
 @click.group()
 @click.version_option(__version__)
 def mlfoundry_cli():
     """MlFoundry CLI"""
```

### Comparing `mlfoundry-0.7.7/mlfoundry/cli/commands/download.py` & `mlfoundry-0.7.8/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/cli/commands/login.py` & `mlfoundry-0.7.8/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/constants.py` & `mlfoundry-0.7.8/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/dataset.py` & `mlfoundry-0.7.8/mlfoundry/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/schema.py` & `mlfoundry-0.7.8/mlfoundry/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/serde.py` & `mlfoundry-0.7.8/mlfoundry/dataset/serde.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/serde_utils.py` & `mlfoundry-0.7.8/mlfoundry/dataset/serde_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/stats.py` & `mlfoundry-0.7.8/mlfoundry/dataset/stats.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/types.py` & `mlfoundry-0.7.8/mlfoundry/dataset/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/validation.py` & `mlfoundry-0.7.8/mlfoundry/dataset/validation.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/dataset/whylogs_types/summary.py` & `mlfoundry-0.7.8/mlfoundry/dataset/whylogs_types/summary.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/enums.py` & `mlfoundry-0.7.8/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.7.8/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/git_info.py` & `mlfoundry-0.7.8/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/integrations/lightning.py` & `mlfoundry-0.7.8/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/integrations/transformers.py` & `mlfoundry-0.7.8/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/internal_namespace.py` & `mlfoundry-0.7.8/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/__init__.py` & `mlfoundry-0.7.8/mlfoundry/log_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.7.8/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/dataset_artifact.py` & `mlfoundry-0.7.8/mlfoundry/log_types/dataset_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/image/image.py` & `mlfoundry-0.7.8/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.7.8/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/image/types.py` & `mlfoundry-0.7.8/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/plot.py` & `mlfoundry-0.7.8/mlfoundry/log_types/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import enum
 import json
 import os
 import posixpath
 import sys
 import tempfile
 from typing import Union
-from uuid import uuid4
 
 from mlflow.entities import ArtifactType
 from pydantic import BaseModel
 
 from mlfoundry.exceptions import MlFoundryException
 from mlfoundry.log_types.artifacts.artifact import (
     ArtifactVersionInternalMetadata,
```

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.7.8/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/log_types/utils.py` & `mlfoundry-0.7.8/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/login.py` & `mlfoundry-0.7.8/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v1/base_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from mlfoundry.constants import (
     MULTI_DIMENSIONAL_METRICS,
     NON_MULTI_DIMENSIONAL_METRICS,
     PROB_MULTI_DIMENSIONAL_METRICS,
     PROB_NON_MULTI_DIMENSIONAL_METRICS,
 )
-from mlfoundry.logger import logger
 
 
 class BaseMetrics:
     PERCENTAGE_FEATURE_NULL = "percentage_feature_null"
 
     def __init__(self):
         self.metrics_base = {
```

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import pandas as pd
 from sklearn.metrics import (
     accuracy_score,
     cohen_kappa_score,
     confusion_matrix,
     dcg_score,
     f1_score,
     log_loss,
@@ -15,15 +14,14 @@
 from mlfoundry.constants import (
     MULTI_DIMENSIONAL_METRICS,
     NON_MULTI_DIMENSIONAL_METRICS,
     PROB_MULTI_DIMENSIONAL_METRICS,
     PROB_NON_MULTI_DIMENSIONAL_METRICS,
 )
 from mlfoundry.exceptions import MlFoundryException
-from mlfoundry.logger import logger
 from mlfoundry.metrics.v1.base_metrics import BaseMetrics
 
 
 class BinaryClassificationMetrics(BaseMetrics):
     TYPE_OF_MODEL = "binary_classification"
     ACCURACY = "accuracy"
     F1_SCORE = "f1_score"
```

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import numpy as np
-import pandas as pd
 from sklearn.metrics import (
     accuracy_score,
     cohen_kappa_score,
     confusion_matrix,
     dcg_score,
-    f1_score,
     log_loss,
     ndcg_score,
     precision_recall_curve,
     roc_curve,
 )
-from sklearn.preprocessing import label_binarize
 
 from mlfoundry.constants import (
     MULTI_DIMENSIONAL_METRICS,
     NON_MULTI_DIMENSIONAL_METRICS,
     PROB_MULTI_DIMENSIONAL_METRICS,
     PROB_NON_MULTI_DIMENSIONAL_METRICS,
 )
-from mlfoundry.logger import logger
 from mlfoundry.metrics.v1.base_metrics import BaseMetrics
 
 
 class MultiClassClassificationMetrics(BaseMetrics):
     TYPE_OF_MODEL = "multiclass_classification"
     ACCURACY = "accuracy"
     COHEN_KAPPA_SCORE = "cohen_kappa_score"
```

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import pandas as pd
 from sklearn.metrics import (
     explained_variance_score,
     mean_absolute_error,
     mean_squared_error,
     r2_score,
 )
 
 from mlfoundry.constants import (
     MULTI_DIMENSIONAL_METRICS,
     NON_MULTI_DIMENSIONAL_METRICS,
     PROB_MULTI_DIMENSIONAL_METRICS,
     PROB_NON_MULTI_DIMENSIONAL_METRICS,
 )
-from mlfoundry.logger import logger
 from mlfoundry.metrics.v1.base_metrics import BaseMetrics
 
 
 class RegressionMetrics(BaseMetrics):
     TYPE_OF_MODEL = "regression"
     MEAN_SQUARED_ERROR = "mean_squared_error"
     MEAN_ABSOLUTE_ERROR = "mean_absolute_error"
```

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-import pandas as pd
-from sklearn.metrics import (
-    explained_variance_score,
-    mean_absolute_error,
-    mean_squared_error,
-    r2_score,
-)
+from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
 
 from mlfoundry.constants import (
     MULTI_DIMENSIONAL_METRICS,
     NON_MULTI_DIMENSIONAL_METRICS,
     PROB_MULTI_DIMENSIONAL_METRICS,
     PROB_NON_MULTI_DIMENSIONAL_METRICS,
 )
-from mlfoundry.logger import logger
 from mlfoundry.metrics.v1.base_metrics import BaseMetrics
 
 
 class TimeSeriesMetrics(BaseMetrics):
     TYPE_OF_MODEL = "timeseries"
     MEAN_SQUARED_ERROR = "mean_squared_error"
     MEAN_ABSOLUTE_ERROR = "mean_absolute_error"
```

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     mean_absolute_error,
     mean_squared_error,
     r2_score,
 )
 
 from mlfoundry.enums import ModelType
 from mlfoundry.exceptions import MlFoundryException
-from mlfoundry.logger import logger
 from mlfoundry.metrics.v2.base_metrics import BaseMetrics
 
 
 class RegressionMetrics(BaseMetrics):
     MEAN_SQUARED_ERROR = "mean_squared_error"
     MEAN_ABSOLUTE_ERROR = "mean_absolute_error"
     R2_SCORE = "r2_score"
```

### Comparing `mlfoundry-0.7.7/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.7.8/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing
 
 from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
 
 from mlfoundry.enums import ModelType
 from mlfoundry.exceptions import MlFoundryException
-from mlfoundry.logger import logger
 from mlfoundry.metrics.v2.base_metrics import BaseMetrics
 
 
 class TimeSeriesMetrics(BaseMetrics):
     MEAN_SQUARED_ERROR = "mean_squared_error"
     MEAN_ABSOLUTE_ERROR = "mean_absolute_error"
     R2_SCORE = "r2_score"
```

### Comparing `mlfoundry-0.7.7/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.7.8/mlfoundry/mlfoundry_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 import os
 from datetime import datetime, timedelta, timezone
 from typing import Any, Dict, Generator, Iterator, List, Optional, Sequence, Union
 
 import coolname
 import mlflow
 import pandas as pd
-from mlflow.entities import ArtifactType
+from mlflow.entities import Experiment
 from mlflow.store.tracking import SEARCH_MAX_RESULTS_DEFAULT
 from mlflow.tracking import MlflowClient
 
 from mlfoundry import amplitude, constants, env_vars
 from mlfoundry.enums import ViewType
 from mlfoundry.env_vars import TRACKING_HOST_GLOBAL
 from mlfoundry.exceptions import MlflowException, MlFoundryException
 from mlfoundry.internal_namespace import NAMESPACE
 from mlfoundry.log_types.artifacts.artifact import ArtifactVersion
 from mlfoundry.log_types.artifacts.model import ModelVersion
 from mlfoundry.logger import logger
 from mlfoundry.mlfoundry_run import MlFoundryRun
 from mlfoundry.monitoring.entities import Actual, Prediction
 from mlfoundry.monitoring.store import MonitoringClient
-from mlfoundry.session import Session, init_session
+from mlfoundry.session import Session, get_active_session, init_session
+from mlfoundry.tracking.servicefoundry_service import ServicefoundryService
 
 
 def _get_internal_env_vars_values() -> Dict[str, str]:
     env = {}
     for env_var_name in env_vars.INTERNAL_ENV_VARS:
         value = os.getenv(env_var_name)
         if value:
@@ -79,24 +80,28 @@
         user_id = session.user_info.user_id
 
     amplitude.init(user_id=user_id, disable_analytics=disable_analytics)
     amplitude.track(amplitude.Event.GET_CLIENT)
     return MlFoundry(session=session)
 
 
-def resolve_project_name(
+def resolve_ml_repo_name(
     ml_repo: Optional[str] = None,
     project_name: Optional[str] = None,
 ) -> str:
     if project_name and ml_repo:
         raise MlFoundryException(
             f"Only one of field project_name or ml_repo should be passed"
         )
     if not project_name and not ml_repo:
         raise MlFoundryException(f"ml_repo must be string type and cannot be empty")
+    if project_name:
+        logger.warning(
+            "Field project_name has been depricated and renamed to ml_repo. Please use ml_repo as we will remove project_name in the upcoming versions"
+        )
     if ml_repo:
         project_name = ml_repo
     if project_name == "" or (not isinstance(project_name, str)):
         raise MlFoundryException(
             f"ml_repo must be string type and not empty. "
             f"Got {type(project_name)} type with value {project_name!r}"
         )
@@ -112,63 +117,98 @@
         Args:
             tracking_uri (Optional[str], optional): tracking_uri
         """
         self.mlflow_client = MlflowClient()
         if session:
             self.monitoring_client = MonitoringClient(session=session)
 
-    def _get_or_create_project(self, project_name: str) -> str:
-        """_get_or_create_experiment.
+    def _get_ml_repo(self, ml_repo: str) -> str:
+        """_get_ml_repo.
 
         Args:
-            project_name (str): The name of the project.
+            ml_repo (str): The name of the ML Repo.
 
         Returns:
-            str: The id of the project.
+            str: The id of the ML Repo.
         """
-        experiment_name = project_name
         try:
-            experiment = self.mlflow_client.get_experiment_by_name(experiment_name)
-            if experiment is not None:
-                return experiment.experiment_id
-            else:
-                logger.info(
-                    f"project {experiment_name} does not exist. Creating {experiment_name}."
-                )
-                return self.mlflow_client.create_experiment(experiment_name)
-
+            ml_repo_obj = self.mlflow_client.get_experiment_by_name(name=ml_repo)
         except MlflowException as e:
             err_msg = (
-                f"Error happened in creating or getting project based on project name: "
-                f"{experiment_name}. Error details: {e.message}"
+                f"Error happened in getting ML Repo based on name: "
+                f"{ml_repo}. Error details: {e.message}"
             )
             raise MlFoundryException(err_msg) from e
+        if not ml_repo_obj:
+            err_msg = (
+                f"ML Repo Does Not Exist for name: {ml_repo}. You may either "
+                "create it from the dashboard or using client.create_ml_repo('<ml_repo_name>')"
+            )
+            raise MlFoundryException(err_msg)
+        return ml_repo_obj.experiment_id
 
-    def get_all_projects(self) -> List[str]:
-        """Returns a list of project ids accessible by the current user.
+    def list_ml_repos(self) -> List[str]:
+        """Returns a list of names of ML Repos accessible by the current user.
 
         Returns:
-            List[str]: A list of project ids.
+            List[str]: A list of names of ML Repos
         """
         amplitude.track(amplitude.Event.GET_ALL_PROJECTS)
         try:
-            experiments = self.mlflow_client.list_experiments(view_type=ViewType.ALL)
+            ml_repos = self.mlflow_client.list_experiments(view_type=ViewType.ALL)
         except MlflowException as e:
-            err_msg = (
-                f"Error happened in fetching project names. Error details: {e.message}"
-            )
+            err_msg = f"Error happened in fetching ML Repos. Error details: {e.message}"
             raise MlFoundryException(err_msg) from e
 
-        projects = []
-        for e in experiments:
-            # Experiment ID 0 represents default project which we are removing.
-            if e.experiment_id != "0":
-                projects.append(e.name)
+        ml_repos_names = []
+        for ml_repo in ml_repos:
+            # ML Repo with experiment_id 0 represents default ML Repo which we are removing.
+            if ml_repo.experiment_id != "0":
+                ml_repos_names.append(ml_repo.name)
+
+        return ml_repos_names
+
+    def create_ml_repo(
+        self,
+        ml_repo: Optional[str] = None,
+        storage_integration_fqn: Optional[str] = None,
+    ) -> Experiment:
+        existing_ml_repo = self.mlflow_client.get_experiment_by_name(name=ml_repo)
+        if not existing_ml_repo:  # ml_repo does not exist
+            return self.mlflow_client.get_experiment(
+                experiment_id=self.mlflow_client.create_experiment(
+                    name=ml_repo, storage_integration_fqn=storage_integration_fqn
+                )
+            )
+
+        if storage_integration_fqn:
+            session = get_active_session()
+            servicefoundry_service = ServicefoundryService(
+                tracking_uri=self.get_tracking_uri(),
+                token=session.token.access_token,
+            )
+
+            try:
+                existing_storage_integration = (
+                    servicefoundry_service.get_integration_from_id(
+                        existing_ml_repo.storage_integration_id
+                    )
+                )
+            except Exception as e:
+                err_msg = f"Error happened in getting integration of ML Repo. Error details: {e.message}"
+                raise MlFoundryException(err_msg) from e
+
+            if existing_storage_integration["fqn"] != storage_integration_fqn:
+                raise MlFoundryException(
+                    f"ML Repo with same name already exists with storage integration:"
+                    f"{existing_storage_integration['fqn']}. Cannot update the storage integration to: "
+                    f"{storage_integration_fqn}"
+                )
 
-        return projects
+        return existing_ml_repo
 
     def create_run(
         self,
         project_name: Optional[str] = None,
         ml_repo: Optional[str] = None,
         run_name: Optional[str] = None,
         tags: Optional[Dict[str, Any]] = None,
@@ -242,28 +282,28 @@
 
         if not run_name:
             run_name = coolname.generate_slug(2)
             logger.info(
                 f"No run_name given. Using a randomly generated name {run_name}."
                 " You can pass your own using the `run_name` argument"
             )
-        project_name = resolve_project_name(ml_repo=ml_repo, project_name=project_name)
+        ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
 
-        experiment_id = self._get_or_create_project(project_name)
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
 
         if tags is not None:
             NAMESPACE.validate_namespace_not_used(tags.keys())
         else:
             tags = {}
 
         tags.update(_get_internal_env_vars_values())
-        run = self.mlflow_client.create_run(experiment_id, name=run_name, tags=tags)
+        run = self.mlflow_client.create_run(ml_repo_id, name=run_name, tags=tags)
         mlf_run_id = run.info.run_id
 
-        mlf_run = MlFoundryRun(experiment_id, mlf_run_id, **kwargs)
+        mlf_run = MlFoundryRun(ml_repo_id, mlf_run_id, **kwargs)
         # TODO(Rizwan): Revisit this once run lifecycle is formalised
         mlf_run._add_git_info()
         mlf_run._add_python_mlf_version()
         logger.info(f"Run {run.info.fqn!r} has started.")
         return mlf_run
 
     def get_run(self, run_id: str) -> MlFoundryRun:
@@ -321,29 +361,29 @@
         The user must have `READ` access to the project.
         Args:
             ml_repo (str): Name of the project.
         Returns:
             pd.DataFrame: dataframe with two columns- run_id and run_name
         """
         amplitude.track(amplitude.Event.GET_ALL_RUNS)
-        resolve_project_name(ml_repo=ml_repo, project_name=project_name)
-        experiment = self.mlflow_client.get_experiment_by_name(project_name)
-        if experiment is None:
+        ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
+        ml_repo_obj = self.mlflow_client.get_experiment_by_name(ml_repo)
+        if ml_repo_obj is None:
             return pd.DataFrame(
                 columns=[constants.RUN_ID_COL_NAME, constants.RUN_NAME_COL_NAME]
             )
 
-        experiment_id = experiment.experiment_id
+        ml_repo_id = ml_repo_obj.experiment_id
 
         try:
             all_run_infos = self.mlflow_client.list_run_infos(
-                experiment_id, run_view_type=ViewType.ALL
+                ml_repo_id, run_view_type=ViewType.ALL
             )
         except MlflowException as e:
-            err_msg = f"Error happened in while fetching runs for project {project_name}. Error details: {e.message}"
+            err_msg = f"Error happened in while fetching runs for ML Repo {ml_repo}. Error details: {e.message}"
             raise MlFoundryException(err_msg) from e
 
         runs = []
 
         for run_info in all_run_infos:
             try:
                 run = self.mlflow_client.get_run(run_info.run_id)
@@ -424,36 +464,36 @@
             )
 
             ```
 
         Returns:
             Genarator[MlFoundryRun, None, None]: MLFoundryRuns matching the search query.
         """
-        resolve_project_name(ml_repo=ml_repo, project_name=project_name)
+        ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
         try:
             run_view_type = ViewType.from_string(run_view_type.lower())
         except Exception as e:
             raise MlFoundryException(e) from e
 
         try:
-            experiment = self.mlflow_client.get_experiment_by_name(project_name)
+            ml_repo_obj = self.mlflow_client.get_experiment_by_name(ml_repo)
         except MlflowException as e:
             raise MlFoundryException(e) from e  # user doesnot have READ permission
 
-        if experiment is None:
-            logger.warning(f"Project with name {project_name} does not exist")
+        if ml_repo_obj is None:
+            logger.warning(f"ML Repo with name {ml_repo} does not exist")
             return
 
-        experiment_id = experiment.experiment_id
+        ml_repo_id = ml_repo_obj.experiment_id
 
         page_token = None
         done = False
         while not done:
             all_runs = self.mlflow_client.search_runs(
-                experiment_ids=[experiment_id],
+                experiment_ids=[ml_repo_id],
                 filter_string=filter_string,
                 run_view_type=run_view_type,
                 max_results=SEARCH_MAX_RESULTS_DEFAULT,
                 order_by=order_by,
                 page_token=page_token,
             )
             page_token = all_runs.token
```

### Comparing `mlfoundry-0.7.7/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.7.8/mlfoundry/mlfoundry_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self._experiment_id = str(experiment_id)
         # TODO (chiragjn): mlflow_client be a protected/private member
         self.mlflow_client = MlflowClient()
         self._project_name = self.mlflow_client.get_experiment(self._experiment_id).name
         self._run_id = run_id
         self._run_info: Optional[RunInfo] = None
 
-        from mlfoundry.dataset import DataSet, TabularDatasetDriver
+        from mlfoundry.dataset import TabularDatasetDriver
 
         self._dataset_module: TabularDatasetDriver = TabularDatasetDriver(
             mlflow_client=self.mlflow_client, run_id=run_id
         )
 
         self._terminate_called = False
         ACTIVE_RUNS.add_run(self)
```

### Comparing `mlfoundry-0.7.7/mlfoundry/monitoring/entities.py` & `mlfoundry-0.7.8/mlfoundry/monitoring/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, constr
 
-from mlfoundry.logger import logger
-
 # TODO @nikp1172 Add support for np types https://numpy.org/doc/stable/user/basics.types.html
 EntityValue = Union[str, int, float]
 
 
 class PredictionData(BaseModel):
     value: EntityValue
     probabilities: Dict[str, float] = Field(default_factory=dict)
```

### Comparing `mlfoundry-0.7.7/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.7.8/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.7.8/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import math
 import typing
 from collections import defaultdict
 from datetime import datetime
 from functools import lru_cache
 
-from mlflow.tracking._tracking_service.utils import _get_default_host_creds
 from mlflow.utils.rest_utils import MlflowHostCreds, http_request_safe
 
 from mlfoundry.logger import logger
 from mlfoundry.monitoring.entities import (
     ActualPacket,
     BasePacket,
     DatasetData,
@@ -20,15 +18,14 @@
     BatchInsertRequest,
     BatchUpdateActualRequest,
     ClassPrediction,
     Data,
     GetDatasetResponse,
     MlModelPrediction,
 )
-from mlfoundry.tracking.entities import AuthServerInfo
 
 
 # TODO @nikp1172 add feature of autmatically serializing datetime object in \
 #  mlflow.utils.rest_utils.http_request
 class RestMonitoringStore:
     def __init__(self, get_host_creds: typing.Callable[[], MlflowHostCreds]):
         self._get_host_creds: typing.Callable[[], MlflowHostCreds] = get_host_creds
```

### Comparing `mlfoundry-0.7.7/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.7.8/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/run_utils.py` & `mlfoundry-0.7.8/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/session.py` & `mlfoundry-0.7.8/mlfoundry/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,18 @@
             raise MlFoundryException(
                 "This session has been deactivated.\n"
                 "At a time only one `client` (received from "
                 "`mlfoundry.get_client()` function call) can be used"
             )
 
     @property
+    def token(self) -> Token:
+        return self._cred_provider.token
+
+    @property
     def user_info(self) -> UserInfo:
         self._assert_not_closed()
         return self._user_info
 
     @property
     def tracking_uri(self) -> str:
         return self._cred_provider.tracking_uri
@@ -239,14 +243,18 @@
 
         return builder
 
 
 ACTIVE_SESSION: Optional[Session] = None
 
 
+def get_active_session() -> Session:
+    return ACTIVE_SESSION
+
+
 def init_session() -> Session:
     with SESSION_LOCK:
         final_cred_provider = None
         for cred_provider in [EnvCredentialProvider, FileCredentialProvider]:
             if cred_provider.can_provide():
                 final_cred_provider = cred_provider()
                 break
@@ -271,14 +279,15 @@
 
         tfy_rest_store = TruefoundryRestStore(get_host_creds=host_creds_builder)
         artifact_repository = partial(
             TruefoundryArtifactRepository, rest_store=tfy_rest_store
         )
         _artifact_repository_registry.register("s3", artifact_repository)
         _artifact_repository_registry.register("gs", artifact_repository)
+        _artifact_repository_registry.register("wasbs", artifact_repository)
 
         rest_store = RestStore(get_host_creds=host_creds_builder)
 
         def _get_rest_store(*args, **kwargs):
             return rest_store
 
         for scheme in ["http", "https"]:
```

### Comparing `mlfoundry-0.7.7/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.7.8/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/tracking/entities.py` & `mlfoundry-0.7.8/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.7.8/mlfoundry/tracking/servicefoundry_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 from mlflow.utils.rest_utils import MlflowHostCreds, http_request_safe
 
 from mlfoundry.run_utils import append_servicefoundry_path_to_tracking_ui
 from mlfoundry.tracking.entities import Token
 
 
 class ServicefoundryService:
-    def __init__(self, tracking_uri: str):
+    def __init__(self, tracking_uri: str, token: str = None):
         self.host_creds = MlflowHostCreds(
-            host=append_servicefoundry_path_to_tracking_ui(tracking_uri)
+            host=append_servicefoundry_path_to_tracking_ui(tracking_uri), token=token
         )
 
     def get_token_from_api_key(self, api_key: str) -> Token:
         response = http_request_safe(
             host_creds=self.host_creds,
             endpoint="/v1/oauth/api-key/token",
             method="get",
             params={"apiKey": api_key},
             timeout=3,
             max_retries=0,
         )
         response = response.json()
         return Token.parse_obj(response)
+
+    def get_integration_from_id(self, integration_id: str):
+        integration_id = integration_id or ""
+        response = http_request_safe(
+            host_creds=self.host_creds,
+            endpoint=f"/v1/integrations/{integration_id}",
+            method="get",
+            timeout=3,
+            max_retries=0,
+        )
+        return response.json()
```

### Comparing `mlfoundry-0.7.7/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.7.8/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.7/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.7.8/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 import sys
 import threading
 
 ##
 # Python bindings for the NVML library
 ##
 from ctypes import *
-from ctypes.util import find_library
 
 ## C Type mappings ##
 ## Enums
 _nvmlEnableState_t = c_uint
 NVML_FEATURE_DISABLED = 0
 NVML_FEATURE_ENABLED = 1
```

### Comparing `mlfoundry-0.7.7/pyproject.toml` & `mlfoundry-0.7.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.7.7" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.7.8" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
@@ -31,15 +31,15 @@
 pydantic = ">=1.8.2,<2.0.0"
 scikit-learn = ">=0.24.2,<2.0.0"
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
-tfy-mlflow-client = "0.0.25"
+tfy-mlflow-client = "0.0.28"
 # Check and try to eliminate libs below this comment
 boto3 = ">=1.14.1,<2.0.0"
 fastparquet = ">=0.8.0,<=2022.12.0"
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
 pyarrow = ">=5.0.0,<11.0.0"
 whylogs = [
```

### Comparing `mlfoundry-0.7.7/PKG-INFO` & `mlfoundry-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.7.7
+Version: 0.7.8
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 Requires-Dist: protobuf (>=3.19.0,<3.21.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pyarrow (>=5.0.0,<11.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: tfy-mlflow-client (==0.0.25)
+Requires-Dist: tfy-mlflow-client (==0.0.28)
 Requires-Dist: whylogs (>=0.6.15,<1.0.0) ; python_version < "3.10"
 Requires-Dist: whylogs (>=1.0.0,<2.0.0) ; python_version >= "3.10"
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
```

