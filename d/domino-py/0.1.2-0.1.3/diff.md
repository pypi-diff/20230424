# Comparing `tmp/domino-py-0.1.2.tar.gz` & `tmp/domino-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.1.2.tar", last modified: Thu Apr  6 13:16:22 2023, max compression
+gzip compressed data, was "domino-py-0.1.3.tar", last modified: Mon Apr 24 17:02:15 2023, max compression
```

## Comparing `domino-py-0.1.2.tar` & `domino-py-0.1.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.349886 domino-py-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-06 13:16:12.000000 domino-py-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-06 13:16:12.000000 domino-py-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-06 13:16:22.349886 domino-py-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-06 13:16:12.000000 domino-py-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.341886 domino-py-0.1.2/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.341886 domino-py-0.1.2/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.341886 domino-py-0.1.2/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/utils/create_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/custom_operators/sidecar/sidecar_lifecycle.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/helm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/helm/domino-airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-airflow/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/helm/domino-airflow/charts/
--rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-airflow/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/helm/domino-base/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/Chart.lock
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/helm/domino-base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/domino-backend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/domino-frontend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/domino-postgres-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/ingress-api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/ingress-frontend.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/helm/domino-base/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/jobs/domino-migrations.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/helm/domino-base/templates/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/volumes/domino-backend-volume-claim-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/templates/volumes/domino-backend-volume-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/helm/domino-base/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/piece_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.345886 domino-py-0.1.2/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.349886 domino-py-0.1.2/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/generate_infrasctructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/run_piece_dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.349886 domino-py-0.1.2/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/utils/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/utils/enum_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/utils/types_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 13:16:12.000000 domino-py-0.1.2/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:16:22.349886 domino-py-0.1.2/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-06 13:16:22.000000 domino-py-0.1.2/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-06 13:16:22.000000 domino-py-0.1.2/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:16:22.000000 domino-py-0.1.2/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-06 13:16:22.000000 domino-py-0.1.2/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-06 13:16:22.000000 domino-py-0.1.2/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-06 13:16:22.000000 domino-py-0.1.2/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-06 13:16:12.000000 domino-py-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:16:22.349886 domino-py-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-06 13:16:12.000000 domino-py-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.408615 domino-py-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 17:02:04.000000 domino-py-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-24 17:02:04.000000 domino-py-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:02:15.408615 domino-py-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-24 17:02:04.000000 domino-py-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.400615 domino-py-0.1.3/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.400615 domino-py-0.1.3/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.400615 domino-py-0.1.3/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/utils/config-domino-local.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/utils/create_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    18589 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/sidecar/fuse.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/sidecar/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/sidecar/rclone.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/custom_operators/sidecar/sidecar_lifecycle.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/helm/domino-airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-airflow/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/helm/domino-airflow/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-airflow/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/helm/domino-base/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/Chart.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/helm/domino-base/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/domino-backend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/domino-frontend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/domino-postgres-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/ingress-api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/ingress-frontend.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/helm/domino-base/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/jobs/domino-migrations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/helm/domino-base/templates/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/volumes/domino-backend-volume-claim-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/templates/volumes/domino-backend-volume-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/helm/domino-base/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/piece_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.404615 domino-py-0.1.3/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.408615 domino-py-0.1.3/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/generate_infrasctructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/run_piece_dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.408615 domino-py-0.1.3/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/utils/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/utils/enum_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/utils/types_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 17:02:04.000000 domino-py-0.1.3/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:02:15.408615 domino-py-0.1.3/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:02:15.000000 domino-py-0.1.3/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-24 17:02:15.000000 domino-py-0.1.3/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:02:15.000000 domino-py-0.1.3/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 17:02:15.000000 domino-py-0.1.3/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-24 17:02:15.000000 domino-py-0.1.3/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 17:02:15.000000 domino-py-0.1.3/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 17:02:04.000000 domino-py-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:02:15.408615 domino-py-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-24 17:02:04.000000 domino-py-0.1.3/setup.py
```

### Comparing `domino-py-0.1.2/LICENSE.md` & `domino-py-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/MANIFEST.in` & `domino-py-0.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/PKG-INFO` & `domino-py-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description: [<img src="https://img.shields.io/pypi/v/flowui-project?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">](https://pypi.org/project/flowui-project/)
         [<img src="https://img.shields.io/docker/v/taufferconsulting/flowui-backend?label=Backend&logo=docker&style=flat">](https://hub.docker.com/r/taufferconsulting/flowui-backend)
```

### Comparing `domino-py-0.1.2/README.md` & `domino-py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/base_piece.py` & `domino-py-0.1.3/domino/base_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/cli/cli.py` & `domino-py-0.1.3/domino/cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
 def get_workflows_repository_from_env():
     return os.environ.get("DOMINO_WORKFLOWS_REPOSITORY", None)
 
 def get_local_operators_repository_path():
     return ""
 
+def get_registry_token_from_env():
+    return os.environ.get('REGISTRY_TOKEN', "")
+
 @click.command()
 @click.option(
     '--cluster-name', 
     prompt='Local cluster name', 
     default=get_cluster_name_from_env,
     help='Define the name for the local k8s cluster.'
 )
@@ -213,35 +216,29 @@
     expose_value=True,
     default=False,
     help='If True (default), builds Docker images.'
 )
 @click.option(
     '--publish-images', 
     is_flag=True,
-    prompt='Publish Docker images?',
+    #prompt='Publish Docker images?',
     expose_value=True,
     default=False,
     help='If True (default), publishes Docker images to Dockerhub.'
 )
 @click.option(
-    '--dockerhub-username', 
-    prompt='Dockerhub username',
-    default=get_dockerhub_username_from_env,
-    help='Your username from DockerHub account.'
-)
-@click.option(
-    '--dockerhub-password', 
-    prompt='Dockerhub password',
-    default=get_dockerhub_password_from_env,
-    help='Your password from DockerHub account.'
+    '--registry-token',
+    #prompt='Github Container Registry token',
+    default=get_registry_token_from_env,
+    help='Your Github Container Registry token with access to where the image will be published.'
 )
-def cli_organize_pieces_repository(build_images, publish_images, dockerhub_username, dockerhub_password):
+def cli_organize_pieces_repository(build_images, publish_images, registry_token):
     """Prepare local folder for running a Domino platform."""
-    os.environ['DOCKERHUB_USERNAME'] = dockerhub_username
-    os.environ['DOCKERHUB_PASSWORD'] = dockerhub_password
+    os.environ['CR_PAT'] = registry_token
+    console.print(f"Using registry token to publish images")
     pieces_repository.organize_pieces_repository(build_images, publish_images)
 
 
 @click.command()
 def cli_create_release():
     """
     Get release version for the Pieces repository in github stdout format.
```

### Comparing `domino-py-0.1.2/domino/cli/utils/config-domino-local.toml` & `domino-py-0.1.3/domino/cli/utils/config-domino-local.toml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/cli/utils/create_cluster.sh` & `domino-py-0.1.3/domino/cli/utils/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/cli/utils/pieces_repository.py` & `domino-py-0.1.3/domino/cli/utils/pieces_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,30 +261,37 @@
     console.print("")
 
 
 def create_compiled_pieces_metadata() -> None:  
     """
     Create compiled metadata from Pieces metadata.json files and include input_schema generated from models.py
     """
-    from domino.scripts.load_piece import load_piece_models_from_path
+    from domino.scripts.load_piece import load_piece_models_from_path, load_piece_class_from_path
     from domino.utils.metadata_default import metadata_default
 
     pieces_path = Path(".") / "pieces"
     compiled_metadata = dict()
     for op_dir in pieces_path.glob("*Piece"):
         if op_dir.is_dir():
-            piece_name = op_dir.name
+
+            piece_class = load_piece_class_from_path(
+                pieces_folder_path=str(pieces_path),
+                piece_name=op_dir.name,
+            )
+            piece_name = piece_class.__name__
 
             # Update with user-defined metadata.json
             metadata = copy.deepcopy(metadata_default)
             if (op_dir / "metadata.json").is_file():
                 with open(str(op_dir / "metadata.json"), "r") as f:
                     metadata_op = json.load(f)
-                metadata_op['name'] = piece_name
+                metadata_op['name'] = metadata_op.get('name', piece_name)
                 dict_deep_update(metadata, metadata_op)
+            else:
+                metadata['name'] = piece_name
 
             # Add input and output schemas
             input_model_class, output_model_class, secrets_model_class = load_piece_models_from_path(
                 pieces_folder_path=str(pieces_path), 
                 piece_name=op_dir.name
             )
             metadata["input_schema"] = input_model_class.schema()
```

### Comparing `domino-py-0.1.2/domino/cli/utils/platform.py` & `domino-py-0.1.3/domino/cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/client/airflow_client.py` & `domino-py-0.1.3/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/client/domino_backend_client.py` & `domino-py-0.1.3/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/client/fs_client.py` & `domino-py-0.1.3/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/client/github_rest_client.py` & `domino-py-0.1.3/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/client/local_files_client.py` & `domino-py-0.1.3/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/client/s3_client.py` & `domino-py-0.1.3/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/custom_operators/bash_operator.py` & `domino-py-0.1.3/domino/custom_operators/bash_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/custom_operators/k8s_operator.py` & `domino-py-0.1.3/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/custom_operators/python_operator.py` & `domino-py-0.1.3/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/custom_operators/sidecar/logger.py` & `domino-py-0.1.3/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/custom_operators/sidecar/mount.py` & `domino-py-0.1.3/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/exceptions/exceptions.py` & `domino-py-0.1.3/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz` & `domino-py-0.1.3/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/helm/domino-airflow/values.yaml` & `domino-py-0.1.3/domino/helm/domino-airflow/values.yaml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/helm/domino-base/templates/domino-backend-deployment.yml` & `domino-py-0.1.3/domino/helm/domino-base/templates/domino-backend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/helm/domino-base/templates/domino-frontend-deployment.yml` & `domino-py-0.1.3/domino/helm/domino-base/templates/domino-frontend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/helm/domino-base/templates/domino-postgres-deployment.yml` & `domino-py-0.1.3/domino/helm/domino-base/templates/domino-postgres-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/helm/domino-base/templates/jobs/domino-migrations.yml` & `domino-py-0.1.3/domino/helm/domino-base/templates/jobs/domino-migrations.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/logger.py` & `domino-py-0.1.3/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/schemas/piece_metadata.py` & `domino-py-0.1.3/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/schemas/shared_storage.py` & `domino-py-0.1.3/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.1.3/domino/scripts/build_docker_images_pieces.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,27 +67,27 @@
     # Get information from config.toml file
     with open(config_path, "rb") as f:
         config_dict = tomli.load(f)
     docker_image_repository = config_dict.get("repository").get("REPOSITORY_NAME")
     docker_image_version = config_dict.get("repository").get("VERSION")
 
     if publish:
-        dockerhub_registry_name = config_dict.get("dockerhub").get("REGISTRY_NAME")
+        github_container_registry_name = f'ghcr.io/{config_dict.get("dockerhub").get("REGISTRY_NAME")}'
     else:
-        dockerhub_registry_name = "local"
+        github_container_registry_name = f'ghcr.io/{config_dict.get("dockerhub").get("REGISTRY_NAME")}'
 
     # Load dependencies_map.json file
     with open(domino_path / "dependencies_map.json", "r") as f:
         pieces_dependencies_map = json.load(f)
 
     # Build docker images from unique definitions
     for group, v in pieces_dependencies_map.items():
         dependency_dockerfile = v["dependency"].get("dockerfile", None)
         dependency_requirements = v["dependency"].get("requirements_file", None)
-        source_image_name = f"{dockerhub_registry_name}/{docker_image_repository}:{docker_image_version}-{group}"
+        source_image_name = f"{github_container_registry_name}/{docker_image_repository}:{docker_image_version}-{group}"
 
         # If no extra dependency, use base worker image and just copy Operators source code
         if not any([dependency_dockerfile, dependency_requirements]):
             pieces_dependencies_map[group]["source_image"] = source_image_name
             # TODO change base image to domino when we have it
             dockerfile_str = f"""FROM taufferconsulting/flowui-airflow-pod:latest
 COPY config.toml domino/pieces_repository/
```

### Comparing `domino-py-0.1.2/domino/scripts/create_docker_compose_file.py` & `domino-py-0.1.3/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/scripts/docker_compose_constants.py` & `domino-py-0.1.3/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/scripts/docker_compose_scripts.py` & `domino-py-0.1.3/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/scripts/generate_infrasctructure.py` & `domino-py-0.1.3/domino/scripts/generate_infrasctructure.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/scripts/load_piece.py` & `domino-py-0.1.3/domino/scripts/load_piece.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pathlib import Path
 import importlib
 import sys
 
 
-def load_piece_class_from_path(pieces_folder_path: str, piece_name: str, piece_metadata: dict):
+def load_piece_class_from_path(pieces_folder_path: str, piece_name: str, piece_metadata: dict = None):
     # Import Operator from path, then set up piece module and class
     pieces_folder_path = str(Path(pieces_folder_path).resolve())
     if pieces_folder_path not in sys.path:
         sys.path.append(pieces_folder_path)
 
     importlib.invalidate_caches()
     piece_module = importlib.import_module(f"{piece_name}.piece")
     piece_class = getattr(piece_module, piece_name)
 
     # Set Operator class metadata
-    piece_class.set_metadata(metadata=piece_metadata)
+    if piece_metadata:
+        piece_class.set_metadata(metadata=piece_metadata)
 
     return piece_class
 
 
 def load_piece_models_from_path(pieces_folder_path: str, piece_name: str):
     # Import Operator from mounted volume, then set up piece module and class
     pieces_folder_path = str(Path(pieces_folder_path).resolve())
```

### Comparing `domino-py-0.1.2/domino/scripts/run_piece_bash.py` & `domino-py-0.1.3/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/scripts/run_piece_dry.py` & `domino-py-0.1.3/domino/scripts/run_piece_dry.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/scripts/run_piece_k8s.py` & `domino-py-0.1.3/domino/scripts/run_piece_k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def run_piece():
      # Import Operator from File System, already configured with metadata
     piece_name = os.getenv("DOMINO_K8S_PIECE")
 
     pieces_repository_copy_path = Path("domino/pieces_repository").resolve()
     pieces_folder_path = pieces_repository_copy_path / "pieces"
     compiled_metadata_path = pieces_repository_copy_path / ".domino/compiled_metadata.json"
-    
+
     with open(str(compiled_metadata_path), "r") as f:
         compiled_metadata = json.load(f)
 
     piece_class = load_piece_class_from_path(
         pieces_folder_path=pieces_folder_path,
         piece_name=piece_name,
         piece_metadata=compiled_metadata[piece_name]
```

### Comparing `domino-py-0.1.2/domino/task.py` & `domino-py-0.1.3/domino/task.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino/utils/validators.py` & `domino-py-0.1.3/domino/utils/validators.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/domino_py.egg-info/PKG-INFO` & `domino-py-0.1.3/domino_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description: [<img src="https://img.shields.io/pypi/v/flowui-project?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">](https://pypi.org/project/flowui-project/)
         [<img src="https://img.shields.io/docker/v/taufferconsulting/flowui-backend?label=Backend&logo=docker&style=flat">](https://hub.docker.com/r/taufferconsulting/flowui-backend)
```

### Comparing `domino-py-0.1.2/domino_py.egg-info/SOURCES.txt` & `domino-py-0.1.3/domino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.2/setup.py` & `domino-py-0.1.3/setup.py`

 * *Files identical despite different names*

