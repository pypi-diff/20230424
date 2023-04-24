# Comparing `tmp/geti-sdk-1.4.1.tar.gz` & `tmp/geti-sdk-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geti-sdk-1.4.1.tar", last modified: Wed Apr 12 09:01:33 2023, max compression
+gzip compressed data, was "geti-sdk-1.5.0.tar", last modified: Mon Apr 24 09:21:41 2023, max compression
```

## Comparing `geti-sdk-1.4.1.tar` & `geti-sdk-1.5.0.tar`

### file list

```diff
@@ -1,169 +1,170 @@
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.059914 geti-sdk-1.4.1/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/LICENSE
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/MANIFEST.in
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17146 2023-04-12 09:01:33.059914 geti-sdk-1.4.1/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16281 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/README.md
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.043914 geti-sdk-1.4.1/geti_sdk/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.043914 geti-sdk-1.4.1/geti_sdk/annotation_readers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/annotation_readers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/annotation_readers/base_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.043914 geti-sdk-1.4.1/geti_sdk/annotation_readers/datumaro_annotation_reader/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12643 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11813 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/annotation_readers/geti_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.047914 geti-sdk-1.4.1/geti_sdk/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5009 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/algorithms.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/annotation_scene.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/annotations.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/code_deployment_info.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/configurable_parameter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/configurable_parameter_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/configuration.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/configuration_identifiers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.047914 geti-sdk-1.4.1/geti_sdk/data_models/containers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/containers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/containers/algorithm_list.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/containers/media_list.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.047914 geti-sdk-1.4.1/geti_sdk/data_models/enums/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/annotation_kind.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/configuration_enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/deployment_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/domain.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/job_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/job_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/media_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/model_status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      943 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/optimization_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/prediction_mode.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/shape_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/enums/task_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/job.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/label.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/media.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/media_identifiers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8433 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/model_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/performance.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/predictions.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11704 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/project.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/shapes.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6544 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/task.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/task_annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/data_models/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.047914 geti-sdk-1.4.1/geti_sdk/demos/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/constants.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.039914 geti-sdk-1.4.1/geti_sdk/demos/data/
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.047914 geti-sdk-1.4.1/geti_sdk/demos/data/example/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/data/example/dogs.png
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.051914 geti-sdk-1.4.1/geti_sdk/demos/data_helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/data_helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6113 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/data_helpers/anomaly_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9051 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/data_helpers/coco_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5359 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/data_helpers/download_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1881 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/data_helpers/video_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.051914 geti-sdk-1.4.1/geti_sdk/demos/demo_projects/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/demo_projects/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/demo_projects/anomaly_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/demo_projects/coco_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/demos/demo_projects/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.051914 geti-sdk-1.4.1/geti_sdk/deployment/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.051914 geti-sdk-1.4.1/geti_sdk/deployment/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/data_models/intermediate_inference_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/data_models/region_of_interest.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    23219 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/deployed_model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/deployment.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.051914 geti-sdk-1.4.1/geti_sdk/deployment/resources/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/resources/OVMS_README.md
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/resources/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/deployment/utils.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    53636 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/geti.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.051914 geti-sdk-1.4.1/geti_sdk/http_session/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/http_session/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/http_session/exception.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/http_session/geti_session.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/http_session/server_config.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6021 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/platform_versions.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.051914 geti-sdk-1.4.1/geti_sdk/rest_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3432 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.055914 geti-sdk-1.4.1/geti_sdk/rest_clients/annotation_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/annotation_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14302 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/annotation_clients/annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18136 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/configuration_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/deployment_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.055914 geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7611 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/image_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    13579 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/media_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5508 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/video_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/model_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/prediction_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.055914 geti-sdk-1.4.1/geti_sdk/rest_clients/project_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/project_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    23629 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/project_client/project_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/project_client/task_templates.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_clients/training_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.055914 geti-sdk-1.4.1/geti_sdk/rest_converters/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.055914 geti-sdk-1.4.1/geti_sdk/rest_converters/annotation_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/configuration_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/job_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/media_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/model_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.055914 geti-sdk-1.4.1/geti_sdk/rest_converters/prediction_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/project_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/rest_converters/status_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.055914 geti-sdk-1.4.1/geti_sdk/utils/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/algorithm_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/credentials_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/dictionary_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/label_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/plot_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/serialization_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/geti_sdk/utils/workspace_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.043914 geti-sdk-1.4.1/geti_sdk.egg-info/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17146 2023-04-12 09:01:33.000000 geti-sdk-1.4.1/geti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5678 2023-04-12 09:01:33.000000 geti-sdk-1.4.1/geti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-04-12 09:01:33.000000 geti-sdk-1.4.1/geti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-12 09:01:33.000000 geti-sdk-1.4.1/geti_sdk.egg-info/requires.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-04-12 09:01:33.000000 geti-sdk-1.4.1/geti_sdk.egg-info/top_level.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/pyproject.toml
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.059914 geti-sdk-1.4.1/requirements/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/requirements/requirements-dev.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/requirements/requirements-docs.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/requirements/requirements-notebooks.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/requirements/requirements.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-04-12 09:01:33.059914 geti-sdk-1.4.1/setup.cfg
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/setup.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.059914 geti-sdk-1.4.1/tests/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/conftest.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-12 09:01:33.059914 geti-sdk-1.4.1/tests/helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/constants.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/finalizers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/fixtures.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/plotting.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/project_service.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/training.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-04-12 09:01:13.000000 geti-sdk-1.4.1/tests/helpers/vcr_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/LICENSE
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/MANIFEST.in
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/README.md
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.412743 geti-sdk-1.5.0/geti_sdk/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/annotation_readers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/base_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/annotation_readers/geti_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/algorithms.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/annotation_scene.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/annotations.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/code_deployment_info.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configuration.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/configuration_identifiers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.416743 geti-sdk-1.5.0/geti_sdk/data_models/containers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/containers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/containers/algorithm_list.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/containers/media_list.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/data_models/enums/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_kind.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/configuration_enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/deployment_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/domain.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/job_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/job_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/media_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/model_status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      943 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/optimization_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/prediction_mode.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/shape_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/enums/task_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/job.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/label.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/media.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/media_identifiers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8433 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/model_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/performance.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/predictions.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/project.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/shapes.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6544 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/task.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/task_annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/data_models/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/demos/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/constants.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.412743 geti-sdk-1.5.0/geti_sdk/demos/data/
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/demos/data/example/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data/example/dogs.png
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.420743 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6113 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/anomaly_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9051 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/coco_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5359 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/download_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1881 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/data_helpers/video_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/anomaly_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/coco_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/demos/demo_projects/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/deployment/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/deployment/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/deployment/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/deployment/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-04-24 09:06:25.000000 geti-sdk-1.5.0/geti_sdk/deployment/data_models/intermediate_inference_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/data_models/region_of_interest.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26525 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/deployed_model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/deployment.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/deployment/resources/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/resources/OVMS_README.md
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/resources/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/deployment/utils.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55063 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/geti.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/http_session/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/exception.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/geti_session.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/http_session/server_config.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6021 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/platform_versions.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/rest_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3575 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/configuration_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/dataset_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/deployment_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.424743 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/image_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16827 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/media_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/video_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/model_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/prediction_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/project_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/task_templates.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_clients/training_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/configuration_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/job_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/media_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/model_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/project_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/rest_converters/status_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/geti_sdk/utils/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/algorithm_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/credentials_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/dictionary_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/label_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/plot_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/serialization_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/geti_sdk/utils/workspace_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.412743 geti-sdk-1.5.0/geti_sdk.egg-info/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5718 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/requires.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-04-24 09:21:41.000000 geti-sdk-1.5.0/geti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/pyproject.toml
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/requirements/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements-dev.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements-docs.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements-notebooks.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/requirements/requirements.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/setup.cfg
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/setup.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.428743 geti-sdk-1.5.0/tests/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/conftest.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-04-24 09:21:41.432743 geti-sdk-1.5.0/tests/helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/constants.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/finalizers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/fixtures.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/plotting.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/project_service.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/training.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-04-24 09:06:26.000000 geti-sdk-1.5.0/tests/helpers/vcr_helpers.py
```

### Comparing `geti-sdk-1.4.1/LICENSE` & `geti-sdk-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/PKG-INFO` & `geti-sdk-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.4.1
+Version: 1.5.0
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
@@ -34,16 +34,17 @@
 - Project creation and upload from a previous download
 - Deploying a project for local inference with OpenVINO
 - Getting and setting project and model configuration
 - Launching and monitoring training jobs
 - Media upload and prediction
 
 This repository also contains a set of (tutorial style) Jupyter
