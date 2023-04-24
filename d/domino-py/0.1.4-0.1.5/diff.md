# Comparing `tmp/domino-py-0.1.4.tar.gz` & `tmp/domino-py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.1.4.tar", last modified: Mon Apr 24 17:12:26 2023, max compression
+gzip compressed data, was "domino-py-0.1.5.tar", last modified: Mon Apr 24 17:48:19 2023, max compression
```

## Comparing `domino-py-0.1.4.tar` & `domino-py-0.1.5.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.688560 domino-py-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 17:12:15.000000 domino-py-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-24 17:12:15.000000 domino-py-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:12:26.688560 domino-py-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-24 17:12:15.000000 domino-py-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/utils/create_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/custom_operators/sidecar/sidecar_lifecycle.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.680559 domino-py-0.1.4/domino/helm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/helm/domino-airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-airflow/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/helm/domino-airflow/charts/
--rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-airflow/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/helm/domino-base/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/Chart.lock
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/helm/domino-base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/domino-backend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/domino-frontend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/domino-postgres-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/ingress-api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/ingress-frontend.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/helm/domino-base/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/jobs/domino-migrations.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/helm/domino-base/templates/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/volumes/domino-backend-volume-claim-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/templates/volumes/domino-backend-volume-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/helm/domino-base/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/piece_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/generate_infrasctructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/run_piece_dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.684560 domino-py-0.1.4/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/utils/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/utils/enum_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/utils/types_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 17:12:15.000000 domino-py-0.1.4/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:12:26.688560 domino-py-0.1.4/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:12:26.000000 domino-py-0.1.4/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-24 17:12:26.000000 domino-py-0.1.4/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:12:26.000000 domino-py-0.1.4/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 17:12:26.000000 domino-py-0.1.4/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-24 17:12:26.000000 domino-py-0.1.4/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 17:12:26.000000 domino-py-0.1.4/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 17:12:15.000000 domino-py-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:12:26.688560 domino-py-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-24 17:12:15.000000 domino-py-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.850681 domino-py-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 17:48:08.000000 domino-py-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-24 17:48:08.000000 domino-py-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:48:19.850681 domino-py-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-24 17:48:08.000000 domino-py-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/config-domino-local.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/create_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.842681 domino-py-0.1.5/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/fuse.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/rclone.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/custom_operators/sidecar/sidecar_lifecycle.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-airflow/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-airflow/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-airflow/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/Chart.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/domino-backend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/domino-frontend-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/domino-postgres-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/ingress-api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/ingress-frontend.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/jobs/domino-migrations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/helm/domino-base/templates/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/volumes/domino-backend-volume-claim-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/templates/volumes/domino-backend-volume-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/helm/domino-base/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/piece_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/generate_infrasctructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/run_piece_dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.846681 domino-py-0.1.5/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/enum_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/types_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 17:48:08.000000 domino-py-0.1.5/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:48:19.850681 domino-py-0.1.5/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 17:48:19.000000 domino-py-0.1.5/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 17:48:08.000000 domino-py-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:48:19.850681 domino-py-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-24 17:48:08.000000 domino-py-0.1.5/setup.py
```

### Comparing `domino-py-0.1.4/LICENSE.md` & `domino-py-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/MANIFEST.in` & `domino-py-0.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/PKG-INFO` & `domino-py-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description: [<img src="https://img.shields.io/pypi/v/flowui-project?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">](https://pypi.org/project/flowui-project/)
         [<img src="https://img.shields.io/docker/v/taufferconsulting/flowui-backend?label=Backend&logo=docker&style=flat">](https://hub.docker.com/r/taufferconsulting/flowui-backend)
```

### Comparing `domino-py-0.1.4/README.md` & `domino-py-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/base_piece.py` & `domino-py-0.1.5/domino/base_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/cli/cli.py` & `domino-py-0.1.5/domino/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,28 +50,22 @@
 
 def get_github_token_pieces_from_env():
     return os.environ.get("DOMINO_GITHUB_ACCESS_TOKEN_PIECES", None)
 
 def get_github_token_workflows_from_env():
     return os.environ.get("DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS", None)
 
-def get_dockerhub_username_from_env():
-    return os.environ.get("DOCKERHUB_USERNAME", "")
-
-def get_dockerhub_password_from_env():
-    return os.environ.get("DOCKERHUB_PASSWORD", "")
-
 def get_workflows_repository_from_env():
     return os.environ.get("DOMINO_WORKFLOWS_REPOSITORY", None)
 
 def get_local_operators_repository_path():
     return ""
 
 def get_registry_token_from_env():
-    return os.environ.get('REGISTRY_TOKEN', "")
+    return os.environ.get('GHCR_PASSWORD', "")
 
 @click.command()
 @click.option(
     '--cluster-name', 
     prompt='Local cluster name', 
     default=get_cluster_name_from_env,
     help='Define the name for the local k8s cluster.'
@@ -194,50 +188,51 @@
 @click.option(
     '--name', 
     prompt="Repository's name",
     default=generate_random_repo_name,
     help="Repository's name"
 )
 @click.option(
-    '--dockerhub-registry', 
-    prompt="Dockerhub registry name",
+    '--container-registry', 
+    prompt="Github Container Registry name",
     default="",
-    help="Dockerhub registry name"
+    help="Github container registry name"
 )
-def cli_create_piece_repository(name, dockerhub_registry):
+def cli_create_piece_repository(name, container_registry):
     """Create a basic Pieces repository with placeholder files."""
-    pieces_repository.create_pieces_repository(repository_name=name, dockerhub_registry=dockerhub_registry)
+    pieces_repository.create_pieces_repository(repository_name=name, container_registry=container_registry)
 
 
 @click.command()
 @click.option(
     '--build-images', 
     is_flag=True,
     prompt='Build Docker images?',
     expose_value=True,
     default=False,
     help='If True (default), builds Docker images.'
 )
 @click.option(
     '--publish-images', 
     is_flag=True,
-    #prompt='Publish Docker images?',
+    prompt='Publish Docker images?',
     expose_value=True,
     default=False,
-    help='If True (default), publishes Docker images to Dockerhub.'
+    help='If True (default), publishes Docker images to github container registry.'
 )
 @click.option(
     '--registry-token',
-    #prompt='Github Container Registry token',
+    prompt='Github Container Registry token',
     default=get_registry_token_from_env,
     help='Your Github Container Registry token with access to where the image will be published.'
 )
 def cli_organize_pieces_repository(build_images, publish_images, registry_token):
     """Prepare local folder for running a Domino platform."""
-    os.environ['CR_PAT'] = registry_token
+    if registry_token:
+        os.environ['GHCR_PASSWORD'] = registry_token
     console.print(f"Using registry token to publish images")
     pieces_repository.organize_pieces_repository(build_images, publish_images)
 
 
 @click.command()
 def cli_create_release():
     """
```

### Comparing `domino-py-0.1.4/domino/cli/utils/config-domino-local.toml` & `domino-py-0.1.5/domino/cli/utils/config-domino-local.toml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/cli/utils/create_cluster.sh` & `domino-py-0.1.5/domino/cli/utils/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/cli/utils/pieces_repository.py` & `domino-py-0.1.5/domino/cli/utils/pieces_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
     if len(name_errors) > 0:
         raise Exception(f"The following Pieces have inconsistent names: {', '.join(name_errors)}")
     if len(missing_dependencies_errors) > 0:
         raise Exception("\n" + "\n".join(missing_dependencies_errors))
     
     
-def create_pieces_repository(repository_name: str, dockerhub_registry: str) -> None:
+def create_pieces_repository(repository_name: str, container_registry: str) -> None:
     """
     Create a new Pieces repository from template, with folder structure and placeholder files.
     """
     while not validate_repository_name(repository_name):
         repository_name = input("\nInvalid repository name. Should have only numbers, letters and underscores. \nEnter a new repository name: ") or f"new_repository_{str(uuid.uuid4())[0:8]}"
     cwd = Path.cwd()
     repository_folder = cwd / repository_name
@@ -248,15 +248,15 @@
     shutil.rmtree(f"{repository_name}/.git")
 
     # Update config
     with open(f"{repository_name}/config.toml", "rb") as f:
         repo_config = tomli.load(f)
 
     repo_config["repository"]["REPOSITORY_NAME"] = repository_name
-    repo_config["dockerhub"]["REGISTRY_NAME"] =  dockerhub_registry if dockerhub_registry else "ENTER-YOUR-DOCKERHUB-REGISTRY-NAME-HERE"
+    repo_config["repository"]["REGISTRY_NAME"] =  container_registry if container_registry else "ENTER-YOUR-GITHUB-REGISTRY-NAME-HERE"
 
     with open(f"{repository_name}/config.toml", "wb") as f:
         tomli_w.dump(repo_config, f)
 
     console.print(f"Pieces repository successfully create at: {repository_folder}", style=f"bold {COLOR_PALETTE.get('success')}")
     console.print("")
 
@@ -380,15 +380,15 @@
 
 
 def organize_pieces_repository(build_images: bool, publish_images: bool) -> None:
     """
     Organize Piece's repository for Domino. This will: 
     - validate the folder structure, and create the pieces compiled_metadata.json and dependencies_map.json files
     - build Docker images for the Pieces
-    - publish images at Dockerhub
+    - publish images at github container registry
     """        
     # Validate repository
     console.print("Validating repository structure and files...")
     validate_repository_structure()
     validate_pieces_folders()
     console.print("Validation successful!", style=f"bold {COLOR_PALETTE.get('success')}")
```

### Comparing `domino-py-0.1.4/domino/cli/utils/platform.py` & `domino-py-0.1.5/domino/cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/client/airflow_client.py` & `domino-py-0.1.5/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/client/domino_backend_client.py` & `domino-py-0.1.5/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/client/fs_client.py` & `domino-py-0.1.5/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/client/github_rest_client.py` & `domino-py-0.1.5/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/client/local_files_client.py` & `domino-py-0.1.5/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/client/s3_client.py` & `domino-py-0.1.5/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/custom_operators/bash_operator.py` & `domino-py-0.1.5/domino/custom_operators/bash_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/custom_operators/k8s_operator.py` & `domino-py-0.1.5/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/custom_operators/python_operator.py` & `domino-py-0.1.5/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/custom_operators/sidecar/logger.py` & `domino-py-0.1.5/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/custom_operators/sidecar/mount.py` & `domino-py-0.1.5/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/exceptions/exceptions.py` & `domino-py-0.1.5/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz` & `domino-py-0.1.5/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/helm/domino-airflow/values.yaml` & `domino-py-0.1.5/domino/helm/domino-airflow/values.yaml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/helm/domino-base/templates/domino-backend-deployment.yml` & `domino-py-0.1.5/domino/helm/domino-base/templates/domino-backend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/helm/domino-base/templates/domino-frontend-deployment.yml` & `domino-py-0.1.5/domino/helm/domino-base/templates/domino-frontend-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/helm/domino-base/templates/domino-postgres-deployment.yml` & `domino-py-0.1.5/domino/helm/domino-base/templates/domino-postgres-deployment.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/helm/domino-base/templates/jobs/domino-migrations.yml` & `domino-py-0.1.5/domino/helm/domino-base/templates/jobs/domino-migrations.yml`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/logger.py` & `domino-py-0.1.5/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/schemas/piece_metadata.py` & `domino-py-0.1.5/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/schemas/shared_storage.py` & `domino-py-0.1.5/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.1.5/domino/scripts/build_docker_images_pieces.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,18 @@
             if "stream" in r and r["stream"] != "\n":
                 print(r)
         print(Style.RESET_ALL + Fore.BLUE + f"Finished building: {source_image_name}")
         if publish:
             print(f"Publishing docker image: {source_image_name}")
             print(Style.RESET_ALL + Style.DIM, end='')
             try:
-                dockerhub_username = os.environ.get("DOCKERHUB_USERNAME", None)
-                dockerhub_password = os.environ.get("DOCKERHUB_PASSWORD", None)
-                client.login(username=dockerhub_username, password=dockerhub_password)
+                registry_url = 'https://ghcr.io'
+                ghcr_username = os.environ.get("GHCR_USERNAME", None)
+                ghcr_password = os.environ.get("GHCR_PASSWORD", None)
+                client.login(username=ghcr_username, password=ghcr_password, registry=registry_url)
             except docker.errors.APIError:
                 console.print("Unauthorized login")
                 raise
             response = client.images.push(repository=source_image_name)
             print(response, end='')
             print(Style.RESET_ALL + Fore.BLUE + f"Finished publishing: {source_image_name}")
         print(Style.RESET_ALL)
@@ -67,17 +68,17 @@
     # Get information from config.toml file
     with open(config_path, "rb") as f:
         config_dict = tomli.load(f)
     docker_image_repository = config_dict.get("repository").get("REPOSITORY_NAME")
     docker_image_version = config_dict.get("repository").get("VERSION")
 
     if publish:
-        github_container_registry_name = f'ghcr.io/{config_dict.get("dockerhub").get("REGISTRY_NAME")}'
+        github_container_registry_name = f'ghcr.io/{config_dict.get("repository").get("REGISTRY_NAME")}'
     else:
-        github_container_registry_name = f'ghcr.io/{config_dict.get("dockerhub").get("REGISTRY_NAME")}'
+        github_container_registry_name = f'local'
 
     # Load dependencies_map.json file
     with open(domino_path / "dependencies_map.json", "r") as f:
         pieces_dependencies_map = json.load(f)
 
     # Build docker images from unique definitions
     for group, v in pieces_dependencies_map.items():
```

### Comparing `domino-py-0.1.4/domino/scripts/create_docker_compose_file.py` & `domino-py-0.1.5/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/docker_compose_constants.py` & `domino-py-0.1.5/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/docker_compose_scripts.py` & `domino-py-0.1.5/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/generate_infrasctructure.py` & `domino-py-0.1.5/domino/scripts/generate_infrasctructure.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/load_piece.py` & `domino-py-0.1.5/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/run_piece_bash.py` & `domino-py-0.1.5/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/run_piece_dry.py` & `domino-py-0.1.5/domino/scripts/run_piece_dry.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/scripts/run_piece_k8s.py` & `domino-py-0.1.5/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/task.py` & `domino-py-0.1.5/domino/task.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino/utils/validators.py` & `domino-py-0.1.5/domino/utils/validators.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/domino_py.egg-info/PKG-INFO` & `domino-py-0.1.5/domino_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Domino project
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description: [<img src="https://img.shields.io/pypi/v/flowui-project?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">](https://pypi.org/project/flowui-project/)
         [<img src="https://img.shields.io/docker/v/taufferconsulting/flowui-backend?label=Backend&logo=docker&style=flat">](https://hub.docker.com/r/taufferconsulting/flowui-backend)
```

### Comparing `domino-py-0.1.4/domino_py.egg-info/SOURCES.txt` & `domino-py-0.1.5/domino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.4/setup.py` & `domino-py-0.1.5/setup.py`

 * *Files identical despite different names*