-[notebooks](notebooks/README.md) that demonstrate how to use the SDK. We highly
-recommend checking them out to get a feeling for use cases for the package.
+[notebooks](https://github.com/openvinotoolkit/geti-sdk/tree/main/notebooks)
+that demonstrate how to use the SDK. We highly recommend checking them out to get a
+feeling for use cases for the package.
 
 # Getting started
 
 ## Installation
 Using an environment manager such as
 [Anaconda](https://www.anaconda.com/products/individual) or
 [venv](https://docs.python.org/3/library/venv.html) to create a new
@@ -274,24 +275,25 @@
 The `deployment.infer` method takes a numpy image as input.
 
 The `deployment.save` method will save the deployment to the folder named
 'dummy_project', on the local disk. The deployment can be reloaded again later using
 `Deployment.from_folder('dummy_project')`.
 
 ### Example scripts
-The [examples](examples/README.md) folder contains example scripts, showing various
-use cases for the package. They can be run by navigating to the `examples` directory
-in your terminal, and simply running the scripts like any other python script.
+The [examples](https://github.com/openvinotoolkit/geti-sdk/tree/main/examples)
+folder contains example scripts, showing various use cases for the package. They can
+be run by navigating to the `examples` directory in your terminal, and simply running
+the scripts like any other python script.
 
 ### Jupyter Notebooks
-In addition, the [notebooks](notebooks/README.md) folder contains Jupyter notebooks
-with example use cases for the `geti_sdk`. To run the notebooks,
-make sure that the requirements for the notebooks are installed in your Python
-environment. If you have not installed these when you were installing the SDK, you can
-install them at any time using
+In addition, the [notebooks](https://github.com/openvinotoolkit/geti-sdk/tree/main/notebooks)
+folder contains Jupyter notebooks with example use cases for the `geti_sdk`. To run
+the notebooks, make sure that the requirements for the notebooks are installed in your
+Python environment. If you have not installed these when you were installing the SDK,
+you can install them at any time using
 `pip install -r requirements/requirements-notebooks.txt`
 
 Once the notebook requirements are installed, navigate to the `notebooks` directory in
 your terminal. Then, launch JupyterLab by typing `jupyter lab`. This should open your
 browser and take you to the JupyterLab landing page, with the SDK notebooks open (see
 the screenshot below).
 
@@ -343,15 +345,15 @@
 
 
 - `create_task_chain_project_from_dataset` -- Creates a task chain project on the
   server, potentially using labels and uploading annotations from an external dataset.
 
 For further details regarding these methods, please refer to the method documentation,
 the [code snippets](#downloading-and-uploading-projects), and
-[example scripts](examples/README.md) provided in this repo.
+[example scripts](https://github.com/openvinotoolkit/geti-sdk/tree/main/examples) provided in this repo.
 
 Please visit the full documentation for a complete API reference.
 
 ## Using Docker
 
 The Dockerfile can be used to run the package without having to install python on your
 machine.
```

### Comparing `geti-sdk-1.4.1/README.md` & `geti-sdk-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 - Project creation and upload from a previous download
 - Deploying a project for local inference with OpenVINO
 - Getting and setting project and model configuration
 - Launching and monitoring training jobs
 - Media upload and prediction
 
 This repository also contains a set of (tutorial style) Jupyter
-[notebooks](notebooks/README.md) that demonstrate how to use the SDK. We highly
-recommend checking them out to get a feeling for use cases for the package.
+[notebooks](https://github.com/openvinotoolkit/geti-sdk/tree/main/notebooks)
+that demonstrate how to use the SDK. We highly recommend checking them out to get a
+feeling for use cases for the package.
 
 # Getting started
 
 ## Installation
 Using an environment manager such as
 [Anaconda](https://www.anaconda.com/products/individual) or
 [venv](https://docs.python.org/3/library/venv.html) to create a new
@@ -254,24 +255,25 @@
 The `deployment.infer` method takes a numpy image as input.
 
 The `deployment.save` method will save the deployment to the folder named
 'dummy_project', on the local disk. The deployment can be reloaded again later using
 `Deployment.from_folder('dummy_project')`.
 
 ### Example scripts
-The [examples](examples/README.md) folder contains example scripts, showing various
-use cases for the package. They can be run by navigating to the `examples` directory
-in your terminal, and simply running the scripts like any other python script.
+The [examples](https://github.com/openvinotoolkit/geti-sdk/tree/main/examples)
+folder contains example scripts, showing various use cases for the package. They can
+be run by navigating to the `examples` directory in your terminal, and simply running
+the scripts like any other python script.
 
 ### Jupyter Notebooks
-In addition, the [notebooks](notebooks/README.md) folder contains Jupyter notebooks
-with example use cases for the `geti_sdk`. To run the notebooks,
-make sure that the requirements for the notebooks are installed in your Python
-environment. If you have not installed these when you were installing the SDK, you can
-install them at any time using
+In addition, the [notebooks](https://github.com/openvinotoolkit/geti-sdk/tree/main/notebooks)
+folder contains Jupyter notebooks with example use cases for the `geti_sdk`. To run
+the notebooks, make sure that the requirements for the notebooks are installed in your
+Python environment. If you have not installed these when you were installing the SDK,
+you can install them at any time using
 `pip install -r requirements/requirements-notebooks.txt`
 
 Once the notebook requirements are installed, navigate to the `notebooks` directory in
 your terminal. Then, launch JupyterLab by typing `jupyter lab`. This should open your
 browser and take you to the JupyterLab landing page, with the SDK notebooks open (see
 the screenshot below).
 
@@ -323,15 +325,15 @@
 
 
 - `create_task_chain_project_from_dataset` -- Creates a task chain project on the
   server, potentially using labels and uploading annotations from an external dataset.
 
 For further details regarding these methods, please refer to the method documentation,
 the [code snippets](#downloading-and-uploading-projects), and
-[example scripts](examples/README.md) provided in this repo.
+[example scripts](https://github.com/openvinotoolkit/geti-sdk/tree/main/examples) provided in this repo.
 
 Please visit the full documentation for a complete API reference.
 
 ## Using Docker
 
 The Dockerfile can be used to run the package without having to install python on your
 machine.
```

### Comparing `geti-sdk-1.4.1/geti_sdk/__init__.py` & `geti-sdk-1.5.0/geti_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
    .. automethod:: upload_and_predict_media_folder
 
 """
 
 from .geti import Geti
 
-__version__ = "1.4.1"
+__version__ = "1.5.0"
 
 __all__ = ["Geti"]
```

### Comparing `geti-sdk-1.4.1/geti_sdk/annotation_readers/__init__.py` & `geti-sdk-1.5.0/geti_sdk/annotation_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/annotation_readers/base_annotation_reader.py` & `geti-sdk-1.5.0/geti_sdk/annotation_readers/base_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py` & `geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py` & `geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions
 # and limitations under the License.
 
 import copy
 import logging
 from typing import Dict, List, Optional, Sequence, Union
 
+from datumaro import Image
 from datumaro.components.annotation import Bbox, Polygon
 
 from geti_sdk.annotation_readers.base_annotation_reader import AnnotationReader
 from geti_sdk.data_models import Annotation as SCAnnotation
 from geti_sdk.data_models import TaskType
 from geti_sdk.data_models.enums.task_type import GLOBAL_TASK_TYPES
 from geti_sdk.data_models.media import MediaInformation
@@ -168,15 +169,15 @@
              - True when uploading annotations for a classification like task,
                 following a local task in a task chain project.
 
         :return: List of Annotation objects containing all annotations for the given
             dataset item.
         """
         ds_item = self.dataset.get_item_by_id(filename)
-        image_size = ds_item.image.size
+        image_size = ds_item.media_as(Image).size
         annotation_list: List[SCAnnotation] = []
         labels = []
 
         # Remove duplicate annotations, datumaro does not check for this
         datum_annotations = [
             i
             for n, i in enumerate(ds_item.annotations)
```

### Comparing `geti-sdk-1.4.1/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py` & `geti-sdk-1.5.0/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             'voc', 'coco', 'imagenet', etc.
         :param dataset_path: Path to the dataset on local disk
         """
         self.dataset_format = dataset_format
         self.dataset_path = dataset_path
         self.dataset, self.environment = self.create_datumaro_dataset()
         self._subset_names = self.dataset.subsets().keys()
+        self._filtered_categories = self.dataset.categories()[AnnotationType.label]
 
     def prepare_dataset(
         self, task_type: TaskType, previous_task_type: Optional[TaskType] = None
     ) -> Dataset:
         """
         Prepare the dataset for uploading to Sonoma Creek.
 
@@ -99,16 +100,15 @@
         self._subset_names = self.dataset.subsets().keys()
 
     @property
     def categories(self) -> LabelCategories:
         """
         Return the LabelCategories in the dataset.
         """
-        categories: LabelCategories = self.dataset.categories()[AnnotationType.label]
-        return categories
+        return self._filtered_categories
 
     @property
     def label_names(self) -> List[str]:
         """
         Return a list of all label names in the dataset.
         """
         return [item.name for item in self.categories]
@@ -197,25 +197,26 @@
             # better way in Datumaro but haven't found it yet
             label_categories = LabelCategories.from_iterable(labels)
             new_labelmap = {}
             for label in labels:
                 label_key = get_dict_key_from_value(label_map, label)
                 new_labelmap[label_key] = label
             label_categories._indices = {v: k for k, v in new_labelmap.items()}
-            new_categories = {AnnotationType.label: label_categories}
+            new_categories = label_categories
             # Filter and create a new dataset to update the dataset categories
             self.dataset = Dataset.from_iterable(
                 self.dataset.select(lambda item: select_function(item, labels)),
-                categories=new_categories,
+                categories=self.dataset.categories(),
                 env=self.dataset.env,
             )
             logging.info(
                 f"After filtering, dataset with labels {labels} contains "
                 f"{len(self.dataset)} items."
             )
+            self._filtered_categories = new_categories
 
     def __get_item_by_id_from_subsets(
         self, datum_id: str, search_by_name: bool = False
     ) -> Optional[DatasetItem]:
         """
         Search all subsets for the item with id `datum_id`
```

### Comparing `geti-sdk-1.4.1/geti_sdk/annotation_readers/directory_tree_annotation_reader.py` & `geti-sdk-1.5.0/geti_sdk/annotation_readers/directory_tree_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/annotation_readers/geti_annotation_reader.py` & `geti-sdk-1.5.0/geti_sdk/annotation_readers/geti_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/__init__.py` & `geti-sdk-1.5.0/geti_sdk/data_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 from .job import Job
 from .label import Label, ScoredLabel
 from .media import Image, MediaItem, Video, VideoFrame
 from .model import Model, OptimizedModel
 from .model_group import ModelGroup, ModelSummary
 from .performance import Performance
 from .predictions import Prediction
-from .project import Pipeline, Project
+from .project import Dataset, Pipeline, Project
 from .status import ProjectStatus
 from .task import Task
 
 __all__ = [
     "TaskType",
     "AnnotationKind",
     "Project",
@@ -206,8 +206,9 @@
     "Model",
     "ModelGroup",
     "OptimizedModel",
     "ModelSummary",
     "ProjectStatus",
     "Job",
     "CodeDeploymentInformation",
+    "Dataset",
 ]
```

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/algorithms.py` & `geti-sdk-1.5.0/geti_sdk/data_models/algorithms.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/annotation_scene.py` & `geti-sdk-1.5.0/geti_sdk/data_models/annotation_scene.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/annotations.py` & `geti-sdk-1.5.0/geti_sdk/data_models/annotations.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/code_deployment_info.py` & `geti-sdk-1.5.0/geti_sdk/data_models/code_deployment_info.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/configurable_parameter.py` & `geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/configurable_parameter_group.py` & `geti-sdk-1.5.0/geti_sdk/data_models/configurable_parameter_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/configuration.py` & `geti-sdk-1.5.0/geti_sdk/data_models/configuration.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/configuration_identifiers.py` & `geti-sdk-1.5.0/geti_sdk/data_models/configuration_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/containers/__init__.py` & `geti-sdk-1.5.0/geti_sdk/data_models/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/containers/algorithm_list.py` & `geti-sdk-1.5.0/geti_sdk/data_models/containers/algorithm_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/containers/media_list.py` & `geti-sdk-1.5.0/geti_sdk/data_models/containers/media_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/__init__.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/annotation_kind.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_kind.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/annotation_state.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/configuration_enums.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/configuration_enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/deployment_state.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/deployment_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/domain.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/domain.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/job_state.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/job_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/job_type.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/job_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/media_type.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/media_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/model_status.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/model_status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/optimization_type.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/optimization_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/prediction_mode.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/prediction_mode.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/shape_type.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/shape_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/enums/task_type.py` & `geti-sdk-1.5.0/geti_sdk/data_models/enums/task_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/job.py` & `geti-sdk-1.5.0/geti_sdk/data_models/job.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/label.py` & `geti-sdk-1.5.0/geti_sdk/data_models/label.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/media.py` & `geti-sdk-1.5.0/geti_sdk/data_models/media.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/media_identifiers.py` & `geti-sdk-1.5.0/geti_sdk/data_models/media_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/model.py` & `geti-sdk-1.5.0/geti_sdk/data_models/model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/model_group.py` & `geti-sdk-1.5.0/geti_sdk/data_models/model_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/performance.py` & `geti-sdk-1.5.0/geti_sdk/data_models/performance.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/predictions.py` & `geti-sdk-1.5.0/geti_sdk/data_models/predictions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/project.py` & `geti-sdk-1.5.0/geti_sdk/data_models/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -358,7 +358,16 @@
             zip(self.get_trainable_tasks(), self.pipeline.get_labels_per_task())
         ):
             summary_str += (
                 f"  Task {task_index+1}: {task.title}\n    Labels: "
                 f"{[label.name for label in labels]}\n"
             )
         return summary_str
+
+    @property
+    def training_dataset(self) -> Dataset:
+        """
+        Return the training dataset for the project.
+
+        :return: Training dataset for the project
+        """
+        return [dataset for dataset in self.datasets if dataset.use_for_training][0]
```

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/shapes.py` & `geti-sdk-1.5.0/geti_sdk/data_models/shapes.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/status.py` & `geti-sdk-1.5.0/geti_sdk/data_models/status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/task.py` & `geti-sdk-1.5.0/geti_sdk/data_models/task.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/task_annotation_state.py` & `geti-sdk-1.5.0/geti_sdk/data_models/task_annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/data_models/utils.py` & `geti-sdk-1.5.0/geti_sdk/data_models/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/__init__.py` & `geti-sdk-1.5.0/geti_sdk/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/constants.py` & `geti-sdk-1.5.0/geti_sdk/demos/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/data/example/dogs.png` & `geti-sdk-1.5.0/geti_sdk/demos/data/example/dogs.png`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/data_helpers/__init__.py` & `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/data_helpers/anomaly_helpers.py` & `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/anomaly_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/data_helpers/coco_helpers.py` & `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/coco_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/data_helpers/download_helpers.py` & `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/download_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/data_helpers/video_helpers.py` & `geti-sdk-1.5.0/geti_sdk/demos/data_helpers/video_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/demo_projects/__init__.py` & `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/demo_projects/anomaly_demos.py` & `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/anomaly_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/demo_projects/coco_demos.py` & `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/coco_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/demos/demo_projects/utils.py` & `geti-sdk-1.5.0/geti_sdk/demos/demo_projects/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/__init__.py` & `geti-sdk-1.5.0/geti_sdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/data_models/__init__.py` & `geti-sdk-1.5.0/geti_sdk/deployment/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/data_models/intermediate_inference_result.py` & `geti-sdk-1.5.0/geti_sdk/deployment/data_models/intermediate_inference_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/data_models/region_of_interest.py` & `geti-sdk-1.5.0/geti_sdk/deployment/data_models/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/deployed_model.py` & `geti-sdk-1.5.0/geti_sdk/deployment/deployed_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 WRAPPER_DIR_NAME = "model_wrappers"
 
 LABELS_CONFIG_KEY = "labels"
 LABEL_TREE_KEY = "label_tree"
 LABEL_GROUPS_KEY = "label_groups"
 ALL_LABELS_KEY = "all_labels"
 
+SALIENCY_KEY = "saliency_map"
+ANOMALY_SALIENCY_KEY = "anomaly_map"
+SEGMENTATION_SALIENCY_KEY = "soft_prediction"
+FEATURE_VECTOR_KEY = "feature_vector"
+
 OVMS_TIMEOUT = 10  # Max time to wait for OVMS models to become available
 
 
 @attr.define
 class DeployedModel(OptimizedModel):
     """
     Representation of an Intel® Geti™ model that has been deployed for inference. It
@@ -71,14 +76,21 @@
         super().__attrs_post_init__()
         self._model_data_path: Optional[str] = None
         self._model_python_path: Optional[str] = None
         self._needs_tempdir_deletion: bool = False
         self._tempdir_path: Optional[str] = None
         self._has_custom_model_wrappers: bool = False
         self._label_schema: Optional[LabelSchemaEntity] = None
+
+        # Attributes related to model explainability
+        self._saliency_key: Optional[str] = None
+        self._saliency_location: Optional[str] = None
+        self._feature_vector_key: Optional[str] = None
+        self._feature_vector_location: Optional[str] = None
+
         self.openvino_model_parameters: Optional[Dict[str, Any]] = None
 
     @property
     def model_data_path(self) -> str:
         """
         Return the path to the raw model data
 
@@ -464,38 +476,90 @@
 
         :param inference_results: Dictionary holding the results of inference
         :param metadata: Dictionary holding metadata
         :return: Tuple containing postprocessed outputs, formatted as follows:
             - Numpy array containing the saliency map
             - Numpy array containing the feature vector
         """
-        saliency_key = "saliency_map"
-        fvector_key = "feature_vector"
-        if hasattr(self._inference_model, "postprocess_aux_outputs"):
-            (
-                _,
-                saliency_map,
-                repr_vector,
-                _,
-            ) = self._inference_model.postprocess_aux_outputs(
-                inference_results, metadata
-            )
-        elif (
-            saliency_key in inference_results.keys()
-            and fvector_key in inference_results.keys()
-        ):
-            saliency_map = inference_results[saliency_key]
-            repr_vector = inference_results[fvector_key]
-        elif saliency_key in metadata.keys() and fvector_key in metadata.keys():
-            saliency_map = metadata[saliency_key]
-            repr_vector = metadata[fvector_key]
+        if self._saliency_location is None and self._feature_vector_location is None:
+            # When running postprocessing for the first time, we need to determine the
+            # key and location of the saliency map and feature vector.
+            if hasattr(self._inference_model, "postprocess_aux_outputs"):
+                (
+                    _,
+                    saliency_map,
+                    repr_vector,
+                    _,
+                ) = self._inference_model.postprocess_aux_outputs(
+                    inference_results, metadata
+                )
+                self._saliency_location = "aux"
+                self._feature_vector_location = "aux"
+            else:
+                # Check all possible saliency map keys in outputs and metadata
+                if SALIENCY_KEY in inference_results.keys():
+                    saliency_map = inference_results[SALIENCY_KEY]
+                    self._saliency_location = "output"
+                    self._saliency_key = SALIENCY_KEY
+                elif SALIENCY_KEY in metadata.keys():
+                    saliency_map = metadata[SALIENCY_KEY]
+                    self._saliency_location = "meta"
+                    self._saliency_key = SALIENCY_KEY
+                elif ANOMALY_SALIENCY_KEY in metadata.keys():
+                    saliency_map = metadata[ANOMALY_SALIENCY_KEY]
+                    self._saliency_location = "meta"
+                    self._saliency_key = ANOMALY_SALIENCY_KEY
+                elif SEGMENTATION_SALIENCY_KEY in metadata.keys():
+                    saliency_map = metadata[SEGMENTATION_SALIENCY_KEY]
+                    self._saliency_location = "meta"
+                    self._saliency_key = SEGMENTATION_SALIENCY_KEY
+                else:
+                    logging.warning("No saliency map found in model output")
+                    saliency_map = None
+
+                # Check all possible feature vector keys in outputs and metadata
+                if FEATURE_VECTOR_KEY in inference_results.keys():
+                    repr_vector = inference_results[FEATURE_VECTOR_KEY]
+                    self._feature_vector_location = "output"
+                    self._feature_vector_key = FEATURE_VECTOR_KEY
+                elif FEATURE_VECTOR_KEY in metadata.keys():
+                    repr_vector = metadata[FEATURE_VECTOR_KEY]
+                    self._feature_vector_location = "meta"
+                    self._feature_vector_key = FEATURE_VECTOR_KEY
+                else:
+                    logging.warning("No feature vector found in model output")
+                    repr_vector = None
         else:
-            logging.warning("No saliency map or feature vector found in model output")
-            saliency_map = None
-            repr_vector = None
+            # If location of feature vector and saliency map are already known, we can
+            # use them directly
+            if self._saliency_location == "aux":
+                (
+                    _,
+                    saliency_map,
+                    repr_vector,
+                    _,
+                ) = self._inference_model.postprocess_aux_outputs(
+                    inference_results, metadata
+                )
+                return saliency_map, repr_vector
+            elif self._saliency_location == "meta":
+                saliency_map = metadata[self._saliency_key]
+            elif self._saliency_location == "output":
+                saliency_map = inference_results[self._saliency_key]
+            else:
+                logging.warning("No saliency map found in model output")
+                saliency_map = None
+            if self._feature_vector_location == "meta":
+                repr_vector = metadata[self._feature_vector_key]
+            elif self._feature_vector_location == "output":
+                repr_vector = inference_results[self._feature_vector_key]
+
+            else:
+                logging.warning("No feature vector found in model output")
+                repr_vector = None
         return saliency_map, repr_vector
 
     def infer(self, preprocessed_image: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
         """
         Run inference on an already preprocessed image.
 
         :param preprocessed_image: Dictionary holding the preprocessing results for an
```

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/deployment.py` & `geti-sdk-1.5.0/geti_sdk/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/resources/OVMS_README.md` & `geti-sdk-1.5.0/geti_sdk/deployment/resources/OVMS_README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/resources/__init__.py` & `geti-sdk-1.5.0/geti_sdk/deployment/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/deployment/utils.py` & `geti-sdk-1.5.0/geti_sdk/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/geti.py` & `geti-sdk-1.5.0/geti_sdk/geti.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,27 +24,36 @@
 from tqdm.contrib.logging import logging_redirect_tqdm
 
 from .annotation_readers import (
     AnnotationReader,
     DatumAnnotationReader,
     GetiAnnotationReader,
 )
-from .data_models import Image, Prediction, Project, TaskType, Video, VideoFrame
+from .data_models import (
+    Dataset,
+    Image,
+    Prediction,
+    Project,
+    TaskType,
+    Video,
+    VideoFrame,
+)
 from .data_models.containers import MediaList
 from .data_models.model import BaseModel
 from .deployment import Deployment
 from .http_session import (
     GetiRequestException,
     GetiSession,
     ServerCredentialConfig,
     ServerTokenConfig,
 )
 from .rest_clients import (
     AnnotationClient,
     ConfigurationClient,
+    DatasetClient,
     DeploymentClient,
     ImageClient,
     ModelClient,
     PredictionClient,
     ProjectClient,
     VideoClient,
 )
@@ -329,26 +338,15 @@
                 append_video_uid=videos.has_duplicate_filenames,
             )
 
         # Download annotations
         annotation_client = AnnotationClient(
             session=self.session, project=project, workspace_id=self.workspace_id
         )
-        if len(images) > 0:
-            annotation_client.download_annotations_for_images(
-                images=images,
-                path_to_folder=target_folder,
-                append_image_uid=images.has_duplicate_filenames,
-            )
-        if len(videos) > 0:
-            annotation_client.download_annotations_for_videos(
-                videos=videos,
-                path_to_folder=target_folder,
-                append_video_uid=videos.has_duplicate_filenames,
-            )
+        annotation_client.download_all_annotations(path_to_folder=target_folder)
 
         # Download predictions
         prediction_client = PredictionClient(
             workspace_id=self.workspace_id, session=self.session, project=project
         )
         if prediction_client.ready_to_predict and include_predictions:
             if len(images) > 0:
@@ -431,35 +429,59 @@
 
         # Disable auto-train to prevent the project from training right away
         configuration_client = ConfigurationClient(
             workspace_id=self.workspace_id, session=self.session, project=project
         )
         configuration_client.set_project_auto_train(auto_train=False)
 
-        # Upload images
+        # Upload media
         image_client = ImageClient(
             workspace_id=self.workspace_id, session=self.session, project=project
         )
-        images = image_client.upload_folder(
-            path_to_folder=os.path.join(target_folder, "images")
-        )
-
-        # Upload videos
         video_client = VideoClient(
             workspace_id=self.workspace_id, session=self.session, project=project
         )
-        videos = video_client.upload_folder(
-            path_to_folder=os.path.join(target_folder, "videos")
-        )
 
-        media_lists: List[Union[MediaList[Image], MediaList[Video]]] = []
-        if len(images) > 0:
-            media_lists.append(images)
-        if len(videos) > 0:
-            media_lists.append(videos)
+        # Check the media folders inside the project folder. If they are organized
+        # according to the projects datasets, upload the media into their corresponding
+        # dataset. Otherwise, upload all media into training dataset.
+        dataset_client = DatasetClient(
+            workspace_id=self.workspace_id, session=self.session, project=project
+        )
+        if len(project.datasets) == 1 or not dataset_client.has_dataset_subfolders(
+            target_folder
+        ):
+            # Upload all media directly to the training dataset
+            images = image_client.upload_folder(
+                path_to_folder=os.path.join(target_folder, "images")
+            )
+            videos = video_client.upload_folder(
+                path_to_folder=os.path.join(target_folder, "videos")
+            )
+        else:
+            # Make sure that media is uploaded to the correct dataset
+            images: MediaList[Image] = MediaList([])
+            videos: MediaList[Video] = MediaList([])
+            for dataset in project.datasets:
+                images.extend(
+                    image_client.upload_folder(
+                        path_to_folder=os.path.join(
+                            target_folder, "images", dataset.name
+                        ),
+                        dataset=dataset,
+                    )
+                )
+                videos.extend(
+                    video_client.upload_folder(
+                        path_to_folder=os.path.join(
+                            target_folder, "videos", dataset.name
+                        ),
+                        dataset=dataset,
+                    )
+                )
 
         # Short sleep to make sure all uploaded media is processed server side
         time.sleep(5)
 
         # Upload annotations
         annotation_reader = GetiAnnotationReader(
             base_data_folder=os.path.join(target_folder, "annotations"),
@@ -971,33 +993,44 @@
 
     def upload_and_predict_image(
         self,
         project_name: str,
         image: Union[np.ndarray, Image, VideoFrame, str, os.PathLike],
         visualise_output: bool = True,
         delete_after_prediction: bool = False,
+        dataset_name: Optional[str] = None,
     ) -> Tuple[Image, Prediction]:
         """
         Upload a single image to a project named `project_name` on the Intel® Geti™
         server, and return a prediction for it.
 
         :param project_name: Name of the project to upload the image to
         :param image: Image, numpy array representing an image, or filepath to an
             image to upload and get a prediction for
         :param visualise_output: True to show the resulting prediction, overlayed on
             the image
         :param delete_after_prediction: True to remove the image from the project
             once the prediction is received, False to keep the image in the project.
+        :param dataset_name: Optional name of the dataset to which to upload the
+            image. The dataset must already exist in the project
         :return: Tuple containing:
 
             - Image object representing the image that was uploaded
             - Prediction for the image
         """
         project = self.get_project(project_name=project_name)
 
+        # Get the dataset to upload to
+        dataset: Optional[Dataset] = None
+        if dataset_name is not None:
+            dataset_client = DatasetClient(
+                session=self.session, workspace_id=self.workspace_id, project=project
+            )
+            dataset = dataset_client.get_dataset_by_name(dataset_name=dataset_name)
+
         # Upload the image
         image_client = ImageClient(
             session=self.session, workspace_id=self.workspace_id, project=project
         )
         needs_upload = True
         if isinstance(image, Image):
             if image.id in image_client.get_all_images().ids:
@@ -1009,15 +1042,17 @@
         else:
             image_data = image
         if needs_upload:
             if image_data is None:
                 raise ValueError(
                     f"Cannot upload entity {image}. No data available for upload."
                 )
-            uploaded_image = image_client.upload_image(image=image_data)
+            uploaded_image = image_client.upload_image(
+                image=image_data, dataset=dataset
+            )
         else:
             uploaded_image = image
 
         # Get prediction
         prediction_client = PredictionClient(
             session=self.session, workspace_id=self.workspace_id, project=project
         )
```

### Comparing `geti-sdk-1.4.1/geti_sdk/http_session/__init__.py` & `geti-sdk-1.5.0/geti_sdk/http_session/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/http_session/exception.py` & `geti-sdk-1.5.0/geti_sdk/http_session/exception.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/http_session/geti_session.py` & `geti-sdk-1.5.0/geti_sdk/http_session/geti_session.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/http_session/server_config.py` & `geti-sdk-1.5.0/geti_sdk/http_session/server_config.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/platform_versions.py` & `geti-sdk-1.5.0/geti_sdk/platform_versions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/__init__.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 Module contents
 ---------------
 
 .. autoclass:: geti_sdk.rest_clients.project_client.project_client.ProjectClient
    :members:
    :undoc-members:
 
+.. autoclass:: geti_sdk.rest_clients.dataset_client.DatasetClient
+   :members:
+
 .. autoclass:: geti_sdk.rest_clients.media_client.image_client.ImageClient
    :members:
 
 .. autoclass:: geti_sdk.rest_clients.media_client.video_client.VideoClient
    :members:
 
 .. autoclass:: geti_sdk.rest_clients.annotation_clients.annotation_client.AnnotationClient
@@ -83,24 +86,26 @@
 .. autoclass:: geti_sdk.rest_clients.deployment_client.DeploymentClient
    :members:
 
 """
 
 from .annotation_clients import AnnotationClient
 from .configuration_client import ConfigurationClient
+from .dataset_client import DatasetClient
 from .deployment_client import DeploymentClient
 from .media_client import ImageClient, VideoClient
 from .model_client import ModelClient
 from .prediction_client import PredictionClient
 from .project_client import ProjectClient
 from .training_client import TrainingClient
 
 __all__ = [
     "AnnotationClient",
     "ConfigurationClient",
+    "DatasetClient",
     "ProjectClient",
     "VideoClient",
     "ImageClient",
     "PredictionClient",
     "ModelClient",
     "TrainingClient",
     "DeploymentClient",
```

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/annotation_clients/__init__.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/annotation_clients/annotation_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/annotation_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -260,19 +260,23 @@
 
         :param path_to_folder: Folder to save the annotations to
         """
         image_list = self._get_all_media_by_type(media_type=Image)
         video_list = self._get_all_media_by_type(media_type=Video)
         if len(image_list) > 0:
             self.download_annotations_for_images(
-                images=image_list, path_to_folder=path_to_folder
+                images=image_list,
+                path_to_folder=path_to_folder,
+                append_image_uid=image_list.has_duplicate_filenames,
             )
         if len(video_list) > 0:
             self.download_annotations_for_videos(
-                video_list, path_to_folder=path_to_folder
+                video_list,
+                path_to_folder=path_to_folder,
+                append_video_uid=video_list.has_duplicate_filenames,
             )
 
     def upload_annotations_for_all_media(self, append_annotations: bool = False):
         """
         Upload annotations for all media in the project, If append_annotations is set
         to True, annotations will be appended to the existing annotations for the
         media on the server. If set to False, existing annotations will be overwritten.
```

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     Image,
     Project,
     Video,
     VideoFrame,
 )
 from geti_sdk.data_models.containers.media_list import MediaList
 from geti_sdk.data_models.media import MediaInformation
+from geti_sdk.data_models.project import Dataset
 from geti_sdk.http_session import GetiRequestException, GetiSession
+from geti_sdk.rest_clients.dataset_client import DatasetClient
 from geti_sdk.rest_converters import AnnotationRESTConverter
 from geti_sdk.rest_converters.annotation_rest_converter import (
     NormalizedAnnotationRESTConverter,
 )
 
 AnnotationReaderType = TypeVar("AnnotationReaderType", bound=AnnotationReader)
 MediaType = TypeVar("MediaType", Image, Video)
@@ -59,33 +61,57 @@
         self.annotation_reader = annotation_reader
         self._project = project
         if annotation_reader is None:
             label_mapping = None
         else:
             label_mapping = self.__get_label_mapping(project)
         self._label_mapping = label_mapping
+        self._dataset_client = DatasetClient(
+            session=session, project=project, workspace_id=workspace_id
+        )
 
     def _get_all_media_by_type(
         self, media_type: Type[MediaType]
     ) -> MediaList[MediaType]:
         """
         Get a list holding all media entities of type `media_type` in the project.
 
+        :param media_type: Type of media item to retrieve. Can be 'Image' or 'Video'
         :return: MediaList holding all media of a certain type in the project
         """
+        datasets = self._dataset_client.get_all_datasets()
+        media_list = MediaList[media_type]([])
+        for dataset in datasets:
+            media_list.extend(
+                self._get_all_media_in_dataset_by_type(
+                    media_type=media_type, dataset=dataset
+                )
+            )
+        return media_list
+
+    def _get_all_media_in_dataset_by_type(
+        self, media_type: Type[MediaType], dataset: Dataset
+    ) -> MediaList[MediaType]:
+        """
+        Return a list of all media items of type `media_type` in the dataset `dataset`
+
+        :param media_type: Type of media item to retrieve. Can be 'Image' or 'Video'
+        :param dataset: Dataset to retrieve media items for
+        :return: List of all media items of a certain media_type in the dataset
+        """
         if media_type == Image:
             media_name = "images"
         elif media_type == Video:
             media_name = "videos"
         else:
             raise ValueError(f"Invalid media type specified: {media_type}.")
         get_media_url = (
             f"workspaces/{self.workspace_id}/projects/{self._project.id}"
-            f"/datasets/{self._project.datasets[0].id}/media/"
-            f"{media_name}?top=100000"
+            f"/datasets/{dataset.id}/media/"
+            f"{media_name}?top=500"
         )
         response = self.session.get_rest_response(url=get_media_url, method="GET")
         total_number_of_media: int = response["media_count"][media_name]
         raw_media_list: List[Dict[str, Any]] = []
         while len(raw_media_list) < total_number_of_media:
             for media_item_dict in response["media"]:
                 raw_media_list.append(media_item_dict)
```

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/configuration_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/configuration_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/deployment_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/deployment_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/__init__.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/image_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/image_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,81 +12,96 @@
 # See the License for the specific language governing permissions
 # and limitations under the License.
 
 import datetime
 import glob
 import io
 import os
-from typing import List, Sequence, Union
+from typing import List, Optional, Sequence, Union
 
 import cv2
 import numpy as np
 
 from geti_sdk.data_models import Image, MediaType
 from geti_sdk.data_models.containers import MediaList
+from geti_sdk.data_models.project import Dataset
 from geti_sdk.rest_converters import MediaRESTConverter
 
 from .media_client import MEDIA_SUPPORTED_FORMAT_MAPPING, BaseMediaClient
 
 
 class ImageClient(BaseMediaClient[Image]):
     """
     Class to manage image uploads and downloads for a certain project.
     """
 
     _MEDIA_TYPE = MediaType.IMAGE
 
-    def get_all_images(self) -> MediaList[Image]:
+    def get_all_images(self, dataset: Optional[Dataset] = None) -> MediaList[Image]:
         """
-        Get the ID's and filenames of all images in the project.
+        Get the ID's and filenames of all images in the project, from a specific
+        dataset. If no dataset is passed, images from the training dataset will be
+        returned
 
-        :return: MediaList containing all Image entities in the project
+        :param dataset: Dataset for which to retrieve the images. If no dataset is
+            passed, images from the training dataset are returned.
+        :return: MediaList containing all Image entities in the dataset
         """
-        return self._get_all()
+        return self._get_all(dataset=dataset)
 
-    def upload_image(self, image: Union[np.ndarray, str, os.PathLike]) -> Image:
+    def upload_image(
+        self,
+        image: Union[np.ndarray, str, os.PathLike],
+        dataset: Optional[Dataset] = None,
+    ) -> Image:
         """
         Upload an image file to the server.
 
         :param image: full path to the image on disk, or numpy array representing the
             image
+        :param dataset: Dataset to which to upload the image. If no dataset is
+            passed, the image is uploaded to the training dataset
         :return: Image object representing the uploaded image on the server
         """
         if isinstance(image, (str, os.PathLike)):
-            image_dict = self._upload(image)
+            image_dict = self._upload(image, dataset=dataset)
         elif isinstance(image, np.ndarray):
             image_io = io.BytesIO(cv2.imencode(".jpg", image)[1].tobytes())
             time_now = datetime.datetime.now()
             image_io.name = f"numpy_{time_now.strftime('%Y-%m-%dT%H-%M-%S.%f')}.jpg"
-            image_dict = self._upload_bytes(image_io)
+            image_dict = self._upload_bytes(image_io, dataset=dataset)
         else:
             raise TypeError(f"Invalid image type: {type(image)}.")
         return MediaRESTConverter.from_dict(input_dict=image_dict, media_type=Image)
 
     def upload_folder(
         self,
         path_to_folder: str,
         n_images: int = -1,
         skip_if_filename_exists: bool = False,
+        dataset: Optional[Dataset] = None,
     ) -> MediaList[Image]:
         """
         Upload all images in a folder to the project. Returns a MediaList containing
         all images in the project after upload.
 
         :param path_to_folder: Folder with images to upload
         :param n_images: Number of images to upload from folder
         :param skip_if_filename_exists: Set to True to skip uploading of an image
             if an image with the same filename already exists in the project.
             Defaults to False
+        :param dataset: Dataset to which to upload the images. If no dataset is
+            passed, the images are uploaded to the training dataset
         :return: MediaList containing all image's in the project
         """
         return self._upload_folder(
             path_to_folder=path_to_folder,
             n_media=n_images,
             skip_if_filename_exists=skip_if_filename_exists,
+            dataset=dataset,
         )
 
     def download_all(self, path_to_folder: str, append_image_uid: bool = False) -> None:
         """
         Download all images in a project to a folder on the local disk.
 
         :param path_to_folder: path to the folder in which the images should be saved
@@ -102,15 +117,16 @@
         self,
         path_to_folder: str,
         image_names: List[str],
         extension_included: bool = False,
         n_images: int = -1,
         skip_if_filename_exists: bool = False,
         image_names_as_full_paths: bool = False,
-    ):
+        dataset: Optional[Dataset] = None,
+    ) -> MediaList[Image]:
         """
         From a folder containing images `path_to_folder`, this method uploads only
         those images that have their filenames included in the `image_names` list.
 
         :param path_to_folder: Folder containing the images
         :param image_names: List of names of the images that should be uploaded
         :param extension_included: Set to True if the extension of the image is
@@ -118,17 +134,17 @@
             False
         :param n_images: Number of images to upload from the list
         :param skip_if_filename_exists: Set to True to skip uploading of an image
             if an image with the same filename already exists in the project.
             Defaults to False
         :param image_names_as_full_paths: Set to True if the list of `image_names`
             contains full paths to the images, rather than just the filenames
-        :return: Dictionary containing a mapping between the ID's of the images and
-            their filenames (excluding extensions). NOTE: Filenames are used as keys,
-            ID's as values
+        :param dataset: Dataset to which to upload the images. If no dataset is
+            passed, the images are uploaded to the training dataset
+        :return: List of images that were uploaded
         """
         media_formats = MEDIA_SUPPORTED_FORMAT_MAPPING[self._MEDIA_TYPE]
 
         if n_images > len(image_names) or n_images == -1:
             n_to_upload = len(image_names)
         else:
             n_to_upload = n_images
@@ -166,15 +182,17 @@
                 elif len(matches) != 1:
                     raise ValueError(
                         f"Multiple files found for image with name {image_name}: "
                         f"{matches}"
                     )
                 image_filepaths.append(matches[0])
         return self._upload_loop(
-            filepaths=image_filepaths, skip_if_filename_exists=skip_if_filename_exists
+            filepaths=image_filepaths,
+            skip_if_filename_exists=skip_if_filename_exists,
+            dataset=dataset,
         )
 
     def delete_images(self, images: Sequence[Image]) -> bool:
         """
         Delete all Image entities in `images` from the project.
 
         :param images: List of Image entities to delete
```

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/media_client/media_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/media_client/media_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,27 +11,39 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 import logging
 import os
 import time
 from glob import glob
-from typing import Any, BinaryIO, ClassVar, Dict, Generic, List, Sequence, Type
+from typing import (
+    Any,
+    BinaryIO,
+    ClassVar,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    Sequence,
+    Type,
+)
 
 from tqdm.auto import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
 from geti_sdk.data_models import Image, MediaType, Project, Video, VideoFrame
 from geti_sdk.data_models.containers.media_list import MediaList, MediaTypeVar
 from geti_sdk.data_models.enums.media_type import (
     SUPPORTED_IMAGE_FORMATS,
     SUPPORTED_VIDEO_FORMATS,
 )
+from geti_sdk.data_models.project import Dataset
 from geti_sdk.data_models.utils import numpy_from_buffer
 from geti_sdk.http_session import GetiRequestException, GetiSession
+from geti_sdk.rest_clients.dataset_client import DatasetClient
 from geti_sdk.rest_converters.media_rest_converter import MediaRESTConverter
 
 MEDIA_TYPE_MAPPING = {MediaType.IMAGE: Image, MediaType.VIDEO: Video}
 MEDIA_SUPPORTED_FORMAT_MAPPING = {
     MediaType.IMAGE: SUPPORTED_IMAGE_FORMATS,
     MediaType.VIDEO: SUPPORTED_VIDEO_FORMATS,
 }
@@ -43,31 +55,30 @@
     Class to manage media up and downloads for a certain project.
     """
 
     _MEDIA_TYPE: ClassVar[MediaType]
 
     def __init__(self, session: GetiSession, workspace_id: str, project: Project):
         self.session = session
-        project_id = project.id
-        dataset_id = project.datasets[0].id
-        self._base_url = (
-            f"workspaces/{workspace_id}/projects/{project_id}/datasets/"
-            f"{dataset_id}/media"
-        )
-        self._project_name = project.name
+        self._workspace_id = workspace_id
+        self._base_url = f"workspaces/{workspace_id}/projects/{project.id}/datasets/"
+        self._project = project
         self.__media_type: Type[MediaTypeVar] = self.__get_media_type(self._MEDIA_TYPE)
+        self._dataset_client = DatasetClient(
+            session=session, project=project, workspace_id=workspace_id
+        )
 
-    @property
-    def base_url(self) -> str:
+    def base_url(self, dataset: Dataset) -> str:
         """
         Return the base url for the media endpoint.
 
+        :param dataset: Dataset to retrieve the base url for
         :return: string containing the base url
         """
-        return f"{self._base_url}/{self.plural_media_name}"
+        return f"{self._base_url}/{dataset.id}/media/{self.plural_media_name}"
 
     @property
     def plural_media_name(self) -> str:
         """
         Convert the type of the media entities managed by this media client to a
         string in plural form.
 
@@ -83,22 +94,27 @@
         :param media_type: MediaType Enum instance representing the type of media
             entities
         :return: Type of media entities that can be used to instantiate objects of this
             type
         """
         return MEDIA_TYPE_MAPPING[media_type]
 
-    def _get_all(self) -> MediaList[MediaTypeVar]:
+    def _get_all(self, dataset: Optional[Dataset] = None) -> MediaList[MediaTypeVar]:
         """
         Get a list holding all media entities of a certain type in the project.
 
+        :param dataset: Optional dataset to retrieve the media for. If no dataset is
+            specified, only media from the training dataset will be returned
         :return: MediaList holding all media of a certain type in the project
         """
+        if dataset is None:
+            dataset = self._project.training_dataset
+
         response = self.session.get_rest_response(
-            url=f"{self.base_url}?top=500", method="GET"
+            url=f"{self.base_url(dataset=dataset)}?top=500", method="GET"
         )
         total_number_of_media: int = response["media_count"][self.plural_media_name]
         raw_media_list: List[Dict[str, Any]] = []
         while len(raw_media_list) < total_number_of_media:
             for media_item_dict in response["media"]:
                 raw_media_list.append(media_item_dict)
             if "next_page" in response.keys():
@@ -119,91 +135,108 @@
         """
         if not isinstance(media_list, MediaList) and isinstance(media_list, Sequence):
             media_list = MediaList(media_list)
         if media_list.media_type == VideoFrame:
             raise ValueError("Unable to delete individual video frames.")
         logging.info(
             f"Deleting {len(media_list)} {self.plural_media_name} from project "
-            f"'{self._project_name}'..."
+            f"'{self._project.name}'..."
         )
         for media_item in media_list:
             try:
                 self.session.get_rest_response(url=media_item.base_url, method="DELETE")
             except GetiRequestException as error:
                 if error.status_code == 409:
                     logging.info(
-                        f"Project '{self._project_name}' is locked for deletion, "
+                        f"Project '{self._project.name}' is locked for deletion, "
                         f"unable to delete media. Aborting deletion."
                     )
                     return False
                 if error.status_code == 404 or error.status_code == 204:
                     # Media item has already been deleted, continue with the rest of
                     # the list
                     continue
         return True
 
-    def _upload_bytes(self, buffer: BinaryIO) -> Dict[str, Any]:
+    def _upload_bytes(
+        self, buffer: BinaryIO, dataset: Optional[Dataset] = None
+    ) -> Dict[str, Any]:
         """
         Upload a buffer representing a media file to the server.
 
         :param buffer: BinaryIO object representing a media file
+        :param dataset: Dataset to upload the media to. If no dataset is passed, the
+            media will be uploaded into the default (training) dataset
         :return: Dictionary containing the response of the Intel® Geti™ server, which
             holds the details of the uploaded entity
         """
+        if dataset is None:
+            dataset = self._project.training_dataset
         response = self.session.get_rest_response(
-            url=f"{self.base_url}",
+            url=f"{self.base_url(dataset)}",
             method="POST",
             contenttype="multipart",
             data={"file": buffer},
         )
         return response
 
-    def _upload(self, filepath: str) -> Dict[str, Any]:
+    def _upload(
+        self, filepath: str, dataset: Optional[Dataset] = None
+    ) -> Dict[str, Any]:
         """
         Upload a media file to the server.
 
         :param filepath: full path to the media file on disk
+        :param dataset: Dataset to upload the media to. If no dataset is passed, the
+            media will be uploaded into the default (training) dataset
         :return: Dictionary containing the response of the Intel® Geti™ server, which
             holds the details of the uploaded entity
         """
         media_bytes = open(filepath, "rb")
-        return self._upload_bytes(media_bytes)
+        return self._upload_bytes(media_bytes, dataset=dataset)
 
     def _upload_loop(
         self,
         filepaths: List[str],
         skip_if_filename_exists: bool = False,
+        dataset: Optional[Dataset] = None,
     ) -> MediaList[MediaTypeVar]:
         """
         Upload media from a list of filepaths. Also checks if media items with the same
         filename exist in the project, to make sure no duplicate items are uploaded.
 
         :param filepaths: List of full filepaths for media that should be
             uploaded
         :param skip_if_filename_exists: Set to True to skip uploading of a media item
-            if a media item with the same filename already exists in the project.
+            if a media item with the same filename already exists in the dataset.
             Defaults to False
+        :param dataset: Dataset to upload the media to. If no dataset is passed, the
+            media will be uploaded into the default (training) dataset
         :return: MediaList containing a list of all media entities that were uploaded
             to the project
         """
-        media_in_project = self._get_all()
+        if dataset is None:
+            dataset = self._project.training_dataset
+        media_in_project = self._get_all(dataset=dataset)
         uploaded_media: MediaList[MediaTypeVar] = MediaList[MediaTypeVar]([])
         upload_count = 0
         skip_count = 0
-        logging.info(f"Starting {self._MEDIA_TYPE} upload...")
+        logging.info(
+            f"Starting {self._MEDIA_TYPE} upload to dataset '{dataset.name}'..."
+        )
         tqdm_prefix = f"Uploading {self.plural_media_name}"
 
         t_start = time.time()
         with logging_redirect_tqdm(tqdm_class=tqdm):
             for filepath in tqdm(filepaths, desc=tqdm_prefix):
                 name, ext = os.path.splitext(os.path.basename(filepath))
                 if name in media_in_project.names and skip_if_filename_exists:
                     skip_count += 1
                     continue
-                media_dict = self._upload(filepath=filepath)
+                media_dict = self._upload(filepath=filepath, dataset=dataset)
                 media_item = MediaRESTConverter.from_dict(
                     input_dict=media_dict, media_type=self.__media_type
                 )
                 if isinstance(media_item, Video):
                     media_item._data = filepath
                 media_in_project.append(media_item)
                 uploaded_media.append(media_item)
@@ -227,24 +260,27 @@
         return uploaded_media
 
     def _upload_folder(
         self,
         path_to_folder: str,
         n_media: int = -1,
         skip_if_filename_exists: bool = False,
+        dataset: Optional[Dataset] = None,
     ) -> MediaList[MediaTypeVar]:
         """
         Upload all media in a folder to the project. Returns the mapping of filenames
         to the unique IDs assigned by Sonoma Creek.
 
         :param path_to_folder: Folder with media items to upload
         :param n_media: Number of media to upload from folder
         :param skip_if_filename_exists: Set to True to skip uploading of a media item
             if a media item with the same filename already exists in the project.
             Defaults to False
+        :param dataset: Dataset to upload the media to. If no dataset is passed, the
+            media will be uploaded into the default (training) dataset
         :return: MediaList containing a list of all media entities that were uploaded
             to the project
         """
         media_formats = MEDIA_SUPPORTED_FORMAT_MAPPING[self._MEDIA_TYPE]
         filepaths: List[str] = []
         for media_extension in media_formats:
             filepaths += glob(
@@ -260,34 +296,73 @@
                 f"to signify uploading all files in the folder. "
             )
         else:
             n_to_upload = n_files if n_files < n_media else n_media
         return self._upload_loop(
             filepaths=filepaths[0:n_to_upload],
             skip_if_filename_exists=skip_if_filename_exists,
+            dataset=dataset,
         )
 
     def _download_all(
         self, path_to_folder: str, append_media_uid: bool = False
     ) -> None:
         """
         Download all media entities in a project to a folder on the local disk.
 
         :param path_to_folder: path to the folder in which the media should be saved
         :param append_media_uid: True to append the UID of a media item to the
             filename (separated from the original filename by an underscore, i.e.
             '{filename}_{media_id}').
         :return:
         """
-        media_list = self._get_all()
-        path_to_media_folder = os.path.join(path_to_folder, self.plural_media_name)
+        datasets = self._dataset_client.get_all_datasets()
+        if len(datasets) == 1:
+            # 1 dataset in project, do not split media in separate folder per dataset
+            path_to_media_folder = os.path.join(path_to_folder, self.plural_media_name)
+            self._download_dataset(
+                dataset=datasets[0],
+                path_to_media_folder=path_to_media_folder,
+                append_media_uid=append_media_uid,
+            )
+        else:
+            # Multiple datasets in the project, create a subfolder for media in each
+            # dataset
+            for dataset in datasets:
+                path_to_media_folder = os.path.join(
+                    path_to_folder, self.plural_media_name, dataset.name
+                )
+                self._download_dataset(
+                    dataset=dataset,
+                    path_to_media_folder=path_to_media_folder,
+                    append_media_uid=append_media_uid,
+                )
+
+    def _download_dataset(
+        self,
+        dataset: Dataset,
+        path_to_media_folder: str,
+        append_media_uid: bool = False,
+    ):
+        """
+        Download all media items of a single type in the dataset to a folder on disk
+
+        :param dataset: Dataset to download the media for
+        :param path_to_media_folder: path to the folder in which the media should be
+            saved
+        :param append_media_uid: True to append the UID of a media item to the
+            filename (separated from the original filename by an underscore, i.e.
+            '{filename}_{media_id}').
+        """
+        media_list = self._get_all(dataset=dataset)
         os.makedirs(path_to_media_folder, exist_ok=True, mode=0o770)
         logging.info(
             f"Downloading {len(media_list)} {self.plural_media_name} from project "
-            f"'{self._project_name}' to folder {path_to_media_folder}..."
+            f"'{self._project.name}' and dataset '{dataset.name}' to folder "
+            f"{path_to_media_folder}..."
         )
         t_start = time.time()
         download_count = 0
         existing_count = 0
         tqdm_prefix = f"Downloading {self.plural_media_name}"
         with logging_redirect_tqdm(tqdm_class=tqdm):
             for media_item in tqdm(media_list, desc=tqdm_prefix):
```

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/model_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/model_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/prediction_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/prediction_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/project_client/__init__.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/project_client/project_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/project_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import logging
 import os
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from geti_sdk.data_models import Project, Task, TaskType
 from geti_sdk.data_models.utils import remove_null_fields
 from geti_sdk.http_session import GetiRequestException, GetiSession
+from geti_sdk.rest_clients.dataset_client import DatasetClient
 from geti_sdk.rest_converters import ProjectRESTConverter
 from geti_sdk.utils.label_helpers import generate_unique_label_color
 from geti_sdk.utils.project_helpers import get_task_types_by_project_type
 
 from .task_templates import (
     ANOMALY_CLASSIFICATION_TASK,
     ANOMALY_DETECTION_TASK,
@@ -57,32 +58,44 @@
     """
 
     def __init__(self, session: GetiSession, workspace_id: str):
         self.session = session
         self.workspace_id = workspace_id
         self.base_url = f"workspaces/{workspace_id}/"
 
-    def get_all_projects(self) -> List[Project]:
+    def get_all_projects(self, request_page_size: int = 50) -> List[Project]:
         """
         Return a list of projects found on the Intel® Geti™ server
 
+        :param request_page_size: Max number of projects to fetch in a single HTTP
+            request. Higher values may reduce the response time of this method when
+            there are many projects, but increase the chance of timeout.
         :return: List of Project objects, containing the project information for each
             project on the Intel® Geti™ server
         """
-        project_list = self.session.get_rest_response(
-            url=f"{self.base_url}projects",
-            method="GET",
-        )
         if self.session.version.is_sc_mvp or self.session.version.is_sc_1_1:
             project_key = "items"
         else:
             project_key = "projects"
+        num_total_projects_key = "project_counts"
+
+        # The 'projects' endpoint uses pagination: multiple HTTP may be necessary to
+        # fetch the full list of projects
+        project_list: List[Dict] = []
+        while response := self.session.get_rest_response(
+            url=f"{self.base_url}projects?limit={request_page_size}&skip={len(project_list)}",
+            method="GET",
+        ):
+            project_list.extend(response[project_key])
+            if len(project_list) >= response[num_total_projects_key]:
+                break
+
         return [
             ProjectRESTConverter.from_dict(project_input=project)
-            for project in project_list[project_key]
+            for project in project_list
         ]
 
     def get_project_by_name(self, project_name: str) -> Optional[Project]:
         """
         Get a project from the Intel® Geti™ server by project_name.
 
         :param project_name: Name of the project to get
@@ -288,15 +301,27 @@
         if project_name is not None:
             project.name = project_name
         logging.info(
             f"Creating project '{project.name}' from parameters in "
             f"configuration file at {path_to_project}."
         )
         project.prepare_for_post()
-        return self.get_or_create_project(**project.get_parameters())
+        datasets = project.datasets
+        created_project = self.get_or_create_project(**project.get_parameters())
+        if len(datasets) > 1:
+            # Create the additional datasets if needed
+            dataset_client = DatasetClient(
+                session=self.session,
+                workspace_id=self.workspace_id,
+                project=created_project,
+            )
+            for dataset in datasets:
+                if dataset.name not in [ds.name for ds in created_project.datasets]:
+                    dataset_client.create_dataset(name=dataset.name)
+        return created_project
 
     @staticmethod
     def is_project_dir(path_to_folder: str) -> bool:
         """
         Check if the folder specified in `path_to_folder` is a directory
         containing valid Intel® Geti™ project data that can be used to upload to an
         Intel® Geti™ server.
```

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/project_client/task_templates.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/project_client/task_templates.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_clients/training_client.py` & `geti-sdk-1.5.0/geti_sdk/rest_clients/training_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/__init__.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/annotation_rest_converter/__init__.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/configuration_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/configuration_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/job_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/job_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/media_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/media_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/model_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/model_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/prediction_rest_converter/__init__.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/project_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/project_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/rest_converters/status_rest_converter.py` & `geti-sdk-1.5.0/geti_sdk/rest_converters/status_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/__init__.py` & `geti-sdk-1.5.0/geti_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/algorithm_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/algorithm_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/credentials_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/dictionary_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/dictionary_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/label_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/label_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/plot_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/project_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/serialization_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk/utils/workspace_helpers.py` & `geti-sdk-1.5.0/geti_sdk/utils/workspace_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/geti_sdk.egg-info/PKG-INFO` & `geti-sdk-1.5.0/geti_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.4.1
+Version: 1.5.0
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
@@ -34,16 +34,17 @@
 - Project creation and upload from a previous download
 - Deploying a project for local inference with OpenVINO
 - Getting and setting project and model configuration
 - Launching and monitoring training jobs
 - Media upload and prediction
 
 This repository also contains a set of (tutorial style) Jupyter
-[notebooks](notebooks/README.md) that demonstrate how to use the SDK. We highly
-recommend checking them out to get a feeling for use cases for the package.
+[notebooks](https://github.com/openvinotoolkit/geti-sdk/tree/main/notebooks)
+that demonstrate how to use the SDK. We highly recommend checking them out to get a
+feeling for use cases for the package.
 
 # Getting started
 
 ## Installation
 Using an environment manager such as
 [Anaconda](https://www.anaconda.com/products/individual) or
 [venv](https://docs.python.org/3/library/venv.html) to create a new
@@ -274,24 +275,25 @@
 The `deployment.infer` method takes a numpy image as input.
 
 The `deployment.save` method will save the deployment to the folder named
 'dummy_project', on the local disk. The deployment can be reloaded again later using
 `Deployment.from_folder('dummy_project')`.
 
 ### Example scripts
-The [examples](examples/README.md) folder contains example scripts, showing various
-use cases for the package. They can be run by navigating to the `examples` directory
-in your terminal, and simply running the scripts like any other python script.
+The [examples](https://github.com/openvinotoolkit/geti-sdk/tree/main/examples)
+folder contains example scripts, showing various use cases for the package. They can
+be run by navigating to the `examples` directory in your terminal, and simply running
+the scripts like any other python script.
 
 ### Jupyter Notebooks
-In addition, the [notebooks](notebooks/README.md) folder contains Jupyter notebooks
-with example use cases for the `geti_sdk`. To run the notebooks,
-make sure that the requirements for the notebooks are installed in your Python
-environment. If you have not installed these when you were installing the SDK, you can
-install them at any time using
+In addition, the [notebooks](https://github.com/openvinotoolkit/geti-sdk/tree/main/notebooks)
+folder contains Jupyter notebooks with example use cases for the `geti_sdk`. To run
+the notebooks, make sure that the requirements for the notebooks are installed in your
+Python environment. If you have not installed these when you were installing the SDK,
+you can install them at any time using
 `pip install -r requirements/requirements-notebooks.txt`
 
 Once the notebook requirements are installed, navigate to the `notebooks` directory in
 your terminal. Then, launch JupyterLab by typing `jupyter lab`. This should open your
 browser and take you to the JupyterLab landing page, with the SDK notebooks open (see
 the screenshot below).
 
@@ -343,15 +345,15 @@
 
 
 - `create_task_chain_project_from_dataset` -- Creates a task chain project on the
   server, potentially using labels and uploading annotations from an external dataset.
 
 For further details regarding these methods, please refer to the method documentation,
 the [code snippets](#downloading-and-uploading-projects), and
-[example scripts](examples/README.md) provided in this repo.
+[example scripts](https://github.com/openvinotoolkit/geti-sdk/tree/main/examples) provided in this repo.
 
 Please visit the full documentation for a complete API reference.
 
 ## Using Docker
 
 The Dockerfile can be used to run the package without having to install python on your
 machine.
```

### Comparing `geti-sdk-1.4.1/geti_sdk.egg-info/SOURCES.txt` & `geti-sdk-1.5.0/geti_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 geti_sdk/deployment/resources/__init__.py
 geti_sdk/http_session/__init__.py
 geti_sdk/http_session/exception.py
 geti_sdk/http_session/geti_session.py
 geti_sdk/http_session/server_config.py
 geti_sdk/rest_clients/__init__.py
 geti_sdk/rest_clients/configuration_client.py
+geti_sdk/rest_clients/dataset_client.py
 geti_sdk/rest_clients/deployment_client.py
 geti_sdk/rest_clients/model_client.py
 geti_sdk/rest_clients/prediction_client.py
 geti_sdk/rest_clients/training_client.py
 geti_sdk/rest_clients/annotation_clients/__init__.py
 geti_sdk/rest_clients/annotation_clients/annotation_client.py
 geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
```

### Comparing `geti-sdk-1.4.1/geti_sdk.egg-info/requires.txt` & `geti-sdk-1.5.0/geti_sdk.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-datumaro==1.0.*
+datumaro==1.1.*
 requests==2.28.*
 numpy==1.22.*
-omegaconf==2.1.*
+omegaconf==2.3.*
 opencv-python==4.5.*
 python-dotenv==1.0.*
 tqdm==4.65.*
-Pillow==9.4.*
+Pillow==9.5.*
 pathvalidate>=2.5.0
-simplejson==3.18.*
+simplejson==3.19.*
 ipython==8.11.*
-otx==1.1.0
+otx==1.1.2
 openvino==2022.3.0
 openmodelzoo-modelapi==2022.3.*
 certifi>=2022.12.7
 joblib>=1.1.1
 protobuf>=3.20.2
 ovmsclient>=2022.3
 orjson==3.8.8
```

### Comparing `geti-sdk-1.4.1/setup.py` & `geti-sdk-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/__init__.py` & `geti-sdk-1.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/conftest.py` & `geti-sdk-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/__init__.py` & `geti-sdk-1.5.0/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/constants.py` & `geti-sdk-1.5.0/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/enums.py` & `geti-sdk-1.5.0/tests/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/finalizers.py` & `geti-sdk-1.5.0/tests/helpers/finalizers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/fixtures.py` & `geti-sdk-1.5.0/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/plotting.py` & `geti-sdk-1.5.0/tests/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/project_helpers.py` & `geti-sdk-1.5.0/tests/helpers/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/project_service.py` & `geti-sdk-1.5.0/tests/helpers/project_service.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/training.py` & `geti-sdk-1.5.0/tests/helpers/training.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.4.1/tests/helpers/vcr_helpers.py` & `geti-sdk-1.5.0/tests/helpers/vcr_helpers.py`

 * *Files identical despite different names*

