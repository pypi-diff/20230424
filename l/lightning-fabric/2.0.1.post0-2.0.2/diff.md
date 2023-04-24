# Comparing `tmp/lightning-fabric-2.0.1.post0.tar.gz` & `tmp/lightning-fabric-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-fabric-2.0.1.post0.tar", last modified: Tue Apr 11 18:44:36 2023, max compression
+gzip compressed data, was "lightning-fabric-2.0.2.tar", last modified: Mon Apr 24 13:57:44 2023, max compression
```

## Comparing `lightning-fabric-2.0.1.post0.tar` & `lightning-fabric-2.0.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.967967 lightning-fabric-2.0.1.post0/.actions/
--rw-r--r--   0 runner    (1001) docker     (122)    17395 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    22128 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.967967 lightning-fabric-2.0.1.post0/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/requirements/fabric/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     7917 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (122)    10727 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6967 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2722 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (122)    13986 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4579 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/tpu.py
--rw-r--r--   0 runner    (1001) docker     (122)     7053 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    27495 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (122)    39832 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7694 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4500 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)    12795 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     8127 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     3662 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (122)     7571 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (122)     7610 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2584 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5094 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5025 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu_bf16.py
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (122)    37212 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (122)     3579 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (122)    15697 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.975968 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     8044 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (122)     4208 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (122)    14896 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.979967 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4636 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (122)    20420 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4119 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7329 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4764 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     5486 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (122)     9162 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:36.971968 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4304 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 18:44:36.000000 lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:44:24.000000 lightning-fabric-2.0.1.post0/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.321956 lightning-fabric-2.0.2/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/requirements/fabric/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7917 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-24 13:57:43.000000 lightning-fabric-2.0.2/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/accelerators/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-24 13:57:43.000000 lightning-fabric-2.0.2/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.329956 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu_bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37214 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.333956 lightning-fabric-2.0.2/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-04-24 13:57:43.000000 lightning-fabric-2.0.2/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:44.325955 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 13:57:44.000000 lightning-fabric-2.0.2/src/lightning_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:33.000000 lightning-fabric-2.0.2/src/version.info
```

### Comparing `lightning-fabric-2.0.1.post0/.actions/assistant.py` & `lightning-fabric-2.0.2/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/LICENSE` & `lightning-fabric-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/PKG-INFO` & `lightning-fabric-2.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,518 +1,716 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c69 6768  : 2.1.Name: ligh
 00000020: 746e 696e 672d 6661 6272 6963 0a56 6572  tning-fabric.Ver
-00000030: 7369 6f6e 3a20 322e 302e 312e 706f 7374  sion: 2.0.1.post
-00000040: 300a 5375 6d6d 6172 793a 2055 4e4b 4e4f  0.Summary: UNKNO
-00000050: 574e 0a48 6f6d 652d 7061 6765 3a20 6874  WN.Home-page: ht
-00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000070: 2f4c 6967 6874 6e69 6e67 2d41 492f 6c69  /Lightning-AI/li
-00000080: 6768 746e 696e 670a 4175 7468 6f72 3a20  ghtning.Author: 
-00000090: 4c69 6768 746e 696e 6720 4149 2065 7420  Lightning AI et 
-000000a0: 616c 2e0a 4175 7468 6f72 2d65 6d61 696c  al..Author-email
-000000b0: 3a20 7079 746f 7263 6840 6c69 6768 746e  : pytorch@lightn
-000000c0: 696e 672e 6169 0a4c 6963 656e 7365 3a20  ing.ai.License: 
-000000d0: 4170 6163 6865 2d32 2e30 0a44 6f77 6e6c  Apache-2.0.Downl
-000000e0: 6f61 642d 5552 4c3a 2068 7474 7073 3a2f  oad-URL: https:/
-000000f0: 2f67 6974 6875 622e 636f 6d2f 4c69 6768  /github.com/Ligh
-00000100: 746e 696e 672d 4149 2f6c 6967 6874 6e69  tning-AI/lightni
-00000110: 6e67 0a50 726f 6a65 6374 2d55 524c 3a20  ng.Project-URL: 
-00000120: 4275 6720 5472 6163 6b65 722c 2068 7474  Bug Tracker, htt
-00000130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000140: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
-00000150: 6874 6e69 6e67 2f69 7373 7565 730a 5072  htning/issues.Pr
-00000160: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-00000170: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-00000180: 2f2f 7079 746f 7263 682d 6c69 6768 746e  //pytorch-lightn
-00000190: 696e 672e 7274 6664 2e69 6f2f 656e 2f6c  ing.rtfd.io/en/l
-000001a0: 6174 6573 742f 0a50 726f 6a65 6374 2d55  atest/.Project-U
-000001b0: 524c 3a20 536f 7572 6365 2043 6f64 652c  RL: Source Code,
-000001c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001d0: 636f 6d2f 4c69 6768 746e 696e 672d 4149  com/Lightning-AI
-000001e0: 2f6c 6967 6874 6e69 6e67 0a4b 6579 776f  /lightning.Keywo
-000001f0: 7264 733a 2064 6565 7020 6c65 6172 6e69  rds: deep learni
-00000200: 6e67 2c70 7974 6f72 6368 2c41 490a 506c  ng,pytorch,AI.Pl
-00000210: 6174 666f 726d 3a20 554e 4b4e 4f57 4e0a  atform: UNKNOWN.
-00000220: 436c 6173 7369 6669 6572 3a20 456e 7669  Classifier: Envi
-00000230: 726f 6e6d 656e 7420 3a3a 2043 6f6e 736f  ronment :: Conso
-00000240: 6c65 0a43 6c61 7373 6966 6965 723a 204e  le.Classifier: N
-00000250: 6174 7572 616c 204c 616e 6775 6167 6520  atural Language 
-00000260: 3a3a 2045 6e67 6c69 7368 0a43 6c61 7373  :: English.Class
-00000270: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
-00000280: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
-00000290: 2042 6574 610a 436c 6173 7369 6669 6572   Beta.Classifier
-000002a0: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-000002b0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
-000002c0: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-000002d0: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-000002e0: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-000002f0: 2041 7274 6966 6963 6961 6c20 496e 7465   Artificial Inte
-00000300: 6c6c 6967 656e 6365 0a43 6c61 7373 6966  lligence.Classif
-00000310: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
-00000320: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000330: 7269 6e67 203a 3a20 496e 666f 726d 6174  ring :: Informat
-00000340: 696f 6e20 416e 616c 7973 6973 0a43 6c61  ion Analysis.Cla
-00000350: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-00000360: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000370: 496e 6465 7065 6e64 656e 740a 436c 6173  Independent.Clas
-00000380: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000390: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003a0: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
-000003b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000003c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003d0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
-000003e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000003f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000400: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-00000410: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000420: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000430: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000440: 3130 0a52 6571 7569 7265 732d 5079 7468  10.Requires-Pyth
-00000450: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
-00000460: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000470: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000480: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
-00000490: 3a20 6578 616d 706c 6573 0a50 726f 7669  : examples.Provi
-000004a0: 6465 732d 4578 7472 613a 2074 6573 740a  des-Extra: test.
-000004b0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000004c0: 7374 7261 7465 6769 6573 0a50 726f 7669  strategies.Provi
-000004d0: 6465 732d 4578 7472 613a 2064 6565 7073  des-Extra: deeps
-000004e0: 7065 6564 0a50 726f 7669 6465 732d 4578  peed.Provides-Ex
-000004f0: 7472 613a 2061 6c6c 0a50 726f 7669 6465  tra: all.Provide
-00000500: 732d 4578 7472 613a 2064 6576 0a4c 6963  s-Extra: dev.Lic
-00000510: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000520: 5345 0a0a 3c64 6976 2061 6c69 676e 3d22  SE..<div align="
-00000530: 6365 6e74 6572 223e 0a0a 3c69 6d67 2073  center">..<img s
-00000540: 7263 3d22 6874 7470 733a 2f2f 706c 2d70  rc="https://pl-p
-00000550: 7562 6c69 632d 6461 7461 2e73 332e 616d  ublic-data.s3.am
-00000560: 617a 6f6e 6177 732e 636f 6d2f 6173 7365  azonaws.com/asse
-00000570: 7473 5f6c 6967 6874 6e69 6e67 2f66 6162  ts_lightning/fab
-00000580: 7269 635f 6c6f 676f 2e70 6e67 2220 7769  ric_logo.png" wi
-00000590: 6474 683d 2234 3030 7078 223e 0a0a 2a2a  dth="400px">..**
-000005a0: 4661 6272 6963 2069 7320 7468 6520 6661  Fabric is the fa
-000005b0: 7374 2061 6e64 206c 6967 6874 7765 6967  st and lightweig
-000005c0: 6874 2077 6179 2074 6f20 7363 616c 6520  ht way to scale 
-000005d0: 5079 546f 7263 6820 6d6f 6465 6c73 2077  PyTorch models w
-000005e0: 6974 686f 7574 2062 6f69 6c65 7270 6c61  ithout boilerpla
-000005f0: 7465 2a2a 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f  te**..__________
+00000030: 7369 6f6e 3a20 322e 302e 320a 5375 6d6d  sion: 2.0.2.Summ
+00000040: 6172 793a 2055 4e4b 4e4f 574e 0a48 6f6d  ary: UNKNOWN.Hom
+00000050: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000060: 6769 7468 7562 2e63 6f6d 2f4c 6967 6874  github.com/Light
+00000070: 6e69 6e67 2d41 492f 6c69 6768 746e 696e  ning-AI/lightnin
+00000080: 670a 4175 7468 6f72 3a20 4c69 6768 746e  g.Author: Lightn
+00000090: 696e 6720 4149 2065 7420 616c 2e0a 4175  ing AI et al..Au
+000000a0: 7468 6f72 2d65 6d61 696c 3a20 7079 746f  thor-email: pyto
+000000b0: 7263 6840 6c69 6768 746e 696e 672e 6169  rch@lightning.ai
+000000c0: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
+000000d0: 2d32 2e30 0a44 6f77 6e6c 6f61 642d 5552  -2.0.Download-UR
+000000e0: 4c3a 2068 7474 7073 3a2f 2f67 6974 6875  L: https://githu
+000000f0: 622e 636f 6d2f 4c69 6768 746e 696e 672d  b.com/Lightning-
+00000100: 4149 2f6c 6967 6874 6e69 6e67 0a50 726f  AI/lightning.Pro
+00000110: 6a65 6374 2d55 524c 3a20 4275 6720 5472  ject-URL: Bug Tr
+00000120: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
+00000130: 6974 6875 622e 636f 6d2f 4c69 6768 746e  ithub.com/Lightn
+00000140: 696e 672d 4149 2f6c 6967 6874 6e69 6e67  ing-AI/lightning
+00000150: 2f69 7373 7565 730a 5072 6f6a 6563 742d  /issues.Project-
+00000160: 5552 4c3a 2044 6f63 756d 656e 7461 7469  URL: Documentati
+00000170: 6f6e 2c20 6874 7470 733a 2f2f 7079 746f  on, https://pyto
+00000180: 7263 682d 6c69 6768 746e 696e 672e 7274  rch-lightning.rt
+00000190: 6664 2e69 6f2f 656e 2f6c 6174 6573 742f  fd.io/en/latest/
+000001a0: 0a50 726f 6a65 6374 2d55 524c 3a20 536f  .Project-URL: So
+000001b0: 7572 6365 2043 6f64 652c 2068 7474 7073  urce Code, https
+000001c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c69  ://github.com/Li
+000001d0: 6768 746e 696e 672d 4149 2f6c 6967 6874  ghtning-AI/light
+000001e0: 6e69 6e67 0a4b 6579 776f 7264 733a 2064  ning.Keywords: d
+000001f0: 6565 7020 6c65 6172 6e69 6e67 2c70 7974  eep learning,pyt
+00000200: 6f72 6368 2c41 490a 506c 6174 666f 726d  orch,AI.Platform
+00000210: 3a20 554e 4b4e 4f57 4e0a 436c 6173 7369  : UNKNOWN.Classi
+00000220: 6669 6572 3a20 456e 7669 726f 6e6d 656e  fier: Environmen
+00000230: 7420 3a3a 2043 6f6e 736f 6c65 0a43 6c61  t :: Console.Cla
+00000240: 7373 6966 6965 723a 204e 6174 7572 616c  ssifier: Natural
+00000250: 204c 616e 6775 6167 6520 3a3a 2045 6e67   Language :: Eng
+00000260: 6c69 7368 0a43 6c61 7373 6966 6965 723a  lish.Classifier:
+00000270: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
+00000280: 7475 7320 3a3a 2034 202d 2042 6574 610a  tus :: 4 - Beta.
+00000290: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+000002a0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+000002b0: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
+000002c0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000002d0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+000002e0: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+000002f0: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+00000300: 6365 0a43 6c61 7373 6966 6965 723a 2054  ce.Classifier: T
+00000310: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+00000320: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
+00000330: 3a20 496e 666f 726d 6174 696f 6e20 416e  : Information An
+00000340: 616c 7973 6973 0a43 6c61 7373 6966 6965  alysis.Classifie
+00000350: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+00000360: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000370: 6e64 656e 740a 436c 6173 7369 6669 6572  ndent.Classifier
+00000380: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000390: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000003a0: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+000003b0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000003c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000003d0: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+000003e0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000003f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000400: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
+00000410: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000420: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000430: 7468 6f6e 203a 3a20 332e 3130 0a52 6571  thon :: 3.10.Req
+00000440: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+00000450: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
+00000460: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000470: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
+00000480: 6964 6573 2d45 7874 7261 3a20 7374 7261  ides-Extra: stra
+00000490: 7465 6769 6573 0a50 726f 7669 6465 732d  tegies.Provides-
+000004a0: 4578 7472 613a 2074 6573 740a 5072 6f76  Extra: test.Prov
+000004b0: 6964 6573 2d45 7874 7261 3a20 6578 616d  ides-Extra: exam
+000004c0: 706c 6573 0a50 726f 7669 6465 732d 4578  ples.Provides-Ex
+000004d0: 7472 613a 2064 6565 7073 7065 6564 0a50  tra: deepspeed.P
+000004e0: 726f 7669 6465 732d 4578 7472 613a 2061  rovides-Extra: a
+000004f0: 6c6c 0a50 726f 7669 6465 732d 4578 7472  ll.Provides-Extr
+00000500: 613a 2064 6576 0a4c 6963 656e 7365 2d46  a: dev.License-F
+00000510: 696c 653a 204c 4943 454e 5345 0a0a 3c64  ile: LICENSE..<d
+00000520: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00000530: 223e 0a0a 3c69 6d67 2073 7263 3d22 6874  ">..<img src="ht
+00000540: 7470 733a 2f2f 706c 2d70 7562 6c69 632d  tps://pl-public-
+00000550: 6461 7461 2e73 332e 616d 617a 6f6e 6177  data.s3.amazonaw
+00000560: 732e 636f 6d2f 6173 7365 7473 5f6c 6967  s.com/assets_lig
+00000570: 6874 6e69 6e67 2f66 6162 7269 635f 6c6f  htning/fabric_lo
+00000580: 676f 2e70 6e67 2220 7769 6474 683d 2234  go.png" width="4
+00000590: 3030 7078 223e 0a0a 2a2a 4661 6272 6963  00px">..**Fabric
+000005a0: 2069 7320 7468 6520 6661 7374 2061 6e64   is the fast and
+000005b0: 206c 6967 6874 7765 6967 6874 2077 6179   lightweight way
+000005c0: 2074 6f20 7363 616c 6520 5079 546f 7263   to scale PyTorc
+000005d0: 6820 6d6f 6465 6c73 2077 6974 686f 7574  h models without
+000005e0: 2062 6f69 6c65 7270 6c61 7465 2a2a 0a0a   boilerplate**..
+000005f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000600: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000610: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000620: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000630: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a 3c70  ____________..<p
-00000640: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000650: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00000660: 733a 2f2f 6c69 6768 746e 696e 672e 6169  s://lightning.ai
-00000670: 2f22 3e57 6562 7369 7465 3c2f 613e 20e2  /">Website</a> .
-00000680: 80a2 0a20 203c 6120 6872 6566 3d22 6874  ...  <a href="ht
-00000690: 7470 733a 2f2f 6c69 6768 746e 696e 672e  tps://lightning.
-000006a0: 6169 2f64 6f63 732f 6661 6272 6963 2f22  ai/docs/fabric/"
-000006b0: 3e44 6f63 733c 2f61 3e20 e280 a20a 2020  >Docs</a> ....  
-000006c0: 3c61 2068 7265 663d 2223 6765 7474 696e  <a href="#gettin
-000006d0: 672d 7374 6172 7465 6422 3e47 6574 7469  g-started">Getti
-000006e0: 6e67 2073 7461 7274 6564 3c2f 613e 20e2  ng started</a> .
-000006f0: 80a2 0a20 203c 6120 6872 6566 3d22 2366  ...  <a href="#f
-00000700: 6171 223e 4641 513c 2f61 3e20 e280 a20a  aq">FAQ</a> ....
-00000710: 2020 3c61 2068 7265 663d 2223 6173 6b69    <a href="#aski
-00000720: 6e67 2d66 6f72 2d68 656c 7022 3e48 656c  ng-for-help">Hel
-00000730: 703c 2f61 3e20 e280 a20a 2020 3c61 2068  p</a> ....  <a h
-00000740: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
-00000750: 636f 7264 2e67 672f 5670 7450 435a 6b47  cord.gg/VptPCZkG
-00000760: 4e61 223e 4469 7363 6f72 643c 2f61 3e0a  Na">Discord</a>.
-00000770: 3c2f 703e 0a0a 5b21 5b50 7950 4920 2d20  </p>..[![PyPI - 
-00000780: 5079 7468 6f6e 2056 6572 7369 6f6e 5d28  Python Version](
-00000790: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000007a0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
-000007b0: 7273 696f 6e73 2f6c 6967 6874 6e69 6e67  rsions/lightning
-000007c0: 5f66 6162 7269 6329 5d28 6874 7470 733a  _fabric)](https:
-000007d0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000007e0: 6374 2f6c 6967 6874 6e69 6e67 5f66 6162  ct/lightning_fab
-000007f0: 7269 632f 290a 5b21 5b50 7950 4920 5374  ric/).[![PyPI St
-00000800: 6174 7573 5d28 6874 7470 733a 2f2f 6261  atus](https://ba
-00000810: 6467 652e 6675 7279 2e69 6f2f 7079 2f6c  dge.fury.io/py/l
-00000820: 6967 6874 6e69 6e67 5f66 6162 7269 632e  ightning_fabric.
-00000830: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
-00000840: 6467 652e 6675 7279 2e69 6f2f 7079 2f6c  dge.fury.io/py/l
-00000850: 6967 6874 6e69 6e67 5f66 6162 7269 6329  ightning_fabric)
-00000860: 0a5b 215b 5079 5049 2053 7461 7475 735d  .[![PyPI Status]
-00000870: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-00000880: 6368 2f62 6164 6765 2f6c 6967 6874 6e69  ch/badge/lightni
-00000890: 6e67 5f66 6162 7269 6329 5d28 6874 7470  ng_fabric)](http
-000008a0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
-000008b0: 6f6a 6563 742f 6c69 6768 746e 696e 675f  oject/lightning_
-000008c0: 6661 6272 6963 290a 5b21 5b43 6f6e 6461  fabric).[![Conda
-000008d0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000008e0: 6965 6c64 732e 696f 2f63 6f6e 6461 2f76  ields.io/conda/v
-000008f0: 2f63 6f6e 6461 2d66 6f72 6765 2f6c 6967  /conda-forge/lig
-00000900: 6874 6e69 6e67 5f66 6162 7269 633f 6c61  htning_fabric?la
-00000910: 6265 6c3d 636f 6e64 6126 636f 6c6f 723d  bel=conda&color=
-00000920: 7375 6363 6573 7329 5d28 6874 7470 733a  success)](https:
-00000930: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
-00000940: 6f6e 6461 2d66 6f72 6765 2f6c 6967 6874  onda-forge/light
-00000950: 6e69 6e67 5f66 6162 7269 6329 0a0a 3c2f  ning_fabric)..</
-00000960: 6469 763e 0a0a 2323 204d 6178 696d 756d  div>..## Maximum
-00000970: 2066 6c65 7869 6269 6c69 7479 2c20 6d69   flexibility, mi
-00000980: 6e69 6d75 6d20 636f 6465 2063 6861 6e67  nimum code chang
-00000990: 6573 0a0a 5769 7468 206a 7573 7420 6120  es..With just a 
-000009a0: 6665 7720 636f 6465 2063 6861 6e67 6573  few code changes
-000009b0: 2c20 7275 6e20 616e 7920 5079 546f 7263  , run any PyTorc
-000009c0: 6820 6d6f 6465 6c20 6f6e 2061 6e79 2064  h model on any d
-000009d0: 6973 7472 6962 7574 6564 2068 6172 6477  istributed hardw
-000009e0: 6172 652c 206e 6f20 626f 696c 6572 706c  are, no boilerpl
-000009f0: 6174 6521 0a0a 2d20 4561 7369 6c79 2073  ate!..- Easily s
-00000a00: 7769 7463 6820 6672 6f6d 2072 756e 6e69  witch from runni
-00000a10: 6e67 206f 6e20 4350 5520 746f 2047 5055  ng on CPU to GPU
-00000a20: 2028 4170 706c 6520 5369 6c69 636f 6e2c   (Apple Silicon,
-00000a30: 2043 5544 412c 20e2 80a6 292c 2054 5055   CUDA, ...), TPU
-00000a40: 2c20 6d75 6c74 692d 4750 5520 6f72 2065  , multi-GPU or e
-00000a50: 7665 6e20 6d75 6c74 692d 6e6f 6465 2074  ven multi-node t
-00000a60: 7261 696e 696e 670a 2d20 5573 6520 7374  raining.- Use st
-00000a70: 6174 652d 6f66 2d74 6865 2d61 7274 2064  ate-of-the-art d
-00000a80: 6973 7472 6962 7574 6564 2074 7261 696e  istributed train
-00000a90: 696e 6720 7374 7261 7465 6769 6573 2028  ing strategies (
-00000aa0: 4444 502c 2046 5344 502c 2044 6565 7053  DDP, FSDP, DeepS
-00000ab0: 7065 6564 2920 616e 6420 6d69 7865 6420  peed) and mixed 
-00000ac0: 7072 6563 6973 696f 6e20 6f75 7420 6f66  precision out of
-00000ad0: 2074 6865 2062 6f78 0a2d 2041 6c6c 2074   the box.- All t
-00000ae0: 6865 2064 6576 6963 6520 6c6f 6769 6320  he device logic 
-00000af0: 626f 696c 6572 706c 6174 6520 6973 2068  boilerplate is h
-00000b00: 616e 646c 6564 2066 6f72 2079 6f75 0a2d  andled for you.-
-00000b10: 2044 6573 6967 6e65 6420 7769 7468 206d   Designed with m
-00000b20: 756c 7469 2d62 696c 6c69 6f6e 2070 6172  ulti-billion par
-00000b30: 616d 6574 6572 206d 6f64 656c 7320 696e  ameter models in
-00000b40: 206d 696e 640a 2d20 4275 696c 6420 796f   mind.- Build yo
-00000b50: 7572 206f 776e 2063 7573 746f 6d20 5472  ur own custom Tr
-00000b60: 6169 6e65 7220 7573 696e 6720 4661 6272  ainer using Fabr
-00000b70: 6963 2070 7269 6d69 7469 7665 7320 666f  ic primitives fo
-00000b80: 7220 7472 6169 6e69 6e67 2063 6865 636b  r training check
-00000b90: 706f 696e 7469 6e67 2c20 6c6f 6767 696e  pointing, loggin
-00000ba0: 672c 2061 6e64 206d 6f72 650a 0a60 6060  g, and more..```
-00000bb0: 6469 6666 0a2b 2069 6d70 6f72 7420 6c69  diff.+ import li
-00000bc0: 6768 746e 696e 6720 6173 204c 0a0a 2020  ghtning as L..  
-00000bd0: 696d 706f 7274 2074 6f72 6368 0a20 2069  import torch.  i
-00000be0: 6d70 6f72 7420 746f 7263 682e 6e6e 2061  mport torch.nn a
-00000bf0: 7320 6e6e 0a20 2066 726f 6d20 746f 7263  s nn.  from torc
-00000c00: 682e 7574 696c 732e 6461 7461 2069 6d70  h.utils.data imp
-00000c10: 6f72 7420 4461 7461 4c6f 6164 6572 2c20  ort DataLoader, 
-00000c20: 4461 7461 7365 740a 0a20 2063 6c61 7373  Dataset..  class
-00000c30: 2050 7954 6f72 6368 4d6f 6465 6c28 6e6e   PyTorchModel(nn
-00000c40: 2e4d 6f64 756c 6529 3a0a 2020 2020 2020  .Module):.      
-00000c50: 2e2e 2e0a 0a20 2063 6c61 7373 2050 7954  .....  class PyT
-00000c60: 6f72 6368 4461 7461 7365 7428 4461 7461  orchDataset(Data
-00000c70: 7365 7429 3a0a 2020 2020 2020 2e2e 2e0a  set):.      ....
-00000c80: 0a2b 2066 6162 7269 6320 3d20 4c2e 4661  .+ fabric = L.Fa
-00000c90: 6272 6963 2861 6363 656c 6572 6174 6f72  bric(accelerator
-00000ca0: 3d22 6375 6461 222c 2064 6576 6963 6573  ="cuda", devices
-00000cb0: 3d38 2c20 7374 7261 7465 6779 3d22 6464  =8, strategy="dd
-00000cc0: 7022 290a 2b20 6661 6272 6963 2e6c 6175  p").+ fabric.lau
-00000cd0: 6e63 6828 290a 0a2d 2064 6576 6963 6520  nch()..- device 
-00000ce0: 3d20 2263 7564 6122 2069 6620 746f 7263  = "cuda" if torc
-00000cf0: 682e 6375 6461 2e69 735f 6176 6169 6c61  h.cuda.is_availa
-00000d00: 626c 6528 2920 656c 7365 2022 6370 750a  ble() else "cpu.
-00000d10: 2020 6d6f 6465 6c20 3d20 5079 546f 7263    model = PyTorc
-00000d20: 684d 6f64 656c 282e 2e2e 290a 2020 6f70  hModel(...).  op
-00000d30: 7469 6d69 7a65 7220 3d20 746f 7263 682e  timizer = torch.
-00000d40: 6f70 7469 6d2e 5347 4428 6d6f 6465 6c2e  optim.SGD(model.
-00000d50: 7061 7261 6d65 7465 7273 2829 290a 2b20  parameters()).+ 
-00000d60: 6d6f 6465 6c2c 206f 7074 696d 697a 6572  model, optimizer
-00000d70: 203d 2066 6162 7269 632e 7365 7475 7028   = fabric.setup(
-00000d80: 6d6f 6465 6c2c 206f 7074 696d 697a 6572  model, optimizer
-00000d90: 290a 2020 6461 7461 6c6f 6164 6572 203d  ).  dataloader =
-00000da0: 2044 6174 614c 6f61 6465 7228 5079 546f   DataLoader(PyTo
-00000db0: 7263 6844 6174 6173 6574 282e 2e2e 292c  rchDataset(...),
-00000dc0: 202e 2e2e 290a 2b20 6461 7461 6c6f 6164   ...).+ dataload
-00000dd0: 6572 203d 2066 6162 7269 632e 7365 7475  er = fabric.setu
-00000de0: 705f 6461 7461 6c6f 6164 6572 7328 6461  p_dataloaders(da
-00000df0: 7461 6c6f 6164 6572 290a 2020 6d6f 6465  taloader).  mode
-00000e00: 6c2e 7472 6169 6e28 290a 0a20 2066 6f72  l.train()..  for
-00000e10: 2065 706f 6368 2069 6e20 7261 6e67 6528   epoch in range(
-00000e20: 6e75 6d5f 6570 6f63 6873 293a 0a20 2020  num_epochs):.   
-00000e30: 2020 2066 6f72 2062 6174 6368 2069 6e20     for batch in 
-00000e40: 6461 7461 6c6f 6164 6572 3a0a 2020 2020  dataloader:.    
-00000e50: 2020 2020 2020 696e 7075 742c 2074 6172        input, tar
-00000e60: 6765 7420 3d20 6261 7463 680a 2d20 2020  get = batch.-   
-00000e70: 2020 2020 2020 696e 7075 742c 2074 6172        input, tar
-00000e80: 6765 7420 3d20 696e 7075 742e 746f 2864  get = input.to(d
-00000e90: 6576 6963 6529 2c20 7461 7267 6574 2e74  evice), target.t
-00000ea0: 6f28 6465 7669 6365 290a 2020 2020 2020  o(device).      
-00000eb0: 2020 2020 6f70 7469 6d69 7a65 722e 7a65      optimizer.ze
-00000ec0: 726f 5f67 7261 6428 290a 2020 2020 2020  ro_grad().      
-00000ed0: 2020 2020 6f75 7470 7574 203d 206d 6f64      output = mod
-00000ee0: 656c 2869 6e70 7574 290a 2020 2020 2020  el(input).      
-00000ef0: 2020 2020 6c6f 7373 203d 206c 6f73 735f      loss = loss_
-00000f00: 666e 286f 7574 7075 742c 2074 6172 6765  fn(output, targe
-00000f10: 7429 0a2d 2020 2020 2020 2020 206c 6f73  t).-         los
-00000f20: 732e 6261 636b 7761 7264 2829 0a2b 2020  s.backward().+  
-00000f30: 2020 2020 2020 2066 6162 7269 632e 6261         fabric.ba
-00000f40: 636b 7761 7264 286c 6f73 7329 0a20 2020  ckward(loss).   
-00000f50: 2020 2020 2020 206f 7074 696d 697a 6572         optimizer
-00000f60: 2e73 7465 7028 290a 2020 2020 2020 2020  .step().        
-00000f70: 2020 6c72 5f73 6368 6564 756c 6572 2e73    lr_scheduler.s
-00000f80: 7465 7028 290a 6060 600a 0a5f 5f5f 5f5f  tep().```.._____
-00000f90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fa0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fb0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fc0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fd0: 5f0a 0a23 2047 6574 7469 6e67 2073 7461  _..# Getting sta
-00000fe0: 7274 6564 0a0a 2323 2049 6e73 7461 6c6c  rted..## Install
-00000ff0: 204c 6967 6874 6e69 6e67 0a0a 3c64 6574   Lightning..<det
-00001000: 6169 6c73 3e0a 0a3c 7375 6d6d 6172 793e  ails>..<summary>
-00001010: 5072 6572 6571 7569 7369 7465 733c 2f73  Prerequisites</s
-00001020: 756d 6d61 7279 3e0a 0a3e 2054 4950 3a20  ummary>..> TIP: 
-00001030: 5765 2073 7472 6f6e 676c 7920 7265 636f  We strongly reco
-00001040: 6d6d 656e 6420 6372 6561 7469 6e67 2061  mmend creating a
-00001050: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
-00001060: 6d65 6e74 2066 6972 7374 2e0a 3e20 446f  ment first..> Do
-00001070: 6ee2 8099 7420 6b6e 6f77 2077 6861 7420  n...t know what 
-00001080: 7468 6973 2069 733f 2046 6f6c 6c6f 7720  this is? Follow 
-00001090: 6f75 7220 5b62 6567 696e 6e65 7220 6775  our [beginner gu
-000010a0: 6964 6520 6865 7265 5d28 6874 7470 733a  ide here](https:
-000010b0: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
-000010c0: 6f63 732f 7374 6162 6c65 2f69 6e73 7461  ocs/stable/insta
-000010d0: 6c6c 2f69 6e73 7461 6c6c 6174 696f 6e2e  ll/installation.
-000010e0: 6874 6d6c 292e 0a0a 2d20 5079 7468 6f6e  html)...- Python
-000010f0: 2033 2e38 2e78 206f 7220 6c61 7465 7220   3.8.x or later 
-00001100: 2833 2e38 2e78 2c20 332e 392e 782c 2033  (3.8.x, 3.9.x, 3
-00001110: 2e31 302e 782c 202e 2e2e 290a 0a3c 2f64  .10.x, ...)..</d
-00001120: 6574 6169 6c73 3e0a 0a60 6060 6261 7368  etails>..```bash
-00001130: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
-00001140: 6c69 6768 746e 696e 670a 6060 600a 0a23  lightning.```..#
-00001150: 2320 436f 6e76 6572 7420 796f 7572 2050  # Convert your P
-00001160: 7954 6f72 6368 2074 6f20 4661 6272 6963  yTorch to Fabric
-00001170: 0a0a 312e 2043 7265 6174 6520 7468 6520  ..1. Create the 
-00001180: 6046 6162 7269 6360 206f 626a 6563 7420  `Fabric` object 
-00001190: 6174 2074 6865 2062 6567 696e 6e69 6e67  at the beginning
-000011a0: 206f 6620 796f 7572 2074 7261 696e 696e   of your trainin
-000011b0: 6720 636f 6465 2e0a 0a20 2020 6060 600a  g code...   ```.
-000011c0: 2020 2069 6d70 6f72 7420 4c69 6768 746e     import Lightn
-000011d0: 696e 6720 6173 204c 0a0a 2020 2066 6162  ing as L..   fab
-000011e0: 7269 6320 3d20 4c2e 4661 6272 6963 2829  ric = L.Fabric()
-000011f0: 0a20 2020 6060 600a 0a31 2e20 4361 6c6c  .   ```..1. Call
-00001200: 2060 7365 7475 7028 2960 206f 6e20 6561   `setup()` on ea
-00001210: 6368 206d 6f64 656c 2061 6e64 206f 7074  ch model and opt
-00001220: 696d 697a 6572 2070 6169 7220 616e 6420  imizer pair and 
-00001230: 6073 6574 7570 5f64 6174 616c 6f61 6465  `setup_dataloade
-00001240: 7273 2829 6020 6f6e 2061 6c6c 2079 6f75  rs()` on all you
-00001250: 7220 6461 7461 206c 6f61 6465 7273 2e0a  r data loaders..
-00001260: 0a20 2020 6060 600a 2020 206d 6f64 656c  .   ```.   model
-00001270: 2c20 6f70 7469 6d69 7a65 7220 3d20 6661  , optimizer = fa
-00001280: 6272 6963 2e73 6574 7570 286d 6f64 656c  bric.setup(model
-00001290: 2c20 6f70 7469 6d69 7a65 7229 0a20 2020  , optimizer).   
-000012a0: 6461 7461 6c6f 6164 6572 203d 2066 6162  dataloader = fab
-000012b0: 7269 632e 7365 7475 705f 6461 7461 6c6f  ric.setup_datalo
-000012c0: 6164 6572 7328 6461 7461 6c6f 6164 6572  aders(dataloader
-000012d0: 290a 2020 2060 6060 0a0a 312e 2052 656d  ).   ```..1. Rem
-000012e0: 6f76 6520 616c 6c20 602e 746f 6020 616e  ove all `.to` an
-000012f0: 6420 602e 6375 6461 6020 6361 6c6c 7320  d `.cuda` calls 
-00001300: 2d3e 2046 6162 7269 6320 7769 6c6c 2074  -> Fabric will t
-00001310: 616b 6520 6361 7265 206f 6620 6974 2e0a  ake care of it..
-00001320: 0a20 2020 6060 6064 6966 660a 2020 202d  .   ```diff.   -
-00001330: 206d 6f64 656c 2e74 6f28 6465 7669 6365   model.to(device
-00001340: 290a 2020 202d 2062 6174 6368 2e74 6f28  ).   - batch.to(
-00001350: 6465 7669 6365 290a 2020 2060 6060 0a0a  device).   ```..
-00001360: 312e 2052 6570 6c61 6365 2060 6c6f 7373  1. Replace `loss
-00001370: 2e62 6163 6b77 6172 6428 2960 2062 7920  .backward()` by 
-00001380: 6066 6162 7269 632e 6261 636b 7761 7264  `fabric.backward
-00001390: 286c 6f73 7329 602e 0a0a 2020 2060 6060  (loss)`...   ```
-000013a0: 6469 6666 0a20 2020 2d20 6c6f 7373 2e62  diff.   - loss.b
-000013b0: 6163 6b77 6172 6428 290a 2020 202b 2066  ackward().   + f
-000013c0: 6162 7269 632e 6261 636b 7761 7264 286c  abric.backward(l
-000013d0: 6f73 7329 0a20 2020 6060 600a 0a31 2e20  oss).   ```..1. 
-000013e0: 5275 6e20 7468 6520 7363 7269 7074 2066  Run the script f
-000013f0: 726f 6d20 7468 6520 7465 726d 696e 616c  rom the terminal
-00001400: 2077 6974 680a 0a20 2020 6060 6062 6173   with..   ```bas
-00001410: 680a 2020 206c 6967 6874 6e69 6e67 2072  h.   lightning r
-00001420: 756e 206d 6f64 656c 2070 6174 682f 746f  un model path/to
-00001430: 2f74 7261 696e 2e70 790a 2020 2060 6060  /train.py.   ```
-00001440: 0a0a 6f72 2075 7365 2074 6865 206c 6175  ..or use the lau
-00001450: 6e63 6828 2920 6d65 7468 6f64 2069 6e20  nch() method in 
-00001460: 6120 6e6f 7465 626f 6f6b 2e20 4c65 6172  a notebook. Lear
-00001470: 6e20 6d6f 7265 2061 626f 7574 205b 6c61  n more about [la
-00001480: 756e 6368 696e 6720 6469 7374 7269 6275  unching distribu
-00001490: 7465 6420 7472 6169 6e69 6e67 5d28 6874  ted training](ht
-000014a0: 7470 733a 2f2f 6c69 6768 746e 696e 672e  tps://lightning.
-000014b0: 6169 2f64 6f63 732f 6661 6272 6963 2f73  ai/docs/fabric/s
-000014c0: 7461 626c 652f 6675 6e64 616d 656e 7461  table/fundamenta
-000014d0: 6c73 2f6c 6175 6e63 682e 6874 6d6c 292e  ls/launch.html).
-000014e0: 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ..______________
-000014f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001500: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001510: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001520: 5f5f 5f5f 5f5f 5f5f 0a0a 2320 4641 510a  ________..# FAQ.
-00001530: 0a23 2320 5768 656e 2074 6f20 7573 6520  .## When to use 
-00001540: 4661 6272 6963 3f0a 0a2d 202a 2a4d 696e  Fabric?..- **Min
-00001550: 696d 756d 2063 6f64 6520 6368 616e 6765  imum code change
-00001560: 732a 2a2d 2059 6f75 2077 616e 7420 746f  s**- You want to
-00001570: 2073 6361 6c65 2079 6f75 7220 5079 546f   scale your PyTo
-00001580: 7263 6820 6d6f 6465 6c20 746f 2075 7365  rch model to use
-00001590: 206d 756c 7469 2d47 5055 206f 7220 7573   multi-GPU or us
-000015a0: 6520 6164 7661 6e63 6564 2073 7472 6174  e advanced strat
-000015b0: 6567 6965 7320 6c69 6b65 2044 6565 7053  egies like DeepS
-000015c0: 7065 6564 2077 6974 686f 7574 2068 6176  peed without hav
-000015d0: 696e 6720 746f 2072 6566 6163 746f 722e  ing to refactor.
-000015e0: 2059 6f75 2064 6f6e e280 9974 2063 6172   You don...t car
-000015f0: 6520 6162 6f75 7420 7374 7275 6374 7572  e about structur
-00001600: 696e 6720 796f 7572 2063 6f64 652d 2079  ing your code- y
-00001610: 6f75 206a 7573 7420 7761 6e74 2074 6f20  ou just want to 
-00001620: 7363 616c 6520 6974 2061 7320 6661 7374  scale it as fast
-00001630: 2061 7320 706f 7373 6962 6c65 2e0a 2d20   as possible..- 
-00001640: 2a2a 4d61 786d 6975 6d20 636f 6e74 726f  **Maxmium contro
-00001650: 6c2a 2a2d 2057 7269 7465 2079 6f75 7220  l**- Write your 
-00001660: 6f77 6e20 7472 6169 6e69 6e67 2061 6e64  own training and
-00001670: 2f6f 7220 696e 6665 7265 6e63 6520 6c6f  /or inference lo
-00001680: 6769 6320 646f 776e 2074 6f20 7468 6520  gic down to the 
-00001690: 696e 6469 7669 6475 616c 206f 7074 696d  individual optim
-000016a0: 697a 6572 2063 616c 6c73 2e20 596f 7520  izer calls. You 
-000016b0: 6172 656e e280 9974 2066 6f72 6365 6420  aren...t forced 
-000016c0: 746f 2063 6f6e 666f 726d 2074 6f20 6120  to conform to a 
-000016d0: 7374 616e 6461 7264 697a 6564 2065 706f  standardized epo
-000016e0: 6368 2d62 6173 6564 2074 7261 696e 696e  ch-based trainin
-000016f0: 6720 6c6f 6f70 206c 696b 6520 7468 6520  g loop like the 
-00001700: 6f6e 6520 696e 204c 6967 6874 6e69 6e67  one in Lightning
-00001710: 2054 7261 696e 6572 2e20 596f 7520 6361   Trainer. You ca
-00001720: 6e20 646f 2066 6c65 7869 626c 6520 6974  n do flexible it
-00001730: 6572 6174 696f 6e20 6261 7365 6420 7472  eration based tr
-00001740: 6169 6e69 6e67 2c20 6d65 7461 2d6c 6561  aining, meta-lea
-00001750: 726e 696e 672c 2063 726f 7373 2d76 616c  rning, cross-val
-00001760: 6964 6174 696f 6e20 616e 6420 6f74 6865  idation and othe
-00001770: 7220 7479 7065 7320 6f66 206f 7074 696d  r types of optim
-00001780: 697a 6174 696f 6e20 616c 676f 7269 7468  ization algorith
-00001790: 6d73 2077 6974 686f 7574 2064 6967 6769  ms without diggi
-000017a0: 6e67 2069 6e74 6f20 6672 616d 6577 6f72  ng into framewor
-000017b0: 6b20 696e 7465 726e 616c 732e 2054 6869  k internals. Thi
-000017c0: 7320 616c 736f 206d 616b 6573 2069 7420  s also makes it 
-000017d0: 7375 7065 7220 6561 7379 2074 6f20 6164  super easy to ad
-000017e0: 6f70 7420 4661 6272 6963 2069 6e20 6578  opt Fabric in ex
-000017f0: 6973 7469 6e67 2050 7954 6f72 6368 2070  isting PyTorch p
-00001800: 726f 6a65 6374 7320 746f 2073 7065 6564  rojects to speed
-00001810: 2d75 7020 616e 6420 7363 616c 6520 796f  -up and scale yo
-00001820: 7572 206d 6f64 656c 7320 7769 7468 6f75  ur models withou
-00001830: 7420 7468 6520 636f 6d70 726f 6d69 7365  t the compromise
-00001840: 206f 6e20 6c61 7267 6520 7265 6661 6374   on large refact
-00001850: 6f72 732e 204a 7573 7420 7265 6d65 6d62  ors. Just rememb
-00001860: 6572 3a20 5769 7468 2067 7265 6174 2070  er: With great p
-00001870: 6f77 6572 2063 6f6d 6573 2061 2067 7265  ower comes a gre
-00001880: 6174 2072 6573 706f 6e73 6962 696c 6974  at responsibilit
-00001890: 792e 0a2d 202a 2a4d 6178 6d69 756d 2066  y..- **Maxmium f
-000018a0: 6c65 7869 6269 6c69 7479 2a2a 2d20 596f  lexibility**- Yo
-000018b0: 7520 7761 6e74 2074 6f20 6861 7665 2066  u want to have f
-000018c0: 756c 6c20 636f 6e74 726f 6c20 6f76 6572  ull control over
-000018d0: 2079 6f75 7220 656e 7469 7265 2074 7261   your entire tra
-000018e0: 696e 696e 672d 2069 6e20 4661 6272 6963  ining- in Fabric
-000018f0: 2061 6c6c 2066 6561 7475 7265 7320 6172   all features ar
-00001900: 6520 6f70 742d 696e 2c20 616e 6420 6974  e opt-in, and it
-00001910: 2070 726f 7669 6465 7320 796f 7520 7769   provides you wi
-00001920: 7468 2061 2074 6f6f 6c20 626f 7820 6f66  th a tool box of
-00001930: 2070 7269 6d69 7469 7665 7320 736f 2079   primitives so y
-00001940: 6f75 2063 616e 2062 7569 6c64 2079 6f75  ou can build you
-00001950: 7220 6f77 6e20 5472 6169 6e65 722e 0a0a  r own Trainer...
-00001960: 2323 2057 6865 6e20 746f 2075 7365 2074  ## When to use t
-00001970: 6865 205b 4c69 6768 746e 696e 6720 5472  he [Lightning Tr
-00001980: 6169 6e65 725d 2868 7474 7073 3a2f 2f6c  ainer](https://l
-00001990: 6967 6874 6e69 6e67 2e61 692f 646f 6373  ightning.ai/docs
-000019a0: 2f70 7974 6f72 6368 2f73 7461 626c 652f  /pytorch/stable/
-000019b0: 636f 6d6d 6f6e 2f74 7261 696e 6572 2e68  common/trainer.h
-000019c0: 746d 6c29 3f0a 0a2d 2059 6f75 2077 616e  tml)?..- You wan
-000019d0: 7420 746f 2068 6176 6520 616c 6c20 7468  t to have all th
-000019e0: 6520 656e 6769 6e65 6572 696e 6720 626f  e engineering bo
-000019f0: 696c 6572 706c 6174 6520 6861 6e64 6c65  ilerplate handle
-00001a00: 6420 666f 7220 796f 7520 2d20 646f 7a65  d for you - doze
-00001a10: 6e73 206f 6620 6665 6174 7572 6573 206c  ns of features l
-00001a20: 696b 6520 6368 6563 6b70 6f69 6e74 696e  ike checkpointin
-00001a30: 672c 206c 6f67 6769 6e67 2061 6e64 2065  g, logging and e
-00001a40: 6172 6c79 2073 746f 7070 696e 6720 6f75  arly stopping ou
-00001a50: 7420 6f66 2074 6865 2062 6f78 2e20 4c65  t of the box. Le
-00001a60: 7373 2068 6173 736c 652c 206c 6573 7320  ss hassle, less 
-00001a70: 6572 726f 7220 7072 6f6e 652c 2065 6173  error prone, eas
-00001a80: 7920 746f 2074 7279 2064 6966 6665 7265  y to try differe
-00001a90: 6e74 2074 6563 686e 6971 7565 7320 616e  nt techniques an
-00001aa0: 6420 6665 6174 7572 6573 2e0a 2d20 596f  d features..- Yo
-00001ab0: 7520 7761 6e74 2074 6f20 6861 7665 2067  u want to have g
-00001ac0: 6f6f 6420 6465 6661 756c 7473 2063 686f  ood defaults cho
-00001ad0: 7365 6e20 666f 7220 796f 7520 2d20 736f  sen for you - so
-00001ae0: 2079 6f75 2063 616e 2068 6176 6520 6120   you can have a 
-00001af0: 6265 7474 6572 2073 7461 7274 696e 6720  better starting 
-00001b00: 706f 696e 742e 0a2d 2059 6f75 2077 616e  point..- You wan
-00001b10: 7420 796f 7572 2063 6f64 6520 746f 2062  t your code to b
-00001b20: 6520 6d6f 6475 6c61 722c 2072 6561 6461  e modular, reada
-00001b30: 626c 6520 616e 6420 7765 6c6c 2073 7472  ble and well str
-00001b40: 7563 7475 7265 6420 2d20 6561 7379 2074  uctured - easy t
-00001b50: 6f20 7368 6172 6520 6265 7477 6565 6e20  o share between 
-00001b60: 7072 6f6a 6563 7473 2061 6e64 2077 6974  projects and wit
-00001b70: 6820 636f 6c6c 6162 6f72 6174 6f72 732e  h collaborators.
-00001b80: 0a0a 2323 2043 616e 2049 2075 7365 2046  ..## Can I use F
-00001b90: 6162 7269 6320 7769 7468 206d 7920 4c69  abric with my Li
-00001ba0: 6768 746e 696e 674d 6f64 756c 6520 6f72  ghtningModule or
-00001bb0: 204c 6967 6874 6e69 6e67 2043 616c 6c62   Lightning Callb
-00001bc0: 6163 6b3f 0a0a 5965 7320 3a29 2046 6162  ack?..Yes :) Fab
-00001bd0: 7269 6320 776f 726b 7320 7769 7468 2050  ric works with P
-00001be0: 7954 6f72 6368 204c 6967 6874 6e69 6e67  yTorch Lightning
-00001bf0: 4d6f 6475 6c65 7320 616e 6420 4361 6c6c  Modules and Call
-00001c00: 6261 636b 732c 2073 6f20 796f 7520 6361  backs, so you ca
-00001c10: 6e20 6368 6f6f 7365 2068 6f77 2074 6f20  n choose how to 
-00001c20: 7374 7275 6374 7572 6520 796f 7572 2063  structure your c
-00001c30: 6f64 6520 616e 6420 7265 7573 6520 6578  ode and reuse ex
-00001c40: 6973 7469 6e67 206d 6f64 656c 7320 616e  isting models an
-00001c50: 6420 6361 6c6c 6261 636b 7320 6173 2079  d callbacks as y
-00001c60: 6f75 2077 6973 682e 2052 6561 6420 6d6f  ou wish. Read mo
-00001c70: 7265 205b 6865 7265 5d28 6874 7470 733a  re [here](https:
-00001c80: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
-00001c90: 6f63 732f 6661 6272 6963 2f73 7461 626c  ocs/fabric/stabl
-00001ca0: 652f 6675 6e64 616d 656e 7461 6c73 2f63  e/fundamentals/c
-00001cb0: 6f64 655f 7374 7275 6374 7572 652e 6874  ode_structure.ht
-00001cc0: 6d6c 292e 0a0a 3c69 6d67 2073 7263 3d22  ml)...<img src="
-00001cd0: 6874 7470 733a 2f2f 706c 2d70 7562 6c69  https://pl-publi
-00001ce0: 632d 6461 7461 2e73 332e 616d 617a 6f6e  c-data.s3.amazon
-00001cf0: 6177 732e 636f 6d2f 6173 7365 7473 5f6c  aws.com/assets_l
-00001d00: 6967 6874 6e69 6e67 2f63 6f6e 7469 6e75  ightning/continu
-00001d10: 756d 2e70 6e67 2220 7769 6474 683d 2238  um.png" width="8
-00001d20: 3030 7078 223e 0a0a 5f5f 5f5f 5f5f 5f5f  00px">..________
-00001d30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001d40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001d50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001d60: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a  ______________..
-00001d70: 2320 4578 616d 706c 6573 0a0a 2d20 5b47  # Examples..- [G
-00001d80: 414e 5d28 6874 7470 733a 2f2f 6769 7468  AN](https://gith
-00001d90: 7562 2e63 6f6d 2f4c 6967 6874 6e69 6e67  ub.com/Lightning
-00001da0: 2d41 492f 6c69 6768 746e 696e 672f 7472  -AI/lightning/tr
-00001db0: 6565 2f6d 6173 7465 722f 6578 616d 706c  ee/master/exampl
-00001dc0: 6573 2f66 6162 7269 632f 6463 6761 6e29  es/fabric/dcgan)
-00001dd0: 0a2d 205b 4d65 7461 206c 6561 726e 696e  .- [Meta learnin
-00001de0: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001df0: 622e 636f 6d2f 4c69 6768 746e 696e 672d  b.com/Lightning-
-00001e00: 4149 2f6c 6967 6874 6e69 6e67 2f74 7265  AI/lightning/tre
-00001e10: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
-00001e20: 732f 6661 6272 6963 2f6d 6574 615f 6c65  s/fabric/meta_le
-00001e30: 6172 6e69 6e67 290a 2d20 5b52 6569 6e66  arning).- [Reinf
-00001e40: 6f72 6365 6d65 6e74 206c 6561 726e 696e  orcement learnin
-00001e50: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001e60: 622e 636f 6d2f 4c69 6768 746e 696e 672d  b.com/Lightning-
-00001e70: 4149 2f6c 6967 6874 6e69 6e67 2f74 7265  AI/lightning/tre
-00001e80: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
-00001e90: 732f 6661 6272 6963 2f72 6569 6e66 6f72  s/fabric/reinfor
-00001ea0: 6365 6d65 6e74 5f6c 6561 726e 696e 6729  cement_learning)
-00001eb0: 0a2d 205b 4b2d 466f 6c64 2063 726f 7373  .- [K-Fold cross
-00001ec0: 2076 616c 6964 6174 696f 6e5d 2868 7474   validation](htt
-00001ed0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001ee0: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
-00001ef0: 6874 6e69 6e67 2f74 7265 652f 6d61 7374  htning/tree/mast
-00001f00: 6572 2f65 7861 6d70 6c65 732f 6661 6272  er/examples/fabr
-00001f10: 6963 2f6b 666f 6c64 5f63 7629 0a0a 5f5f  ic/kfold_cv)..__
-00001f20: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f60: 5f5f 5f5f 0a0a 2323 2041 736b 696e 6720  ____..## Asking 
-00001f70: 666f 7220 6865 6c70 0a0a 4966 2079 6f75  for help..If you
-00001f80: 2068 6176 6520 616e 7920 7175 6573 7469   have any questi
-00001f90: 6f6e 7320 706c 6561 7365 3a0a 0a31 2e20  ons please:..1. 
-00001fa0: 5b52 6561 6420 7468 6520 646f 6373 5d28  [Read the docs](
-00001fb0: 6874 7470 733a 2f2f 6c69 6768 746e 696e  https://lightnin
-00001fc0: 672e 6169 2f64 6f63 732f 6661 6272 6963  g.ai/docs/fabric
-00001fd0: 292e 0a31 2e20 5b41 736b 2061 2071 7565  )..1. [Ask a que
-00001fe0: 7374 696f 6e20 696e 206f 7572 2066 6f72  stion in our for
-00001ff0: 756d 5d28 6874 7470 733a 2f2f 6c69 6768  um](https://ligh
-00002000: 746e 696e 672e 6169 2f66 6f72 756d 732f  tning.ai/forums/
-00002010: 292e 0a31 2e20 5b4a 6f69 6e20 6f75 7220  )..1. [Join our 
-00002020: 6469 7363 6f72 6420 636f 6d6d 756e 6974  discord communit
-00002030: 795d 2868 7474 7073 3a2f 2f64 6973 636f  y](https://disco
-00002040: 7264 2e63 6f6d 2f69 6e76 6974 652f 7466  rd.com/invite/tf
-00002050: 5846 6574 455a 7876 292e 0a0a 0a         XFetEZxv)....
+00000630: 5f5f 5f5f 5f5f 0a0a 3c70 2061 6c69 676e  ______..<p align
+00000640: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+00000650: 6872 6566 3d22 6874 7470 733a 2f2f 6c69  href="https://li
+00000660: 6768 746e 696e 672e 6169 2f22 3e57 6562  ghtning.ai/">Web
+00000670: 7369 7465 3c2f 613e 20e2 80a2 0a20 203c  site</a> ....  <
+00000680: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000690: 6c69 6768 746e 696e 672e 6169 2f64 6f63  lightning.ai/doc
+000006a0: 732f 6661 6272 6963 2f22 3e44 6f63 733c  s/fabric/">Docs<
+000006b0: 2f61 3e20 e280 a20a 2020 3c61 2068 7265  /a> ....  <a hre
+000006c0: 663d 2223 6765 7474 696e 672d 7374 6172  f="#getting-star
+000006d0: 7465 6422 3e47 6574 7469 6e67 2073 7461  ted">Getting sta
+000006e0: 7274 6564 3c2f 613e 20e2 80a2 0a20 203c  rted</a> ....  <
+000006f0: 6120 6872 6566 3d22 2366 6171 223e 4641  a href="#faq">FA
+00000700: 513c 2f61 3e20 e280 a20a 2020 3c61 2068  Q</a> ....  <a h
+00000710: 7265 663d 2223 6173 6b69 6e67 2d66 6f72  ref="#asking-for
+00000720: 2d68 656c 7022 3e48 656c 703c 2f61 3e20  -help">Help</a> 
+00000730: e280 a20a 2020 3c61 2068 7265 663d 2268  ....  <a href="h
+00000740: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
+00000750: 672f 5670 7450 435a 6b47 4e61 223e 4469  g/VptPCZkGNa">Di
+00000760: 7363 6f72 643c 2f61 3e0a 3c2f 703e 0a0a  scord</a>.</p>..
+00000770: 5b21 5b50 7950 4920 2d20 5079 7468 6f6e  [![PyPI - Python
+00000780: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00000790: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007a0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+000007b0: 2f6c 6967 6874 6e69 6e67 5f66 6162 7269  /lightning_fabri
+000007c0: 6329 5d28 6874 7470 733a 2f2f 7079 7069  c)](https://pypi
+000007d0: 2e6f 7267 2f70 726f 6a65 6374 2f6c 6967  .org/project/lig
+000007e0: 6874 6e69 6e67 5f66 6162 7269 632f 290a  htning_fabric/).
+000007f0: 5b21 5b50 7950 4920 5374 6174 7573 5d28  [![PyPI Status](
+00000800: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000810: 7279 2e69 6f2f 7079 2f6c 6967 6874 6e69  ry.io/py/lightni
+00000820: 6e67 5f66 6162 7269 632e 7376 6729 5d28  ng_fabric.svg)](
+00000830: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000840: 7279 2e69 6f2f 7079 2f6c 6967 6874 6e69  ry.io/py/lightni
+00000850: 6e67 5f66 6162 7269 6329 0a5b 215b 5079  ng_fabric).[![Py
+00000860: 5049 2053 7461 7475 735d 2868 7474 7073  PI Status](https
+00000870: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
+00000880: 6765 2f6c 6967 6874 6e69 6e67 5f66 6162  ge/lightning_fab
+00000890: 7269 6329 5d28 6874 7470 733a 2f2f 7065  ric)](https://pe
+000008a0: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
+000008b0: 6c69 6768 746e 696e 675f 6661 6272 6963  lightning_fabric
+000008c0: 290a 5b21 5b43 6f6e 6461 5d28 6874 7470  ).[![Conda](http
+000008d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000008e0: 696f 2f63 6f6e 6461 2f76 2f63 6f6e 6461  io/conda/v/conda
+000008f0: 2d66 6f72 6765 2f6c 6967 6874 6e69 6e67  -forge/lightning
+00000900: 5f66 6162 7269 633f 6c61 6265 6c3d 636f  _fabric?label=co
+00000910: 6e64 6126 636f 6c6f 723d 7375 6363 6573  nda&color=succes
+00000920: 7329 5d28 6874 7470 733a 2f2f 616e 6163  s)](https://anac
+00000930: 6f6e 6461 2e6f 7267 2f63 6f6e 6461 2d66  onda.org/conda-f
+00000940: 6f72 6765 2f6c 6967 6874 6e69 6e67 5f66  orge/lightning_f
+00000950: 6162 7269 6329 0a0a 3c2f 6469 763e 0a0a  abric)..</div>..
+00000960: 2320 4c69 6768 746e 696e 6720 4661 6272  # Lightning Fabr
+00000970: 6963 3a20 4578 7065 7274 2063 6f6e 7472  ic: Expert contr
+00000980: 6f6c 2e0a 0a52 756e 206f 6e20 616e 7920  ol...Run on any 
+00000990: 6465 7669 6365 2061 7420 616e 7920 7363  device at any sc
+000009a0: 616c 6520 7769 7468 2065 7870 6572 742d  ale with expert-
+000009b0: 6c65 7665 6c20 636f 6e74 726f 6c20 6f76  level control ov
+000009c0: 6572 2050 7954 6f72 6368 2074 7261 696e  er PyTorch train
+000009d0: 696e 6720 6c6f 6f70 2061 6e64 2073 6361  ing loop and sca
+000009e0: 6c69 6e67 2073 7472 6174 6567 792e 2059  ling strategy. Y
+000009f0: 6f75 2063 616e 2065 7665 6e20 7772 6974  ou can even writ
+00000a00: 6520 796f 7572 206f 776e 2054 7261 696e  e your own Train
+00000a10: 6572 2e0a 0a46 6162 7269 6320 6973 2064  er...Fabric is d
+00000a20: 6573 6967 6e65 6420 666f 7220 7468 6520  esigned for the 
+00000a30: 6d6f 7374 2063 6f6d 706c 6578 206d 6f64  most complex mod
+00000a40: 656c 7320 6c69 6b65 2066 6f75 6e64 6174  els like foundat
+00000a50: 696f 6e20 6d6f 6465 6c20 7363 616c 696e  ion model scalin
+00000a60: 672c 204c 4c4d 732c 2064 6966 6675 7369  g, LLMs, diffusi
+00000a70: 6f6e 2c20 7472 616e 7366 6f72 6d65 7273  on, transformers
+00000a80: 2c20 7265 696e 666f 7263 656d 656e 7420  , reinforcement 
+00000a90: 6c65 6172 6e69 6e67 2c20 6163 7469 7665  learning, active
+00000aa0: 206c 6561 726e 696e 672e 204f 6620 616e   learning. Of an
+00000ab0: 7920 7369 7a65 2e0a 0a3c 7461 626c 653e  y size...<table>
+00000ac0: 0a3c 7472 3e0a 3c74 683e 5768 6174 2074  .<tr>.<th>What t
+00000ad0: 6f20 6368 616e 6765 3c2f 7468 3e0a 3c74  o change</th>.<t
+00000ae0: 683e 5265 7375 6c74 696e 6720 4661 6272  h>Resulting Fabr
+00000af0: 6963 2043 6f64 6520 2863 6f70 7920 6d65  ic Code (copy me
+00000b00: 2129 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74  !)</th>.</tr>.<t
+00000b10: 723e 0a3c 7464 3e0a 3c73 7562 3e0a 0a60  r>.<td>.<sub>..`
+00000b20: 6060 6469 6666 0a2b 2069 6d70 6f72 7420  ``diff.+ import 
+00000b30: 6c69 6768 746e 696e 6720 6173 204c 0a20  lightning as L. 
+00000b40: 2069 6d70 6f72 7420 746f 7263 683b 2069   import torch; i
+00000b50: 6d70 6f72 7420 746f 7263 6876 6973 696f  mport torchvisio
+00000b60: 6e20 6173 2074 760a 0a2b 2066 6162 7269  n as tv..+ fabri
+00000b70: 6320 3d20 4c2e 4661 6272 6963 2829 0a2b  c = L.Fabric().+
+00000b80: 2066 6162 7269 632e 6c61 756e 6368 2829   fabric.launch()
+00000b90: 0a0a 2020 6d6f 6465 6c20 3d20 7476 2e6d  ..  model = tv.m
+00000ba0: 6f64 656c 732e 7265 736e 6574 3138 2829  odels.resnet18()
+00000bb0: 0a20 206f 7074 696d 697a 6572 203d 2074  .  optimizer = t
+00000bc0: 6f72 6368 2e6f 7074 696d 2e53 4744 286d  orch.optim.SGD(m
+00000bd0: 6f64 656c 2e70 6172 616d 6574 6572 7328  odel.parameters(
+00000be0: 292c 206c 723d 302e 3030 3129 0a2d 2064  ), lr=0.001).- d
+00000bf0: 6576 6963 6520 3d20 2263 7564 6122 2069  evice = "cuda" i
+00000c00: 6620 746f 7263 682e 6375 6461 2e69 735f  f torch.cuda.is_
+00000c10: 6176 6169 6c61 626c 6528 2920 656c 7365  available() else
+00000c20: 2022 6370 7522 0a2d 206d 6f64 656c 2e74   "cpu".- model.t
+00000c30: 6f28 6465 7669 6365 290a 2b20 6d6f 6465  o(device).+ mode
+00000c40: 6c2c 206f 7074 696d 697a 6572 203d 2066  l, optimizer = f
+00000c50: 6162 7269 632e 7365 7475 7028 6d6f 6465  abric.setup(mode
+00000c60: 6c2c 206f 7074 696d 697a 6572 290a 0a20  l, optimizer).. 
+00000c70: 2064 6174 6173 6574 203d 2074 762e 6461   dataset = tv.da
+00000c80: 7461 7365 7473 2e43 4946 4152 3130 2822  tasets.CIFAR10("
+00000c90: 6461 7461 222c 2064 6f77 6e6c 6f61 643d  data", download=
+00000ca0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 2020 2020 2020 7472 6169 6e3d 5472 7565        train=True
+00000cd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cf0: 2020 7472 616e 7366 6f72 6d3d 7476 2e74    transform=tv.t
+00000d00: 7261 6e73 666f 726d 732e 546f 5465 6e73  ransforms.ToTens
+00000d10: 6f72 2829 290a 2020 6461 7461 6c6f 6164  or()).  dataload
+00000d20: 6572 203d 2074 6f72 6368 2e75 7469 6c73  er = torch.utils
+00000d30: 2e64 6174 612e 4461 7461 4c6f 6164 6572  .data.DataLoader
+00000d40: 2864 6174 6173 6574 2c20 6261 7463 685f  (dataset, batch_
+00000d50: 7369 7a65 3d38 290a 2b20 6461 7461 6c6f  size=8).+ datalo
+00000d60: 6164 6572 203d 2066 6162 7269 632e 7365  ader = fabric.se
+00000d70: 7475 705f 6461 7461 6c6f 6164 6572 7328  tup_dataloaders(
+00000d80: 6461 7461 6c6f 6164 6572 290a 0a20 206d  dataloader)..  m
+00000d90: 6f64 656c 2e74 7261 696e 2829 0a20 206e  odel.train().  n
+00000da0: 756d 5f65 706f 6368 7320 3d20 3130 0a20  um_epochs = 10. 
+00000db0: 2066 6f72 2065 706f 6368 2069 6e20 7261   for epoch in ra
+00000dc0: 6e67 6528 6e75 6d5f 6570 6f63 6873 293a  nge(num_epochs):
+00000dd0: 0a20 2020 2020 2066 6f72 2062 6174 6368  .      for batch
+00000de0: 2069 6e20 6461 7461 6c6f 6164 6572 3a0a   in dataloader:.
+00000df0: 2020 2020 2020 2020 2020 696e 7075 7473            inputs
+00000e00: 2c20 6c61 6265 6c73 203d 2062 6174 6368  , labels = batch
+00000e10: 0a2d 2020 2020 2020 2020 2069 6e70 7574  .-         input
+00000e20: 732c 206c 6162 656c 7320 3d20 696e 7075  s, labels = inpu
+00000e30: 7473 2e74 6f28 6465 7669 6365 292c 206c  ts.to(device), l
+00000e40: 6162 656c 732e 746f 2864 6576 6963 6529  abels.to(device)
+00000e50: 0a20 2020 2020 2020 2020 206f 7074 696d  .          optim
+00000e60: 697a 6572 2e7a 6572 6f5f 6772 6164 2829  izer.zero_grad()
+00000e70: 0a20 2020 2020 2020 2020 206f 7574 7075  .          outpu
+00000e80: 7473 203d 206d 6f64 656c 2869 6e70 7574  ts = model(input
+00000e90: 7329 0a20 2020 2020 2020 2020 206c 6f73  s).          los
+00000ea0: 7320 3d20 746f 7263 682e 6e6e 2e66 756e  s = torch.nn.fun
+00000eb0: 6374 696f 6e61 6c2e 6372 6f73 735f 656e  ctional.cross_en
+00000ec0: 7472 6f70 7928 6f75 7470 7574 732c 206c  tropy(outputs, l
+00000ed0: 6162 656c 7329 0a2d 2020 2020 2020 2020  abels).-        
+00000ee0: 206c 6f73 732e 6261 636b 7761 7264 2829   loss.backward()
+00000ef0: 0a2b 2020 2020 2020 2020 2066 6162 7269  .+         fabri
+00000f00: 632e 6261 636b 7761 7264 286c 6f73 7329  c.backward(loss)
+00000f10: 0a20 2020 2020 2020 2020 206f 7074 696d  .          optim
+00000f20: 697a 6572 2e73 7465 7028 290a 6060 600a  izer.step().```.
+00000f30: 0a3c 2f73 7562 3e0a 3c74 643e 0a3c 7375  .</sub>.<td>.<su
+00000f40: 623e 0a0a 6060 6050 7974 686f 6e0a 696d  b>..```Python.im
+00000f50: 706f 7274 206c 6967 6874 6e69 6e67 2061  port lightning a
+00000f60: 7320 4c0a 696d 706f 7274 2074 6f72 6368  s L.import torch
+00000f70: 3b20 696d 706f 7274 2074 6f72 6368 7669  ; import torchvi
+00000f80: 7369 6f6e 2061 7320 7476 0a0a 6661 6272  sion as tv..fabr
+00000f90: 6963 203d 204c 2e46 6162 7269 6328 290a  ic = L.Fabric().
+00000fa0: 6661 6272 6963 2e6c 6175 6e63 6828 290a  fabric.launch().
+00000fb0: 0a6d 6f64 656c 203d 2074 762e 6d6f 6465  .model = tv.mode
+00000fc0: 6c73 2e72 6573 6e65 7431 3828 290a 6f70  ls.resnet18().op
+00000fd0: 7469 6d69 7a65 7220 3d20 746f 7263 682e  timizer = torch.
+00000fe0: 6f70 7469 6d2e 5347 4428 6d6f 6465 6c2e  optim.SGD(model.
+00000ff0: 7061 7261 6d65 7465 7273 2829 2c20 6c72  parameters(), lr
+00001000: 3d30 2e30 3031 290a 6d6f 6465 6c2c 206f  =0.001).model, o
+00001010: 7074 696d 697a 6572 203d 2066 6162 7269  ptimizer = fabri
+00001020: 632e 7365 7475 7028 6d6f 6465 6c2c 206f  c.setup(model, o
+00001030: 7074 696d 697a 6572 290a 0a64 6174 6173  ptimizer)..datas
+00001040: 6574 203d 2074 762e 6461 7461 7365 7473  et = tv.datasets
+00001050: 2e43 4946 4152 3130 2822 6461 7461 222c  .CIFAR10("data",
+00001060: 2064 6f77 6e6c 6f61 643d 5472 7565 2c0a   download=True,.
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00001090: 6169 6e3d 5472 7565 2c0a 2020 2020 2020  ain=True,.      
+000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+000010c0: 6d3d 7476 2e74 7261 6e73 666f 726d 732e  m=tv.transforms.
+000010d0: 546f 5465 6e73 6f72 2829 290a 6461 7461  ToTensor()).data
+000010e0: 6c6f 6164 6572 203d 2074 6f72 6368 2e75  loader = torch.u
+000010f0: 7469 6c73 2e64 6174 612e 4461 7461 4c6f  tils.data.DataLo
+00001100: 6164 6572 2864 6174 6173 6574 2c20 6261  ader(dataset, ba
+00001110: 7463 685f 7369 7a65 3d38 290a 6461 7461  tch_size=8).data
+00001120: 6c6f 6164 6572 203d 2066 6162 7269 632e  loader = fabric.
+00001130: 7365 7475 705f 6461 7461 6c6f 6164 6572  setup_dataloader
+00001140: 7328 6461 7461 6c6f 6164 6572 290a 0a6d  s(dataloader)..m
+00001150: 6f64 656c 2e74 7261 696e 2829 0a6e 756d  odel.train().num
+00001160: 5f65 706f 6368 7320 3d20 3130 0a66 6f72  _epochs = 10.for
+00001170: 2065 706f 6368 2069 6e20 7261 6e67 6528   epoch in range(
+00001180: 6e75 6d5f 6570 6f63 6873 293a 0a20 2020  num_epochs):.   
+00001190: 2066 6f72 2062 6174 6368 2069 6e20 6461   for batch in da
+000011a0: 7461 6c6f 6164 6572 3a0a 2020 2020 2020  taloader:.      
+000011b0: 2020 696e 7075 7473 2c20 6c61 6265 6c73    inputs, labels
+000011c0: 203d 2062 6174 6368 0a20 2020 2020 2020   = batch.       
+000011d0: 206f 7074 696d 697a 6572 2e7a 6572 6f5f   optimizer.zero_
+000011e0: 6772 6164 2829 0a20 2020 2020 2020 206f  grad().        o
+000011f0: 7574 7075 7473 203d 206d 6f64 656c 2869  utputs = model(i
+00001200: 6e70 7574 7329 0a20 2020 2020 2020 206c  nputs).        l
+00001210: 6f73 7320 3d20 746f 7263 682e 6e6e 2e66  oss = torch.nn.f
+00001220: 756e 6374 696f 6e61 6c2e 6372 6f73 735f  unctional.cross_
+00001230: 656e 7472 6f70 7928 6f75 7470 7574 732c  entropy(outputs,
+00001240: 206c 6162 656c 7329 0a20 2020 2020 2020   labels).       
+00001250: 2066 6162 7269 632e 6261 636b 7761 7264   fabric.backward
+00001260: 286c 6f73 7329 0a20 2020 2020 2020 206f  (loss).        o
+00001270: 7074 696d 697a 6572 2e73 7465 7028 290a  ptimizer.step().
+00001280: 6060 600a 0a3c 2f73 7562 3e0a 3c2f 7464  ```..</sub>.</td
+00001290: 3e0a 3c2f 7472 3e0a 3c2f 7461 626c 653e  >.</tr>.</table>
+000012a0: 0a0a 2323 204b 6579 2066 6561 7475 7265  ..## Key feature
+000012b0: 730a 0a3c 6465 7461 696c 733e 0a20 203c  s..<details>.  <
+000012c0: 7375 6d6d 6172 793e 4561 7369 6c79 2073  summary>Easily s
+000012d0: 7769 7463 6820 6672 6f6d 2072 756e 6e69  witch from runni
+000012e0: 6e67 206f 6e20 4350 5520 746f 2047 5055  ng on CPU to GPU
+000012f0: 2028 4170 706c 6520 5369 6c69 636f 6e2c   (Apple Silicon,
+00001300: 2043 5544 412c 20e2 80a6 292c 2054 5055   CUDA, ...), TPU
+00001310: 2c20 6d75 6c74 692d 4750 5520 6f72 2065  , multi-GPU or e
+00001320: 7665 6e20 6d75 6c74 692d 6e6f 6465 2074  ven multi-node t
+00001330: 7261 696e 696e 673c 2f73 756d 6d61 7279  raining</summary
+00001340: 3e0a 0a60 6060 7079 7468 6f6e 0a23 2055  >..```python.# U
+00001350: 7365 2079 6f75 7220 6176 6169 6c61 626c  se your availabl
+00001360: 6520 6861 7264 7761 7265 0a23 206e 6f20  e hardware.# no 
+00001370: 636f 6465 2063 6861 6e67 6573 206e 6565  code changes nee
+00001380: 6465 640a 6661 6272 6963 203d 2046 6162  ded.fabric = Fab
+00001390: 7269 6328 290a 0a23 2052 756e 206f 6e20  ric()..# Run on 
+000013a0: 4750 5573 2028 4355 4441 206f 7220 4d50  GPUs (CUDA or MP
+000013b0: 5329 0a66 6162 7269 6320 3d20 4661 6272  S).fabric = Fabr
+000013c0: 6963 2861 6363 656c 6572 6174 6f72 3d22  ic(accelerator="
+000013d0: 6770 7522 290a 0a23 2038 2047 5055 730a  gpu")..# 8 GPUs.
+000013e0: 6661 6272 6963 203d 2046 6162 7269 6328  fabric = Fabric(
+000013f0: 6163 6365 6c65 7261 746f 723d 2267 7075  accelerator="gpu
+00001400: 222c 2064 6576 6963 6573 3d38 290a 0a23  ", devices=8)..#
+00001410: 2032 3536 2047 5055 732c 206d 756c 7469   256 GPUs, multi
+00001420: 2d6e 6f64 650a 6661 6272 6963 203d 2046  -node.fabric = F
+00001430: 6162 7269 6328 6163 6365 6c65 7261 746f  abric(accelerato
+00001440: 723d 2267 7075 222c 2064 6576 6963 6573  r="gpu", devices
+00001450: 3d38 2c20 6e75 6d5f 6e6f 6465 733d 3332  =8, num_nodes=32
+00001460: 290a 0a23 2052 756e 206f 6e20 5450 5573  )..# Run on TPUs
+00001470: 0a66 6162 7269 6320 3d20 4661 6272 6963  .fabric = Fabric
+00001480: 2861 6363 656c 6572 6174 6f72 3d22 7470  (accelerator="tp
+00001490: 7522 290a 6060 600a 0a3c 2f64 6574 6169  u").```..</detai
+000014a0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a20  ls>..<details>. 
+000014b0: 203c 7375 6d6d 6172 793e 5573 6520 7374   <summary>Use st
+000014c0: 6174 652d 6f66 2d74 6865 2d61 7274 2064  ate-of-the-art d
+000014d0: 6973 7472 6962 7574 6564 2074 7261 696e  istributed train
+000014e0: 696e 6720 7374 7261 7465 6769 6573 2028  ing strategies (
+000014f0: 4444 502c 2046 5344 502c 2044 6565 7053  DDP, FSDP, DeepS
+00001500: 7065 6564 2920 616e 6420 6d69 7865 6420  peed) and mixed 
+00001510: 7072 6563 6973 696f 6e20 6f75 7420 6f66  precision out of
+00001520: 2074 6865 2062 6f78 3c2f 7375 6d6d 6172   the box</summar
+00001530: 793e 0a0a 6060 6070 7974 686f 6e0a 2320  y>..```python.# 
+00001540: 5573 6520 7374 6174 652d 6f66 2d74 6865  Use state-of-the
+00001550: 2d61 7274 2064 6973 7472 6962 7574 6564  -art distributed
+00001560: 2074 7261 696e 696e 6720 7465 6368 6e69   training techni
+00001570: 7175 6573 0a66 6162 7269 6320 3d20 4661  ques.fabric = Fa
+00001580: 6272 6963 2873 7472 6174 6567 793d 2264  bric(strategy="d
+00001590: 6470 2229 0a66 6162 7269 6320 3d20 4661  dp").fabric = Fa
+000015a0: 6272 6963 2873 7472 6174 6567 793d 2264  bric(strategy="d
+000015b0: 6565 7073 7065 6564 2229 0a66 6162 7269  eepspeed").fabri
+000015c0: 6320 3d20 4661 6272 6963 2873 7472 6174  c = Fabric(strat
+000015d0: 6567 793d 2266 7364 7022 290a 0a23 2053  egy="fsdp")..# S
+000015e0: 7769 7463 6820 7468 6520 7072 6563 6973  witch the precis
+000015f0: 696f 6e0a 6661 6272 6963 203d 2046 6162  ion.fabric = Fab
+00001600: 7269 6328 7072 6563 6973 696f 6e3d 2231  ric(precision="1
+00001610: 362d 6d69 7865 6422 290a 6661 6272 6963  6-mixed").fabric
+00001620: 203d 2046 6162 7269 6328 7072 6563 6973   = Fabric(precis
+00001630: 696f 6e3d 2236 3422 290a 6060 600a 0a3c  ion="64").```..<
+00001640: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
+00001650: 696c 733e 0a20 203c 7375 6d6d 6172 793e  ils>.  <summary>
+00001660: 416c 6c20 7468 6520 6465 7669 6365 206c  All the device l
+00001670: 6f67 6963 2062 6f69 6c65 7270 6c61 7465  ogic boilerplate
+00001680: 2069 7320 6861 6e64 6c65 6420 666f 7220   is handled for 
+00001690: 796f 753c 2f73 756d 6d61 7279 3e0a 0a60  you</summary>..`
+000016a0: 6060 6469 6666 0a20 2023 206e 6f20 6d6f  ``diff.  # no mo
+000016b0: 7265 206f 6620 7468 6973 210a 2d20 6d6f  re of this!.- mo
+000016c0: 6465 6c2e 746f 2864 6576 6963 6529 0a2d  del.to(device).-
+000016d0: 2062 6174 6368 2e74 6f28 6465 7669 6365   batch.to(device
+000016e0: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
+000016f0: 3e0a 0a3c 6465 7461 696c 733e 0a20 203c  >..<details>.  <
+00001700: 7375 6d6d 6172 793e 4275 696c 6420 796f  summary>Build yo
+00001710: 7572 206f 776e 2063 7573 746f 6d20 5472  ur own custom Tr
+00001720: 6169 6e65 7220 7573 696e 6720 4661 6272  ainer using Fabr
+00001730: 6963 2070 7269 6d69 7469 7665 7320 666f  ic primitives fo
+00001740: 7220 7472 6169 6e69 6e67 2063 6865 636b  r training check
+00001750: 706f 696e 7469 6e67 2c20 6c6f 6767 696e  pointing, loggin
+00001760: 672c 2061 6e64 206d 6f72 653c 2f73 756d  g, and more</sum
+00001770: 6d61 7279 3e0a 0a60 6060 7079 7468 6f6e  mary>..```python
+00001780: 0a69 6d70 6f72 7420 6c69 6768 746e 696e  .import lightnin
+00001790: 6720 6173 204c 0a0a 0a63 6c61 7373 204d  g as L...class M
+000017a0: 7943 7573 746f 6d54 7261 696e 6572 3a0a  yCustomTrainer:.
+000017b0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000017c0: 2873 656c 662c 2061 6363 656c 6572 6174  (self, accelerat
+000017d0: 6f72 3d22 6175 746f 222c 2073 7472 6174  or="auto", strat
+000017e0: 6567 793d 2261 7574 6f22 2c20 6465 7669  egy="auto", devi
+000017f0: 6365 733d 2261 7574 6f22 2c20 7072 6563  ces="auto", prec
+00001800: 6973 696f 6e3d 2233 322d 7472 7565 2229  ision="32-true")
+00001810: 3a0a 2020 2020 2020 2020 7365 6c66 2e66  :.        self.f
+00001820: 6162 7269 6320 3d20 4c2e 4661 6272 6963  abric = L.Fabric
+00001830: 2861 6363 656c 6572 6174 6f72 3d61 6363  (accelerator=acc
+00001840: 656c 6572 6174 6f72 2c20 7374 7261 7465  elerator, strate
+00001850: 6779 3d73 7472 6174 6567 792c 2064 6576  gy=strategy, dev
+00001860: 6963 6573 3d64 6576 6963 6573 2c20 7072  ices=devices, pr
+00001870: 6563 6973 696f 6e3d 7072 6563 6973 696f  ecision=precisio
+00001880: 6e29 0a0a 2020 2020 6465 6620 6669 7428  n)..    def fit(
+00001890: 7365 6c66 2c20 6d6f 6465 6c2c 206f 7074  self, model, opt
+000018a0: 696d 697a 6572 2c20 6461 7461 6c6f 6164  imizer, dataload
+000018b0: 6572 2c20 6d61 785f 6570 6f63 6873 293a  er, max_epochs):
+000018c0: 0a20 2020 2020 2020 2073 656c 662e 6661  .        self.fa
+000018d0: 6272 6963 2e6c 6175 6e63 6828 290a 0a20  bric.launch().. 
+000018e0: 2020 2020 2020 206d 6f64 656c 2c20 6f70         model, op
+000018f0: 7469 6d69 7a65 7220 3d20 7365 6c66 2e66  timizer = self.f
+00001900: 6162 7269 632e 7365 7475 7028 6d6f 6465  abric.setup(mode
+00001910: 6c2c 206f 7074 696d 697a 6572 290a 2020  l, optimizer).  
+00001920: 2020 2020 2020 6461 7461 6c6f 6164 6572        dataloader
+00001930: 203d 2073 656c 662e 6661 6272 6963 2e73   = self.fabric.s
+00001940: 6574 7570 5f64 6174 616c 6f61 6465 7273  etup_dataloaders
+00001950: 2864 6174 616c 6f61 6465 7229 0a20 2020  (dataloader).   
+00001960: 2020 2020 206d 6f64 656c 2e74 7261 696e       model.train
+00001970: 2829 0a0a 2020 2020 2020 2020 666f 7220  ()..        for 
+00001980: 6570 6f63 6820 696e 2072 616e 6765 286d  epoch in range(m
+00001990: 6178 5f65 706f 6368 7329 3a0a 2020 2020  ax_epochs):.    
+000019a0: 2020 2020 2020 2020 666f 7220 6261 7463          for batc
+000019b0: 6820 696e 2064 6174 616c 6f61 6465 723a  h in dataloader:
+000019c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000019d0: 2069 6e70 7574 2c20 7461 7267 6574 203d   input, target =
+000019e0: 2062 6174 6368 0a20 2020 2020 2020 2020   batch.         
+000019f0: 2020 2020 2020 206f 7074 696d 697a 6572         optimizer
+00001a00: 2e7a 6572 6f5f 6772 6164 2829 0a20 2020  .zero_grad().   
+00001a10: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00001a20: 7075 7420 3d20 6d6f 6465 6c28 696e 7075  put = model(inpu
+00001a30: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00001a40: 2020 206c 6f73 7320 3d20 6c6f 7373 5f66     loss = loss_f
+00001a50: 6e28 6f75 7470 7574 2c20 7461 7267 6574  n(output, target
+00001a60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00001a70: 2020 7365 6c66 2e66 6162 7269 632e 6261    self.fabric.ba
+00001a80: 636b 7761 7264 286c 6f73 7329 0a20 2020  ckward(loss).   
+00001a90: 2020 2020 2020 2020 2020 2020 206f 7074               opt
+00001aa0: 696d 697a 6572 2e73 7465 7028 290a 6060  imizer.step().``
+00001ab0: 600a 0a59 6f75 2063 616e 2066 696e 6420  `..You can find 
+00001ac0: 6120 6d6f 7265 2065 7874 656e 7369 7665  a more extensive
+00001ad0: 2065 7861 6d70 6c65 2069 6e20 6f75 7220   example in our 
+00001ae0: 5b65 7861 6d70 6c65 735d 282e 2e2f 2e2e  [examples](../..
+00001af0: 2f65 7861 6d70 6c65 732f 6661 6272 6963  /examples/fabric
+00001b00: 2f62 7569 6c64 5f79 6f75 725f 6f77 6e5f  /build_your_own_
+00001b10: 7472 6169 6e65 7229 0a0a 3c2f 6465 7461  trainer)..</deta
+00001b20: 696c 733e 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f  ils>..__________
+00001b30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001b40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001b50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001b60: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a 3c64  ____________..<d
+00001b70: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00001b80: 223e 0a20 2020 203c 6120 6872 6566 3d22  ">.    <a href="
+00001b90: 6874 7470 733a 2f2f 6c69 6768 746e 696e  https://lightnin
+00001ba0: 672e 6169 2f64 6f63 732f 6661 6272 6963  g.ai/docs/fabric
+00001bb0: 2f73 7461 626c 652f 223e 5265 6164 2074  /stable/">Read t
+00001bc0: 6865 204c 6967 6874 6e69 6e67 2046 6162  he Lightning Fab
+00001bd0: 7269 6320 646f 6373 3c2f 613e 0a3c 2f64  ric docs</a>.</d
+00001be0: 6976 3e0a 0a5f 5f5f 5f5f 5f5f 5f5f 5f5f  iv>..___________
+00001bf0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c00: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c10: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c20: 5f5f 5f5f 5f5f 5f5f 5f5f 5f0a 0a23 2047  ___________..# G
+00001c30: 6574 7469 6e67 2073 7461 7274 6564 0a0a  etting started..
+00001c40: 2323 2049 6e73 7461 6c6c 204c 6967 6874  ## Install Light
+00001c50: 6e69 6e67 0a0a 3c64 6574 6169 6c73 3e0a  ning..<details>.
+00001c60: 0a3c 7375 6d6d 6172 793e 5072 6572 6571  .<summary>Prereq
+00001c70: 7569 7369 7465 733c 2f73 756d 6d61 7279  uisites</summary
+00001c80: 3e0a 0a3e 2054 4950 3a20 5765 2073 7472  >..> TIP: We str
+00001c90: 6f6e 676c 7920 7265 636f 6d6d 656e 6420  ongly recommend 
+00001ca0: 6372 6561 7469 6e67 2061 2076 6972 7475  creating a virtu
+00001cb0: 616c 2065 6e76 6972 6f6e 6d65 6e74 2066  al environment f
+00001cc0: 6972 7374 2e0a 3e20 446f 6ee2 8099 7420  irst..> Don...t 
+00001cd0: 6b6e 6f77 2077 6861 7420 7468 6973 2069  know what this i
+00001ce0: 733f 2046 6f6c 6c6f 7720 6f75 7220 5b62  s? Follow our [b
+00001cf0: 6567 696e 6e65 7220 6775 6964 6520 6865  eginner guide he
+00001d00: 7265 5d28 6874 7470 733a 2f2f 6c69 6768  re](https://ligh
+00001d10: 746e 696e 672e 6169 2f64 6f63 732f 7374  tning.ai/docs/st
+00001d20: 6162 6c65 2f69 6e73 7461 6c6c 2f69 6e73  able/install/ins
+00001d30: 7461 6c6c 6174 696f 6e2e 6874 6d6c 292e  tallation.html).
+00001d40: 0a0a 2d20 5079 7468 6f6e 2033 2e38 2e78  ..- Python 3.8.x
+00001d50: 206f 7220 6c61 7465 7220 2833 2e38 2e78   or later (3.8.x
+00001d60: 2c20 332e 392e 782c 2033 2e31 302e 782c  , 3.9.x, 3.10.x,
+00001d70: 202e 2e2e 290a 0a3c 2f64 6574 6169 6c73   ...)..</details
+00001d80: 3e0a 0a60 6060 6261 7368 0a70 6970 2069  >..```bash.pip i
+00001d90: 6e73 7461 6c6c 202d 5520 6c69 6768 746e  nstall -U lightn
+00001da0: 696e 670a 6060 600a 0a23 2320 436f 6e76  ing.```..## Conv
+00001db0: 6572 7420 796f 7572 2050 7954 6f72 6368  ert your PyTorch
+00001dc0: 2074 6f20 4661 6272 6963 0a0a 312e 2043   to Fabric..1. C
+00001dd0: 7265 6174 6520 7468 6520 6046 6162 7269  reate the `Fabri
+00001de0: 6360 206f 626a 6563 7420 6174 2074 6865  c` object at the
+00001df0: 2062 6567 696e 6e69 6e67 206f 6620 796f   beginning of yo
+00001e00: 7572 2074 7261 696e 696e 6720 636f 6465  ur training code
+00001e10: 2e0a 0a20 2020 6060 600a 2020 2069 6d70  ...   ```.   imp
+00001e20: 6f72 7420 4c69 6768 746e 696e 6720 6173  ort Lightning as
+00001e30: 204c 0a0a 2020 2066 6162 7269 6320 3d20   L..   fabric = 
+00001e40: 4c2e 4661 6272 6963 2829 0a20 2020 6060  L.Fabric().   ``
+00001e50: 600a 0a31 2e20 4361 6c6c 2060 7365 7475  `..1. Call `setu
+00001e60: 7028 2960 206f 6e20 6561 6368 206d 6f64  p()` on each mod
+00001e70: 656c 2061 6e64 206f 7074 696d 697a 6572  el and optimizer
+00001e80: 2070 6169 7220 616e 6420 6073 6574 7570   pair and `setup
+00001e90: 5f64 6174 616c 6f61 6465 7273 2829 6020  _dataloaders()` 
+00001ea0: 6f6e 2061 6c6c 2079 6f75 7220 6461 7461  on all your data
+00001eb0: 206c 6f61 6465 7273 2e0a 0a20 2020 6060   loaders...   ``
+00001ec0: 600a 2020 206d 6f64 656c 2c20 6f70 7469  `.   model, opti
+00001ed0: 6d69 7a65 7220 3d20 6661 6272 6963 2e73  mizer = fabric.s
+00001ee0: 6574 7570 286d 6f64 656c 2c20 6f70 7469  etup(model, opti
+00001ef0: 6d69 7a65 7229 0a20 2020 6461 7461 6c6f  mizer).   datalo
+00001f00: 6164 6572 203d 2066 6162 7269 632e 7365  ader = fabric.se
+00001f10: 7475 705f 6461 7461 6c6f 6164 6572 7328  tup_dataloaders(
+00001f20: 6461 7461 6c6f 6164 6572 290a 2020 2060  dataloader).   `
+00001f30: 6060 0a0a 312e 2052 656d 6f76 6520 616c  ``..1. Remove al
+00001f40: 6c20 602e 746f 6020 616e 6420 602e 6375  l `.to` and `.cu
+00001f50: 6461 6020 6361 6c6c 7320 2d3e 2046 6162  da` calls -> Fab
+00001f60: 7269 6320 7769 6c6c 2074 616b 6520 6361  ric will take ca
+00001f70: 7265 206f 6620 6974 2e0a 0a20 2020 6060  re of it...   ``
+00001f80: 6064 6966 660a 2020 202d 206d 6f64 656c  `diff.   - model
+00001f90: 2e74 6f28 6465 7669 6365 290a 2020 202d  .to(device).   -
+00001fa0: 2062 6174 6368 2e74 6f28 6465 7669 6365   batch.to(device
+00001fb0: 290a 2020 2060 6060 0a0a 312e 2052 6570  ).   ```..1. Rep
+00001fc0: 6c61 6365 2060 6c6f 7373 2e62 6163 6b77  lace `loss.backw
+00001fd0: 6172 6428 2960 2062 7920 6066 6162 7269  ard()` by `fabri
+00001fe0: 632e 6261 636b 7761 7264 286c 6f73 7329  c.backward(loss)
+00001ff0: 602e 0a0a 2020 2060 6060 6469 6666 0a20  `...   ```diff. 
+00002000: 2020 2d20 6c6f 7373 2e62 6163 6b77 6172    - loss.backwar
+00002010: 6428 290a 2020 202b 2066 6162 7269 632e  d().   + fabric.
+00002020: 6261 636b 7761 7264 286c 6f73 7329 0a20  backward(loss). 
+00002030: 2020 6060 600a 0a31 2e20 5275 6e20 7468    ```..1. Run th
+00002040: 6520 7363 7269 7074 2066 726f 6d20 7468  e script from th
+00002050: 6520 7465 726d 696e 616c 2077 6974 680a  e terminal with.
+00002060: 0a20 2020 6060 6062 6173 680a 2020 206c  .   ```bash.   l
+00002070: 6967 6874 6e69 6e67 2072 756e 206d 6f64  ightning run mod
+00002080: 656c 2070 6174 682f 746f 2f74 7261 696e  el path/to/train
+00002090: 2e70 790a 2020 2060 6060 0a0a 6f72 2075  .py.   ```..or u
+000020a0: 7365 2074 6865 206c 6175 6e63 6828 2920  se the launch() 
+000020b0: 6d65 7468 6f64 2069 6e20 6120 6e6f 7465  method in a note
+000020c0: 626f 6f6b 2e20 4c65 6172 6e20 6d6f 7265  book. Learn more
+000020d0: 2061 626f 7574 205b 6c61 756e 6368 696e   about [launchin
+000020e0: 6720 6469 7374 7269 6275 7465 6420 7472  g distributed tr
+000020f0: 6169 6e69 6e67 5d28 6874 7470 733a 2f2f  aining](https://
+00002100: 6c69 6768 746e 696e 672e 6169 2f64 6f63  lightning.ai/doc
+00002110: 732f 6661 6272 6963 2f73 7461 626c 652f  s/fabric/stable/
+00002120: 6675 6e64 616d 656e 7461 6c73 2f6c 6175  fundamentals/lau
+00002130: 6e63 682e 6874 6d6c 292e 0a0a 5f5f 5f5f  nch.html)...____
+00002140: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002150: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002160: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002170: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002180: 5f5f 0a0a 2320 4641 510a 0a23 2320 5768  __..# FAQ..## Wh
+00002190: 656e 2074 6f20 7573 6520 4661 6272 6963  en to use Fabric
+000021a0: 3f0a 0a2d 202a 2a4d 696e 696d 756d 2063  ?..- **Minimum c
+000021b0: 6f64 6520 6368 616e 6765 732a 2a2d 2059  ode changes**- Y
+000021c0: 6f75 2077 616e 7420 746f 2073 6361 6c65  ou want to scale
+000021d0: 2079 6f75 7220 5079 546f 7263 6820 6d6f   your PyTorch mo
+000021e0: 6465 6c20 746f 2075 7365 206d 756c 7469  del to use multi
+000021f0: 2d47 5055 206f 7220 7573 6520 6164 7661  -GPU or use adva
+00002200: 6e63 6564 2073 7472 6174 6567 6965 7320  nced strategies 
+00002210: 6c69 6b65 2044 6565 7053 7065 6564 2077  like DeepSpeed w
+00002220: 6974 686f 7574 2068 6176 696e 6720 746f  ithout having to
+00002230: 2072 6566 6163 746f 722e 2059 6f75 2064   refactor. You d
+00002240: 6f6e e280 9974 2063 6172 6520 6162 6f75  on...t care abou
+00002250: 7420 7374 7275 6374 7572 696e 6720 796f  t structuring yo
+00002260: 7572 2063 6f64 652d 2079 6f75 206a 7573  ur code- you jus
+00002270: 7420 7761 6e74 2074 6f20 7363 616c 6520  t want to scale 
+00002280: 6974 2061 7320 6661 7374 2061 7320 706f  it as fast as po
+00002290: 7373 6962 6c65 2e0a 2d20 2a2a 4d61 786d  ssible..- **Maxm
+000022a0: 6975 6d20 636f 6e74 726f 6c2a 2a2d 2057  ium control**- W
+000022b0: 7269 7465 2079 6f75 7220 6f77 6e20 7472  rite your own tr
+000022c0: 6169 6e69 6e67 2061 6e64 2f6f 7220 696e  aining and/or in
+000022d0: 6665 7265 6e63 6520 6c6f 6769 6320 646f  ference logic do
+000022e0: 776e 2074 6f20 7468 6520 696e 6469 7669  wn to the indivi
+000022f0: 6475 616c 206f 7074 696d 697a 6572 2063  dual optimizer c
+00002300: 616c 6c73 2e20 596f 7520 6172 656e e280  alls. You aren..
+00002310: 9974 2066 6f72 6365 6420 746f 2063 6f6e  .t forced to con
+00002320: 666f 726d 2074 6f20 6120 7374 616e 6461  form to a standa
+00002330: 7264 697a 6564 2065 706f 6368 2d62 6173  rdized epoch-bas
+00002340: 6564 2074 7261 696e 696e 6720 6c6f 6f70  ed training loop
+00002350: 206c 696b 6520 7468 6520 6f6e 6520 696e   like the one in
+00002360: 204c 6967 6874 6e69 6e67 2054 7261 696e   Lightning Train
+00002370: 6572 2e20 596f 7520 6361 6e20 646f 2066  er. You can do f
+00002380: 6c65 7869 626c 6520 6974 6572 6174 696f  lexible iteratio
+00002390: 6e20 6261 7365 6420 7472 6169 6e69 6e67  n based training
+000023a0: 2c20 6d65 7461 2d6c 6561 726e 696e 672c  , meta-learning,
+000023b0: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
+000023c0: 6e20 616e 6420 6f74 6865 7220 7479 7065  n and other type
+000023d0: 7320 6f66 206f 7074 696d 697a 6174 696f  s of optimizatio
+000023e0: 6e20 616c 676f 7269 7468 6d73 2077 6974  n algorithms wit
+000023f0: 686f 7574 2064 6967 6769 6e67 2069 6e74  hout digging int
+00002400: 6f20 6672 616d 6577 6f72 6b20 696e 7465  o framework inte
+00002410: 726e 616c 732e 2054 6869 7320 616c 736f  rnals. This also
+00002420: 206d 616b 6573 2069 7420 7375 7065 7220   makes it super 
+00002430: 6561 7379 2074 6f20 6164 6f70 7420 4661  easy to adopt Fa
+00002440: 6272 6963 2069 6e20 6578 6973 7469 6e67  bric in existing
+00002450: 2050 7954 6f72 6368 2070 726f 6a65 6374   PyTorch project
+00002460: 7320 746f 2073 7065 6564 2d75 7020 616e  s to speed-up an
+00002470: 6420 7363 616c 6520 796f 7572 206d 6f64  d scale your mod
+00002480: 656c 7320 7769 7468 6f75 7420 7468 6520  els without the 
+00002490: 636f 6d70 726f 6d69 7365 206f 6e20 6c61  compromise on la
+000024a0: 7267 6520 7265 6661 6374 6f72 732e 204a  rge refactors. J
+000024b0: 7573 7420 7265 6d65 6d62 6572 3a20 5769  ust remember: Wi
+000024c0: 7468 2067 7265 6174 2070 6f77 6572 2063  th great power c
+000024d0: 6f6d 6573 2061 2067 7265 6174 2072 6573  omes a great res
+000024e0: 706f 6e73 6962 696c 6974 792e 0a2d 202a  ponsibility..- *
+000024f0: 2a4d 6178 6d69 756d 2066 6c65 7869 6269  *Maxmium flexibi
+00002500: 6c69 7479 2a2a 2d20 596f 7520 7761 6e74  lity**- You want
+00002510: 2074 6f20 6861 7665 2066 756c 6c20 636f   to have full co
+00002520: 6e74 726f 6c20 6f76 6572 2079 6f75 7220  ntrol over your 
+00002530: 656e 7469 7265 2074 7261 696e 696e 672d  entire training-
+00002540: 2069 6e20 4661 6272 6963 2061 6c6c 2066   in Fabric all f
+00002550: 6561 7475 7265 7320 6172 6520 6f70 742d  eatures are opt-
+00002560: 696e 2c20 616e 6420 6974 2070 726f 7669  in, and it provi
+00002570: 6465 7320 796f 7520 7769 7468 2061 2074  des you with a t
+00002580: 6f6f 6c20 626f 7820 6f66 2070 7269 6d69  ool box of primi
+00002590: 7469 7665 7320 736f 2079 6f75 2063 616e  tives so you can
+000025a0: 2062 7569 6c64 2079 6f75 7220 6f77 6e20   build your own 
+000025b0: 5472 6169 6e65 722e 0a0a 2323 2057 6865  Trainer...## Whe
+000025c0: 6e20 746f 2075 7365 2074 6865 205b 4c69  n to use the [Li
+000025d0: 6768 746e 696e 6720 5472 6169 6e65 725d  ghtning Trainer]
+000025e0: 2868 7474 7073 3a2f 2f6c 6967 6874 6e69  (https://lightni
+000025f0: 6e67 2e61 692f 646f 6373 2f70 7974 6f72  ng.ai/docs/pytor
+00002600: 6368 2f73 7461 626c 652f 636f 6d6d 6f6e  ch/stable/common
+00002610: 2f74 7261 696e 6572 2e68 746d 6c29 3f0a  /trainer.html)?.
+00002620: 0a2d 2059 6f75 2077 616e 7420 746f 2068  .- You want to h
+00002630: 6176 6520 616c 6c20 7468 6520 656e 6769  ave all the engi
+00002640: 6e65 6572 696e 6720 626f 696c 6572 706c  neering boilerpl
+00002650: 6174 6520 6861 6e64 6c65 6420 666f 7220  ate handled for 
+00002660: 796f 7520 2d20 646f 7a65 6e73 206f 6620  you - dozens of 
+00002670: 6665 6174 7572 6573 206c 696b 6520 6368  features like ch
+00002680: 6563 6b70 6f69 6e74 696e 672c 206c 6f67  eckpointing, log
+00002690: 6769 6e67 2061 6e64 2065 6172 6c79 2073  ging and early s
+000026a0: 746f 7070 696e 6720 6f75 7420 6f66 2074  topping out of t
+000026b0: 6865 2062 6f78 2e20 4c65 7373 2068 6173  he box. Less has
+000026c0: 736c 652c 206c 6573 7320 6572 726f 7220  sle, less error 
+000026d0: 7072 6f6e 652c 2065 6173 7920 746f 2074  prone, easy to t
+000026e0: 7279 2064 6966 6665 7265 6e74 2074 6563  ry different tec
+000026f0: 686e 6971 7565 7320 616e 6420 6665 6174  hniques and feat
+00002700: 7572 6573 2e0a 2d20 596f 7520 7761 6e74  ures..- You want
+00002710: 2074 6f20 6861 7665 2067 6f6f 6420 6465   to have good de
+00002720: 6661 756c 7473 2063 686f 7365 6e20 666f  faults chosen fo
+00002730: 7220 796f 7520 2d20 736f 2079 6f75 2063  r you - so you c
+00002740: 616e 2068 6176 6520 6120 6265 7474 6572  an have a better
+00002750: 2073 7461 7274 696e 6720 706f 696e 742e   starting point.
+00002760: 0a2d 2059 6f75 2077 616e 7420 796f 7572  .- You want your
+00002770: 2063 6f64 6520 746f 2062 6520 6d6f 6475   code to be modu
+00002780: 6c61 722c 2072 6561 6461 626c 6520 616e  lar, readable an
+00002790: 6420 7765 6c6c 2073 7472 7563 7475 7265  d well structure
+000027a0: 6420 2d20 6561 7379 2074 6f20 7368 6172  d - easy to shar
+000027b0: 6520 6265 7477 6565 6e20 7072 6f6a 6563  e between projec
+000027c0: 7473 2061 6e64 2077 6974 6820 636f 6c6c  ts and with coll
+000027d0: 6162 6f72 6174 6f72 732e 0a0a 2323 2043  aborators...## C
+000027e0: 616e 2049 2075 7365 2046 6162 7269 6320  an I use Fabric 
+000027f0: 7769 7468 206d 7920 4c69 6768 746e 696e  with my Lightnin
+00002800: 674d 6f64 756c 6520 6f72 204c 6967 6874  gModule or Light
+00002810: 6e69 6e67 2043 616c 6c62 6163 6b3f 0a0a  ning Callback?..
+00002820: 5965 7320 3a29 2046 6162 7269 6320 776f  Yes :) Fabric wo
+00002830: 726b 7320 7769 7468 2050 7954 6f72 6368  rks with PyTorch
+00002840: 204c 6967 6874 6e69 6e67 4d6f 6475 6c65   LightningModule
+00002850: 7320 616e 6420 4361 6c6c 6261 636b 732c  s and Callbacks,
+00002860: 2073 6f20 796f 7520 6361 6e20 6368 6f6f   so you can choo
+00002870: 7365 2068 6f77 2074 6f20 7374 7275 6374  se how to struct
+00002880: 7572 6520 796f 7572 2063 6f64 6520 616e  ure your code an
+00002890: 6420 7265 7573 6520 6578 6973 7469 6e67  d reuse existing
+000028a0: 206d 6f64 656c 7320 616e 6420 6361 6c6c   models and call
+000028b0: 6261 636b 7320 6173 2079 6f75 2077 6973  backs as you wis
+000028c0: 682e 2052 6561 6420 6d6f 7265 205b 6865  h. Read more [he
+000028d0: 7265 5d28 6874 7470 733a 2f2f 6c69 6768  re](https://ligh
+000028e0: 746e 696e 672e 6169 2f64 6f63 732f 6661  tning.ai/docs/fa
+000028f0: 6272 6963 2f73 7461 626c 652f 6675 6e64  bric/stable/fund
+00002900: 616d 656e 7461 6c73 2f63 6f64 655f 7374  amentals/code_st
+00002910: 7275 6374 7572 652e 6874 6d6c 292e 0a0a  ructure.html)...
+00002920: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00002930: 2f2f 706c 2d70 7562 6c69 632d 6461 7461  //pl-public-data
+00002940: 2e73 332e 616d 617a 6f6e 6177 732e 636f  .s3.amazonaws.co
+00002950: 6d2f 6173 7365 7473 5f6c 6967 6874 6e69  m/assets_lightni
+00002960: 6e67 2f63 6f6e 7469 6e75 756d 2e70 6e67  ng/continuum.png
+00002970: 2220 7769 6474 683d 2238 3030 7078 223e  " width="800px">
+00002980: 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ..______________
+00002990: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000029a0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000029b0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000029c0: 5f5f 5f5f 5f5f 5f5f 0a0a 2320 4578 616d  ________..# Exam
+000029d0: 706c 6573 0a0a 2d20 5b47 414e 5d28 6874  ples..- [GAN](ht
+000029e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000029f0: 2f4c 6967 6874 6e69 6e67 2d41 492f 6c69  /Lightning-AI/li
+00002a00: 6768 746e 696e 672f 7472 6565 2f6d 6173  ghtning/tree/mas
+00002a10: 7465 722f 6578 616d 706c 6573 2f66 6162  ter/examples/fab
+00002a20: 7269 632f 6463 6761 6e29 0a2d 205b 4d65  ric/dcgan).- [Me
+00002a30: 7461 206c 6561 726e 696e 675d 2868 7474  ta learning](htt
+00002a40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002a50: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
+00002a60: 6874 6e69 6e67 2f74 7265 652f 6d61 7374  htning/tree/mast
+00002a70: 6572 2f65 7861 6d70 6c65 732f 6661 6272  er/examples/fabr
+00002a80: 6963 2f6d 6574 615f 6c65 6172 6e69 6e67  ic/meta_learning
+00002a90: 290a 2d20 5b52 6569 6e66 6f72 6365 6d65  ).- [Reinforceme
+00002aa0: 6e74 206c 6561 726e 696e 675d 2868 7474  nt learning](htt
+00002ab0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002ac0: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
+00002ad0: 6874 6e69 6e67 2f74 7265 652f 6d61 7374  htning/tree/mast
+00002ae0: 6572 2f65 7861 6d70 6c65 732f 6661 6272  er/examples/fabr
+00002af0: 6963 2f72 6569 6e66 6f72 6365 6d65 6e74  ic/reinforcement
+00002b00: 5f6c 6561 726e 696e 6729 0a2d 205b 4b2d  _learning).- [K-
+00002b10: 466f 6c64 2063 726f 7373 2076 616c 6964  Fold cross valid
+00002b20: 6174 696f 6e5d 2868 7474 7073 3a2f 2f67  ation](https://g
+00002b30: 6974 6875 622e 636f 6d2f 4c69 6768 746e  ithub.com/Lightn
+00002b40: 696e 672d 4149 2f6c 6967 6874 6e69 6e67  ing-AI/lightning
+00002b50: 2f74 7265 652f 6d61 7374 6572 2f65 7861  /tree/master/exa
+00002b60: 6d70 6c65 732f 6661 6272 6963 2f6b 666f  mples/fabric/kfo
+00002b70: 6c64 5f63 7629 0a0a 5f5f 5f5f 5f5f 5f5f  ld_cv)..________
+00002b80: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002b90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002ba0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002bb0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a  ______________..
+00002bc0: 2323 2041 736b 696e 6720 666f 7220 6865  ## Asking for he
+00002bd0: 6c70 0a0a 4966 2079 6f75 2068 6176 6520  lp..If you have 
+00002be0: 616e 7920 7175 6573 7469 6f6e 7320 706c  any questions pl
+00002bf0: 6561 7365 3a0a 0a31 2e20 5b52 6561 6420  ease:..1. [Read 
+00002c00: 7468 6520 646f 6373 5d28 6874 7470 733a  the docs](https:
+00002c10: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
+00002c20: 6f63 732f 6661 6272 6963 292e 0a31 2e20  ocs/fabric)..1. 
+00002c30: 5b41 736b 2061 2071 7565 7374 696f 6e20  [Ask a question 
+00002c40: 696e 206f 7572 2066 6f72 756d 5d28 6874  in our forum](ht
+00002c50: 7470 733a 2f2f 6c69 6768 746e 696e 672e  tps://lightning.
+00002c60: 6169 2f66 6f72 756d 732f 292e 0a31 2e20  ai/forums/)..1. 
+00002c70: 5b4a 6f69 6e20 6f75 7220 6469 7363 6f72  [Join our discor
+00002c80: 6420 636f 6d6d 756e 6974 795d 2868 7474  d community](htt
+00002c90: 7073 3a2f 2f64 6973 636f 7264 2e63 6f6d  ps://discord.com
+00002ca0: 2f69 6e76 6974 652f 7466 5846 6574 455a  /invite/tfXFetEZ
+00002cb0: 7876 292e 0a0a 0a                        xv)....
```

### Comparing `lightning-fabric-2.0.1.post0/README.md` & `lightning-fabric-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/pyproject.toml` & `lightning-fabric-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 [tool.ruff]
 line-length = 120
 # Enable Pyflakes `E` and `F` codes by default.
 select = [
     "E", "W",  # see: https://pypi.org/project/pycodestyle
     "F",  # see: https://pypi.org/project/pyflakes
 ]
+extend-select = [
+    "C4",  # see: https://pypi.org/project/flake8-comprehensions
+]
 ignore = [
     "E731",  # Do not assign a lambda expression, use a def
 ]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".git",
     "docs",
```

### Comparing `lightning-fabric-2.0.1.post0/setup.py` & `lightning-fabric-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/CHANGELOG.md` & `lightning-fabric-2.0.2/src/lightning_fabric/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.2] - 2023-04-24
+
+### Changed
+
+- Enable precision autocast for LightningModule step methods in Fabric ([#17439](https://github.com/Lightning-AI/lightning/pull/17439))
+
+### Fixed
+
+- Fixed an issue with `LightningModule.*_step` methods bypassing the DDP/FSDP wrapper ([#17424](https://github.com/Lightning-AI/lightning/pull/17424))
+- Fixed device handling in `Fabric.setup()` when the model has no parameters ([#17441](https://github.com/Lightning-AI/lightning/pull/17441))
+
+
 ## [2.0.1] - 2023-03-30
 
 ### Changed
 
 - Generalized `Optimizer` validation to accommodate both FSDP 1.x and 2.x ([#16733](https://github.com/Lightning-AI/lightning/pull/16733))
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/README.md` & `lightning-fabric-2.0.2/src/lightning_fabric/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -62,375 +62,573 @@
 000003d0: 6461 2d66 6f72 6765 2f6c 6967 6874 6e69  da-forge/lightni
 000003e0: 6e67 5f66 6162 7269 633f 6c61 6265 6c3d  ng_fabric?label=
 000003f0: 636f 6e64 6126 636f 6c6f 723d 7375 6363  conda&color=succ
 00000400: 6573 7329 5d28 6874 7470 733a 2f2f 616e  ess)](https://an
 00000410: 6163 6f6e 6461 2e6f 7267 2f63 6f6e 6461  aconda.org/conda
 00000420: 2d66 6f72 6765 2f6c 6967 6874 6e69 6e67  -forge/lightning
 00000430: 5f66 6162 7269 6329 0a0a 3c2f 6469 763e  _fabric)..</div>
-00000440: 0a0a 2323 204d 6178 696d 756d 2066 6c65  ..## Maximum fle
-00000450: 7869 6269 6c69 7479 2c20 6d69 6e69 6d75  xibility, minimu
-00000460: 6d20 636f 6465 2063 6861 6e67 6573 0a0a  m code changes..
-00000470: 5769 7468 206a 7573 7420 6120 6665 7720  With just a few 
-00000480: 636f 6465 2063 6861 6e67 6573 2c20 7275  code changes, ru
-00000490: 6e20 616e 7920 5079 546f 7263 6820 6d6f  n any PyTorch mo
-000004a0: 6465 6c20 6f6e 2061 6e79 2064 6973 7472  del on any distr
-000004b0: 6962 7574 6564 2068 6172 6477 6172 652c  ibuted hardware,
-000004c0: 206e 6f20 626f 696c 6572 706c 6174 6521   no boilerplate!
-000004d0: 0a0a 2d20 4561 7369 6c79 2073 7769 7463  ..- Easily switc
-000004e0: 6820 6672 6f6d 2072 756e 6e69 6e67 206f  h from running o
-000004f0: 6e20 4350 5520 746f 2047 5055 2028 4170  n CPU to GPU (Ap
-00000500: 706c 6520 5369 6c69 636f 6e2c 2043 5544  ple Silicon, CUD
-00000510: 412c 20e2 80a6 292c 2054 5055 2c20 6d75  A, ...), TPU, mu
-00000520: 6c74 692d 4750 5520 6f72 2065 7665 6e20  lti-GPU or even 
-00000530: 6d75 6c74 692d 6e6f 6465 2074 7261 696e  multi-node train
-00000540: 696e 670a 2d20 5573 6520 7374 6174 652d  ing.- Use state-
-00000550: 6f66 2d74 6865 2d61 7274 2064 6973 7472  of-the-art distr
-00000560: 6962 7574 6564 2074 7261 696e 696e 6720  ibuted training 
-00000570: 7374 7261 7465 6769 6573 2028 4444 502c  strategies (DDP,
-00000580: 2046 5344 502c 2044 6565 7053 7065 6564   FSDP, DeepSpeed
-00000590: 2920 616e 6420 6d69 7865 6420 7072 6563  ) and mixed prec
-000005a0: 6973 696f 6e20 6f75 7420 6f66 2074 6865  ision out of the
-000005b0: 2062 6f78 0a2d 2041 6c6c 2074 6865 2064   box.- All the d
-000005c0: 6576 6963 6520 6c6f 6769 6320 626f 696c  evice logic boil
-000005d0: 6572 706c 6174 6520 6973 2068 616e 646c  erplate is handl
-000005e0: 6564 2066 6f72 2079 6f75 0a2d 2044 6573  ed for you.- Des
-000005f0: 6967 6e65 6420 7769 7468 206d 756c 7469  igned with multi
-00000600: 2d62 696c 6c69 6f6e 2070 6172 616d 6574  -billion paramet
-00000610: 6572 206d 6f64 656c 7320 696e 206d 696e  er models in min
-00000620: 640a 2d20 4275 696c 6420 796f 7572 206f  d.- Build your o
-00000630: 776e 2063 7573 746f 6d20 5472 6169 6e65  wn custom Traine
-00000640: 7220 7573 696e 6720 4661 6272 6963 2070  r using Fabric p
-00000650: 7269 6d69 7469 7665 7320 666f 7220 7472  rimitives for tr
-00000660: 6169 6e69 6e67 2063 6865 636b 706f 696e  aining checkpoin
-00000670: 7469 6e67 2c20 6c6f 6767 696e 672c 2061  ting, logging, a
-00000680: 6e64 206d 6f72 650a 0a60 6060 6469 6666  nd more..```diff
-00000690: 0a2b 2069 6d70 6f72 7420 6c69 6768 746e  .+ import lightn
-000006a0: 696e 6720 6173 204c 0a0a 2020 696d 706f  ing as L..  impo
-000006b0: 7274 2074 6f72 6368 0a20 2069 6d70 6f72  rt torch.  impor
-000006c0: 7420 746f 7263 682e 6e6e 2061 7320 6e6e  t torch.nn as nn
-000006d0: 0a20 2066 726f 6d20 746f 7263 682e 7574  .  from torch.ut
-000006e0: 696c 732e 6461 7461 2069 6d70 6f72 7420  ils.data import 
-000006f0: 4461 7461 4c6f 6164 6572 2c20 4461 7461  DataLoader, Data
-00000700: 7365 740a 0a20 2063 6c61 7373 2050 7954  set..  class PyT
-00000710: 6f72 6368 4d6f 6465 6c28 6e6e 2e4d 6f64  orchModel(nn.Mod
-00000720: 756c 6529 3a0a 2020 2020 2020 2e2e 2e0a  ule):.      ....
-00000730: 0a20 2063 6c61 7373 2050 7954 6f72 6368  .  class PyTorch
-00000740: 4461 7461 7365 7428 4461 7461 7365 7429  Dataset(Dataset)
-00000750: 3a0a 2020 2020 2020 2e2e 2e0a 0a2b 2066  :.      .....+ f
-00000760: 6162 7269 6320 3d20 4c2e 4661 6272 6963  abric = L.Fabric
-00000770: 2861 6363 656c 6572 6174 6f72 3d22 6375  (accelerator="cu
-00000780: 6461 222c 2064 6576 6963 6573 3d38 2c20  da", devices=8, 
-00000790: 7374 7261 7465 6779 3d22 6464 7022 290a  strategy="ddp").
-000007a0: 2b20 6661 6272 6963 2e6c 6175 6e63 6828  + fabric.launch(
-000007b0: 290a 0a2d 2064 6576 6963 6520 3d20 2263  )..- device = "c
-000007c0: 7564 6122 2069 6620 746f 7263 682e 6375  uda" if torch.cu
-000007d0: 6461 2e69 735f 6176 6169 6c61 626c 6528  da.is_available(
-000007e0: 2920 656c 7365 2022 6370 750a 2020 6d6f  ) else "cpu.  mo
-000007f0: 6465 6c20 3d20 5079 546f 7263 684d 6f64  del = PyTorchMod
-00000800: 656c 282e 2e2e 290a 2020 6f70 7469 6d69  el(...).  optimi
-00000810: 7a65 7220 3d20 746f 7263 682e 6f70 7469  zer = torch.opti
-00000820: 6d2e 5347 4428 6d6f 6465 6c2e 7061 7261  m.SGD(model.para
-00000830: 6d65 7465 7273 2829 290a 2b20 6d6f 6465  meters()).+ mode
-00000840: 6c2c 206f 7074 696d 697a 6572 203d 2066  l, optimizer = f
-00000850: 6162 7269 632e 7365 7475 7028 6d6f 6465  abric.setup(mode
-00000860: 6c2c 206f 7074 696d 697a 6572 290a 2020  l, optimizer).  
-00000870: 6461 7461 6c6f 6164 6572 203d 2044 6174  dataloader = Dat
-00000880: 614c 6f61 6465 7228 5079 546f 7263 6844  aLoader(PyTorchD
-00000890: 6174 6173 6574 282e 2e2e 292c 202e 2e2e  ataset(...), ...
-000008a0: 290a 2b20 6461 7461 6c6f 6164 6572 203d  ).+ dataloader =
-000008b0: 2066 6162 7269 632e 7365 7475 705f 6461   fabric.setup_da
-000008c0: 7461 6c6f 6164 6572 7328 6461 7461 6c6f  taloaders(datalo
-000008d0: 6164 6572 290a 2020 6d6f 6465 6c2e 7472  ader).  model.tr
-000008e0: 6169 6e28 290a 0a20 2066 6f72 2065 706f  ain()..  for epo
-000008f0: 6368 2069 6e20 7261 6e67 6528 6e75 6d5f  ch in range(num_
-00000900: 6570 6f63 6873 293a 0a20 2020 2020 2066  epochs):.      f
-00000910: 6f72 2062 6174 6368 2069 6e20 6461 7461  or batch in data
-00000920: 6c6f 6164 6572 3a0a 2020 2020 2020 2020  loader:.        
-00000930: 2020 696e 7075 742c 2074 6172 6765 7420    input, target 
-00000940: 3d20 6261 7463 680a 2d20 2020 2020 2020  = batch.-       
-00000950: 2020 696e 7075 742c 2074 6172 6765 7420    input, target 
-00000960: 3d20 696e 7075 742e 746f 2864 6576 6963  = input.to(devic
-00000970: 6529 2c20 7461 7267 6574 2e74 6f28 6465  e), target.to(de
-00000980: 7669 6365 290a 2020 2020 2020 2020 2020  vice).          
-00000990: 6f70 7469 6d69 7a65 722e 7a65 726f 5f67  optimizer.zero_g
-000009a0: 7261 6428 290a 2020 2020 2020 2020 2020  rad().          
-000009b0: 6f75 7470 7574 203d 206d 6f64 656c 2869  output = model(i
-000009c0: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
-000009d0: 6c6f 7373 203d 206c 6f73 735f 666e 286f  loss = loss_fn(o
-000009e0: 7574 7075 742c 2074 6172 6765 7429 0a2d  utput, target).-
-000009f0: 2020 2020 2020 2020 206c 6f73 732e 6261           loss.ba
-00000a00: 636b 7761 7264 2829 0a2b 2020 2020 2020  ckward().+      
-00000a10: 2020 2066 6162 7269 632e 6261 636b 7761     fabric.backwa
-00000a20: 7264 286c 6f73 7329 0a20 2020 2020 2020  rd(loss).       
-00000a30: 2020 206f 7074 696d 697a 6572 2e73 7465     optimizer.ste
-00000a40: 7028 290a 2020 2020 2020 2020 2020 6c72  p().          lr
-00000a50: 5f73 6368 6564 756c 6572 2e73 7465 7028  _scheduler.step(
-00000a60: 290a 6060 600a 0a5f 5f5f 5f5f 5f5f 5f5f  ).```.._________
-00000a70: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000a80: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000a90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000aa0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f0a 0a23  _____________..#
-00000ab0: 2047 6574 7469 6e67 2073 7461 7274 6564   Getting started
-00000ac0: 0a0a 2323 2049 6e73 7461 6c6c 204c 6967  ..## Install Lig
-00000ad0: 6874 6e69 6e67 0a0a 3c64 6574 6169 6c73  htning..<details
-00000ae0: 3e0a 0a3c 7375 6d6d 6172 793e 5072 6572  >..<summary>Prer
-00000af0: 6571 7569 7369 7465 733c 2f73 756d 6d61  equisites</summa
-00000b00: 7279 3e0a 0a3e 2054 4950 3a20 5765 2073  ry>..> TIP: We s
-00000b10: 7472 6f6e 676c 7920 7265 636f 6d6d 656e  trongly recommen
-00000b20: 6420 6372 6561 7469 6e67 2061 2076 6972  d creating a vir
-00000b30: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00000b40: 2066 6972 7374 2e0a 3e20 446f 6ee2 8099   first..> Don...
-00000b50: 7420 6b6e 6f77 2077 6861 7420 7468 6973  t know what this
-00000b60: 2069 733f 2046 6f6c 6c6f 7720 6f75 7220   is? Follow our 
-00000b70: 5b62 6567 696e 6e65 7220 6775 6964 6520  [beginner guide 
-00000b80: 6865 7265 5d28 6874 7470 733a 2f2f 6c69  here](https://li
-00000b90: 6768 746e 696e 672e 6169 2f64 6f63 732f  ghtning.ai/docs/
-00000ba0: 7374 6162 6c65 2f69 6e73 7461 6c6c 2f69  stable/install/i
-00000bb0: 6e73 7461 6c6c 6174 696f 6e2e 6874 6d6c  nstallation.html
-00000bc0: 292e 0a0a 2d20 5079 7468 6f6e 2033 2e38  )...- Python 3.8
-00000bd0: 2e78 206f 7220 6c61 7465 7220 2833 2e38  .x or later (3.8
-00000be0: 2e78 2c20 332e 392e 782c 2033 2e31 302e  .x, 3.9.x, 3.10.
-00000bf0: 782c 202e 2e2e 290a 0a3c 2f64 6574 6169  x, ...)..</detai
-00000c00: 6c73 3e0a 0a60 6060 6261 7368 0a70 6970  ls>..```bash.pip
-00000c10: 2069 6e73 7461 6c6c 202d 5520 6c69 6768   install -U ligh
-00000c20: 746e 696e 670a 6060 600a 0a23 2320 436f  tning.```..## Co
-00000c30: 6e76 6572 7420 796f 7572 2050 7954 6f72  nvert your PyTor
-00000c40: 6368 2074 6f20 4661 6272 6963 0a0a 312e  ch to Fabric..1.
-00000c50: 2043 7265 6174 6520 7468 6520 6046 6162   Create the `Fab
-00000c60: 7269 6360 206f 626a 6563 7420 6174 2074  ric` object at t
-00000c70: 6865 2062 6567 696e 6e69 6e67 206f 6620  he beginning of 
-00000c80: 796f 7572 2074 7261 696e 696e 6720 636f  your training co
-00000c90: 6465 2e0a 0a20 2020 6060 600a 2020 2069  de...   ```.   i
-00000ca0: 6d70 6f72 7420 4c69 6768 746e 696e 6720  mport Lightning 
-00000cb0: 6173 204c 0a0a 2020 2066 6162 7269 6320  as L..   fabric 
-00000cc0: 3d20 4c2e 4661 6272 6963 2829 0a20 2020  = L.Fabric().   
-00000cd0: 6060 600a 0a31 2e20 4361 6c6c 2060 7365  ```..1. Call `se
-00000ce0: 7475 7028 2960 206f 6e20 6561 6368 206d  tup()` on each m
-00000cf0: 6f64 656c 2061 6e64 206f 7074 696d 697a  odel and optimiz
-00000d00: 6572 2070 6169 7220 616e 6420 6073 6574  er pair and `set
-00000d10: 7570 5f64 6174 616c 6f61 6465 7273 2829  up_dataloaders()
-00000d20: 6020 6f6e 2061 6c6c 2079 6f75 7220 6461  ` on all your da
-00000d30: 7461 206c 6f61 6465 7273 2e0a 0a20 2020  ta loaders...   
-00000d40: 6060 600a 2020 206d 6f64 656c 2c20 6f70  ```.   model, op
-00000d50: 7469 6d69 7a65 7220 3d20 6661 6272 6963  timizer = fabric
-00000d60: 2e73 6574 7570 286d 6f64 656c 2c20 6f70  .setup(model, op
-00000d70: 7469 6d69 7a65 7229 0a20 2020 6461 7461  timizer).   data
-00000d80: 6c6f 6164 6572 203d 2066 6162 7269 632e  loader = fabric.
-00000d90: 7365 7475 705f 6461 7461 6c6f 6164 6572  setup_dataloader
-00000da0: 7328 6461 7461 6c6f 6164 6572 290a 2020  s(dataloader).  
-00000db0: 2060 6060 0a0a 312e 2052 656d 6f76 6520   ```..1. Remove 
-00000dc0: 616c 6c20 602e 746f 6020 616e 6420 602e  all `.to` and `.
-00000dd0: 6375 6461 6020 6361 6c6c 7320 2d3e 2046  cuda` calls -> F
-00000de0: 6162 7269 6320 7769 6c6c 2074 616b 6520  abric will take 
-00000df0: 6361 7265 206f 6620 6974 2e0a 0a20 2020  care of it...   
-00000e00: 6060 6064 6966 660a 2020 202d 206d 6f64  ```diff.   - mod
-00000e10: 656c 2e74 6f28 6465 7669 6365 290a 2020  el.to(device).  
-00000e20: 202d 2062 6174 6368 2e74 6f28 6465 7669   - batch.to(devi
-00000e30: 6365 290a 2020 2060 6060 0a0a 312e 2052  ce).   ```..1. R
-00000e40: 6570 6c61 6365 2060 6c6f 7373 2e62 6163  eplace `loss.bac
-00000e50: 6b77 6172 6428 2960 2062 7920 6066 6162  kward()` by `fab
-00000e60: 7269 632e 6261 636b 7761 7264 286c 6f73  ric.backward(los
-00000e70: 7329 602e 0a0a 2020 2060 6060 6469 6666  s)`...   ```diff
-00000e80: 0a20 2020 2d20 6c6f 7373 2e62 6163 6b77  .   - loss.backw
-00000e90: 6172 6428 290a 2020 202b 2066 6162 7269  ard().   + fabri
-00000ea0: 632e 6261 636b 7761 7264 286c 6f73 7329  c.backward(loss)
-00000eb0: 0a20 2020 6060 600a 0a31 2e20 5275 6e20  .   ```..1. Run 
-00000ec0: 7468 6520 7363 7269 7074 2066 726f 6d20  the script from 
-00000ed0: 7468 6520 7465 726d 696e 616c 2077 6974  the terminal wit
-00000ee0: 680a 0a20 2020 6060 6062 6173 680a 2020  h..   ```bash.  
-00000ef0: 206c 6967 6874 6e69 6e67 2072 756e 206d   lightning run m
-00000f00: 6f64 656c 2070 6174 682f 746f 2f74 7261  odel path/to/tra
-00000f10: 696e 2e70 790a 2020 2060 6060 0a0a 6f72  in.py.   ```..or
-00000f20: 2075 7365 2074 6865 206c 6175 6e63 6828   use the launch(
-00000f30: 2920 6d65 7468 6f64 2069 6e20 6120 6e6f  ) method in a no
-00000f40: 7465 626f 6f6b 2e20 4c65 6172 6e20 6d6f  tebook. Learn mo
-00000f50: 7265 2061 626f 7574 205b 6c61 756e 6368  re about [launch
-00000f60: 696e 6720 6469 7374 7269 6275 7465 6420  ing distributed 
-00000f70: 7472 6169 6e69 6e67 5d28 6874 7470 733a  training](https:
-00000f80: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
-00000f90: 6f63 732f 6661 6272 6963 2f73 7461 626c  ocs/fabric/stabl
-00000fa0: 652f 6675 6e64 616d 656e 7461 6c73 2f6c  e/fundamentals/l
-00000fb0: 6175 6e63 682e 6874 6d6c 292e 0a0a 5f5f  aunch.html)...__
-00000fc0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fd0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fe0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000ff0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001000: 5f5f 5f5f 0a0a 2320 4641 510a 0a23 2320  ____..# FAQ..## 
-00001010: 5768 656e 2074 6f20 7573 6520 4661 6272  When to use Fabr
-00001020: 6963 3f0a 0a2d 202a 2a4d 696e 696d 756d  ic?..- **Minimum
-00001030: 2063 6f64 6520 6368 616e 6765 732a 2a2d   code changes**-
-00001040: 2059 6f75 2077 616e 7420 746f 2073 6361   You want to sca
-00001050: 6c65 2079 6f75 7220 5079 546f 7263 6820  le your PyTorch 
-00001060: 6d6f 6465 6c20 746f 2075 7365 206d 756c  model to use mul
-00001070: 7469 2d47 5055 206f 7220 7573 6520 6164  ti-GPU or use ad
-00001080: 7661 6e63 6564 2073 7472 6174 6567 6965  vanced strategie
-00001090: 7320 6c69 6b65 2044 6565 7053 7065 6564  s like DeepSpeed
-000010a0: 2077 6974 686f 7574 2068 6176 696e 6720   without having 
-000010b0: 746f 2072 6566 6163 746f 722e 2059 6f75  to refactor. You
-000010c0: 2064 6f6e e280 9974 2063 6172 6520 6162   don...t care ab
-000010d0: 6f75 7420 7374 7275 6374 7572 696e 6720  out structuring 
-000010e0: 796f 7572 2063 6f64 652d 2079 6f75 206a  your code- you j
-000010f0: 7573 7420 7761 6e74 2074 6f20 7363 616c  ust want to scal
-00001100: 6520 6974 2061 7320 6661 7374 2061 7320  e it as fast as 
-00001110: 706f 7373 6962 6c65 2e0a 2d20 2a2a 4d61  possible..- **Ma
-00001120: 786d 6975 6d20 636f 6e74 726f 6c2a 2a2d  xmium control**-
-00001130: 2057 7269 7465 2079 6f75 7220 6f77 6e20   Write your own 
-00001140: 7472 6169 6e69 6e67 2061 6e64 2f6f 7220  training and/or 
-00001150: 696e 6665 7265 6e63 6520 6c6f 6769 6320  inference logic 
-00001160: 646f 776e 2074 6f20 7468 6520 696e 6469  down to the indi
-00001170: 7669 6475 616c 206f 7074 696d 697a 6572  vidual optimizer
-00001180: 2063 616c 6c73 2e20 596f 7520 6172 656e   calls. You aren
-00001190: e280 9974 2066 6f72 6365 6420 746f 2063  ...t forced to c
-000011a0: 6f6e 666f 726d 2074 6f20 6120 7374 616e  onform to a stan
-000011b0: 6461 7264 697a 6564 2065 706f 6368 2d62  dardized epoch-b
-000011c0: 6173 6564 2074 7261 696e 696e 6720 6c6f  ased training lo
-000011d0: 6f70 206c 696b 6520 7468 6520 6f6e 6520  op like the one 
-000011e0: 696e 204c 6967 6874 6e69 6e67 2054 7261  in Lightning Tra
-000011f0: 696e 6572 2e20 596f 7520 6361 6e20 646f  iner. You can do
-00001200: 2066 6c65 7869 626c 6520 6974 6572 6174   flexible iterat
-00001210: 696f 6e20 6261 7365 6420 7472 6169 6e69  ion based traini
-00001220: 6e67 2c20 6d65 7461 2d6c 6561 726e 696e  ng, meta-learnin
-00001230: 672c 2063 726f 7373 2d76 616c 6964 6174  g, cross-validat
-00001240: 696f 6e20 616e 6420 6f74 6865 7220 7479  ion and other ty
-00001250: 7065 7320 6f66 206f 7074 696d 697a 6174  pes of optimizat
-00001260: 696f 6e20 616c 676f 7269 7468 6d73 2077  ion algorithms w
-00001270: 6974 686f 7574 2064 6967 6769 6e67 2069  ithout digging i
-00001280: 6e74 6f20 6672 616d 6577 6f72 6b20 696e  nto framework in
-00001290: 7465 726e 616c 732e 2054 6869 7320 616c  ternals. This al
-000012a0: 736f 206d 616b 6573 2069 7420 7375 7065  so makes it supe
-000012b0: 7220 6561 7379 2074 6f20 6164 6f70 7420  r easy to adopt 
-000012c0: 4661 6272 6963 2069 6e20 6578 6973 7469  Fabric in existi
-000012d0: 6e67 2050 7954 6f72 6368 2070 726f 6a65  ng PyTorch proje
-000012e0: 6374 7320 746f 2073 7065 6564 2d75 7020  cts to speed-up 
-000012f0: 616e 6420 7363 616c 6520 796f 7572 206d  and scale your m
-00001300: 6f64 656c 7320 7769 7468 6f75 7420 7468  odels without th
-00001310: 6520 636f 6d70 726f 6d69 7365 206f 6e20  e compromise on 
-00001320: 6c61 7267 6520 7265 6661 6374 6f72 732e  large refactors.
-00001330: 204a 7573 7420 7265 6d65 6d62 6572 3a20   Just remember: 
-00001340: 5769 7468 2067 7265 6174 2070 6f77 6572  With great power
-00001350: 2063 6f6d 6573 2061 2067 7265 6174 2072   comes a great r
-00001360: 6573 706f 6e73 6962 696c 6974 792e 0a2d  esponsibility..-
-00001370: 202a 2a4d 6178 6d69 756d 2066 6c65 7869   **Maxmium flexi
-00001380: 6269 6c69 7479 2a2a 2d20 596f 7520 7761  bility**- You wa
-00001390: 6e74 2074 6f20 6861 7665 2066 756c 6c20  nt to have full 
-000013a0: 636f 6e74 726f 6c20 6f76 6572 2079 6f75  control over you
-000013b0: 7220 656e 7469 7265 2074 7261 696e 696e  r entire trainin
-000013c0: 672d 2069 6e20 4661 6272 6963 2061 6c6c  g- in Fabric all
-000013d0: 2066 6561 7475 7265 7320 6172 6520 6f70   features are op
-000013e0: 742d 696e 2c20 616e 6420 6974 2070 726f  t-in, and it pro
-000013f0: 7669 6465 7320 796f 7520 7769 7468 2061  vides you with a
-00001400: 2074 6f6f 6c20 626f 7820 6f66 2070 7269   tool box of pri
-00001410: 6d69 7469 7665 7320 736f 2079 6f75 2063  mitives so you c
-00001420: 616e 2062 7569 6c64 2079 6f75 7220 6f77  an build your ow
-00001430: 6e20 5472 6169 6e65 722e 0a0a 2323 2057  n Trainer...## W
-00001440: 6865 6e20 746f 2075 7365 2074 6865 205b  hen to use the [
-00001450: 4c69 6768 746e 696e 6720 5472 6169 6e65  Lightning Traine
-00001460: 725d 2868 7474 7073 3a2f 2f6c 6967 6874  r](https://light
-00001470: 6e69 6e67 2e61 692f 646f 6373 2f70 7974  ning.ai/docs/pyt
-00001480: 6f72 6368 2f73 7461 626c 652f 636f 6d6d  orch/stable/comm
-00001490: 6f6e 2f74 7261 696e 6572 2e68 746d 6c29  on/trainer.html)
-000014a0: 3f0a 0a2d 2059 6f75 2077 616e 7420 746f  ?..- You want to
-000014b0: 2068 6176 6520 616c 6c20 7468 6520 656e   have all the en
-000014c0: 6769 6e65 6572 696e 6720 626f 696c 6572  gineering boiler
-000014d0: 706c 6174 6520 6861 6e64 6c65 6420 666f  plate handled fo
-000014e0: 7220 796f 7520 2d20 646f 7a65 6e73 206f  r you - dozens o
-000014f0: 6620 6665 6174 7572 6573 206c 696b 6520  f features like 
-00001500: 6368 6563 6b70 6f69 6e74 696e 672c 206c  checkpointing, l
-00001510: 6f67 6769 6e67 2061 6e64 2065 6172 6c79  ogging and early
-00001520: 2073 746f 7070 696e 6720 6f75 7420 6f66   stopping out of
-00001530: 2074 6865 2062 6f78 2e20 4c65 7373 2068   the box. Less h
-00001540: 6173 736c 652c 206c 6573 7320 6572 726f  assle, less erro
-00001550: 7220 7072 6f6e 652c 2065 6173 7920 746f  r prone, easy to
-00001560: 2074 7279 2064 6966 6665 7265 6e74 2074   try different t
-00001570: 6563 686e 6971 7565 7320 616e 6420 6665  echniques and fe
-00001580: 6174 7572 6573 2e0a 2d20 596f 7520 7761  atures..- You wa
-00001590: 6e74 2074 6f20 6861 7665 2067 6f6f 6420  nt to have good 
-000015a0: 6465 6661 756c 7473 2063 686f 7365 6e20  defaults chosen 
-000015b0: 666f 7220 796f 7520 2d20 736f 2079 6f75  for you - so you
-000015c0: 2063 616e 2068 6176 6520 6120 6265 7474   can have a bett
-000015d0: 6572 2073 7461 7274 696e 6720 706f 696e  er starting poin
-000015e0: 742e 0a2d 2059 6f75 2077 616e 7420 796f  t..- You want yo
-000015f0: 7572 2063 6f64 6520 746f 2062 6520 6d6f  ur code to be mo
-00001600: 6475 6c61 722c 2072 6561 6461 626c 6520  dular, readable 
-00001610: 616e 6420 7765 6c6c 2073 7472 7563 7475  and well structu
-00001620: 7265 6420 2d20 6561 7379 2074 6f20 7368  red - easy to sh
-00001630: 6172 6520 6265 7477 6565 6e20 7072 6f6a  are between proj
-00001640: 6563 7473 2061 6e64 2077 6974 6820 636f  ects and with co
-00001650: 6c6c 6162 6f72 6174 6f72 732e 0a0a 2323  llaborators...##
-00001660: 2043 616e 2049 2075 7365 2046 6162 7269   Can I use Fabri
-00001670: 6320 7769 7468 206d 7920 4c69 6768 746e  c with my Lightn
-00001680: 696e 674d 6f64 756c 6520 6f72 204c 6967  ingModule or Lig
-00001690: 6874 6e69 6e67 2043 616c 6c62 6163 6b3f  htning Callback?
-000016a0: 0a0a 5965 7320 3a29 2046 6162 7269 6320  ..Yes :) Fabric 
-000016b0: 776f 726b 7320 7769 7468 2050 7954 6f72  works with PyTor
-000016c0: 6368 204c 6967 6874 6e69 6e67 4d6f 6475  ch LightningModu
-000016d0: 6c65 7320 616e 6420 4361 6c6c 6261 636b  les and Callback
-000016e0: 732c 2073 6f20 796f 7520 6361 6e20 6368  s, so you can ch
-000016f0: 6f6f 7365 2068 6f77 2074 6f20 7374 7275  oose how to stru
-00001700: 6374 7572 6520 796f 7572 2063 6f64 6520  cture your code 
-00001710: 616e 6420 7265 7573 6520 6578 6973 7469  and reuse existi
-00001720: 6e67 206d 6f64 656c 7320 616e 6420 6361  ng models and ca
-00001730: 6c6c 6261 636b 7320 6173 2079 6f75 2077  llbacks as you w
-00001740: 6973 682e 2052 6561 6420 6d6f 7265 205b  ish. Read more [
-00001750: 6865 7265 5d28 6874 7470 733a 2f2f 6c69  here](https://li
-00001760: 6768 746e 696e 672e 6169 2f64 6f63 732f  ghtning.ai/docs/
-00001770: 6661 6272 6963 2f73 7461 626c 652f 6675  fabric/stable/fu
-00001780: 6e64 616d 656e 7461 6c73 2f63 6f64 655f  ndamentals/code_
-00001790: 7374 7275 6374 7572 652e 6874 6d6c 292e  structure.html).
-000017a0: 0a0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
-000017b0: 733a 2f2f 706c 2d70 7562 6c69 632d 6461  s://pl-public-da
-000017c0: 7461 2e73 332e 616d 617a 6f6e 6177 732e  ta.s3.amazonaws.
-000017d0: 636f 6d2f 6173 7365 7473 5f6c 6967 6874  com/assets_light
-000017e0: 6e69 6e67 2f63 6f6e 7469 6e75 756d 2e70  ning/continuum.p
-000017f0: 6e67 2220 7769 6474 683d 2238 3030 7078  ng" width="800px
-00001800: 223e 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ">..____________
-00001810: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001820: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001830: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001840: 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a 2320 4578  __________..# Ex
-00001850: 616d 706c 6573 0a0a 2d20 5b47 414e 5d28  amples..- [GAN](
-00001860: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001870: 6f6d 2f4c 6967 6874 6e69 6e67 2d41 492f  om/Lightning-AI/
-00001880: 6c69 6768 746e 696e 672f 7472 6565 2f6d  lightning/tree/m
-00001890: 6173 7465 722f 6578 616d 706c 6573 2f66  aster/examples/f
-000018a0: 6162 7269 632f 6463 6761 6e29 0a2d 205b  abric/dcgan).- [
-000018b0: 4d65 7461 206c 6561 726e 696e 675d 2868  Meta learning](h
-000018c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000018d0: 6d2f 4c69 6768 746e 696e 672d 4149 2f6c  m/Lightning-AI/l
-000018e0: 6967 6874 6e69 6e67 2f74 7265 652f 6d61  ightning/tree/ma
-000018f0: 7374 6572 2f65 7861 6d70 6c65 732f 6661  ster/examples/fa
-00001900: 6272 6963 2f6d 6574 615f 6c65 6172 6e69  bric/meta_learni
-00001910: 6e67 290a 2d20 5b52 6569 6e66 6f72 6365  ng).- [Reinforce
-00001920: 6d65 6e74 206c 6561 726e 696e 675d 2868  ment learning](h
-00001930: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001940: 6d2f 4c69 6768 746e 696e 672d 4149 2f6c  m/Lightning-AI/l
-00001950: 6967 6874 6e69 6e67 2f74 7265 652f 6d61  ightning/tree/ma
-00001960: 7374 6572 2f65 7861 6d70 6c65 732f 6661  ster/examples/fa
-00001970: 6272 6963 2f72 6569 6e66 6f72 6365 6d65  bric/reinforceme
-00001980: 6e74 5f6c 6561 726e 696e 6729 0a2d 205b  nt_learning).- [
-00001990: 4b2d 466f 6c64 2063 726f 7373 2076 616c  K-Fold cross val
-000019a0: 6964 6174 696f 6e5d 2868 7474 7073 3a2f  idation](https:/
-000019b0: 2f67 6974 6875 622e 636f 6d2f 4c69 6768  /github.com/Ligh
-000019c0: 746e 696e 672d 4149 2f6c 6967 6874 6e69  tning-AI/lightni
-000019d0: 6e67 2f74 7265 652f 6d61 7374 6572 2f65  ng/tree/master/e
-000019e0: 7861 6d70 6c65 732f 6661 6272 6963 2f6b  xamples/fabric/k
-000019f0: 666f 6c64 5f63 7629 0a0a 5f5f 5f5f 5f5f  fold_cv)..______
-00001a00: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a10: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a20: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001a40: 0a0a 2323 2041 736b 696e 6720 666f 7220  ..## Asking for 
-00001a50: 6865 6c70 0a0a 4966 2079 6f75 2068 6176  help..If you hav
-00001a60: 6520 616e 7920 7175 6573 7469 6f6e 7320  e any questions 
-00001a70: 706c 6561 7365 3a0a 0a31 2e20 5b52 6561  please:..1. [Rea
-00001a80: 6420 7468 6520 646f 6373 5d28 6874 7470  d the docs](http
-00001a90: 733a 2f2f 6c69 6768 746e 696e 672e 6169  s://lightning.ai
-00001aa0: 2f64 6f63 732f 6661 6272 6963 292e 0a31  /docs/fabric)..1
-00001ab0: 2e20 5b41 736b 2061 2071 7565 7374 696f  . [Ask a questio
-00001ac0: 6e20 696e 206f 7572 2066 6f72 756d 5d28  n in our forum](
-00001ad0: 6874 7470 733a 2f2f 6c69 6768 746e 696e  https://lightnin
-00001ae0: 672e 6169 2f66 6f72 756d 732f 292e 0a31  g.ai/forums/)..1
-00001af0: 2e20 5b4a 6f69 6e20 6f75 7220 6469 7363  . [Join our disc
-00001b00: 6f72 6420 636f 6d6d 756e 6974 795d 2868  ord community](h
-00001b10: 7474 7073 3a2f 2f64 6973 636f 7264 2e63  ttps://discord.c
-00001b20: 6f6d 2f69 6e76 6974 652f 7466 5846 6574  om/invite/tfXFet
-00001b30: 455a 7876 292e 0a                        EZxv)..
+00000440: 0a0a 2320 4c69 6768 746e 696e 6720 4661  ..# Lightning Fa
+00000450: 6272 6963 3a20 4578 7065 7274 2063 6f6e  bric: Expert con
+00000460: 7472 6f6c 2e0a 0a52 756e 206f 6e20 616e  trol...Run on an
+00000470: 7920 6465 7669 6365 2061 7420 616e 7920  y device at any 
+00000480: 7363 616c 6520 7769 7468 2065 7870 6572  scale with exper
+00000490: 742d 6c65 7665 6c20 636f 6e74 726f 6c20  t-level control 
+000004a0: 6f76 6572 2050 7954 6f72 6368 2074 7261  over PyTorch tra
+000004b0: 696e 696e 6720 6c6f 6f70 2061 6e64 2073  ining loop and s
+000004c0: 6361 6c69 6e67 2073 7472 6174 6567 792e  caling strategy.
+000004d0: 2059 6f75 2063 616e 2065 7665 6e20 7772   You can even wr
+000004e0: 6974 6520 796f 7572 206f 776e 2054 7261  ite your own Tra
+000004f0: 696e 6572 2e0a 0a46 6162 7269 6320 6973  iner...Fabric is
+00000500: 2064 6573 6967 6e65 6420 666f 7220 7468   designed for th
+00000510: 6520 6d6f 7374 2063 6f6d 706c 6578 206d  e most complex m
+00000520: 6f64 656c 7320 6c69 6b65 2066 6f75 6e64  odels like found
+00000530: 6174 696f 6e20 6d6f 6465 6c20 7363 616c  ation model scal
+00000540: 696e 672c 204c 4c4d 732c 2064 6966 6675  ing, LLMs, diffu
+00000550: 7369 6f6e 2c20 7472 616e 7366 6f72 6d65  sion, transforme
+00000560: 7273 2c20 7265 696e 666f 7263 656d 656e  rs, reinforcemen
+00000570: 7420 6c65 6172 6e69 6e67 2c20 6163 7469  t learning, acti
+00000580: 7665 206c 6561 726e 696e 672e 204f 6620  ve learning. Of 
+00000590: 616e 7920 7369 7a65 2e0a 0a3c 7461 626c  any size...<tabl
+000005a0: 653e 0a3c 7472 3e0a 3c74 683e 5768 6174  e>.<tr>.<th>What
+000005b0: 2074 6f20 6368 616e 6765 3c2f 7468 3e0a   to change</th>.
+000005c0: 3c74 683e 5265 7375 6c74 696e 6720 4661  <th>Resulting Fa
+000005d0: 6272 6963 2043 6f64 6520 2863 6f70 7920  bric Code (copy 
+000005e0: 6d65 2129 3c2f 7468 3e0a 3c2f 7472 3e0a  me!)</th>.</tr>.
+000005f0: 3c74 723e 0a3c 7464 3e0a 3c73 7562 3e0a  <tr>.<td>.<sub>.
+00000600: 0a60 6060 6469 6666 0a2b 2069 6d70 6f72  .```diff.+ impor
+00000610: 7420 6c69 6768 746e 696e 6720 6173 204c  t lightning as L
+00000620: 0a20 2069 6d70 6f72 7420 746f 7263 683b  .  import torch;
+00000630: 2069 6d70 6f72 7420 746f 7263 6876 6973   import torchvis
+00000640: 696f 6e20 6173 2074 760a 0a2b 2066 6162  ion as tv..+ fab
+00000650: 7269 6320 3d20 4c2e 4661 6272 6963 2829  ric = L.Fabric()
+00000660: 0a2b 2066 6162 7269 632e 6c61 756e 6368  .+ fabric.launch
+00000670: 2829 0a0a 2020 6d6f 6465 6c20 3d20 7476  ()..  model = tv
+00000680: 2e6d 6f64 656c 732e 7265 736e 6574 3138  .models.resnet18
+00000690: 2829 0a20 206f 7074 696d 697a 6572 203d  ().  optimizer =
+000006a0: 2074 6f72 6368 2e6f 7074 696d 2e53 4744   torch.optim.SGD
+000006b0: 286d 6f64 656c 2e70 6172 616d 6574 6572  (model.parameter
+000006c0: 7328 292c 206c 723d 302e 3030 3129 0a2d  s(), lr=0.001).-
+000006d0: 2064 6576 6963 6520 3d20 2263 7564 6122   device = "cuda"
+000006e0: 2069 6620 746f 7263 682e 6375 6461 2e69   if torch.cuda.i
+000006f0: 735f 6176 6169 6c61 626c 6528 2920 656c  s_available() el
+00000700: 7365 2022 6370 7522 0a2d 206d 6f64 656c  se "cpu".- model
+00000710: 2e74 6f28 6465 7669 6365 290a 2b20 6d6f  .to(device).+ mo
+00000720: 6465 6c2c 206f 7074 696d 697a 6572 203d  del, optimizer =
+00000730: 2066 6162 7269 632e 7365 7475 7028 6d6f   fabric.setup(mo
+00000740: 6465 6c2c 206f 7074 696d 697a 6572 290a  del, optimizer).
+00000750: 0a20 2064 6174 6173 6574 203d 2074 762e  .  dataset = tv.
+00000760: 6461 7461 7365 7473 2e43 4946 4152 3130  datasets.CIFAR10
+00000770: 2822 6461 7461 222c 2064 6f77 6e6c 6f61  ("data", downloa
+00000780: 643d 5472 7565 2c0a 2020 2020 2020 2020  d=True,.        
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2020 2020 2020 2020 7472 6169 6e3d 5472          train=Tr
+000007b0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007d0: 2020 2020 7472 616e 7366 6f72 6d3d 7476      transform=tv
+000007e0: 2e74 7261 6e73 666f 726d 732e 546f 5465  .transforms.ToTe
+000007f0: 6e73 6f72 2829 290a 2020 6461 7461 6c6f  nsor()).  datalo
+00000800: 6164 6572 203d 2074 6f72 6368 2e75 7469  ader = torch.uti
+00000810: 6c73 2e64 6174 612e 4461 7461 4c6f 6164  ls.data.DataLoad
+00000820: 6572 2864 6174 6173 6574 2c20 6261 7463  er(dataset, batc
+00000830: 685f 7369 7a65 3d38 290a 2b20 6461 7461  h_size=8).+ data
+00000840: 6c6f 6164 6572 203d 2066 6162 7269 632e  loader = fabric.
+00000850: 7365 7475 705f 6461 7461 6c6f 6164 6572  setup_dataloader
+00000860: 7328 6461 7461 6c6f 6164 6572 290a 0a20  s(dataloader).. 
+00000870: 206d 6f64 656c 2e74 7261 696e 2829 0a20   model.train(). 
+00000880: 206e 756d 5f65 706f 6368 7320 3d20 3130   num_epochs = 10
+00000890: 0a20 2066 6f72 2065 706f 6368 2069 6e20  .  for epoch in 
+000008a0: 7261 6e67 6528 6e75 6d5f 6570 6f63 6873  range(num_epochs
+000008b0: 293a 0a20 2020 2020 2066 6f72 2062 6174  ):.      for bat
+000008c0: 6368 2069 6e20 6461 7461 6c6f 6164 6572  ch in dataloader
+000008d0: 3a0a 2020 2020 2020 2020 2020 696e 7075  :.          inpu
+000008e0: 7473 2c20 6c61 6265 6c73 203d 2062 6174  ts, labels = bat
+000008f0: 6368 0a2d 2020 2020 2020 2020 2069 6e70  ch.-         inp
+00000900: 7574 732c 206c 6162 656c 7320 3d20 696e  uts, labels = in
+00000910: 7075 7473 2e74 6f28 6465 7669 6365 292c  puts.to(device),
+00000920: 206c 6162 656c 732e 746f 2864 6576 6963   labels.to(devic
+00000930: 6529 0a20 2020 2020 2020 2020 206f 7074  e).          opt
+00000940: 696d 697a 6572 2e7a 6572 6f5f 6772 6164  imizer.zero_grad
+00000950: 2829 0a20 2020 2020 2020 2020 206f 7574  ().          out
+00000960: 7075 7473 203d 206d 6f64 656c 2869 6e70  puts = model(inp
+00000970: 7574 7329 0a20 2020 2020 2020 2020 206c  uts).          l
+00000980: 6f73 7320 3d20 746f 7263 682e 6e6e 2e66  oss = torch.nn.f
+00000990: 756e 6374 696f 6e61 6c2e 6372 6f73 735f  unctional.cross_
+000009a0: 656e 7472 6f70 7928 6f75 7470 7574 732c  entropy(outputs,
+000009b0: 206c 6162 656c 7329 0a2d 2020 2020 2020   labels).-      
+000009c0: 2020 206c 6f73 732e 6261 636b 7761 7264     loss.backward
+000009d0: 2829 0a2b 2020 2020 2020 2020 2066 6162  ().+         fab
+000009e0: 7269 632e 6261 636b 7761 7264 286c 6f73  ric.backward(los
+000009f0: 7329 0a20 2020 2020 2020 2020 206f 7074  s).          opt
+00000a00: 696d 697a 6572 2e73 7465 7028 290a 6060  imizer.step().``
+00000a10: 600a 0a3c 2f73 7562 3e0a 3c74 643e 0a3c  `..</sub>.<td>.<
+00000a20: 7375 623e 0a0a 6060 6050 7974 686f 6e0a  sub>..```Python.
+00000a30: 696d 706f 7274 206c 6967 6874 6e69 6e67  import lightning
+00000a40: 2061 7320 4c0a 696d 706f 7274 2074 6f72   as L.import tor
+00000a50: 6368 3b20 696d 706f 7274 2074 6f72 6368  ch; import torch
+00000a60: 7669 7369 6f6e 2061 7320 7476 0a0a 6661  vision as tv..fa
+00000a70: 6272 6963 203d 204c 2e46 6162 7269 6328  bric = L.Fabric(
+00000a80: 290a 6661 6272 6963 2e6c 6175 6e63 6828  ).fabric.launch(
+00000a90: 290a 0a6d 6f64 656c 203d 2074 762e 6d6f  )..model = tv.mo
+00000aa0: 6465 6c73 2e72 6573 6e65 7431 3828 290a  dels.resnet18().
+00000ab0: 6f70 7469 6d69 7a65 7220 3d20 746f 7263  optimizer = torc
+00000ac0: 682e 6f70 7469 6d2e 5347 4428 6d6f 6465  h.optim.SGD(mode
+00000ad0: 6c2e 7061 7261 6d65 7465 7273 2829 2c20  l.parameters(), 
+00000ae0: 6c72 3d30 2e30 3031 290a 6d6f 6465 6c2c  lr=0.001).model,
+00000af0: 206f 7074 696d 697a 6572 203d 2066 6162   optimizer = fab
+00000b00: 7269 632e 7365 7475 7028 6d6f 6465 6c2c  ric.setup(model,
+00000b10: 206f 7074 696d 697a 6572 290a 0a64 6174   optimizer)..dat
+00000b20: 6173 6574 203d 2074 762e 6461 7461 7365  aset = tv.datase
+00000b30: 7473 2e43 4946 4152 3130 2822 6461 7461  ts.CIFAR10("data
+00000b40: 222c 2064 6f77 6e6c 6f61 643d 5472 7565  ", download=True
+00000b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 7472 6169 6e3d 5472 7565 2c0a 2020 2020  train=True,.    
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2020 2020 2020 2020 7472 616e 7366            transf
+00000ba0: 6f72 6d3d 7476 2e74 7261 6e73 666f 726d  orm=tv.transform
+00000bb0: 732e 546f 5465 6e73 6f72 2829 290a 6461  s.ToTensor()).da
+00000bc0: 7461 6c6f 6164 6572 203d 2074 6f72 6368  taloader = torch
+00000bd0: 2e75 7469 6c73 2e64 6174 612e 4461 7461  .utils.data.Data
+00000be0: 4c6f 6164 6572 2864 6174 6173 6574 2c20  Loader(dataset, 
+00000bf0: 6261 7463 685f 7369 7a65 3d38 290a 6461  batch_size=8).da
+00000c00: 7461 6c6f 6164 6572 203d 2066 6162 7269  taloader = fabri
+00000c10: 632e 7365 7475 705f 6461 7461 6c6f 6164  c.setup_dataload
+00000c20: 6572 7328 6461 7461 6c6f 6164 6572 290a  ers(dataloader).
+00000c30: 0a6d 6f64 656c 2e74 7261 696e 2829 0a6e  .model.train().n
+00000c40: 756d 5f65 706f 6368 7320 3d20 3130 0a66  um_epochs = 10.f
+00000c50: 6f72 2065 706f 6368 2069 6e20 7261 6e67  or epoch in rang
+00000c60: 6528 6e75 6d5f 6570 6f63 6873 293a 0a20  e(num_epochs):. 
+00000c70: 2020 2066 6f72 2062 6174 6368 2069 6e20     for batch in 
+00000c80: 6461 7461 6c6f 6164 6572 3a0a 2020 2020  dataloader:.    
+00000c90: 2020 2020 696e 7075 7473 2c20 6c61 6265      inputs, labe
+00000ca0: 6c73 203d 2062 6174 6368 0a20 2020 2020  ls = batch.     
+00000cb0: 2020 206f 7074 696d 697a 6572 2e7a 6572     optimizer.zer
+00000cc0: 6f5f 6772 6164 2829 0a20 2020 2020 2020  o_grad().       
+00000cd0: 206f 7574 7075 7473 203d 206d 6f64 656c   outputs = model
+00000ce0: 2869 6e70 7574 7329 0a20 2020 2020 2020  (inputs).       
+00000cf0: 206c 6f73 7320 3d20 746f 7263 682e 6e6e   loss = torch.nn
+00000d00: 2e66 756e 6374 696f 6e61 6c2e 6372 6f73  .functional.cros
+00000d10: 735f 656e 7472 6f70 7928 6f75 7470 7574  s_entropy(output
+00000d20: 732c 206c 6162 656c 7329 0a20 2020 2020  s, labels).     
+00000d30: 2020 2066 6162 7269 632e 6261 636b 7761     fabric.backwa
+00000d40: 7264 286c 6f73 7329 0a20 2020 2020 2020  rd(loss).       
+00000d50: 206f 7074 696d 697a 6572 2e73 7465 7028   optimizer.step(
+00000d60: 290a 6060 600a 0a3c 2f73 7562 3e0a 3c2f  ).```..</sub>.</
+00000d70: 7464 3e0a 3c2f 7472 3e0a 3c2f 7461 626c  td>.</tr>.</tabl
+00000d80: 653e 0a0a 2323 204b 6579 2066 6561 7475  e>..## Key featu
+00000d90: 7265 730a 0a3c 6465 7461 696c 733e 0a20  res..<details>. 
+00000da0: 203c 7375 6d6d 6172 793e 4561 7369 6c79   <summary>Easily
+00000db0: 2073 7769 7463 6820 6672 6f6d 2072 756e   switch from run
+00000dc0: 6e69 6e67 206f 6e20 4350 5520 746f 2047  ning on CPU to G
+00000dd0: 5055 2028 4170 706c 6520 5369 6c69 636f  PU (Apple Silico
+00000de0: 6e2c 2043 5544 412c 20e2 80a6 292c 2054  n, CUDA, ...), T
+00000df0: 5055 2c20 6d75 6c74 692d 4750 5520 6f72  PU, multi-GPU or
+00000e00: 2065 7665 6e20 6d75 6c74 692d 6e6f 6465   even multi-node
+00000e10: 2074 7261 696e 696e 673c 2f73 756d 6d61   training</summa
+00000e20: 7279 3e0a 0a60 6060 7079 7468 6f6e 0a23  ry>..```python.#
+00000e30: 2055 7365 2079 6f75 7220 6176 6169 6c61   Use your availa
+00000e40: 626c 6520 6861 7264 7761 7265 0a23 206e  ble hardware.# n
+00000e50: 6f20 636f 6465 2063 6861 6e67 6573 206e  o code changes n
+00000e60: 6565 6465 640a 6661 6272 6963 203d 2046  eeded.fabric = F
+00000e70: 6162 7269 6328 290a 0a23 2052 756e 206f  abric()..# Run o
+00000e80: 6e20 4750 5573 2028 4355 4441 206f 7220  n GPUs (CUDA or 
+00000e90: 4d50 5329 0a66 6162 7269 6320 3d20 4661  MPS).fabric = Fa
+00000ea0: 6272 6963 2861 6363 656c 6572 6174 6f72  bric(accelerator
+00000eb0: 3d22 6770 7522 290a 0a23 2038 2047 5055  ="gpu")..# 8 GPU
+00000ec0: 730a 6661 6272 6963 203d 2046 6162 7269  s.fabric = Fabri
+00000ed0: 6328 6163 6365 6c65 7261 746f 723d 2267  c(accelerator="g
+00000ee0: 7075 222c 2064 6576 6963 6573 3d38 290a  pu", devices=8).
+00000ef0: 0a23 2032 3536 2047 5055 732c 206d 756c  .# 256 GPUs, mul
+00000f00: 7469 2d6e 6f64 650a 6661 6272 6963 203d  ti-node.fabric =
+00000f10: 2046 6162 7269 6328 6163 6365 6c65 7261   Fabric(accelera
+00000f20: 746f 723d 2267 7075 222c 2064 6576 6963  tor="gpu", devic
+00000f30: 6573 3d38 2c20 6e75 6d5f 6e6f 6465 733d  es=8, num_nodes=
+00000f40: 3332 290a 0a23 2052 756e 206f 6e20 5450  32)..# Run on TP
+00000f50: 5573 0a66 6162 7269 6320 3d20 4661 6272  Us.fabric = Fabr
+00000f60: 6963 2861 6363 656c 6572 6174 6f72 3d22  ic(accelerator="
+00000f70: 7470 7522 290a 6060 600a 0a3c 2f64 6574  tpu").```..</det
+00000f80: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
+00000f90: 0a20 203c 7375 6d6d 6172 793e 5573 6520  .  <summary>Use 
+00000fa0: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
+00000fb0: 2064 6973 7472 6962 7574 6564 2074 7261   distributed tra
+00000fc0: 696e 696e 6720 7374 7261 7465 6769 6573  ining strategies
+00000fd0: 2028 4444 502c 2046 5344 502c 2044 6565   (DDP, FSDP, Dee
+00000fe0: 7053 7065 6564 2920 616e 6420 6d69 7865  pSpeed) and mixe
+00000ff0: 6420 7072 6563 6973 696f 6e20 6f75 7420  d precision out 
+00001000: 6f66 2074 6865 2062 6f78 3c2f 7375 6d6d  of the box</summ
+00001010: 6172 793e 0a0a 6060 6070 7974 686f 6e0a  ary>..```python.
+00001020: 2320 5573 6520 7374 6174 652d 6f66 2d74  # Use state-of-t
+00001030: 6865 2d61 7274 2064 6973 7472 6962 7574  he-art distribut
+00001040: 6564 2074 7261 696e 696e 6720 7465 6368  ed training tech
+00001050: 6e69 7175 6573 0a66 6162 7269 6320 3d20  niques.fabric = 
+00001060: 4661 6272 6963 2873 7472 6174 6567 793d  Fabric(strategy=
+00001070: 2264 6470 2229 0a66 6162 7269 6320 3d20  "ddp").fabric = 
+00001080: 4661 6272 6963 2873 7472 6174 6567 793d  Fabric(strategy=
+00001090: 2264 6565 7073 7065 6564 2229 0a66 6162  "deepspeed").fab
+000010a0: 7269 6320 3d20 4661 6272 6963 2873 7472  ric = Fabric(str
+000010b0: 6174 6567 793d 2266 7364 7022 290a 0a23  ategy="fsdp")..#
+000010c0: 2053 7769 7463 6820 7468 6520 7072 6563   Switch the prec
+000010d0: 6973 696f 6e0a 6661 6272 6963 203d 2046  ision.fabric = F
+000010e0: 6162 7269 6328 7072 6563 6973 696f 6e3d  abric(precision=
+000010f0: 2231 362d 6d69 7865 6422 290a 6661 6272  "16-mixed").fabr
+00001100: 6963 203d 2046 6162 7269 6328 7072 6563  ic = Fabric(prec
+00001110: 6973 696f 6e3d 2236 3422 290a 6060 600a  ision="64").```.
+00001120: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00001130: 7461 696c 733e 0a20 203c 7375 6d6d 6172  tails>.  <summar
+00001140: 793e 416c 6c20 7468 6520 6465 7669 6365  y>All the device
+00001150: 206c 6f67 6963 2062 6f69 6c65 7270 6c61   logic boilerpla
+00001160: 7465 2069 7320 6861 6e64 6c65 6420 666f  te is handled fo
+00001170: 7220 796f 753c 2f73 756d 6d61 7279 3e0a  r you</summary>.
+00001180: 0a60 6060 6469 6666 0a20 2023 206e 6f20  .```diff.  # no 
+00001190: 6d6f 7265 206f 6620 7468 6973 210a 2d20  more of this!.- 
+000011a0: 6d6f 6465 6c2e 746f 2864 6576 6963 6529  model.to(device)
+000011b0: 0a2d 2062 6174 6368 2e74 6f28 6465 7669  .- batch.to(devi
+000011c0: 6365 290a 6060 600a 0a3c 2f64 6574 6169  ce).```..</detai
+000011d0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a20  ls>..<details>. 
+000011e0: 203c 7375 6d6d 6172 793e 4275 696c 6420   <summary>Build 
+000011f0: 796f 7572 206f 776e 2063 7573 746f 6d20  your own custom 
+00001200: 5472 6169 6e65 7220 7573 696e 6720 4661  Trainer using Fa
+00001210: 6272 6963 2070 7269 6d69 7469 7665 7320  bric primitives 
+00001220: 666f 7220 7472 6169 6e69 6e67 2063 6865  for training che
+00001230: 636b 706f 696e 7469 6e67 2c20 6c6f 6767  ckpointing, logg
+00001240: 696e 672c 2061 6e64 206d 6f72 653c 2f73  ing, and more</s
+00001250: 756d 6d61 7279 3e0a 0a60 6060 7079 7468  ummary>..```pyth
+00001260: 6f6e 0a69 6d70 6f72 7420 6c69 6768 746e  on.import lightn
+00001270: 696e 6720 6173 204c 0a0a 0a63 6c61 7373  ing as L...class
+00001280: 204d 7943 7573 746f 6d54 7261 696e 6572   MyCustomTrainer
+00001290: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000012a0: 5f5f 2873 656c 662c 2061 6363 656c 6572  __(self, acceler
+000012b0: 6174 6f72 3d22 6175 746f 222c 2073 7472  ator="auto", str
+000012c0: 6174 6567 793d 2261 7574 6f22 2c20 6465  ategy="auto", de
+000012d0: 7669 6365 733d 2261 7574 6f22 2c20 7072  vices="auto", pr
+000012e0: 6563 6973 696f 6e3d 2233 322d 7472 7565  ecision="32-true
+000012f0: 2229 3a0a 2020 2020 2020 2020 7365 6c66  "):.        self
+00001300: 2e66 6162 7269 6320 3d20 4c2e 4661 6272  .fabric = L.Fabr
+00001310: 6963 2861 6363 656c 6572 6174 6f72 3d61  ic(accelerator=a
+00001320: 6363 656c 6572 6174 6f72 2c20 7374 7261  ccelerator, stra
+00001330: 7465 6779 3d73 7472 6174 6567 792c 2064  tegy=strategy, d
+00001340: 6576 6963 6573 3d64 6576 6963 6573 2c20  evices=devices, 
+00001350: 7072 6563 6973 696f 6e3d 7072 6563 6973  precision=precis
+00001360: 696f 6e29 0a0a 2020 2020 6465 6620 6669  ion)..    def fi
+00001370: 7428 7365 6c66 2c20 6d6f 6465 6c2c 206f  t(self, model, o
+00001380: 7074 696d 697a 6572 2c20 6461 7461 6c6f  ptimizer, datalo
+00001390: 6164 6572 2c20 6d61 785f 6570 6f63 6873  ader, max_epochs
+000013a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000013b0: 6661 6272 6963 2e6c 6175 6e63 6828 290a  fabric.launch().
+000013c0: 0a20 2020 2020 2020 206d 6f64 656c 2c20  .        model, 
+000013d0: 6f70 7469 6d69 7a65 7220 3d20 7365 6c66  optimizer = self
+000013e0: 2e66 6162 7269 632e 7365 7475 7028 6d6f  .fabric.setup(mo
+000013f0: 6465 6c2c 206f 7074 696d 697a 6572 290a  del, optimizer).
+00001400: 2020 2020 2020 2020 6461 7461 6c6f 6164          dataload
+00001410: 6572 203d 2073 656c 662e 6661 6272 6963  er = self.fabric
+00001420: 2e73 6574 7570 5f64 6174 616c 6f61 6465  .setup_dataloade
+00001430: 7273 2864 6174 616c 6f61 6465 7229 0a20  rs(dataloader). 
+00001440: 2020 2020 2020 206d 6f64 656c 2e74 7261         model.tra
+00001450: 696e 2829 0a0a 2020 2020 2020 2020 666f  in()..        fo
+00001460: 7220 6570 6f63 6820 696e 2072 616e 6765  r epoch in range
+00001470: 286d 6178 5f65 706f 6368 7329 3a0a 2020  (max_epochs):.  
+00001480: 2020 2020 2020 2020 2020 666f 7220 6261            for ba
+00001490: 7463 6820 696e 2064 6174 616c 6f61 6465  tch in dataloade
+000014a0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+000014b0: 2020 2069 6e70 7574 2c20 7461 7267 6574     input, target
+000014c0: 203d 2062 6174 6368 0a20 2020 2020 2020   = batch.       
+000014d0: 2020 2020 2020 2020 206f 7074 696d 697a           optimiz
+000014e0: 6572 2e7a 6572 6f5f 6772 6164 2829 0a20  er.zero_grad(). 
+000014f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00001500: 7574 7075 7420 3d20 6d6f 6465 6c28 696e  utput = model(in
+00001510: 7075 7429 0a20 2020 2020 2020 2020 2020  put).           
+00001520: 2020 2020 206c 6f73 7320 3d20 6c6f 7373       loss = loss
+00001530: 5f66 6e28 6f75 7470 7574 2c20 7461 7267  _fn(output, targ
+00001540: 6574 290a 2020 2020 2020 2020 2020 2020  et).            
+00001550: 2020 2020 7365 6c66 2e66 6162 7269 632e      self.fabric.
+00001560: 6261 636b 7761 7264 286c 6f73 7329 0a20  backward(loss). 
+00001570: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00001580: 7074 696d 697a 6572 2e73 7465 7028 290a  ptimizer.step().
+00001590: 6060 600a 0a59 6f75 2063 616e 2066 696e  ```..You can fin
+000015a0: 6420 6120 6d6f 7265 2065 7874 656e 7369  d a more extensi
+000015b0: 7665 2065 7861 6d70 6c65 2069 6e20 6f75  ve example in ou
+000015c0: 7220 5b65 7861 6d70 6c65 735d 282e 2e2f  r [examples](../
+000015d0: 2e2e 2f65 7861 6d70 6c65 732f 6661 6272  ../examples/fabr
+000015e0: 6963 2f62 7569 6c64 5f79 6f75 725f 6f77  ic/build_your_ow
+000015f0: 6e5f 7472 6169 6e65 7229 0a0a 3c2f 6465  n_trainer)..</de
+00001600: 7461 696c 733e 0a0a 5f5f 5f5f 5f5f 5f5f  tails>..________
+00001610: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001620: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001630: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001640: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a  ______________..
+00001650: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00001660: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+00001670: 3d22 6874 7470 733a 2f2f 6c69 6768 746e  ="https://lightn
+00001680: 696e 672e 6169 2f64 6f63 732f 6661 6272  ing.ai/docs/fabr
+00001690: 6963 2f73 7461 626c 652f 223e 5265 6164  ic/stable/">Read
+000016a0: 2074 6865 204c 6967 6874 6e69 6e67 2046   the Lightning F
+000016b0: 6162 7269 6320 646f 6373 3c2f 613e 0a3c  abric docs</a>.<
+000016c0: 2f64 6976 3e0a 0a5f 5f5f 5f5f 5f5f 5f5f  /div>.._________
+000016d0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000016e0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000016f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001700: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f0a 0a23  _____________..#
+00001710: 2047 6574 7469 6e67 2073 7461 7274 6564   Getting started
+00001720: 0a0a 2323 2049 6e73 7461 6c6c 204c 6967  ..## Install Lig
+00001730: 6874 6e69 6e67 0a0a 3c64 6574 6169 6c73  htning..<details
+00001740: 3e0a 0a3c 7375 6d6d 6172 793e 5072 6572  >..<summary>Prer
+00001750: 6571 7569 7369 7465 733c 2f73 756d 6d61  equisites</summa
+00001760: 7279 3e0a 0a3e 2054 4950 3a20 5765 2073  ry>..> TIP: We s
+00001770: 7472 6f6e 676c 7920 7265 636f 6d6d 656e  trongly recommen
+00001780: 6420 6372 6561 7469 6e67 2061 2076 6972  d creating a vir
+00001790: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
+000017a0: 2066 6972 7374 2e0a 3e20 446f 6ee2 8099   first..> Don...
+000017b0: 7420 6b6e 6f77 2077 6861 7420 7468 6973  t know what this
+000017c0: 2069 733f 2046 6f6c 6c6f 7720 6f75 7220   is? Follow our 
+000017d0: 5b62 6567 696e 6e65 7220 6775 6964 6520  [beginner guide 
+000017e0: 6865 7265 5d28 6874 7470 733a 2f2f 6c69  here](https://li
+000017f0: 6768 746e 696e 672e 6169 2f64 6f63 732f  ghtning.ai/docs/
+00001800: 7374 6162 6c65 2f69 6e73 7461 6c6c 2f69  stable/install/i
+00001810: 6e73 7461 6c6c 6174 696f 6e2e 6874 6d6c  nstallation.html
+00001820: 292e 0a0a 2d20 5079 7468 6f6e 2033 2e38  )...- Python 3.8
+00001830: 2e78 206f 7220 6c61 7465 7220 2833 2e38  .x or later (3.8
+00001840: 2e78 2c20 332e 392e 782c 2033 2e31 302e  .x, 3.9.x, 3.10.
+00001850: 782c 202e 2e2e 290a 0a3c 2f64 6574 6169  x, ...)..</detai
+00001860: 6c73 3e0a 0a60 6060 6261 7368 0a70 6970  ls>..```bash.pip
+00001870: 2069 6e73 7461 6c6c 202d 5520 6c69 6768   install -U ligh
+00001880: 746e 696e 670a 6060 600a 0a23 2320 436f  tning.```..## Co
+00001890: 6e76 6572 7420 796f 7572 2050 7954 6f72  nvert your PyTor
+000018a0: 6368 2074 6f20 4661 6272 6963 0a0a 312e  ch to Fabric..1.
+000018b0: 2043 7265 6174 6520 7468 6520 6046 6162   Create the `Fab
+000018c0: 7269 6360 206f 626a 6563 7420 6174 2074  ric` object at t
+000018d0: 6865 2062 6567 696e 6e69 6e67 206f 6620  he beginning of 
+000018e0: 796f 7572 2074 7261 696e 696e 6720 636f  your training co
+000018f0: 6465 2e0a 0a20 2020 6060 600a 2020 2069  de...   ```.   i
+00001900: 6d70 6f72 7420 4c69 6768 746e 696e 6720  mport Lightning 
+00001910: 6173 204c 0a0a 2020 2066 6162 7269 6320  as L..   fabric 
+00001920: 3d20 4c2e 4661 6272 6963 2829 0a20 2020  = L.Fabric().   
+00001930: 6060 600a 0a31 2e20 4361 6c6c 2060 7365  ```..1. Call `se
+00001940: 7475 7028 2960 206f 6e20 6561 6368 206d  tup()` on each m
+00001950: 6f64 656c 2061 6e64 206f 7074 696d 697a  odel and optimiz
+00001960: 6572 2070 6169 7220 616e 6420 6073 6574  er pair and `set
+00001970: 7570 5f64 6174 616c 6f61 6465 7273 2829  up_dataloaders()
+00001980: 6020 6f6e 2061 6c6c 2079 6f75 7220 6461  ` on all your da
+00001990: 7461 206c 6f61 6465 7273 2e0a 0a20 2020  ta loaders...   
+000019a0: 6060 600a 2020 206d 6f64 656c 2c20 6f70  ```.   model, op
+000019b0: 7469 6d69 7a65 7220 3d20 6661 6272 6963  timizer = fabric
+000019c0: 2e73 6574 7570 286d 6f64 656c 2c20 6f70  .setup(model, op
+000019d0: 7469 6d69 7a65 7229 0a20 2020 6461 7461  timizer).   data
+000019e0: 6c6f 6164 6572 203d 2066 6162 7269 632e  loader = fabric.
+000019f0: 7365 7475 705f 6461 7461 6c6f 6164 6572  setup_dataloader
+00001a00: 7328 6461 7461 6c6f 6164 6572 290a 2020  s(dataloader).  
+00001a10: 2060 6060 0a0a 312e 2052 656d 6f76 6520   ```..1. Remove 
+00001a20: 616c 6c20 602e 746f 6020 616e 6420 602e  all `.to` and `.
+00001a30: 6375 6461 6020 6361 6c6c 7320 2d3e 2046  cuda` calls -> F
+00001a40: 6162 7269 6320 7769 6c6c 2074 616b 6520  abric will take 
+00001a50: 6361 7265 206f 6620 6974 2e0a 0a20 2020  care of it...   
+00001a60: 6060 6064 6966 660a 2020 202d 206d 6f64  ```diff.   - mod
+00001a70: 656c 2e74 6f28 6465 7669 6365 290a 2020  el.to(device).  
+00001a80: 202d 2062 6174 6368 2e74 6f28 6465 7669   - batch.to(devi
+00001a90: 6365 290a 2020 2060 6060 0a0a 312e 2052  ce).   ```..1. R
+00001aa0: 6570 6c61 6365 2060 6c6f 7373 2e62 6163  eplace `loss.bac
+00001ab0: 6b77 6172 6428 2960 2062 7920 6066 6162  kward()` by `fab
+00001ac0: 7269 632e 6261 636b 7761 7264 286c 6f73  ric.backward(los
+00001ad0: 7329 602e 0a0a 2020 2060 6060 6469 6666  s)`...   ```diff
+00001ae0: 0a20 2020 2d20 6c6f 7373 2e62 6163 6b77  .   - loss.backw
+00001af0: 6172 6428 290a 2020 202b 2066 6162 7269  ard().   + fabri
+00001b00: 632e 6261 636b 7761 7264 286c 6f73 7329  c.backward(loss)
+00001b10: 0a20 2020 6060 600a 0a31 2e20 5275 6e20  .   ```..1. Run 
+00001b20: 7468 6520 7363 7269 7074 2066 726f 6d20  the script from 
+00001b30: 7468 6520 7465 726d 696e 616c 2077 6974  the terminal wit
+00001b40: 680a 0a20 2020 6060 6062 6173 680a 2020  h..   ```bash.  
+00001b50: 206c 6967 6874 6e69 6e67 2072 756e 206d   lightning run m
+00001b60: 6f64 656c 2070 6174 682f 746f 2f74 7261  odel path/to/tra
+00001b70: 696e 2e70 790a 2020 2060 6060 0a0a 6f72  in.py.   ```..or
+00001b80: 2075 7365 2074 6865 206c 6175 6e63 6828   use the launch(
+00001b90: 2920 6d65 7468 6f64 2069 6e20 6120 6e6f  ) method in a no
+00001ba0: 7465 626f 6f6b 2e20 4c65 6172 6e20 6d6f  tebook. Learn mo
+00001bb0: 7265 2061 626f 7574 205b 6c61 756e 6368  re about [launch
+00001bc0: 696e 6720 6469 7374 7269 6275 7465 6420  ing distributed 
+00001bd0: 7472 6169 6e69 6e67 5d28 6874 7470 733a  training](https:
+00001be0: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
+00001bf0: 6f63 732f 6661 6272 6963 2f73 7461 626c  ocs/fabric/stabl
+00001c00: 652f 6675 6e64 616d 656e 7461 6c73 2f6c  e/fundamentals/l
+00001c10: 6175 6e63 682e 6874 6d6c 292e 0a0a 5f5f  aunch.html)...__
+00001c20: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c60: 5f5f 5f5f 0a0a 2320 4641 510a 0a23 2320  ____..# FAQ..## 
+00001c70: 5768 656e 2074 6f20 7573 6520 4661 6272  When to use Fabr
+00001c80: 6963 3f0a 0a2d 202a 2a4d 696e 696d 756d  ic?..- **Minimum
+00001c90: 2063 6f64 6520 6368 616e 6765 732a 2a2d   code changes**-
+00001ca0: 2059 6f75 2077 616e 7420 746f 2073 6361   You want to sca
+00001cb0: 6c65 2079 6f75 7220 5079 546f 7263 6820  le your PyTorch 
+00001cc0: 6d6f 6465 6c20 746f 2075 7365 206d 756c  model to use mul
+00001cd0: 7469 2d47 5055 206f 7220 7573 6520 6164  ti-GPU or use ad
+00001ce0: 7661 6e63 6564 2073 7472 6174 6567 6965  vanced strategie
+00001cf0: 7320 6c69 6b65 2044 6565 7053 7065 6564  s like DeepSpeed
+00001d00: 2077 6974 686f 7574 2068 6176 696e 6720   without having 
+00001d10: 746f 2072 6566 6163 746f 722e 2059 6f75  to refactor. You
+00001d20: 2064 6f6e e280 9974 2063 6172 6520 6162   don...t care ab
+00001d30: 6f75 7420 7374 7275 6374 7572 696e 6720  out structuring 
+00001d40: 796f 7572 2063 6f64 652d 2079 6f75 206a  your code- you j
+00001d50: 7573 7420 7761 6e74 2074 6f20 7363 616c  ust want to scal
+00001d60: 6520 6974 2061 7320 6661 7374 2061 7320  e it as fast as 
+00001d70: 706f 7373 6962 6c65 2e0a 2d20 2a2a 4d61  possible..- **Ma
+00001d80: 786d 6975 6d20 636f 6e74 726f 6c2a 2a2d  xmium control**-
+00001d90: 2057 7269 7465 2079 6f75 7220 6f77 6e20   Write your own 
+00001da0: 7472 6169 6e69 6e67 2061 6e64 2f6f 7220  training and/or 
+00001db0: 696e 6665 7265 6e63 6520 6c6f 6769 6320  inference logic 
+00001dc0: 646f 776e 2074 6f20 7468 6520 696e 6469  down to the indi
+00001dd0: 7669 6475 616c 206f 7074 696d 697a 6572  vidual optimizer
+00001de0: 2063 616c 6c73 2e20 596f 7520 6172 656e   calls. You aren
+00001df0: e280 9974 2066 6f72 6365 6420 746f 2063  ...t forced to c
+00001e00: 6f6e 666f 726d 2074 6f20 6120 7374 616e  onform to a stan
+00001e10: 6461 7264 697a 6564 2065 706f 6368 2d62  dardized epoch-b
+00001e20: 6173 6564 2074 7261 696e 696e 6720 6c6f  ased training lo
+00001e30: 6f70 206c 696b 6520 7468 6520 6f6e 6520  op like the one 
+00001e40: 696e 204c 6967 6874 6e69 6e67 2054 7261  in Lightning Tra
+00001e50: 696e 6572 2e20 596f 7520 6361 6e20 646f  iner. You can do
+00001e60: 2066 6c65 7869 626c 6520 6974 6572 6174   flexible iterat
+00001e70: 696f 6e20 6261 7365 6420 7472 6169 6e69  ion based traini
+00001e80: 6e67 2c20 6d65 7461 2d6c 6561 726e 696e  ng, meta-learnin
+00001e90: 672c 2063 726f 7373 2d76 616c 6964 6174  g, cross-validat
+00001ea0: 696f 6e20 616e 6420 6f74 6865 7220 7479  ion and other ty
+00001eb0: 7065 7320 6f66 206f 7074 696d 697a 6174  pes of optimizat
+00001ec0: 696f 6e20 616c 676f 7269 7468 6d73 2077  ion algorithms w
+00001ed0: 6974 686f 7574 2064 6967 6769 6e67 2069  ithout digging i
+00001ee0: 6e74 6f20 6672 616d 6577 6f72 6b20 696e  nto framework in
+00001ef0: 7465 726e 616c 732e 2054 6869 7320 616c  ternals. This al
+00001f00: 736f 206d 616b 6573 2069 7420 7375 7065  so makes it supe
+00001f10: 7220 6561 7379 2074 6f20 6164 6f70 7420  r easy to adopt 
+00001f20: 4661 6272 6963 2069 6e20 6578 6973 7469  Fabric in existi
+00001f30: 6e67 2050 7954 6f72 6368 2070 726f 6a65  ng PyTorch proje
+00001f40: 6374 7320 746f 2073 7065 6564 2d75 7020  cts to speed-up 
+00001f50: 616e 6420 7363 616c 6520 796f 7572 206d  and scale your m
+00001f60: 6f64 656c 7320 7769 7468 6f75 7420 7468  odels without th
+00001f70: 6520 636f 6d70 726f 6d69 7365 206f 6e20  e compromise on 
+00001f80: 6c61 7267 6520 7265 6661 6374 6f72 732e  large refactors.
+00001f90: 204a 7573 7420 7265 6d65 6d62 6572 3a20   Just remember: 
+00001fa0: 5769 7468 2067 7265 6174 2070 6f77 6572  With great power
+00001fb0: 2063 6f6d 6573 2061 2067 7265 6174 2072   comes a great r
+00001fc0: 6573 706f 6e73 6962 696c 6974 792e 0a2d  esponsibility..-
+00001fd0: 202a 2a4d 6178 6d69 756d 2066 6c65 7869   **Maxmium flexi
+00001fe0: 6269 6c69 7479 2a2a 2d20 596f 7520 7761  bility**- You wa
+00001ff0: 6e74 2074 6f20 6861 7665 2066 756c 6c20  nt to have full 
+00002000: 636f 6e74 726f 6c20 6f76 6572 2079 6f75  control over you
+00002010: 7220 656e 7469 7265 2074 7261 696e 696e  r entire trainin
+00002020: 672d 2069 6e20 4661 6272 6963 2061 6c6c  g- in Fabric all
+00002030: 2066 6561 7475 7265 7320 6172 6520 6f70   features are op
+00002040: 742d 696e 2c20 616e 6420 6974 2070 726f  t-in, and it pro
+00002050: 7669 6465 7320 796f 7520 7769 7468 2061  vides you with a
+00002060: 2074 6f6f 6c20 626f 7820 6f66 2070 7269   tool box of pri
+00002070: 6d69 7469 7665 7320 736f 2079 6f75 2063  mitives so you c
+00002080: 616e 2062 7569 6c64 2079 6f75 7220 6f77  an build your ow
+00002090: 6e20 5472 6169 6e65 722e 0a0a 2323 2057  n Trainer...## W
+000020a0: 6865 6e20 746f 2075 7365 2074 6865 205b  hen to use the [
+000020b0: 4c69 6768 746e 696e 6720 5472 6169 6e65  Lightning Traine
+000020c0: 725d 2868 7474 7073 3a2f 2f6c 6967 6874  r](https://light
+000020d0: 6e69 6e67 2e61 692f 646f 6373 2f70 7974  ning.ai/docs/pyt
+000020e0: 6f72 6368 2f73 7461 626c 652f 636f 6d6d  orch/stable/comm
+000020f0: 6f6e 2f74 7261 696e 6572 2e68 746d 6c29  on/trainer.html)
+00002100: 3f0a 0a2d 2059 6f75 2077 616e 7420 746f  ?..- You want to
+00002110: 2068 6176 6520 616c 6c20 7468 6520 656e   have all the en
+00002120: 6769 6e65 6572 696e 6720 626f 696c 6572  gineering boiler
+00002130: 706c 6174 6520 6861 6e64 6c65 6420 666f  plate handled fo
+00002140: 7220 796f 7520 2d20 646f 7a65 6e73 206f  r you - dozens o
+00002150: 6620 6665 6174 7572 6573 206c 696b 6520  f features like 
+00002160: 6368 6563 6b70 6f69 6e74 696e 672c 206c  checkpointing, l
+00002170: 6f67 6769 6e67 2061 6e64 2065 6172 6c79  ogging and early
+00002180: 2073 746f 7070 696e 6720 6f75 7420 6f66   stopping out of
+00002190: 2074 6865 2062 6f78 2e20 4c65 7373 2068   the box. Less h
+000021a0: 6173 736c 652c 206c 6573 7320 6572 726f  assle, less erro
+000021b0: 7220 7072 6f6e 652c 2065 6173 7920 746f  r prone, easy to
+000021c0: 2074 7279 2064 6966 6665 7265 6e74 2074   try different t
+000021d0: 6563 686e 6971 7565 7320 616e 6420 6665  echniques and fe
+000021e0: 6174 7572 6573 2e0a 2d20 596f 7520 7761  atures..- You wa
+000021f0: 6e74 2074 6f20 6861 7665 2067 6f6f 6420  nt to have good 
+00002200: 6465 6661 756c 7473 2063 686f 7365 6e20  defaults chosen 
+00002210: 666f 7220 796f 7520 2d20 736f 2079 6f75  for you - so you
+00002220: 2063 616e 2068 6176 6520 6120 6265 7474   can have a bett
+00002230: 6572 2073 7461 7274 696e 6720 706f 696e  er starting poin
+00002240: 742e 0a2d 2059 6f75 2077 616e 7420 796f  t..- You want yo
+00002250: 7572 2063 6f64 6520 746f 2062 6520 6d6f  ur code to be mo
+00002260: 6475 6c61 722c 2072 6561 6461 626c 6520  dular, readable 
+00002270: 616e 6420 7765 6c6c 2073 7472 7563 7475  and well structu
+00002280: 7265 6420 2d20 6561 7379 2074 6f20 7368  red - easy to sh
+00002290: 6172 6520 6265 7477 6565 6e20 7072 6f6a  are between proj
+000022a0: 6563 7473 2061 6e64 2077 6974 6820 636f  ects and with co
+000022b0: 6c6c 6162 6f72 6174 6f72 732e 0a0a 2323  llaborators...##
+000022c0: 2043 616e 2049 2075 7365 2046 6162 7269   Can I use Fabri
+000022d0: 6320 7769 7468 206d 7920 4c69 6768 746e  c with my Lightn
+000022e0: 696e 674d 6f64 756c 6520 6f72 204c 6967  ingModule or Lig
+000022f0: 6874 6e69 6e67 2043 616c 6c62 6163 6b3f  htning Callback?
+00002300: 0a0a 5965 7320 3a29 2046 6162 7269 6320  ..Yes :) Fabric 
+00002310: 776f 726b 7320 7769 7468 2050 7954 6f72  works with PyTor
+00002320: 6368 204c 6967 6874 6e69 6e67 4d6f 6475  ch LightningModu
+00002330: 6c65 7320 616e 6420 4361 6c6c 6261 636b  les and Callback
+00002340: 732c 2073 6f20 796f 7520 6361 6e20 6368  s, so you can ch
+00002350: 6f6f 7365 2068 6f77 2074 6f20 7374 7275  oose how to stru
+00002360: 6374 7572 6520 796f 7572 2063 6f64 6520  cture your code 
+00002370: 616e 6420 7265 7573 6520 6578 6973 7469  and reuse existi
+00002380: 6e67 206d 6f64 656c 7320 616e 6420 6361  ng models and ca
+00002390: 6c6c 6261 636b 7320 6173 2079 6f75 2077  llbacks as you w
+000023a0: 6973 682e 2052 6561 6420 6d6f 7265 205b  ish. Read more [
+000023b0: 6865 7265 5d28 6874 7470 733a 2f2f 6c69  here](https://li
+000023c0: 6768 746e 696e 672e 6169 2f64 6f63 732f  ghtning.ai/docs/
+000023d0: 6661 6272 6963 2f73 7461 626c 652f 6675  fabric/stable/fu
+000023e0: 6e64 616d 656e 7461 6c73 2f63 6f64 655f  ndamentals/code_
+000023f0: 7374 7275 6374 7572 652e 6874 6d6c 292e  structure.html).
+00002400: 0a0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
+00002410: 733a 2f2f 706c 2d70 7562 6c69 632d 6461  s://pl-public-da
+00002420: 7461 2e73 332e 616d 617a 6f6e 6177 732e  ta.s3.amazonaws.
+00002430: 636f 6d2f 6173 7365 7473 5f6c 6967 6874  com/assets_light
+00002440: 6e69 6e67 2f63 6f6e 7469 6e75 756d 2e70  ning/continuum.p
+00002450: 6e67 2220 7769 6474 683d 2238 3030 7078  ng" width="800px
+00002460: 223e 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ">..____________
+00002470: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002480: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002490: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000024a0: 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a 2320 4578  __________..# Ex
+000024b0: 616d 706c 6573 0a0a 2d20 5b47 414e 5d28  amples..- [GAN](
+000024c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000024d0: 6f6d 2f4c 6967 6874 6e69 6e67 2d41 492f  om/Lightning-AI/
+000024e0: 6c69 6768 746e 696e 672f 7472 6565 2f6d  lightning/tree/m
+000024f0: 6173 7465 722f 6578 616d 706c 6573 2f66  aster/examples/f
+00002500: 6162 7269 632f 6463 6761 6e29 0a2d 205b  abric/dcgan).- [
+00002510: 4d65 7461 206c 6561 726e 696e 675d 2868  Meta learning](h
+00002520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002530: 6d2f 4c69 6768 746e 696e 672d 4149 2f6c  m/Lightning-AI/l
+00002540: 6967 6874 6e69 6e67 2f74 7265 652f 6d61  ightning/tree/ma
+00002550: 7374 6572 2f65 7861 6d70 6c65 732f 6661  ster/examples/fa
+00002560: 6272 6963 2f6d 6574 615f 6c65 6172 6e69  bric/meta_learni
+00002570: 6e67 290a 2d20 5b52 6569 6e66 6f72 6365  ng).- [Reinforce
+00002580: 6d65 6e74 206c 6561 726e 696e 675d 2868  ment learning](h
+00002590: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000025a0: 6d2f 4c69 6768 746e 696e 672d 4149 2f6c  m/Lightning-AI/l
+000025b0: 6967 6874 6e69 6e67 2f74 7265 652f 6d61  ightning/tree/ma
+000025c0: 7374 6572 2f65 7861 6d70 6c65 732f 6661  ster/examples/fa
+000025d0: 6272 6963 2f72 6569 6e66 6f72 6365 6d65  bric/reinforceme
+000025e0: 6e74 5f6c 6561 726e 696e 6729 0a2d 205b  nt_learning).- [
+000025f0: 4b2d 466f 6c64 2063 726f 7373 2076 616c  K-Fold cross val
+00002600: 6964 6174 696f 6e5d 2868 7474 7073 3a2f  idation](https:/
+00002610: 2f67 6974 6875 622e 636f 6d2f 4c69 6768  /github.com/Ligh
+00002620: 746e 696e 672d 4149 2f6c 6967 6874 6e69  tning-AI/lightni
+00002630: 6e67 2f74 7265 652f 6d61 7374 6572 2f65  ng/tree/master/e
+00002640: 7861 6d70 6c65 732f 6661 6272 6963 2f6b  xamples/fabric/k
+00002650: 666f 6c64 5f63 7629 0a0a 5f5f 5f5f 5f5f  fold_cv)..______
+00002660: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002670: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002680: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002690: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000026a0: 0a0a 2323 2041 736b 696e 6720 666f 7220  ..## Asking for 
+000026b0: 6865 6c70 0a0a 4966 2079 6f75 2068 6176  help..If you hav
+000026c0: 6520 616e 7920 7175 6573 7469 6f6e 7320  e any questions 
+000026d0: 706c 6561 7365 3a0a 0a31 2e20 5b52 6561  please:..1. [Rea
+000026e0: 6420 7468 6520 646f 6373 5d28 6874 7470  d the docs](http
+000026f0: 733a 2f2f 6c69 6768 746e 696e 672e 6169  s://lightning.ai
+00002700: 2f64 6f63 732f 6661 6272 6963 292e 0a31  /docs/fabric)..1
+00002710: 2e20 5b41 736b 2061 2071 7565 7374 696f  . [Ask a questio
+00002720: 6e20 696e 206f 7572 2066 6f72 756d 5d28  n in our forum](
+00002730: 6874 7470 733a 2f2f 6c69 6768 746e 696e  https://lightnin
+00002740: 672e 6169 2f66 6f72 756d 732f 292e 0a31  g.ai/forums/)..1
+00002750: 2e20 5b4a 6f69 6e20 6f75 7220 6469 7363  . [Join our disc
+00002760: 6f72 6420 636f 6d6d 756e 6974 795d 2868  ord community](h
+00002770: 7474 7073 3a2f 2f64 6973 636f 7264 2e63  ttps://discord.c
+00002780: 6f6d 2f69 6e76 6974 652f 7466 5846 6574  om/invite/tfXFet
+00002790: 455a 7876 292e 0a                        EZxv)..
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/__setup__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/__setup__.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 def _prepare_extras() -> Dict[str, Any]:
     assistant = _load_assistant()
     # https://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-extras
     # Define package extras. These are only installed if you specify them.
     # From remote, use like `pip install pytorch-lightning[dev, docs]`
     # From local copy of repo, use like `pip install ".[dev, docs]"`
-    common_args = dict(path_dir=_PATH_REQUIREMENTS, unfreeze="none" if _FREEZE_REQUIREMENTS else "all")
+    common_args = {"path_dir": _PATH_REQUIREMENTS, "unfreeze": "none" if _FREEZE_REQUIREMENTS else "all"}
     req_files = [Path(p) for p in glob.glob(os.path.join(_PATH_REQUIREMENTS, "*.txt"))]
     extras = {
         p.stem: assistant.load_requirements(file_name=p.name, **common_args)
         for p in req_files
         if p.name not in ("docs.txt", "devel.txt", "base.txt")
     }
     for req in parse_requirements(extras["strategies"]):
@@ -53,42 +53,42 @@
     assistant = _load_assistant()
     about = _load_py_module("about", os.path.join(_PACKAGE_ROOT, "__about__.py"))
     version = _load_py_module("version", os.path.join(_PACKAGE_ROOT, "__version__.py"))
     long_description = assistant.load_readme_description(
         _PACKAGE_ROOT, homepage=about.__homepage__, version=version.version
     )
 
-    return dict(
-        name="lightning-fabric",
-        version=version.version,
-        description=about.__docs__,
-        author=about.__author__,
-        author_email=about.__author_email__,
-        url=about.__homepage__,
-        download_url="https://github.com/Lightning-AI/lightning",
-        license=about.__license__,
-        packages=find_packages(where="src", include=["lightning_fabric", "lightning_fabric.*"]),
-        package_dir={"": "src"},
-        long_description=long_description,
-        long_description_content_type="text/markdown",
-        include_package_data=True,
-        zip_safe=False,
-        keywords=["deep learning", "pytorch", "AI"],
-        python_requires=">=3.8",
-        setup_requires=["wheel"],
-        install_requires=assistant.load_requirements(
+    return {
+        "name": "lightning-fabric",
+        "version": version.version,
+        "description": about.__docs__,
+        "author": about.__author__,
+        "author_email": about.__author_email__,
+        "url": about.__homepage__,
+        "download_url": "https://github.com/Lightning-AI/lightning",
+        "license": about.__license__,
+        "packages": find_packages(where="src", include=["lightning_fabric", "lightning_fabric.*"]),
+        "package_dir": {"": "src"},
+        "long_description": long_description,
+        "long_description_content_type": "text/markdown",
+        "include_package_data": True,
+        "zip_safe": False,
+        "keywords": ["deep learning", "pytorch", "AI"],
+        "python_requires": ">=3.8",
+        "setup_requires": ["wheel"],
+        "install_requires": assistant.load_requirements(
             _PATH_REQUIREMENTS, unfreeze="none" if _FREEZE_REQUIREMENTS else "all"
         ),
-        extras_require=_prepare_extras(),
-        project_urls={
+        "extras_require": _prepare_extras(),
+        "project_urls": {
             "Bug Tracker": "https://github.com/Lightning-AI/lightning/issues",
             "Documentation": "https://pytorch-lightning.rtfd.io/en/latest/",
             "Source Code": "https://github.com/Lightning-AI/lightning",
         },
-        classifiers=[
+        "classifiers": [
             "Environment :: Console",
             "Natural Language :: English",
             # How mature is this project? Common values are
             #   3 - Alpha, 4 - Beta, 5 - Production/Stable
             "Development Status :: 4 - Beta",
             # Indicate who your project is intended for
             "Intended Audience :: Developers",
@@ -100,8 +100,8 @@
             # Specify the Python versions you support here. In particular, ensure
             # that you indicate whether you support Python 2, Python 3 or both.
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
         ],
-    )
+    }
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/accelerator.py` & `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cpu.py` & `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/cuda.py` & `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/mps.py` & `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/registry.py` & `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/accelerators/tpu.py` & `lightning-fabric-2.0.2/src/lightning_fabric/accelerators/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/cli.py` & `lightning-fabric-2.0.2/src/lightning_fabric/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
 
 if _CLICK_AVAILABLE:
     import click
 
     @click.command(
         "model",
-        context_settings=dict(
-            ignore_unknown_options=True,
-        ),
+        context_settings={
+            "ignore_unknown_options": True,
+        },
     )
     @click.argument(
         "script",
         type=click.Path(exists=True),
     )
     @click.option(
         "--accelerator",
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/connector.py` & `lightning-fabric-2.0.2/src/lightning_fabric/connector.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/fabric.py` & `lightning-fabric-2.0.2/src/lightning_fabric/fabric.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,27 +200,27 @@
             )
         else:
             module = self._strategy.setup_module(module)
 
         module = _FabricModule(module, self._precision, original_module=original_module)
 
         # Update the _DeviceDtypeModuleMixin's device parameter
-        module.to(self.device if move_to_device else next(module.parameters()).device)
+        module.to(self.device if move_to_device else next(module.parameters(), torch.tensor(0)).device)
 
         optimizers = [_FabricOptimizer(optimizer=optimizer, strategy=self._strategy) for optimizer in optimizers]
 
         self._models_setup += 1
 
         if hasattr(original_module, "_fabric"):  # this is probably a LightningModule
             original_module._fabric = self  # type: ignore[assignment]
             original_module._fabric_optimizers = optimizers  # type: ignore[assignment]
 
         if optimizers:
             # join both types in a tuple for API convenience
-            return tuple((module, *optimizers))
+            return (module, *optimizers)
         return module
 
     def setup_module(self, module: nn.Module, move_to_device: bool = True) -> _FabricModule:
         """Set up a model for accelerated training or inference.
 
         This is the same as calling ``.setup(model)`` with no optimizers. It is useful for inference or for certain
         strategies like `FSDP` that require setting up the module before the optimizer can be created and set up.
@@ -244,15 +244,15 @@
 
         # Let strategy wrap and connect the module alone
         module = self._strategy.setup_module(module)
         module = _FabricModule(module, self._precision, original_module=original_module)
 
         if not isinstance(self._strategy, FSDPStrategy):
             # Update the _DeviceDtypeModuleMixin's device parameter
-            module.to(self.device if move_to_device else next(module.parameters()).device)
+            module.to(self.device if move_to_device else next(module.parameters(), torch.tensor(0)).device)
 
         if hasattr(original_module, "_fabric"):  # this is probably a LightningModule
             original_module._fabric = self  # type: ignore[assignment]
 
         self._models_setup += 1
         return module
 
@@ -737,15 +737,15 @@
         # apply sharded context to prevent OOM
         with self.sharded_model(), _replace_dunder_methods(DataLoader, "dataset"), _replace_dunder_methods(
             BatchSampler
         ):
             return run_function(*args, **kwargs)
 
     def _move_model_to_device(self, model: nn.Module, optimizers: List[Optimizer]) -> nn.Module:
-        initial_device = next(model.parameters()).device
+        initial_device = next(model.parameters(), torch.tensor(0)).device
         if any(param.device != initial_device for param in model.parameters()):
             rank_zero_warn(
                 "The model passed to `Fabric.setup()` has parameters on different devices. Since `move_to_device=True`,"
                 " all parameters will be moved to the new device. If this is not desired, set "
                 " `Fabric.setup(..., move_to_device=False)`.",
                 category=PossibleUserWarning,
             )
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/csv_logs.py` & `lightning-fabric-2.0.2/src/lightning_fabric/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/logger.py` & `lightning-fabric-2.0.2/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/loggers/tensorboard.py` & `lightning-fabric-2.0.2/src/lightning_fabric/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/collective.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/single_device.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/collectives/torch_collective.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/cluster_environment.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/kubeflow.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lightning.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/lsf.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/mpi.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/slurm.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/torchelastic.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/environments/xla.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/checkpoint_io.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/torch_io.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/io/xla.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/amp.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/deepspeed.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/double.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/fsdp.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/precision.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/tpu_bf16.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/tpu_bf16.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/plugins/precision/utils.py` & `lightning-fabric-2.0.2/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/ddp.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/ddp.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     @property
     def num_processes(self) -> int:
         return len(self.parallel_devices) if self.parallel_devices is not None else 0
 
     @property
     def distributed_sampler_kwargs(self) -> Dict[str, Any]:
-        return dict(num_replicas=(self.num_nodes * self.num_processes), rank=self.global_rank)
+        return {"num_replicas": (self.num_nodes * self.num_processes), "rank": self.global_rank}
 
     @property
     def process_group_backend(self) -> Optional[str]:
         return self._process_group_backend
 
     def _configure_launcher(self) -> None:
         assert self.cluster_environment is not None
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/deepspeed.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/deepspeed.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
     def zero_stage_3(self) -> bool:
         assert isinstance(self.config, dict)
         zero_optimization = self.config.get("zero_optimization")
         return zero_optimization is not None and zero_optimization.get("stage") == 3
 
     @property
     def distributed_sampler_kwargs(self) -> Dict[str, int]:
-        return dict(num_replicas=self.world_size, rank=self.global_rank)
+        return {"num_replicas": self.world_size, "rank": self.global_rank}
 
     @property
     def model(self) -> "deepspeed.DeepSpeedEngine":
         return self._deepspeed_engine
 
     def setup_module_and_optimizers(
         self, module: Module, optimizers: List[Optimizer]
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/dp.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/fsdp.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/fsdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     @property
     def num_processes(self) -> int:
         return len(self.parallel_devices) if self.parallel_devices is not None else 0
 
     @property
     def distributed_sampler_kwargs(self) -> Dict[str, Any]:
-        return dict(num_replicas=(self.num_nodes * self.num_processes), rank=self.global_rank)
+        return {"num_replicas": (self.num_nodes * self.num_processes), "rank": self.global_rank}
 
     @property
     def process_group_backend(self) -> Optional[str]:
         return self._process_group_backend
 
     @property
     def mixed_precision_config(self) -> Optional["MixedPrecision"]:
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/base.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/base.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/launcher.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/launchers/xla.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/parallel.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/registry.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_device.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/single_tpu.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/single_tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/strategy.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/strategies/xla.py` & `lightning-fabric-2.0.2/src/lightning_fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/__init__.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/apply_func.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/cloud_io.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/data.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
             f" can be passed to its parent's `{argument}=...` `__init__` argument. This is likely caused by allowing"
             f" passing both a custom argument that will map to the `{argument}` argument as well as `**kwargs`."
             f" `kwargs` should be filtered to make sure they don't contain the `{argument}` key."
             " This argument was automatically passed to your object by PyTorch Lightning."
         )
         raise MisconfigurationException(message) from e
 
-    attrs_record = getattr(orig_object, "__pl_attrs_record", list())
+    attrs_record = getattr(orig_object, "__pl_attrs_record", [])
     for args, fn in attrs_record:
         fn(result, *args)
 
     return result
 
 
 def _wrap_init_method(init: Callable, store_explicit_arg: Optional[str] = None) -> Callable:
@@ -349,15 +349,15 @@
         object.__setattr__(obj, "__pl_current_call", (name, tag))
 
         # call original method
         method(obj, *args)
         if first_call and not getattr(obj, "__pl_inside_init", True):
             # and save the value it was called with to the internal list,
             # if we're outside of __init__ and the original call did not fail and we're the first call
-            attrs_record = getattr(obj, "__pl_attrs_record", list())
+            attrs_record = getattr(obj, "__pl_attrs_record", [])
             attrs_record.append((args, tag))
             object.__setattr__(obj, "__pl_attrs_record", attrs_record)
         object.__setattr__(obj, "__pl_current_call", (prev_call_name, prev_call_method))
 
     return wrapper
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_dtype_mixin.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/device_parser.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/distributed.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/enums.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/exceptions.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/imports.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/logger.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/optimizer.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/rank_zero.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/registry.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/seed.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/types.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/utilities/warnings.py` & `lightning-fabric-2.0.2/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric/wrappers.py` & `lightning-fabric-2.0.2/src/lightning_fabric/wrappers.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
 from typing import Any, Callable, Dict, Generator, Iterator, Mapping, Optional, overload, TypeVar, Union
 
 import torch
+from lightning_utilities import WarningCache
 from lightning_utilities.core.apply_func import apply_to_collection
 from torch import nn as nn
 from torch import Tensor
 from torch.nn.modules.module import _IncompatibleKeys
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 
 from lightning_fabric.plugins import Precision
 from lightning_fabric.strategies import Strategy
 from lightning_fabric.utilities import move_data_to_device
 from lightning_fabric.utilities.data import _set_sampler_epoch
 from lightning_fabric.utilities.device_dtype_mixin import _DeviceDtypeModuleMixin
 from lightning_fabric.utilities.types import Optimizable
+from lightning_fabric.utilities.warnings import PossibleUserWarning
 
+warning_cache = WarningCache()
 T_destination = TypeVar("T_destination", bound=Dict[str, Any])
+_LIGHTNING_MODULE_STEP_METHODS = ("training_step", "validation_step", "test_step", "predict_step")
 
 
 class _FabricOptimizer:
     def __init__(self, optimizer: Optimizer, strategy: Strategy) -> None:
         """FabricOptimizer is a thin wrapper around the :class:`~torch.optim.Optimizer` that delegates the
         optimizer step calls to the strategy plugin.
 
@@ -56,15 +60,15 @@
     def optimizer(self) -> Optimizer:
         return self._optimizer
 
     def state_dict(self) -> Dict[str, Tensor]:
         return self._strategy.get_optimizer_state(self.optimizer)
 
     def step(self, closure: Optional[Callable] = None) -> Any:
-        kwargs = dict(closure=closure) if closure is not None else {}
+        kwargs = {"closure": closure} if closure is not None else {}
         if hasattr(self._strategy, "model") and isinstance(self._strategy.model, Optimizable):
             # only DeepSpeed defines this
             optimizer = self._strategy.model
         else:
             optimizer = self.optimizer
         return self._strategy.optimizer_step(
             optimizer,
@@ -128,23 +132,60 @@
             prefix=prefix,
             keep_vars=keep_vars,
         )
 
     def load_state_dict(self, state_dict: Mapping[str, Any], strict: bool = True) -> _IncompatibleKeys:
         return self._original_module.load_state_dict(state_dict=state_dict, strict=strict)
 
+    def _redirection_through_forward(self, method_name: str) -> Callable:
+        assert method_name != "forward"
+        original_forward = self._original_module.forward
+
+        def wrapped_forward(*args: Any, **kwargs: Any) -> Any:
+            # Unpatch ourselves immediately before calling the method `method_name`
+            # because itself may want to call the real `forward`
+            self._original_module.forward = original_forward
+            # Call the actual method e.g. `.training_step(...)`
+            method = getattr(self._original_module, method_name)
+            return method(*args, **kwargs)
+
+        # We make the caller "unknowingly" send their arguments through the forward_module's `__call__`.
+        # We expect that the `forward_module` will eventually call `original_module.forward`, which we
+        # have patched to redirect back to `original_module.method_name()`.
+        def call_forward_module(*args: Any, **kwargs: Any) -> Any:
+            # Patch the original_module's forward so we can redirect the arguments back to the real method
+            self._original_module.forward = wrapped_forward
+            return self.forward(*args, **kwargs)
+
+        return call_forward_module
+
+    def _validate_method_access(self, name: str, attribute: Any) -> None:
+        if inspect.ismethod(attribute) and self._forward_module != self._original_module:
+            warning_cache.warn(
+                f"You are calling the method `{type(self._original_module).__name__}.{name}()` from outside the"
+                " model. This will bypass the wrapper from the strategy and result in incorrect behavior in"
+                f" `.backward()`. You should pass your inputs through `{type(self._original_module)}.forward()`.",
+                category=PossibleUserWarning,
+            )
+
     def __getattr__(self, item: Any) -> Any:
+        if item in _LIGHTNING_MODULE_STEP_METHODS and self._forward_module != self._original_module:
+            # Special support for `LightningModule`, to prevent bypassing DDP's forward
+            return self._redirection_through_forward(item)
+
         try:
             # __getattr__ gets called as a last resort if the attribute does not exist
             # call nn.Module's implementation first
             return super().__getattr__(item)
         except AttributeError:
             # If the attribute is not available on the _FabricModule wrapper, redirect to the wrapped nn.Module
             original_module = super().__getattr__("_original_module")
-            return getattr(original_module, item)
+            attr = getattr(original_module, item)
+            self._validate_method_access(item, attr)
+            return attr
 
 
 class _FabricDataLoader:
     def __init__(self, dataloader: DataLoader, device: Optional[torch.device] = None) -> None:
         """The FabricDataLoader is a wrapper for the :class:`~torch.utils.data.DataLoader`. It moves the data to
         the device automatically if the device is specified.
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/PKG-INFO` & `lightning-fabric-2.0.2/src/lightning_fabric.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,518 +1,716 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c69 6768  : 2.1.Name: ligh
 00000020: 746e 696e 672d 6661 6272 6963 0a56 6572  tning-fabric.Ver
-00000030: 7369 6f6e 3a20 322e 302e 312e 706f 7374  sion: 2.0.1.post
-00000040: 300a 5375 6d6d 6172 793a 2055 4e4b 4e4f  0.Summary: UNKNO
-00000050: 574e 0a48 6f6d 652d 7061 6765 3a20 6874  WN.Home-page: ht
-00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000070: 2f4c 6967 6874 6e69 6e67 2d41 492f 6c69  /Lightning-AI/li
-00000080: 6768 746e 696e 670a 4175 7468 6f72 3a20  ghtning.Author: 
-00000090: 4c69 6768 746e 696e 6720 4149 2065 7420  Lightning AI et 
-000000a0: 616c 2e0a 4175 7468 6f72 2d65 6d61 696c  al..Author-email
-000000b0: 3a20 7079 746f 7263 6840 6c69 6768 746e  : pytorch@lightn
-000000c0: 696e 672e 6169 0a4c 6963 656e 7365 3a20  ing.ai.License: 
-000000d0: 4170 6163 6865 2d32 2e30 0a44 6f77 6e6c  Apache-2.0.Downl
-000000e0: 6f61 642d 5552 4c3a 2068 7474 7073 3a2f  oad-URL: https:/
-000000f0: 2f67 6974 6875 622e 636f 6d2f 4c69 6768  /github.com/Ligh
-00000100: 746e 696e 672d 4149 2f6c 6967 6874 6e69  tning-AI/lightni
-00000110: 6e67 0a50 726f 6a65 6374 2d55 524c 3a20  ng.Project-URL: 
-00000120: 4275 6720 5472 6163 6b65 722c 2068 7474  Bug Tracker, htt
-00000130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000140: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
-00000150: 6874 6e69 6e67 2f69 7373 7565 730a 5072  htning/issues.Pr
-00000160: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-00000170: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-00000180: 2f2f 7079 746f 7263 682d 6c69 6768 746e  //pytorch-lightn
-00000190: 696e 672e 7274 6664 2e69 6f2f 656e 2f6c  ing.rtfd.io/en/l
-000001a0: 6174 6573 742f 0a50 726f 6a65 6374 2d55  atest/.Project-U
-000001b0: 524c 3a20 536f 7572 6365 2043 6f64 652c  RL: Source Code,
-000001c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001d0: 636f 6d2f 4c69 6768 746e 696e 672d 4149  com/Lightning-AI
-000001e0: 2f6c 6967 6874 6e69 6e67 0a4b 6579 776f  /lightning.Keywo
-000001f0: 7264 733a 2064 6565 7020 6c65 6172 6e69  rds: deep learni
-00000200: 6e67 2c70 7974 6f72 6368 2c41 490a 506c  ng,pytorch,AI.Pl
-00000210: 6174 666f 726d 3a20 554e 4b4e 4f57 4e0a  atform: UNKNOWN.
-00000220: 436c 6173 7369 6669 6572 3a20 456e 7669  Classifier: Envi
-00000230: 726f 6e6d 656e 7420 3a3a 2043 6f6e 736f  ronment :: Conso
-00000240: 6c65 0a43 6c61 7373 6966 6965 723a 204e  le.Classifier: N
-00000250: 6174 7572 616c 204c 616e 6775 6167 6520  atural Language 
-00000260: 3a3a 2045 6e67 6c69 7368 0a43 6c61 7373  :: English.Class
-00000270: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
-00000280: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
-00000290: 2042 6574 610a 436c 6173 7369 6669 6572   Beta.Classifier
-000002a0: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-000002b0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
-000002c0: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-000002d0: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-000002e0: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
-000002f0: 2041 7274 6966 6963 6961 6c20 496e 7465   Artificial Inte
-00000300: 6c6c 6967 656e 6365 0a43 6c61 7373 6966  lligence.Classif
-00000310: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
-00000320: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000330: 7269 6e67 203a 3a20 496e 666f 726d 6174  ring :: Informat
-00000340: 696f 6e20 416e 616c 7973 6973 0a43 6c61  ion Analysis.Cla
-00000350: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-00000360: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000370: 496e 6465 7065 6e64 656e 740a 436c 6173  Independent.Clas
-00000380: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000390: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003a0: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
-000003b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000003c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003d0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
-000003e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000003f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000400: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-00000410: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000420: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000430: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000440: 3130 0a52 6571 7569 7265 732d 5079 7468  10.Requires-Pyth
-00000450: 6f6e 3a20 3e3d 332e 380a 4465 7363 7269  on: >=3.8.Descri
-00000460: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000470: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000480: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
-00000490: 3a20 6578 616d 706c 6573 0a50 726f 7669  : examples.Provi
-000004a0: 6465 732d 4578 7472 613a 2074 6573 740a  des-Extra: test.
-000004b0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000004c0: 7374 7261 7465 6769 6573 0a50 726f 7669  strategies.Provi
-000004d0: 6465 732d 4578 7472 613a 2064 6565 7073  des-Extra: deeps
-000004e0: 7065 6564 0a50 726f 7669 6465 732d 4578  peed.Provides-Ex
-000004f0: 7472 613a 2061 6c6c 0a50 726f 7669 6465  tra: all.Provide
-00000500: 732d 4578 7472 613a 2064 6576 0a4c 6963  s-Extra: dev.Lic
-00000510: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000520: 5345 0a0a 3c64 6976 2061 6c69 676e 3d22  SE..<div align="
-00000530: 6365 6e74 6572 223e 0a0a 3c69 6d67 2073  center">..<img s
-00000540: 7263 3d22 6874 7470 733a 2f2f 706c 2d70  rc="https://pl-p
-00000550: 7562 6c69 632d 6461 7461 2e73 332e 616d  ublic-data.s3.am
-00000560: 617a 6f6e 6177 732e 636f 6d2f 6173 7365  azonaws.com/asse
-00000570: 7473 5f6c 6967 6874 6e69 6e67 2f66 6162  ts_lightning/fab
-00000580: 7269 635f 6c6f 676f 2e70 6e67 2220 7769  ric_logo.png" wi
-00000590: 6474 683d 2234 3030 7078 223e 0a0a 2a2a  dth="400px">..**
-000005a0: 4661 6272 6963 2069 7320 7468 6520 6661  Fabric is the fa
-000005b0: 7374 2061 6e64 206c 6967 6874 7765 6967  st and lightweig
-000005c0: 6874 2077 6179 2074 6f20 7363 616c 6520  ht way to scale 
-000005d0: 5079 546f 7263 6820 6d6f 6465 6c73 2077  PyTorch models w
-000005e0: 6974 686f 7574 2062 6f69 6c65 7270 6c61  ithout boilerpla
-000005f0: 7465 2a2a 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f  te**..__________
+00000030: 7369 6f6e 3a20 322e 302e 320a 5375 6d6d  sion: 2.0.2.Summ
+00000040: 6172 793a 2055 4e4b 4e4f 574e 0a48 6f6d  ary: UNKNOWN.Hom
+00000050: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000060: 6769 7468 7562 2e63 6f6d 2f4c 6967 6874  github.com/Light
+00000070: 6e69 6e67 2d41 492f 6c69 6768 746e 696e  ning-AI/lightnin
+00000080: 670a 4175 7468 6f72 3a20 4c69 6768 746e  g.Author: Lightn
+00000090: 696e 6720 4149 2065 7420 616c 2e0a 4175  ing AI et al..Au
+000000a0: 7468 6f72 2d65 6d61 696c 3a20 7079 746f  thor-email: pyto
+000000b0: 7263 6840 6c69 6768 746e 696e 672e 6169  rch@lightning.ai
+000000c0: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
+000000d0: 2d32 2e30 0a44 6f77 6e6c 6f61 642d 5552  -2.0.Download-UR
+000000e0: 4c3a 2068 7474 7073 3a2f 2f67 6974 6875  L: https://githu
+000000f0: 622e 636f 6d2f 4c69 6768 746e 696e 672d  b.com/Lightning-
+00000100: 4149 2f6c 6967 6874 6e69 6e67 0a50 726f  AI/lightning.Pro
+00000110: 6a65 6374 2d55 524c 3a20 4275 6720 5472  ject-URL: Bug Tr
+00000120: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
+00000130: 6974 6875 622e 636f 6d2f 4c69 6768 746e  ithub.com/Lightn
+00000140: 696e 672d 4149 2f6c 6967 6874 6e69 6e67  ing-AI/lightning
+00000150: 2f69 7373 7565 730a 5072 6f6a 6563 742d  /issues.Project-
+00000160: 5552 4c3a 2044 6f63 756d 656e 7461 7469  URL: Documentati
+00000170: 6f6e 2c20 6874 7470 733a 2f2f 7079 746f  on, https://pyto
+00000180: 7263 682d 6c69 6768 746e 696e 672e 7274  rch-lightning.rt
+00000190: 6664 2e69 6f2f 656e 2f6c 6174 6573 742f  fd.io/en/latest/
+000001a0: 0a50 726f 6a65 6374 2d55 524c 3a20 536f  .Project-URL: So
+000001b0: 7572 6365 2043 6f64 652c 2068 7474 7073  urce Code, https
+000001c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c69  ://github.com/Li
+000001d0: 6768 746e 696e 672d 4149 2f6c 6967 6874  ghtning-AI/light
+000001e0: 6e69 6e67 0a4b 6579 776f 7264 733a 2064  ning.Keywords: d
+000001f0: 6565 7020 6c65 6172 6e69 6e67 2c70 7974  eep learning,pyt
+00000200: 6f72 6368 2c41 490a 506c 6174 666f 726d  orch,AI.Platform
+00000210: 3a20 554e 4b4e 4f57 4e0a 436c 6173 7369  : UNKNOWN.Classi
+00000220: 6669 6572 3a20 456e 7669 726f 6e6d 656e  fier: Environmen
+00000230: 7420 3a3a 2043 6f6e 736f 6c65 0a43 6c61  t :: Console.Cla
+00000240: 7373 6966 6965 723a 204e 6174 7572 616c  ssifier: Natural
+00000250: 204c 616e 6775 6167 6520 3a3a 2045 6e67   Language :: Eng
+00000260: 6c69 7368 0a43 6c61 7373 6966 6965 723a  lish.Classifier:
+00000270: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
+00000280: 7475 7320 3a3a 2034 202d 2042 6574 610a  tus :: 4 - Beta.
+00000290: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+000002a0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+000002b0: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
+000002c0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000002d0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+000002e0: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+000002f0: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+00000300: 6365 0a43 6c61 7373 6966 6965 723a 2054  ce.Classifier: T
+00000310: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
+00000320: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
+00000330: 3a20 496e 666f 726d 6174 696f 6e20 416e  : Information An
+00000340: 616c 7973 6973 0a43 6c61 7373 6966 6965  alysis.Classifie
+00000350: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+00000360: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000370: 6e64 656e 740a 436c 6173 7369 6669 6572  ndent.Classifier
+00000380: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000390: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000003a0: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+000003b0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000003c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000003d0: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+000003e0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000003f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000400: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
+00000410: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000420: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000430: 7468 6f6e 203a 3a20 332e 3130 0a52 6571  thon :: 3.10.Req
+00000440: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+00000450: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
+00000460: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000470: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
+00000480: 6964 6573 2d45 7874 7261 3a20 7374 7261  ides-Extra: stra
+00000490: 7465 6769 6573 0a50 726f 7669 6465 732d  tegies.Provides-
+000004a0: 4578 7472 613a 2074 6573 740a 5072 6f76  Extra: test.Prov
+000004b0: 6964 6573 2d45 7874 7261 3a20 6578 616d  ides-Extra: exam
+000004c0: 706c 6573 0a50 726f 7669 6465 732d 4578  ples.Provides-Ex
+000004d0: 7472 613a 2064 6565 7073 7065 6564 0a50  tra: deepspeed.P
+000004e0: 726f 7669 6465 732d 4578 7472 613a 2061  rovides-Extra: a
+000004f0: 6c6c 0a50 726f 7669 6465 732d 4578 7472  ll.Provides-Extr
+00000500: 613a 2064 6576 0a4c 6963 656e 7365 2d46  a: dev.License-F
+00000510: 696c 653a 204c 4943 454e 5345 0a0a 3c64  ile: LICENSE..<d
+00000520: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00000530: 223e 0a0a 3c69 6d67 2073 7263 3d22 6874  ">..<img src="ht
+00000540: 7470 733a 2f2f 706c 2d70 7562 6c69 632d  tps://pl-public-
+00000550: 6461 7461 2e73 332e 616d 617a 6f6e 6177  data.s3.amazonaw
+00000560: 732e 636f 6d2f 6173 7365 7473 5f6c 6967  s.com/assets_lig
+00000570: 6874 6e69 6e67 2f66 6162 7269 635f 6c6f  htning/fabric_lo
+00000580: 676f 2e70 6e67 2220 7769 6474 683d 2234  go.png" width="4
+00000590: 3030 7078 223e 0a0a 2a2a 4661 6272 6963  00px">..**Fabric
+000005a0: 2069 7320 7468 6520 6661 7374 2061 6e64   is the fast and
+000005b0: 206c 6967 6874 7765 6967 6874 2077 6179   lightweight way
+000005c0: 2074 6f20 7363 616c 6520 5079 546f 7263   to scale PyTorc
+000005d0: 6820 6d6f 6465 6c73 2077 6974 686f 7574  h models without
+000005e0: 2062 6f69 6c65 7270 6c61 7465 2a2a 0a0a   boilerplate**..
+000005f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000600: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000610: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00000620: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000630: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a 3c70  ____________..<p
-00000640: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000650: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00000660: 733a 2f2f 6c69 6768 746e 696e 672e 6169  s://lightning.ai
-00000670: 2f22 3e57 6562 7369 7465 3c2f 613e 20e2  /">Website</a> .
-00000680: 80a2 0a20 203c 6120 6872 6566 3d22 6874  ...  <a href="ht
-00000690: 7470 733a 2f2f 6c69 6768 746e 696e 672e  tps://lightning.
-000006a0: 6169 2f64 6f63 732f 6661 6272 6963 2f22  ai/docs/fabric/"
-000006b0: 3e44 6f63 733c 2f61 3e20 e280 a20a 2020  >Docs</a> ....  
-000006c0: 3c61 2068 7265 663d 2223 6765 7474 696e  <a href="#gettin
-000006d0: 672d 7374 6172 7465 6422 3e47 6574 7469  g-started">Getti
-000006e0: 6e67 2073 7461 7274 6564 3c2f 613e 20e2  ng started</a> .
-000006f0: 80a2 0a20 203c 6120 6872 6566 3d22 2366  ...  <a href="#f
-00000700: 6171 223e 4641 513c 2f61 3e20 e280 a20a  aq">FAQ</a> ....
-00000710: 2020 3c61 2068 7265 663d 2223 6173 6b69    <a href="#aski
-00000720: 6e67 2d66 6f72 2d68 656c 7022 3e48 656c  ng-for-help">Hel
-00000730: 703c 2f61 3e20 e280 a20a 2020 3c61 2068  p</a> ....  <a h
-00000740: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
-00000750: 636f 7264 2e67 672f 5670 7450 435a 6b47  cord.gg/VptPCZkG
-00000760: 4e61 223e 4469 7363 6f72 643c 2f61 3e0a  Na">Discord</a>.
-00000770: 3c2f 703e 0a0a 5b21 5b50 7950 4920 2d20  </p>..[![PyPI - 
-00000780: 5079 7468 6f6e 2056 6572 7369 6f6e 5d28  Python Version](
-00000790: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000007a0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
-000007b0: 7273 696f 6e73 2f6c 6967 6874 6e69 6e67  rsions/lightning
-000007c0: 5f66 6162 7269 6329 5d28 6874 7470 733a  _fabric)](https:
-000007d0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000007e0: 6374 2f6c 6967 6874 6e69 6e67 5f66 6162  ct/lightning_fab
-000007f0: 7269 632f 290a 5b21 5b50 7950 4920 5374  ric/).[![PyPI St
-00000800: 6174 7573 5d28 6874 7470 733a 2f2f 6261  atus](https://ba
-00000810: 6467 652e 6675 7279 2e69 6f2f 7079 2f6c  dge.fury.io/py/l
-00000820: 6967 6874 6e69 6e67 5f66 6162 7269 632e  ightning_fabric.
-00000830: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
-00000840: 6467 652e 6675 7279 2e69 6f2f 7079 2f6c  dge.fury.io/py/l
-00000850: 6967 6874 6e69 6e67 5f66 6162 7269 6329  ightning_fabric)
-00000860: 0a5b 215b 5079 5049 2053 7461 7475 735d  .[![PyPI Status]
-00000870: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-00000880: 6368 2f62 6164 6765 2f6c 6967 6874 6e69  ch/badge/lightni
-00000890: 6e67 5f66 6162 7269 6329 5d28 6874 7470  ng_fabric)](http
-000008a0: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
-000008b0: 6f6a 6563 742f 6c69 6768 746e 696e 675f  oject/lightning_
-000008c0: 6661 6272 6963 290a 5b21 5b43 6f6e 6461  fabric).[![Conda
-000008d0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000008e0: 6965 6c64 732e 696f 2f63 6f6e 6461 2f76  ields.io/conda/v
-000008f0: 2f63 6f6e 6461 2d66 6f72 6765 2f6c 6967  /conda-forge/lig
-00000900: 6874 6e69 6e67 5f66 6162 7269 633f 6c61  htning_fabric?la
-00000910: 6265 6c3d 636f 6e64 6126 636f 6c6f 723d  bel=conda&color=
-00000920: 7375 6363 6573 7329 5d28 6874 7470 733a  success)](https:
-00000930: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
-00000940: 6f6e 6461 2d66 6f72 6765 2f6c 6967 6874  onda-forge/light
-00000950: 6e69 6e67 5f66 6162 7269 6329 0a0a 3c2f  ning_fabric)..</
-00000960: 6469 763e 0a0a 2323 204d 6178 696d 756d  div>..## Maximum
-00000970: 2066 6c65 7869 6269 6c69 7479 2c20 6d69   flexibility, mi
-00000980: 6e69 6d75 6d20 636f 6465 2063 6861 6e67  nimum code chang
-00000990: 6573 0a0a 5769 7468 206a 7573 7420 6120  es..With just a 
-000009a0: 6665 7720 636f 6465 2063 6861 6e67 6573  few code changes
-000009b0: 2c20 7275 6e20 616e 7920 5079 546f 7263  , run any PyTorc
-000009c0: 6820 6d6f 6465 6c20 6f6e 2061 6e79 2064  h model on any d
-000009d0: 6973 7472 6962 7574 6564 2068 6172 6477  istributed hardw
-000009e0: 6172 652c 206e 6f20 626f 696c 6572 706c  are, no boilerpl
-000009f0: 6174 6521 0a0a 2d20 4561 7369 6c79 2073  ate!..- Easily s
-00000a00: 7769 7463 6820 6672 6f6d 2072 756e 6e69  witch from runni
-00000a10: 6e67 206f 6e20 4350 5520 746f 2047 5055  ng on CPU to GPU
-00000a20: 2028 4170 706c 6520 5369 6c69 636f 6e2c   (Apple Silicon,
-00000a30: 2043 5544 412c 20e2 80a6 292c 2054 5055   CUDA, ...), TPU
-00000a40: 2c20 6d75 6c74 692d 4750 5520 6f72 2065  , multi-GPU or e
-00000a50: 7665 6e20 6d75 6c74 692d 6e6f 6465 2074  ven multi-node t
-00000a60: 7261 696e 696e 670a 2d20 5573 6520 7374  raining.- Use st
-00000a70: 6174 652d 6f66 2d74 6865 2d61 7274 2064  ate-of-the-art d
-00000a80: 6973 7472 6962 7574 6564 2074 7261 696e  istributed train
-00000a90: 696e 6720 7374 7261 7465 6769 6573 2028  ing strategies (
-00000aa0: 4444 502c 2046 5344 502c 2044 6565 7053  DDP, FSDP, DeepS
-00000ab0: 7065 6564 2920 616e 6420 6d69 7865 6420  peed) and mixed 
-00000ac0: 7072 6563 6973 696f 6e20 6f75 7420 6f66  precision out of
-00000ad0: 2074 6865 2062 6f78 0a2d 2041 6c6c 2074   the box.- All t
-00000ae0: 6865 2064 6576 6963 6520 6c6f 6769 6320  he device logic 
-00000af0: 626f 696c 6572 706c 6174 6520 6973 2068  boilerplate is h
-00000b00: 616e 646c 6564 2066 6f72 2079 6f75 0a2d  andled for you.-
-00000b10: 2044 6573 6967 6e65 6420 7769 7468 206d   Designed with m
-00000b20: 756c 7469 2d62 696c 6c69 6f6e 2070 6172  ulti-billion par
-00000b30: 616d 6574 6572 206d 6f64 656c 7320 696e  ameter models in
-00000b40: 206d 696e 640a 2d20 4275 696c 6420 796f   mind.- Build yo
-00000b50: 7572 206f 776e 2063 7573 746f 6d20 5472  ur own custom Tr
-00000b60: 6169 6e65 7220 7573 696e 6720 4661 6272  ainer using Fabr
-00000b70: 6963 2070 7269 6d69 7469 7665 7320 666f  ic primitives fo
-00000b80: 7220 7472 6169 6e69 6e67 2063 6865 636b  r training check
-00000b90: 706f 696e 7469 6e67 2c20 6c6f 6767 696e  pointing, loggin
-00000ba0: 672c 2061 6e64 206d 6f72 650a 0a60 6060  g, and more..```
-00000bb0: 6469 6666 0a2b 2069 6d70 6f72 7420 6c69  diff.+ import li
-00000bc0: 6768 746e 696e 6720 6173 204c 0a0a 2020  ghtning as L..  
-00000bd0: 696d 706f 7274 2074 6f72 6368 0a20 2069  import torch.  i
-00000be0: 6d70 6f72 7420 746f 7263 682e 6e6e 2061  mport torch.nn a
-00000bf0: 7320 6e6e 0a20 2066 726f 6d20 746f 7263  s nn.  from torc
-00000c00: 682e 7574 696c 732e 6461 7461 2069 6d70  h.utils.data imp
-00000c10: 6f72 7420 4461 7461 4c6f 6164 6572 2c20  ort DataLoader, 
-00000c20: 4461 7461 7365 740a 0a20 2063 6c61 7373  Dataset..  class
-00000c30: 2050 7954 6f72 6368 4d6f 6465 6c28 6e6e   PyTorchModel(nn
-00000c40: 2e4d 6f64 756c 6529 3a0a 2020 2020 2020  .Module):.      
-00000c50: 2e2e 2e0a 0a20 2063 6c61 7373 2050 7954  .....  class PyT
-00000c60: 6f72 6368 4461 7461 7365 7428 4461 7461  orchDataset(Data
-00000c70: 7365 7429 3a0a 2020 2020 2020 2e2e 2e0a  set):.      ....
-00000c80: 0a2b 2066 6162 7269 6320 3d20 4c2e 4661  .+ fabric = L.Fa
-00000c90: 6272 6963 2861 6363 656c 6572 6174 6f72  bric(accelerator
-00000ca0: 3d22 6375 6461 222c 2064 6576 6963 6573  ="cuda", devices
-00000cb0: 3d38 2c20 7374 7261 7465 6779 3d22 6464  =8, strategy="dd
-00000cc0: 7022 290a 2b20 6661 6272 6963 2e6c 6175  p").+ fabric.lau
-00000cd0: 6e63 6828 290a 0a2d 2064 6576 6963 6520  nch()..- device 
-00000ce0: 3d20 2263 7564 6122 2069 6620 746f 7263  = "cuda" if torc
-00000cf0: 682e 6375 6461 2e69 735f 6176 6169 6c61  h.cuda.is_availa
-00000d00: 626c 6528 2920 656c 7365 2022 6370 750a  ble() else "cpu.
-00000d10: 2020 6d6f 6465 6c20 3d20 5079 546f 7263    model = PyTorc
-00000d20: 684d 6f64 656c 282e 2e2e 290a 2020 6f70  hModel(...).  op
-00000d30: 7469 6d69 7a65 7220 3d20 746f 7263 682e  timizer = torch.
-00000d40: 6f70 7469 6d2e 5347 4428 6d6f 6465 6c2e  optim.SGD(model.
-00000d50: 7061 7261 6d65 7465 7273 2829 290a 2b20  parameters()).+ 
-00000d60: 6d6f 6465 6c2c 206f 7074 696d 697a 6572  model, optimizer
-00000d70: 203d 2066 6162 7269 632e 7365 7475 7028   = fabric.setup(
-00000d80: 6d6f 6465 6c2c 206f 7074 696d 697a 6572  model, optimizer
-00000d90: 290a 2020 6461 7461 6c6f 6164 6572 203d  ).  dataloader =
-00000da0: 2044 6174 614c 6f61 6465 7228 5079 546f   DataLoader(PyTo
-00000db0: 7263 6844 6174 6173 6574 282e 2e2e 292c  rchDataset(...),
-00000dc0: 202e 2e2e 290a 2b20 6461 7461 6c6f 6164   ...).+ dataload
-00000dd0: 6572 203d 2066 6162 7269 632e 7365 7475  er = fabric.setu
-00000de0: 705f 6461 7461 6c6f 6164 6572 7328 6461  p_dataloaders(da
-00000df0: 7461 6c6f 6164 6572 290a 2020 6d6f 6465  taloader).  mode
-00000e00: 6c2e 7472 6169 6e28 290a 0a20 2066 6f72  l.train()..  for
-00000e10: 2065 706f 6368 2069 6e20 7261 6e67 6528   epoch in range(
-00000e20: 6e75 6d5f 6570 6f63 6873 293a 0a20 2020  num_epochs):.   
-00000e30: 2020 2066 6f72 2062 6174 6368 2069 6e20     for batch in 
-00000e40: 6461 7461 6c6f 6164 6572 3a0a 2020 2020  dataloader:.    
-00000e50: 2020 2020 2020 696e 7075 742c 2074 6172        input, tar
-00000e60: 6765 7420 3d20 6261 7463 680a 2d20 2020  get = batch.-   
-00000e70: 2020 2020 2020 696e 7075 742c 2074 6172        input, tar
-00000e80: 6765 7420 3d20 696e 7075 742e 746f 2864  get = input.to(d
-00000e90: 6576 6963 6529 2c20 7461 7267 6574 2e74  evice), target.t
-00000ea0: 6f28 6465 7669 6365 290a 2020 2020 2020  o(device).      
-00000eb0: 2020 2020 6f70 7469 6d69 7a65 722e 7a65      optimizer.ze
-00000ec0: 726f 5f67 7261 6428 290a 2020 2020 2020  ro_grad().      
-00000ed0: 2020 2020 6f75 7470 7574 203d 206d 6f64      output = mod
-00000ee0: 656c 2869 6e70 7574 290a 2020 2020 2020  el(input).      
-00000ef0: 2020 2020 6c6f 7373 203d 206c 6f73 735f      loss = loss_
-00000f00: 666e 286f 7574 7075 742c 2074 6172 6765  fn(output, targe
-00000f10: 7429 0a2d 2020 2020 2020 2020 206c 6f73  t).-         los
-00000f20: 732e 6261 636b 7761 7264 2829 0a2b 2020  s.backward().+  
-00000f30: 2020 2020 2020 2066 6162 7269 632e 6261         fabric.ba
-00000f40: 636b 7761 7264 286c 6f73 7329 0a20 2020  ckward(loss).   
-00000f50: 2020 2020 2020 206f 7074 696d 697a 6572         optimizer
-00000f60: 2e73 7465 7028 290a 2020 2020 2020 2020  .step().        
-00000f70: 2020 6c72 5f73 6368 6564 756c 6572 2e73    lr_scheduler.s
-00000f80: 7465 7028 290a 6060 600a 0a5f 5f5f 5f5f  tep().```.._____
-00000f90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fa0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fb0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fc0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000fd0: 5f0a 0a23 2047 6574 7469 6e67 2073 7461  _..# Getting sta
-00000fe0: 7274 6564 0a0a 2323 2049 6e73 7461 6c6c  rted..## Install
-00000ff0: 204c 6967 6874 6e69 6e67 0a0a 3c64 6574   Lightning..<det
-00001000: 6169 6c73 3e0a 0a3c 7375 6d6d 6172 793e  ails>..<summary>
-00001010: 5072 6572 6571 7569 7369 7465 733c 2f73  Prerequisites</s
-00001020: 756d 6d61 7279 3e0a 0a3e 2054 4950 3a20  ummary>..> TIP: 
-00001030: 5765 2073 7472 6f6e 676c 7920 7265 636f  We strongly reco
-00001040: 6d6d 656e 6420 6372 6561 7469 6e67 2061  mmend creating a
-00001050: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
-00001060: 6d65 6e74 2066 6972 7374 2e0a 3e20 446f  ment first..> Do
-00001070: 6ee2 8099 7420 6b6e 6f77 2077 6861 7420  n...t know what 
-00001080: 7468 6973 2069 733f 2046 6f6c 6c6f 7720  this is? Follow 
-00001090: 6f75 7220 5b62 6567 696e 6e65 7220 6775  our [beginner gu
-000010a0: 6964 6520 6865 7265 5d28 6874 7470 733a  ide here](https:
-000010b0: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
-000010c0: 6f63 732f 7374 6162 6c65 2f69 6e73 7461  ocs/stable/insta
-000010d0: 6c6c 2f69 6e73 7461 6c6c 6174 696f 6e2e  ll/installation.
-000010e0: 6874 6d6c 292e 0a0a 2d20 5079 7468 6f6e  html)...- Python
-000010f0: 2033 2e38 2e78 206f 7220 6c61 7465 7220   3.8.x or later 
-00001100: 2833 2e38 2e78 2c20 332e 392e 782c 2033  (3.8.x, 3.9.x, 3
-00001110: 2e31 302e 782c 202e 2e2e 290a 0a3c 2f64  .10.x, ...)..</d
-00001120: 6574 6169 6c73 3e0a 0a60 6060 6261 7368  etails>..```bash
-00001130: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
-00001140: 6c69 6768 746e 696e 670a 6060 600a 0a23  lightning.```..#
-00001150: 2320 436f 6e76 6572 7420 796f 7572 2050  # Convert your P
-00001160: 7954 6f72 6368 2074 6f20 4661 6272 6963  yTorch to Fabric
-00001170: 0a0a 312e 2043 7265 6174 6520 7468 6520  ..1. Create the 
-00001180: 6046 6162 7269 6360 206f 626a 6563 7420  `Fabric` object 
-00001190: 6174 2074 6865 2062 6567 696e 6e69 6e67  at the beginning
-000011a0: 206f 6620 796f 7572 2074 7261 696e 696e   of your trainin
-000011b0: 6720 636f 6465 2e0a 0a20 2020 6060 600a  g code...   ```.
-000011c0: 2020 2069 6d70 6f72 7420 4c69 6768 746e     import Lightn
-000011d0: 696e 6720 6173 204c 0a0a 2020 2066 6162  ing as L..   fab
-000011e0: 7269 6320 3d20 4c2e 4661 6272 6963 2829  ric = L.Fabric()
-000011f0: 0a20 2020 6060 600a 0a31 2e20 4361 6c6c  .   ```..1. Call
-00001200: 2060 7365 7475 7028 2960 206f 6e20 6561   `setup()` on ea
-00001210: 6368 206d 6f64 656c 2061 6e64 206f 7074  ch model and opt
-00001220: 696d 697a 6572 2070 6169 7220 616e 6420  imizer pair and 
-00001230: 6073 6574 7570 5f64 6174 616c 6f61 6465  `setup_dataloade
-00001240: 7273 2829 6020 6f6e 2061 6c6c 2079 6f75  rs()` on all you
-00001250: 7220 6461 7461 206c 6f61 6465 7273 2e0a  r data loaders..
-00001260: 0a20 2020 6060 600a 2020 206d 6f64 656c  .   ```.   model
-00001270: 2c20 6f70 7469 6d69 7a65 7220 3d20 6661  , optimizer = fa
-00001280: 6272 6963 2e73 6574 7570 286d 6f64 656c  bric.setup(model
-00001290: 2c20 6f70 7469 6d69 7a65 7229 0a20 2020  , optimizer).   
-000012a0: 6461 7461 6c6f 6164 6572 203d 2066 6162  dataloader = fab
-000012b0: 7269 632e 7365 7475 705f 6461 7461 6c6f  ric.setup_datalo
-000012c0: 6164 6572 7328 6461 7461 6c6f 6164 6572  aders(dataloader
-000012d0: 290a 2020 2060 6060 0a0a 312e 2052 656d  ).   ```..1. Rem
-000012e0: 6f76 6520 616c 6c20 602e 746f 6020 616e  ove all `.to` an
-000012f0: 6420 602e 6375 6461 6020 6361 6c6c 7320  d `.cuda` calls 
-00001300: 2d3e 2046 6162 7269 6320 7769 6c6c 2074  -> Fabric will t
-00001310: 616b 6520 6361 7265 206f 6620 6974 2e0a  ake care of it..
-00001320: 0a20 2020 6060 6064 6966 660a 2020 202d  .   ```diff.   -
-00001330: 206d 6f64 656c 2e74 6f28 6465 7669 6365   model.to(device
-00001340: 290a 2020 202d 2062 6174 6368 2e74 6f28  ).   - batch.to(
-00001350: 6465 7669 6365 290a 2020 2060 6060 0a0a  device).   ```..
-00001360: 312e 2052 6570 6c61 6365 2060 6c6f 7373  1. Replace `loss
-00001370: 2e62 6163 6b77 6172 6428 2960 2062 7920  .backward()` by 
-00001380: 6066 6162 7269 632e 6261 636b 7761 7264  `fabric.backward
-00001390: 286c 6f73 7329 602e 0a0a 2020 2060 6060  (loss)`...   ```
-000013a0: 6469 6666 0a20 2020 2d20 6c6f 7373 2e62  diff.   - loss.b
-000013b0: 6163 6b77 6172 6428 290a 2020 202b 2066  ackward().   + f
-000013c0: 6162 7269 632e 6261 636b 7761 7264 286c  abric.backward(l
-000013d0: 6f73 7329 0a20 2020 6060 600a 0a31 2e20  oss).   ```..1. 
-000013e0: 5275 6e20 7468 6520 7363 7269 7074 2066  Run the script f
-000013f0: 726f 6d20 7468 6520 7465 726d 696e 616c  rom the terminal
-00001400: 2077 6974 680a 0a20 2020 6060 6062 6173   with..   ```bas
-00001410: 680a 2020 206c 6967 6874 6e69 6e67 2072  h.   lightning r
-00001420: 756e 206d 6f64 656c 2070 6174 682f 746f  un model path/to
-00001430: 2f74 7261 696e 2e70 790a 2020 2060 6060  /train.py.   ```
-00001440: 0a0a 6f72 2075 7365 2074 6865 206c 6175  ..or use the lau
-00001450: 6e63 6828 2920 6d65 7468 6f64 2069 6e20  nch() method in 
-00001460: 6120 6e6f 7465 626f 6f6b 2e20 4c65 6172  a notebook. Lear
-00001470: 6e20 6d6f 7265 2061 626f 7574 205b 6c61  n more about [la
-00001480: 756e 6368 696e 6720 6469 7374 7269 6275  unching distribu
-00001490: 7465 6420 7472 6169 6e69 6e67 5d28 6874  ted training](ht
-000014a0: 7470 733a 2f2f 6c69 6768 746e 696e 672e  tps://lightning.
-000014b0: 6169 2f64 6f63 732f 6661 6272 6963 2f73  ai/docs/fabric/s
-000014c0: 7461 626c 652f 6675 6e64 616d 656e 7461  table/fundamenta
-000014d0: 6c73 2f6c 6175 6e63 682e 6874 6d6c 292e  ls/launch.html).
-000014e0: 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ..______________
-000014f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001500: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001510: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001520: 5f5f 5f5f 5f5f 5f5f 0a0a 2320 4641 510a  ________..# FAQ.
-00001530: 0a23 2320 5768 656e 2074 6f20 7573 6520  .## When to use 
-00001540: 4661 6272 6963 3f0a 0a2d 202a 2a4d 696e  Fabric?..- **Min
-00001550: 696d 756d 2063 6f64 6520 6368 616e 6765  imum code change
-00001560: 732a 2a2d 2059 6f75 2077 616e 7420 746f  s**- You want to
-00001570: 2073 6361 6c65 2079 6f75 7220 5079 546f   scale your PyTo
-00001580: 7263 6820 6d6f 6465 6c20 746f 2075 7365  rch model to use
-00001590: 206d 756c 7469 2d47 5055 206f 7220 7573   multi-GPU or us
-000015a0: 6520 6164 7661 6e63 6564 2073 7472 6174  e advanced strat
-000015b0: 6567 6965 7320 6c69 6b65 2044 6565 7053  egies like DeepS
-000015c0: 7065 6564 2077 6974 686f 7574 2068 6176  peed without hav
-000015d0: 696e 6720 746f 2072 6566 6163 746f 722e  ing to refactor.
-000015e0: 2059 6f75 2064 6f6e e280 9974 2063 6172   You don...t car
-000015f0: 6520 6162 6f75 7420 7374 7275 6374 7572  e about structur
-00001600: 696e 6720 796f 7572 2063 6f64 652d 2079  ing your code- y
-00001610: 6f75 206a 7573 7420 7761 6e74 2074 6f20  ou just want to 
-00001620: 7363 616c 6520 6974 2061 7320 6661 7374  scale it as fast
-00001630: 2061 7320 706f 7373 6962 6c65 2e0a 2d20   as possible..- 
-00001640: 2a2a 4d61 786d 6975 6d20 636f 6e74 726f  **Maxmium contro
-00001650: 6c2a 2a2d 2057 7269 7465 2079 6f75 7220  l**- Write your 
-00001660: 6f77 6e20 7472 6169 6e69 6e67 2061 6e64  own training and
-00001670: 2f6f 7220 696e 6665 7265 6e63 6520 6c6f  /or inference lo
-00001680: 6769 6320 646f 776e 2074 6f20 7468 6520  gic down to the 
-00001690: 696e 6469 7669 6475 616c 206f 7074 696d  individual optim
-000016a0: 697a 6572 2063 616c 6c73 2e20 596f 7520  izer calls. You 
-000016b0: 6172 656e e280 9974 2066 6f72 6365 6420  aren...t forced 
-000016c0: 746f 2063 6f6e 666f 726d 2074 6f20 6120  to conform to a 
-000016d0: 7374 616e 6461 7264 697a 6564 2065 706f  standardized epo
-000016e0: 6368 2d62 6173 6564 2074 7261 696e 696e  ch-based trainin
-000016f0: 6720 6c6f 6f70 206c 696b 6520 7468 6520  g loop like the 
-00001700: 6f6e 6520 696e 204c 6967 6874 6e69 6e67  one in Lightning
-00001710: 2054 7261 696e 6572 2e20 596f 7520 6361   Trainer. You ca
-00001720: 6e20 646f 2066 6c65 7869 626c 6520 6974  n do flexible it
-00001730: 6572 6174 696f 6e20 6261 7365 6420 7472  eration based tr
-00001740: 6169 6e69 6e67 2c20 6d65 7461 2d6c 6561  aining, meta-lea
-00001750: 726e 696e 672c 2063 726f 7373 2d76 616c  rning, cross-val
-00001760: 6964 6174 696f 6e20 616e 6420 6f74 6865  idation and othe
-00001770: 7220 7479 7065 7320 6f66 206f 7074 696d  r types of optim
-00001780: 697a 6174 696f 6e20 616c 676f 7269 7468  ization algorith
-00001790: 6d73 2077 6974 686f 7574 2064 6967 6769  ms without diggi
-000017a0: 6e67 2069 6e74 6f20 6672 616d 6577 6f72  ng into framewor
-000017b0: 6b20 696e 7465 726e 616c 732e 2054 6869  k internals. Thi
-000017c0: 7320 616c 736f 206d 616b 6573 2069 7420  s also makes it 
-000017d0: 7375 7065 7220 6561 7379 2074 6f20 6164  super easy to ad
-000017e0: 6f70 7420 4661 6272 6963 2069 6e20 6578  opt Fabric in ex
-000017f0: 6973 7469 6e67 2050 7954 6f72 6368 2070  isting PyTorch p
-00001800: 726f 6a65 6374 7320 746f 2073 7065 6564  rojects to speed
-00001810: 2d75 7020 616e 6420 7363 616c 6520 796f  -up and scale yo
-00001820: 7572 206d 6f64 656c 7320 7769 7468 6f75  ur models withou
-00001830: 7420 7468 6520 636f 6d70 726f 6d69 7365  t the compromise
-00001840: 206f 6e20 6c61 7267 6520 7265 6661 6374   on large refact
-00001850: 6f72 732e 204a 7573 7420 7265 6d65 6d62  ors. Just rememb
-00001860: 6572 3a20 5769 7468 2067 7265 6174 2070  er: With great p
-00001870: 6f77 6572 2063 6f6d 6573 2061 2067 7265  ower comes a gre
-00001880: 6174 2072 6573 706f 6e73 6962 696c 6974  at responsibilit
-00001890: 792e 0a2d 202a 2a4d 6178 6d69 756d 2066  y..- **Maxmium f
-000018a0: 6c65 7869 6269 6c69 7479 2a2a 2d20 596f  lexibility**- Yo
-000018b0: 7520 7761 6e74 2074 6f20 6861 7665 2066  u want to have f
-000018c0: 756c 6c20 636f 6e74 726f 6c20 6f76 6572  ull control over
-000018d0: 2079 6f75 7220 656e 7469 7265 2074 7261   your entire tra
-000018e0: 696e 696e 672d 2069 6e20 4661 6272 6963  ining- in Fabric
-000018f0: 2061 6c6c 2066 6561 7475 7265 7320 6172   all features ar
-00001900: 6520 6f70 742d 696e 2c20 616e 6420 6974  e opt-in, and it
-00001910: 2070 726f 7669 6465 7320 796f 7520 7769   provides you wi
-00001920: 7468 2061 2074 6f6f 6c20 626f 7820 6f66  th a tool box of
-00001930: 2070 7269 6d69 7469 7665 7320 736f 2079   primitives so y
-00001940: 6f75 2063 616e 2062 7569 6c64 2079 6f75  ou can build you
-00001950: 7220 6f77 6e20 5472 6169 6e65 722e 0a0a  r own Trainer...
-00001960: 2323 2057 6865 6e20 746f 2075 7365 2074  ## When to use t
-00001970: 6865 205b 4c69 6768 746e 696e 6720 5472  he [Lightning Tr
-00001980: 6169 6e65 725d 2868 7474 7073 3a2f 2f6c  ainer](https://l
-00001990: 6967 6874 6e69 6e67 2e61 692f 646f 6373  ightning.ai/docs
-000019a0: 2f70 7974 6f72 6368 2f73 7461 626c 652f  /pytorch/stable/
-000019b0: 636f 6d6d 6f6e 2f74 7261 696e 6572 2e68  common/trainer.h
-000019c0: 746d 6c29 3f0a 0a2d 2059 6f75 2077 616e  tml)?..- You wan
-000019d0: 7420 746f 2068 6176 6520 616c 6c20 7468  t to have all th
-000019e0: 6520 656e 6769 6e65 6572 696e 6720 626f  e engineering bo
-000019f0: 696c 6572 706c 6174 6520 6861 6e64 6c65  ilerplate handle
-00001a00: 6420 666f 7220 796f 7520 2d20 646f 7a65  d for you - doze
-00001a10: 6e73 206f 6620 6665 6174 7572 6573 206c  ns of features l
-00001a20: 696b 6520 6368 6563 6b70 6f69 6e74 696e  ike checkpointin
-00001a30: 672c 206c 6f67 6769 6e67 2061 6e64 2065  g, logging and e
-00001a40: 6172 6c79 2073 746f 7070 696e 6720 6f75  arly stopping ou
-00001a50: 7420 6f66 2074 6865 2062 6f78 2e20 4c65  t of the box. Le
-00001a60: 7373 2068 6173 736c 652c 206c 6573 7320  ss hassle, less 
-00001a70: 6572 726f 7220 7072 6f6e 652c 2065 6173  error prone, eas
-00001a80: 7920 746f 2074 7279 2064 6966 6665 7265  y to try differe
-00001a90: 6e74 2074 6563 686e 6971 7565 7320 616e  nt techniques an
-00001aa0: 6420 6665 6174 7572 6573 2e0a 2d20 596f  d features..- Yo
-00001ab0: 7520 7761 6e74 2074 6f20 6861 7665 2067  u want to have g
-00001ac0: 6f6f 6420 6465 6661 756c 7473 2063 686f  ood defaults cho
-00001ad0: 7365 6e20 666f 7220 796f 7520 2d20 736f  sen for you - so
-00001ae0: 2079 6f75 2063 616e 2068 6176 6520 6120   you can have a 
-00001af0: 6265 7474 6572 2073 7461 7274 696e 6720  better starting 
-00001b00: 706f 696e 742e 0a2d 2059 6f75 2077 616e  point..- You wan
-00001b10: 7420 796f 7572 2063 6f64 6520 746f 2062  t your code to b
-00001b20: 6520 6d6f 6475 6c61 722c 2072 6561 6461  e modular, reada
-00001b30: 626c 6520 616e 6420 7765 6c6c 2073 7472  ble and well str
-00001b40: 7563 7475 7265 6420 2d20 6561 7379 2074  uctured - easy t
-00001b50: 6f20 7368 6172 6520 6265 7477 6565 6e20  o share between 
-00001b60: 7072 6f6a 6563 7473 2061 6e64 2077 6974  projects and wit
-00001b70: 6820 636f 6c6c 6162 6f72 6174 6f72 732e  h collaborators.
-00001b80: 0a0a 2323 2043 616e 2049 2075 7365 2046  ..## Can I use F
-00001b90: 6162 7269 6320 7769 7468 206d 7920 4c69  abric with my Li
-00001ba0: 6768 746e 696e 674d 6f64 756c 6520 6f72  ghtningModule or
-00001bb0: 204c 6967 6874 6e69 6e67 2043 616c 6c62   Lightning Callb
-00001bc0: 6163 6b3f 0a0a 5965 7320 3a29 2046 6162  ack?..Yes :) Fab
-00001bd0: 7269 6320 776f 726b 7320 7769 7468 2050  ric works with P
-00001be0: 7954 6f72 6368 204c 6967 6874 6e69 6e67  yTorch Lightning
-00001bf0: 4d6f 6475 6c65 7320 616e 6420 4361 6c6c  Modules and Call
-00001c00: 6261 636b 732c 2073 6f20 796f 7520 6361  backs, so you ca
-00001c10: 6e20 6368 6f6f 7365 2068 6f77 2074 6f20  n choose how to 
-00001c20: 7374 7275 6374 7572 6520 796f 7572 2063  structure your c
-00001c30: 6f64 6520 616e 6420 7265 7573 6520 6578  ode and reuse ex
-00001c40: 6973 7469 6e67 206d 6f64 656c 7320 616e  isting models an
-00001c50: 6420 6361 6c6c 6261 636b 7320 6173 2079  d callbacks as y
-00001c60: 6f75 2077 6973 682e 2052 6561 6420 6d6f  ou wish. Read mo
-00001c70: 7265 205b 6865 7265 5d28 6874 7470 733a  re [here](https:
-00001c80: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
-00001c90: 6f63 732f 6661 6272 6963 2f73 7461 626c  ocs/fabric/stabl
-00001ca0: 652f 6675 6e64 616d 656e 7461 6c73 2f63  e/fundamentals/c
-00001cb0: 6f64 655f 7374 7275 6374 7572 652e 6874  ode_structure.ht
-00001cc0: 6d6c 292e 0a0a 3c69 6d67 2073 7263 3d22  ml)...<img src="
-00001cd0: 6874 7470 733a 2f2f 706c 2d70 7562 6c69  https://pl-publi
-00001ce0: 632d 6461 7461 2e73 332e 616d 617a 6f6e  c-data.s3.amazon
-00001cf0: 6177 732e 636f 6d2f 6173 7365 7473 5f6c  aws.com/assets_l
-00001d00: 6967 6874 6e69 6e67 2f63 6f6e 7469 6e75  ightning/continu
-00001d10: 756d 2e70 6e67 2220 7769 6474 683d 2238  um.png" width="8
-00001d20: 3030 7078 223e 0a0a 5f5f 5f5f 5f5f 5f5f  00px">..________
-00001d30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001d40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001d50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001d60: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a  ______________..
-00001d70: 2320 4578 616d 706c 6573 0a0a 2d20 5b47  # Examples..- [G
-00001d80: 414e 5d28 6874 7470 733a 2f2f 6769 7468  AN](https://gith
-00001d90: 7562 2e63 6f6d 2f4c 6967 6874 6e69 6e67  ub.com/Lightning
-00001da0: 2d41 492f 6c69 6768 746e 696e 672f 7472  -AI/lightning/tr
-00001db0: 6565 2f6d 6173 7465 722f 6578 616d 706c  ee/master/exampl
-00001dc0: 6573 2f66 6162 7269 632f 6463 6761 6e29  es/fabric/dcgan)
-00001dd0: 0a2d 205b 4d65 7461 206c 6561 726e 696e  .- [Meta learnin
-00001de0: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001df0: 622e 636f 6d2f 4c69 6768 746e 696e 672d  b.com/Lightning-
-00001e00: 4149 2f6c 6967 6874 6e69 6e67 2f74 7265  AI/lightning/tre
-00001e10: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
-00001e20: 732f 6661 6272 6963 2f6d 6574 615f 6c65  s/fabric/meta_le
-00001e30: 6172 6e69 6e67 290a 2d20 5b52 6569 6e66  arning).- [Reinf
-00001e40: 6f72 6365 6d65 6e74 206c 6561 726e 696e  orcement learnin
-00001e50: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001e60: 622e 636f 6d2f 4c69 6768 746e 696e 672d  b.com/Lightning-
-00001e70: 4149 2f6c 6967 6874 6e69 6e67 2f74 7265  AI/lightning/tre
-00001e80: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
-00001e90: 732f 6661 6272 6963 2f72 6569 6e66 6f72  s/fabric/reinfor
-00001ea0: 6365 6d65 6e74 5f6c 6561 726e 696e 6729  cement_learning)
-00001eb0: 0a2d 205b 4b2d 466f 6c64 2063 726f 7373  .- [K-Fold cross
-00001ec0: 2076 616c 6964 6174 696f 6e5d 2868 7474   validation](htt
-00001ed0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001ee0: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
-00001ef0: 6874 6e69 6e67 2f74 7265 652f 6d61 7374  htning/tree/mast
-00001f00: 6572 2f65 7861 6d70 6c65 732f 6661 6272  er/examples/fabr
-00001f10: 6963 2f6b 666f 6c64 5f63 7629 0a0a 5f5f  ic/kfold_cv)..__
-00001f20: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00001f60: 5f5f 5f5f 0a0a 2323 2041 736b 696e 6720  ____..## Asking 
-00001f70: 666f 7220 6865 6c70 0a0a 4966 2079 6f75  for help..If you
-00001f80: 2068 6176 6520 616e 7920 7175 6573 7469   have any questi
-00001f90: 6f6e 7320 706c 6561 7365 3a0a 0a31 2e20  ons please:..1. 
-00001fa0: 5b52 6561 6420 7468 6520 646f 6373 5d28  [Read the docs](
-00001fb0: 6874 7470 733a 2f2f 6c69 6768 746e 696e  https://lightnin
-00001fc0: 672e 6169 2f64 6f63 732f 6661 6272 6963  g.ai/docs/fabric
-00001fd0: 292e 0a31 2e20 5b41 736b 2061 2071 7565  )..1. [Ask a que
-00001fe0: 7374 696f 6e20 696e 206f 7572 2066 6f72  stion in our for
-00001ff0: 756d 5d28 6874 7470 733a 2f2f 6c69 6768  um](https://ligh
-00002000: 746e 696e 672e 6169 2f66 6f72 756d 732f  tning.ai/forums/
-00002010: 292e 0a31 2e20 5b4a 6f69 6e20 6f75 7220  )..1. [Join our 
-00002020: 6469 7363 6f72 6420 636f 6d6d 756e 6974  discord communit
-00002030: 795d 2868 7474 7073 3a2f 2f64 6973 636f  y](https://disco
-00002040: 7264 2e63 6f6d 2f69 6e76 6974 652f 7466  rd.com/invite/tf
-00002050: 5846 6574 455a 7876 292e 0a0a 0a         XFetEZxv)....
+00000630: 5f5f 5f5f 5f5f 0a0a 3c70 2061 6c69 676e  ______..<p align
+00000640: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+00000650: 6872 6566 3d22 6874 7470 733a 2f2f 6c69  href="https://li
+00000660: 6768 746e 696e 672e 6169 2f22 3e57 6562  ghtning.ai/">Web
+00000670: 7369 7465 3c2f 613e 20e2 80a2 0a20 203c  site</a> ....  <
+00000680: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000690: 6c69 6768 746e 696e 672e 6169 2f64 6f63  lightning.ai/doc
+000006a0: 732f 6661 6272 6963 2f22 3e44 6f63 733c  s/fabric/">Docs<
+000006b0: 2f61 3e20 e280 a20a 2020 3c61 2068 7265  /a> ....  <a hre
+000006c0: 663d 2223 6765 7474 696e 672d 7374 6172  f="#getting-star
+000006d0: 7465 6422 3e47 6574 7469 6e67 2073 7461  ted">Getting sta
+000006e0: 7274 6564 3c2f 613e 20e2 80a2 0a20 203c  rted</a> ....  <
+000006f0: 6120 6872 6566 3d22 2366 6171 223e 4641  a href="#faq">FA
+00000700: 513c 2f61 3e20 e280 a20a 2020 3c61 2068  Q</a> ....  <a h
+00000710: 7265 663d 2223 6173 6b69 6e67 2d66 6f72  ref="#asking-for
+00000720: 2d68 656c 7022 3e48 656c 703c 2f61 3e20  -help">Help</a> 
+00000730: e280 a20a 2020 3c61 2068 7265 663d 2268  ....  <a href="h
+00000740: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
+00000750: 672f 5670 7450 435a 6b47 4e61 223e 4469  g/VptPCZkGNa">Di
+00000760: 7363 6f72 643c 2f61 3e0a 3c2f 703e 0a0a  scord</a>.</p>..
+00000770: 5b21 5b50 7950 4920 2d20 5079 7468 6f6e  [![PyPI - Python
+00000780: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00000790: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007a0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+000007b0: 2f6c 6967 6874 6e69 6e67 5f66 6162 7269  /lightning_fabri
+000007c0: 6329 5d28 6874 7470 733a 2f2f 7079 7069  c)](https://pypi
+000007d0: 2e6f 7267 2f70 726f 6a65 6374 2f6c 6967  .org/project/lig
+000007e0: 6874 6e69 6e67 5f66 6162 7269 632f 290a  htning_fabric/).
+000007f0: 5b21 5b50 7950 4920 5374 6174 7573 5d28  [![PyPI Status](
+00000800: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000810: 7279 2e69 6f2f 7079 2f6c 6967 6874 6e69  ry.io/py/lightni
+00000820: 6e67 5f66 6162 7269 632e 7376 6729 5d28  ng_fabric.svg)](
+00000830: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000840: 7279 2e69 6f2f 7079 2f6c 6967 6874 6e69  ry.io/py/lightni
+00000850: 6e67 5f66 6162 7269 6329 0a5b 215b 5079  ng_fabric).[![Py
+00000860: 5049 2053 7461 7475 735d 2868 7474 7073  PI Status](https
+00000870: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
+00000880: 6765 2f6c 6967 6874 6e69 6e67 5f66 6162  ge/lightning_fab
+00000890: 7269 6329 5d28 6874 7470 733a 2f2f 7065  ric)](https://pe
+000008a0: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
+000008b0: 6c69 6768 746e 696e 675f 6661 6272 6963  lightning_fabric
+000008c0: 290a 5b21 5b43 6f6e 6461 5d28 6874 7470  ).[![Conda](http
+000008d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000008e0: 696f 2f63 6f6e 6461 2f76 2f63 6f6e 6461  io/conda/v/conda
+000008f0: 2d66 6f72 6765 2f6c 6967 6874 6e69 6e67  -forge/lightning
+00000900: 5f66 6162 7269 633f 6c61 6265 6c3d 636f  _fabric?label=co
+00000910: 6e64 6126 636f 6c6f 723d 7375 6363 6573  nda&color=succes
+00000920: 7329 5d28 6874 7470 733a 2f2f 616e 6163  s)](https://anac
+00000930: 6f6e 6461 2e6f 7267 2f63 6f6e 6461 2d66  onda.org/conda-f
+00000940: 6f72 6765 2f6c 6967 6874 6e69 6e67 5f66  orge/lightning_f
+00000950: 6162 7269 6329 0a0a 3c2f 6469 763e 0a0a  abric)..</div>..
+00000960: 2320 4c69 6768 746e 696e 6720 4661 6272  # Lightning Fabr
+00000970: 6963 3a20 4578 7065 7274 2063 6f6e 7472  ic: Expert contr
+00000980: 6f6c 2e0a 0a52 756e 206f 6e20 616e 7920  ol...Run on any 
+00000990: 6465 7669 6365 2061 7420 616e 7920 7363  device at any sc
+000009a0: 616c 6520 7769 7468 2065 7870 6572 742d  ale with expert-
+000009b0: 6c65 7665 6c20 636f 6e74 726f 6c20 6f76  level control ov
+000009c0: 6572 2050 7954 6f72 6368 2074 7261 696e  er PyTorch train
+000009d0: 696e 6720 6c6f 6f70 2061 6e64 2073 6361  ing loop and sca
+000009e0: 6c69 6e67 2073 7472 6174 6567 792e 2059  ling strategy. Y
+000009f0: 6f75 2063 616e 2065 7665 6e20 7772 6974  ou can even writ
+00000a00: 6520 796f 7572 206f 776e 2054 7261 696e  e your own Train
+00000a10: 6572 2e0a 0a46 6162 7269 6320 6973 2064  er...Fabric is d
+00000a20: 6573 6967 6e65 6420 666f 7220 7468 6520  esigned for the 
+00000a30: 6d6f 7374 2063 6f6d 706c 6578 206d 6f64  most complex mod
+00000a40: 656c 7320 6c69 6b65 2066 6f75 6e64 6174  els like foundat
+00000a50: 696f 6e20 6d6f 6465 6c20 7363 616c 696e  ion model scalin
+00000a60: 672c 204c 4c4d 732c 2064 6966 6675 7369  g, LLMs, diffusi
+00000a70: 6f6e 2c20 7472 616e 7366 6f72 6d65 7273  on, transformers
+00000a80: 2c20 7265 696e 666f 7263 656d 656e 7420  , reinforcement 
+00000a90: 6c65 6172 6e69 6e67 2c20 6163 7469 7665  learning, active
+00000aa0: 206c 6561 726e 696e 672e 204f 6620 616e   learning. Of an
+00000ab0: 7920 7369 7a65 2e0a 0a3c 7461 626c 653e  y size...<table>
+00000ac0: 0a3c 7472 3e0a 3c74 683e 5768 6174 2074  .<tr>.<th>What t
+00000ad0: 6f20 6368 616e 6765 3c2f 7468 3e0a 3c74  o change</th>.<t
+00000ae0: 683e 5265 7375 6c74 696e 6720 4661 6272  h>Resulting Fabr
+00000af0: 6963 2043 6f64 6520 2863 6f70 7920 6d65  ic Code (copy me
+00000b00: 2129 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74  !)</th>.</tr>.<t
+00000b10: 723e 0a3c 7464 3e0a 3c73 7562 3e0a 0a60  r>.<td>.<sub>..`
+00000b20: 6060 6469 6666 0a2b 2069 6d70 6f72 7420  ``diff.+ import 
+00000b30: 6c69 6768 746e 696e 6720 6173 204c 0a20  lightning as L. 
+00000b40: 2069 6d70 6f72 7420 746f 7263 683b 2069   import torch; i
+00000b50: 6d70 6f72 7420 746f 7263 6876 6973 696f  mport torchvisio
+00000b60: 6e20 6173 2074 760a 0a2b 2066 6162 7269  n as tv..+ fabri
+00000b70: 6320 3d20 4c2e 4661 6272 6963 2829 0a2b  c = L.Fabric().+
+00000b80: 2066 6162 7269 632e 6c61 756e 6368 2829   fabric.launch()
+00000b90: 0a0a 2020 6d6f 6465 6c20 3d20 7476 2e6d  ..  model = tv.m
+00000ba0: 6f64 656c 732e 7265 736e 6574 3138 2829  odels.resnet18()
+00000bb0: 0a20 206f 7074 696d 697a 6572 203d 2074  .  optimizer = t
+00000bc0: 6f72 6368 2e6f 7074 696d 2e53 4744 286d  orch.optim.SGD(m
+00000bd0: 6f64 656c 2e70 6172 616d 6574 6572 7328  odel.parameters(
+00000be0: 292c 206c 723d 302e 3030 3129 0a2d 2064  ), lr=0.001).- d
+00000bf0: 6576 6963 6520 3d20 2263 7564 6122 2069  evice = "cuda" i
+00000c00: 6620 746f 7263 682e 6375 6461 2e69 735f  f torch.cuda.is_
+00000c10: 6176 6169 6c61 626c 6528 2920 656c 7365  available() else
+00000c20: 2022 6370 7522 0a2d 206d 6f64 656c 2e74   "cpu".- model.t
+00000c30: 6f28 6465 7669 6365 290a 2b20 6d6f 6465  o(device).+ mode
+00000c40: 6c2c 206f 7074 696d 697a 6572 203d 2066  l, optimizer = f
+00000c50: 6162 7269 632e 7365 7475 7028 6d6f 6465  abric.setup(mode
+00000c60: 6c2c 206f 7074 696d 697a 6572 290a 0a20  l, optimizer).. 
+00000c70: 2064 6174 6173 6574 203d 2074 762e 6461   dataset = tv.da
+00000c80: 7461 7365 7473 2e43 4946 4152 3130 2822  tasets.CIFAR10("
+00000c90: 6461 7461 222c 2064 6f77 6e6c 6f61 643d  data", download=
+00000ca0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 2020 2020 2020 7472 6169 6e3d 5472 7565        train=True
+00000cd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cf0: 2020 7472 616e 7366 6f72 6d3d 7476 2e74    transform=tv.t
+00000d00: 7261 6e73 666f 726d 732e 546f 5465 6e73  ransforms.ToTens
+00000d10: 6f72 2829 290a 2020 6461 7461 6c6f 6164  or()).  dataload
+00000d20: 6572 203d 2074 6f72 6368 2e75 7469 6c73  er = torch.utils
+00000d30: 2e64 6174 612e 4461 7461 4c6f 6164 6572  .data.DataLoader
+00000d40: 2864 6174 6173 6574 2c20 6261 7463 685f  (dataset, batch_
+00000d50: 7369 7a65 3d38 290a 2b20 6461 7461 6c6f  size=8).+ datalo
+00000d60: 6164 6572 203d 2066 6162 7269 632e 7365  ader = fabric.se
+00000d70: 7475 705f 6461 7461 6c6f 6164 6572 7328  tup_dataloaders(
+00000d80: 6461 7461 6c6f 6164 6572 290a 0a20 206d  dataloader)..  m
+00000d90: 6f64 656c 2e74 7261 696e 2829 0a20 206e  odel.train().  n
+00000da0: 756d 5f65 706f 6368 7320 3d20 3130 0a20  um_epochs = 10. 
+00000db0: 2066 6f72 2065 706f 6368 2069 6e20 7261   for epoch in ra
+00000dc0: 6e67 6528 6e75 6d5f 6570 6f63 6873 293a  nge(num_epochs):
+00000dd0: 0a20 2020 2020 2066 6f72 2062 6174 6368  .      for batch
+00000de0: 2069 6e20 6461 7461 6c6f 6164 6572 3a0a   in dataloader:.
+00000df0: 2020 2020 2020 2020 2020 696e 7075 7473            inputs
+00000e00: 2c20 6c61 6265 6c73 203d 2062 6174 6368  , labels = batch
+00000e10: 0a2d 2020 2020 2020 2020 2069 6e70 7574  .-         input
+00000e20: 732c 206c 6162 656c 7320 3d20 696e 7075  s, labels = inpu
+00000e30: 7473 2e74 6f28 6465 7669 6365 292c 206c  ts.to(device), l
+00000e40: 6162 656c 732e 746f 2864 6576 6963 6529  abels.to(device)
+00000e50: 0a20 2020 2020 2020 2020 206f 7074 696d  .          optim
+00000e60: 697a 6572 2e7a 6572 6f5f 6772 6164 2829  izer.zero_grad()
+00000e70: 0a20 2020 2020 2020 2020 206f 7574 7075  .          outpu
+00000e80: 7473 203d 206d 6f64 656c 2869 6e70 7574  ts = model(input
+00000e90: 7329 0a20 2020 2020 2020 2020 206c 6f73  s).          los
+00000ea0: 7320 3d20 746f 7263 682e 6e6e 2e66 756e  s = torch.nn.fun
+00000eb0: 6374 696f 6e61 6c2e 6372 6f73 735f 656e  ctional.cross_en
+00000ec0: 7472 6f70 7928 6f75 7470 7574 732c 206c  tropy(outputs, l
+00000ed0: 6162 656c 7329 0a2d 2020 2020 2020 2020  abels).-        
+00000ee0: 206c 6f73 732e 6261 636b 7761 7264 2829   loss.backward()
+00000ef0: 0a2b 2020 2020 2020 2020 2066 6162 7269  .+         fabri
+00000f00: 632e 6261 636b 7761 7264 286c 6f73 7329  c.backward(loss)
+00000f10: 0a20 2020 2020 2020 2020 206f 7074 696d  .          optim
+00000f20: 697a 6572 2e73 7465 7028 290a 6060 600a  izer.step().```.
+00000f30: 0a3c 2f73 7562 3e0a 3c74 643e 0a3c 7375  .</sub>.<td>.<su
+00000f40: 623e 0a0a 6060 6050 7974 686f 6e0a 696d  b>..```Python.im
+00000f50: 706f 7274 206c 6967 6874 6e69 6e67 2061  port lightning a
+00000f60: 7320 4c0a 696d 706f 7274 2074 6f72 6368  s L.import torch
+00000f70: 3b20 696d 706f 7274 2074 6f72 6368 7669  ; import torchvi
+00000f80: 7369 6f6e 2061 7320 7476 0a0a 6661 6272  sion as tv..fabr
+00000f90: 6963 203d 204c 2e46 6162 7269 6328 290a  ic = L.Fabric().
+00000fa0: 6661 6272 6963 2e6c 6175 6e63 6828 290a  fabric.launch().
+00000fb0: 0a6d 6f64 656c 203d 2074 762e 6d6f 6465  .model = tv.mode
+00000fc0: 6c73 2e72 6573 6e65 7431 3828 290a 6f70  ls.resnet18().op
+00000fd0: 7469 6d69 7a65 7220 3d20 746f 7263 682e  timizer = torch.
+00000fe0: 6f70 7469 6d2e 5347 4428 6d6f 6465 6c2e  optim.SGD(model.
+00000ff0: 7061 7261 6d65 7465 7273 2829 2c20 6c72  parameters(), lr
+00001000: 3d30 2e30 3031 290a 6d6f 6465 6c2c 206f  =0.001).model, o
+00001010: 7074 696d 697a 6572 203d 2066 6162 7269  ptimizer = fabri
+00001020: 632e 7365 7475 7028 6d6f 6465 6c2c 206f  c.setup(model, o
+00001030: 7074 696d 697a 6572 290a 0a64 6174 6173  ptimizer)..datas
+00001040: 6574 203d 2074 762e 6461 7461 7365 7473  et = tv.datasets
+00001050: 2e43 4946 4152 3130 2822 6461 7461 222c  .CIFAR10("data",
+00001060: 2064 6f77 6e6c 6f61 643d 5472 7565 2c0a   download=True,.
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00001090: 6169 6e3d 5472 7565 2c0a 2020 2020 2020  ain=True,.      
+000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+000010c0: 6d3d 7476 2e74 7261 6e73 666f 726d 732e  m=tv.transforms.
+000010d0: 546f 5465 6e73 6f72 2829 290a 6461 7461  ToTensor()).data
+000010e0: 6c6f 6164 6572 203d 2074 6f72 6368 2e75  loader = torch.u
+000010f0: 7469 6c73 2e64 6174 612e 4461 7461 4c6f  tils.data.DataLo
+00001100: 6164 6572 2864 6174 6173 6574 2c20 6261  ader(dataset, ba
+00001110: 7463 685f 7369 7a65 3d38 290a 6461 7461  tch_size=8).data
+00001120: 6c6f 6164 6572 203d 2066 6162 7269 632e  loader = fabric.
+00001130: 7365 7475 705f 6461 7461 6c6f 6164 6572  setup_dataloader
+00001140: 7328 6461 7461 6c6f 6164 6572 290a 0a6d  s(dataloader)..m
+00001150: 6f64 656c 2e74 7261 696e 2829 0a6e 756d  odel.train().num
+00001160: 5f65 706f 6368 7320 3d20 3130 0a66 6f72  _epochs = 10.for
+00001170: 2065 706f 6368 2069 6e20 7261 6e67 6528   epoch in range(
+00001180: 6e75 6d5f 6570 6f63 6873 293a 0a20 2020  num_epochs):.   
+00001190: 2066 6f72 2062 6174 6368 2069 6e20 6461   for batch in da
+000011a0: 7461 6c6f 6164 6572 3a0a 2020 2020 2020  taloader:.      
+000011b0: 2020 696e 7075 7473 2c20 6c61 6265 6c73    inputs, labels
+000011c0: 203d 2062 6174 6368 0a20 2020 2020 2020   = batch.       
+000011d0: 206f 7074 696d 697a 6572 2e7a 6572 6f5f   optimizer.zero_
+000011e0: 6772 6164 2829 0a20 2020 2020 2020 206f  grad().        o
+000011f0: 7574 7075 7473 203d 206d 6f64 656c 2869  utputs = model(i
+00001200: 6e70 7574 7329 0a20 2020 2020 2020 206c  nputs).        l
+00001210: 6f73 7320 3d20 746f 7263 682e 6e6e 2e66  oss = torch.nn.f
+00001220: 756e 6374 696f 6e61 6c2e 6372 6f73 735f  unctional.cross_
+00001230: 656e 7472 6f70 7928 6f75 7470 7574 732c  entropy(outputs,
+00001240: 206c 6162 656c 7329 0a20 2020 2020 2020   labels).       
+00001250: 2066 6162 7269 632e 6261 636b 7761 7264   fabric.backward
+00001260: 286c 6f73 7329 0a20 2020 2020 2020 206f  (loss).        o
+00001270: 7074 696d 697a 6572 2e73 7465 7028 290a  ptimizer.step().
+00001280: 6060 600a 0a3c 2f73 7562 3e0a 3c2f 7464  ```..</sub>.</td
+00001290: 3e0a 3c2f 7472 3e0a 3c2f 7461 626c 653e  >.</tr>.</table>
+000012a0: 0a0a 2323 204b 6579 2066 6561 7475 7265  ..## Key feature
+000012b0: 730a 0a3c 6465 7461 696c 733e 0a20 203c  s..<details>.  <
+000012c0: 7375 6d6d 6172 793e 4561 7369 6c79 2073  summary>Easily s
+000012d0: 7769 7463 6820 6672 6f6d 2072 756e 6e69  witch from runni
+000012e0: 6e67 206f 6e20 4350 5520 746f 2047 5055  ng on CPU to GPU
+000012f0: 2028 4170 706c 6520 5369 6c69 636f 6e2c   (Apple Silicon,
+00001300: 2043 5544 412c 20e2 80a6 292c 2054 5055   CUDA, ...), TPU
+00001310: 2c20 6d75 6c74 692d 4750 5520 6f72 2065  , multi-GPU or e
+00001320: 7665 6e20 6d75 6c74 692d 6e6f 6465 2074  ven multi-node t
+00001330: 7261 696e 696e 673c 2f73 756d 6d61 7279  raining</summary
+00001340: 3e0a 0a60 6060 7079 7468 6f6e 0a23 2055  >..```python.# U
+00001350: 7365 2079 6f75 7220 6176 6169 6c61 626c  se your availabl
+00001360: 6520 6861 7264 7761 7265 0a23 206e 6f20  e hardware.# no 
+00001370: 636f 6465 2063 6861 6e67 6573 206e 6565  code changes nee
+00001380: 6465 640a 6661 6272 6963 203d 2046 6162  ded.fabric = Fab
+00001390: 7269 6328 290a 0a23 2052 756e 206f 6e20  ric()..# Run on 
+000013a0: 4750 5573 2028 4355 4441 206f 7220 4d50  GPUs (CUDA or MP
+000013b0: 5329 0a66 6162 7269 6320 3d20 4661 6272  S).fabric = Fabr
+000013c0: 6963 2861 6363 656c 6572 6174 6f72 3d22  ic(accelerator="
+000013d0: 6770 7522 290a 0a23 2038 2047 5055 730a  gpu")..# 8 GPUs.
+000013e0: 6661 6272 6963 203d 2046 6162 7269 6328  fabric = Fabric(
+000013f0: 6163 6365 6c65 7261 746f 723d 2267 7075  accelerator="gpu
+00001400: 222c 2064 6576 6963 6573 3d38 290a 0a23  ", devices=8)..#
+00001410: 2032 3536 2047 5055 732c 206d 756c 7469   256 GPUs, multi
+00001420: 2d6e 6f64 650a 6661 6272 6963 203d 2046  -node.fabric = F
+00001430: 6162 7269 6328 6163 6365 6c65 7261 746f  abric(accelerato
+00001440: 723d 2267 7075 222c 2064 6576 6963 6573  r="gpu", devices
+00001450: 3d38 2c20 6e75 6d5f 6e6f 6465 733d 3332  =8, num_nodes=32
+00001460: 290a 0a23 2052 756e 206f 6e20 5450 5573  )..# Run on TPUs
+00001470: 0a66 6162 7269 6320 3d20 4661 6272 6963  .fabric = Fabric
+00001480: 2861 6363 656c 6572 6174 6f72 3d22 7470  (accelerator="tp
+00001490: 7522 290a 6060 600a 0a3c 2f64 6574 6169  u").```..</detai
+000014a0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a20  ls>..<details>. 
+000014b0: 203c 7375 6d6d 6172 793e 5573 6520 7374   <summary>Use st
+000014c0: 6174 652d 6f66 2d74 6865 2d61 7274 2064  ate-of-the-art d
+000014d0: 6973 7472 6962 7574 6564 2074 7261 696e  istributed train
+000014e0: 696e 6720 7374 7261 7465 6769 6573 2028  ing strategies (
+000014f0: 4444 502c 2046 5344 502c 2044 6565 7053  DDP, FSDP, DeepS
+00001500: 7065 6564 2920 616e 6420 6d69 7865 6420  peed) and mixed 
+00001510: 7072 6563 6973 696f 6e20 6f75 7420 6f66  precision out of
+00001520: 2074 6865 2062 6f78 3c2f 7375 6d6d 6172   the box</summar
+00001530: 793e 0a0a 6060 6070 7974 686f 6e0a 2320  y>..```python.# 
+00001540: 5573 6520 7374 6174 652d 6f66 2d74 6865  Use state-of-the
+00001550: 2d61 7274 2064 6973 7472 6962 7574 6564  -art distributed
+00001560: 2074 7261 696e 696e 6720 7465 6368 6e69   training techni
+00001570: 7175 6573 0a66 6162 7269 6320 3d20 4661  ques.fabric = Fa
+00001580: 6272 6963 2873 7472 6174 6567 793d 2264  bric(strategy="d
+00001590: 6470 2229 0a66 6162 7269 6320 3d20 4661  dp").fabric = Fa
+000015a0: 6272 6963 2873 7472 6174 6567 793d 2264  bric(strategy="d
+000015b0: 6565 7073 7065 6564 2229 0a66 6162 7269  eepspeed").fabri
+000015c0: 6320 3d20 4661 6272 6963 2873 7472 6174  c = Fabric(strat
+000015d0: 6567 793d 2266 7364 7022 290a 0a23 2053  egy="fsdp")..# S
+000015e0: 7769 7463 6820 7468 6520 7072 6563 6973  witch the precis
+000015f0: 696f 6e0a 6661 6272 6963 203d 2046 6162  ion.fabric = Fab
+00001600: 7269 6328 7072 6563 6973 696f 6e3d 2231  ric(precision="1
+00001610: 362d 6d69 7865 6422 290a 6661 6272 6963  6-mixed").fabric
+00001620: 203d 2046 6162 7269 6328 7072 6563 6973   = Fabric(precis
+00001630: 696f 6e3d 2236 3422 290a 6060 600a 0a3c  ion="64").```..<
+00001640: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
+00001650: 696c 733e 0a20 203c 7375 6d6d 6172 793e  ils>.  <summary>
+00001660: 416c 6c20 7468 6520 6465 7669 6365 206c  All the device l
+00001670: 6f67 6963 2062 6f69 6c65 7270 6c61 7465  ogic boilerplate
+00001680: 2069 7320 6861 6e64 6c65 6420 666f 7220   is handled for 
+00001690: 796f 753c 2f73 756d 6d61 7279 3e0a 0a60  you</summary>..`
+000016a0: 6060 6469 6666 0a20 2023 206e 6f20 6d6f  ``diff.  # no mo
+000016b0: 7265 206f 6620 7468 6973 210a 2d20 6d6f  re of this!.- mo
+000016c0: 6465 6c2e 746f 2864 6576 6963 6529 0a2d  del.to(device).-
+000016d0: 2062 6174 6368 2e74 6f28 6465 7669 6365   batch.to(device
+000016e0: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
+000016f0: 3e0a 0a3c 6465 7461 696c 733e 0a20 203c  >..<details>.  <
+00001700: 7375 6d6d 6172 793e 4275 696c 6420 796f  summary>Build yo
+00001710: 7572 206f 776e 2063 7573 746f 6d20 5472  ur own custom Tr
+00001720: 6169 6e65 7220 7573 696e 6720 4661 6272  ainer using Fabr
+00001730: 6963 2070 7269 6d69 7469 7665 7320 666f  ic primitives fo
+00001740: 7220 7472 6169 6e69 6e67 2063 6865 636b  r training check
+00001750: 706f 696e 7469 6e67 2c20 6c6f 6767 696e  pointing, loggin
+00001760: 672c 2061 6e64 206d 6f72 653c 2f73 756d  g, and more</sum
+00001770: 6d61 7279 3e0a 0a60 6060 7079 7468 6f6e  mary>..```python
+00001780: 0a69 6d70 6f72 7420 6c69 6768 746e 696e  .import lightnin
+00001790: 6720 6173 204c 0a0a 0a63 6c61 7373 204d  g as L...class M
+000017a0: 7943 7573 746f 6d54 7261 696e 6572 3a0a  yCustomTrainer:.
+000017b0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000017c0: 2873 656c 662c 2061 6363 656c 6572 6174  (self, accelerat
+000017d0: 6f72 3d22 6175 746f 222c 2073 7472 6174  or="auto", strat
+000017e0: 6567 793d 2261 7574 6f22 2c20 6465 7669  egy="auto", devi
+000017f0: 6365 733d 2261 7574 6f22 2c20 7072 6563  ces="auto", prec
+00001800: 6973 696f 6e3d 2233 322d 7472 7565 2229  ision="32-true")
+00001810: 3a0a 2020 2020 2020 2020 7365 6c66 2e66  :.        self.f
+00001820: 6162 7269 6320 3d20 4c2e 4661 6272 6963  abric = L.Fabric
+00001830: 2861 6363 656c 6572 6174 6f72 3d61 6363  (accelerator=acc
+00001840: 656c 6572 6174 6f72 2c20 7374 7261 7465  elerator, strate
+00001850: 6779 3d73 7472 6174 6567 792c 2064 6576  gy=strategy, dev
+00001860: 6963 6573 3d64 6576 6963 6573 2c20 7072  ices=devices, pr
+00001870: 6563 6973 696f 6e3d 7072 6563 6973 696f  ecision=precisio
+00001880: 6e29 0a0a 2020 2020 6465 6620 6669 7428  n)..    def fit(
+00001890: 7365 6c66 2c20 6d6f 6465 6c2c 206f 7074  self, model, opt
+000018a0: 696d 697a 6572 2c20 6461 7461 6c6f 6164  imizer, dataload
+000018b0: 6572 2c20 6d61 785f 6570 6f63 6873 293a  er, max_epochs):
+000018c0: 0a20 2020 2020 2020 2073 656c 662e 6661  .        self.fa
+000018d0: 6272 6963 2e6c 6175 6e63 6828 290a 0a20  bric.launch().. 
+000018e0: 2020 2020 2020 206d 6f64 656c 2c20 6f70         model, op
+000018f0: 7469 6d69 7a65 7220 3d20 7365 6c66 2e66  timizer = self.f
+00001900: 6162 7269 632e 7365 7475 7028 6d6f 6465  abric.setup(mode
+00001910: 6c2c 206f 7074 696d 697a 6572 290a 2020  l, optimizer).  
+00001920: 2020 2020 2020 6461 7461 6c6f 6164 6572        dataloader
+00001930: 203d 2073 656c 662e 6661 6272 6963 2e73   = self.fabric.s
+00001940: 6574 7570 5f64 6174 616c 6f61 6465 7273  etup_dataloaders
+00001950: 2864 6174 616c 6f61 6465 7229 0a20 2020  (dataloader).   
+00001960: 2020 2020 206d 6f64 656c 2e74 7261 696e       model.train
+00001970: 2829 0a0a 2020 2020 2020 2020 666f 7220  ()..        for 
+00001980: 6570 6f63 6820 696e 2072 616e 6765 286d  epoch in range(m
+00001990: 6178 5f65 706f 6368 7329 3a0a 2020 2020  ax_epochs):.    
+000019a0: 2020 2020 2020 2020 666f 7220 6261 7463          for batc
+000019b0: 6820 696e 2064 6174 616c 6f61 6465 723a  h in dataloader:
+000019c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000019d0: 2069 6e70 7574 2c20 7461 7267 6574 203d   input, target =
+000019e0: 2062 6174 6368 0a20 2020 2020 2020 2020   batch.         
+000019f0: 2020 2020 2020 206f 7074 696d 697a 6572         optimizer
+00001a00: 2e7a 6572 6f5f 6772 6164 2829 0a20 2020  .zero_grad().   
+00001a10: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00001a20: 7075 7420 3d20 6d6f 6465 6c28 696e 7075  put = model(inpu
+00001a30: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00001a40: 2020 206c 6f73 7320 3d20 6c6f 7373 5f66     loss = loss_f
+00001a50: 6e28 6f75 7470 7574 2c20 7461 7267 6574  n(output, target
+00001a60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00001a70: 2020 7365 6c66 2e66 6162 7269 632e 6261    self.fabric.ba
+00001a80: 636b 7761 7264 286c 6f73 7329 0a20 2020  ckward(loss).   
+00001a90: 2020 2020 2020 2020 2020 2020 206f 7074               opt
+00001aa0: 696d 697a 6572 2e73 7465 7028 290a 6060  imizer.step().``
+00001ab0: 600a 0a59 6f75 2063 616e 2066 696e 6420  `..You can find 
+00001ac0: 6120 6d6f 7265 2065 7874 656e 7369 7665  a more extensive
+00001ad0: 2065 7861 6d70 6c65 2069 6e20 6f75 7220   example in our 
+00001ae0: 5b65 7861 6d70 6c65 735d 282e 2e2f 2e2e  [examples](../..
+00001af0: 2f65 7861 6d70 6c65 732f 6661 6272 6963  /examples/fabric
+00001b00: 2f62 7569 6c64 5f79 6f75 725f 6f77 6e5f  /build_your_own_
+00001b10: 7472 6169 6e65 7229 0a0a 3c2f 6465 7461  trainer)..</deta
+00001b20: 696c 733e 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f  ils>..__________
+00001b30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001b40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001b50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001b60: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a 3c64  ____________..<d
+00001b70: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+00001b80: 223e 0a20 2020 203c 6120 6872 6566 3d22  ">.    <a href="
+00001b90: 6874 7470 733a 2f2f 6c69 6768 746e 696e  https://lightnin
+00001ba0: 672e 6169 2f64 6f63 732f 6661 6272 6963  g.ai/docs/fabric
+00001bb0: 2f73 7461 626c 652f 223e 5265 6164 2074  /stable/">Read t
+00001bc0: 6865 204c 6967 6874 6e69 6e67 2046 6162  he Lightning Fab
+00001bd0: 7269 6320 646f 6373 3c2f 613e 0a3c 2f64  ric docs</a>.</d
+00001be0: 6976 3e0a 0a5f 5f5f 5f5f 5f5f 5f5f 5f5f  iv>..___________
+00001bf0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c00: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c10: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001c20: 5f5f 5f5f 5f5f 5f5f 5f5f 5f0a 0a23 2047  ___________..# G
+00001c30: 6574 7469 6e67 2073 7461 7274 6564 0a0a  etting started..
+00001c40: 2323 2049 6e73 7461 6c6c 204c 6967 6874  ## Install Light
+00001c50: 6e69 6e67 0a0a 3c64 6574 6169 6c73 3e0a  ning..<details>.
+00001c60: 0a3c 7375 6d6d 6172 793e 5072 6572 6571  .<summary>Prereq
+00001c70: 7569 7369 7465 733c 2f73 756d 6d61 7279  uisites</summary
+00001c80: 3e0a 0a3e 2054 4950 3a20 5765 2073 7472  >..> TIP: We str
+00001c90: 6f6e 676c 7920 7265 636f 6d6d 656e 6420  ongly recommend 
+00001ca0: 6372 6561 7469 6e67 2061 2076 6972 7475  creating a virtu
+00001cb0: 616c 2065 6e76 6972 6f6e 6d65 6e74 2066  al environment f
+00001cc0: 6972 7374 2e0a 3e20 446f 6ee2 8099 7420  irst..> Don...t 
+00001cd0: 6b6e 6f77 2077 6861 7420 7468 6973 2069  know what this i
+00001ce0: 733f 2046 6f6c 6c6f 7720 6f75 7220 5b62  s? Follow our [b
+00001cf0: 6567 696e 6e65 7220 6775 6964 6520 6865  eginner guide he
+00001d00: 7265 5d28 6874 7470 733a 2f2f 6c69 6768  re](https://ligh
+00001d10: 746e 696e 672e 6169 2f64 6f63 732f 7374  tning.ai/docs/st
+00001d20: 6162 6c65 2f69 6e73 7461 6c6c 2f69 6e73  able/install/ins
+00001d30: 7461 6c6c 6174 696f 6e2e 6874 6d6c 292e  tallation.html).
+00001d40: 0a0a 2d20 5079 7468 6f6e 2033 2e38 2e78  ..- Python 3.8.x
+00001d50: 206f 7220 6c61 7465 7220 2833 2e38 2e78   or later (3.8.x
+00001d60: 2c20 332e 392e 782c 2033 2e31 302e 782c  , 3.9.x, 3.10.x,
+00001d70: 202e 2e2e 290a 0a3c 2f64 6574 6169 6c73   ...)..</details
+00001d80: 3e0a 0a60 6060 6261 7368 0a70 6970 2069  >..```bash.pip i
+00001d90: 6e73 7461 6c6c 202d 5520 6c69 6768 746e  nstall -U lightn
+00001da0: 696e 670a 6060 600a 0a23 2320 436f 6e76  ing.```..## Conv
+00001db0: 6572 7420 796f 7572 2050 7954 6f72 6368  ert your PyTorch
+00001dc0: 2074 6f20 4661 6272 6963 0a0a 312e 2043   to Fabric..1. C
+00001dd0: 7265 6174 6520 7468 6520 6046 6162 7269  reate the `Fabri
+00001de0: 6360 206f 626a 6563 7420 6174 2074 6865  c` object at the
+00001df0: 2062 6567 696e 6e69 6e67 206f 6620 796f   beginning of yo
+00001e00: 7572 2074 7261 696e 696e 6720 636f 6465  ur training code
+00001e10: 2e0a 0a20 2020 6060 600a 2020 2069 6d70  ...   ```.   imp
+00001e20: 6f72 7420 4c69 6768 746e 696e 6720 6173  ort Lightning as
+00001e30: 204c 0a0a 2020 2066 6162 7269 6320 3d20   L..   fabric = 
+00001e40: 4c2e 4661 6272 6963 2829 0a20 2020 6060  L.Fabric().   ``
+00001e50: 600a 0a31 2e20 4361 6c6c 2060 7365 7475  `..1. Call `setu
+00001e60: 7028 2960 206f 6e20 6561 6368 206d 6f64  p()` on each mod
+00001e70: 656c 2061 6e64 206f 7074 696d 697a 6572  el and optimizer
+00001e80: 2070 6169 7220 616e 6420 6073 6574 7570   pair and `setup
+00001e90: 5f64 6174 616c 6f61 6465 7273 2829 6020  _dataloaders()` 
+00001ea0: 6f6e 2061 6c6c 2079 6f75 7220 6461 7461  on all your data
+00001eb0: 206c 6f61 6465 7273 2e0a 0a20 2020 6060   loaders...   ``
+00001ec0: 600a 2020 206d 6f64 656c 2c20 6f70 7469  `.   model, opti
+00001ed0: 6d69 7a65 7220 3d20 6661 6272 6963 2e73  mizer = fabric.s
+00001ee0: 6574 7570 286d 6f64 656c 2c20 6f70 7469  etup(model, opti
+00001ef0: 6d69 7a65 7229 0a20 2020 6461 7461 6c6f  mizer).   datalo
+00001f00: 6164 6572 203d 2066 6162 7269 632e 7365  ader = fabric.se
+00001f10: 7475 705f 6461 7461 6c6f 6164 6572 7328  tup_dataloaders(
+00001f20: 6461 7461 6c6f 6164 6572 290a 2020 2060  dataloader).   `
+00001f30: 6060 0a0a 312e 2052 656d 6f76 6520 616c  ``..1. Remove al
+00001f40: 6c20 602e 746f 6020 616e 6420 602e 6375  l `.to` and `.cu
+00001f50: 6461 6020 6361 6c6c 7320 2d3e 2046 6162  da` calls -> Fab
+00001f60: 7269 6320 7769 6c6c 2074 616b 6520 6361  ric will take ca
+00001f70: 7265 206f 6620 6974 2e0a 0a20 2020 6060  re of it...   ``
+00001f80: 6064 6966 660a 2020 202d 206d 6f64 656c  `diff.   - model
+00001f90: 2e74 6f28 6465 7669 6365 290a 2020 202d  .to(device).   -
+00001fa0: 2062 6174 6368 2e74 6f28 6465 7669 6365   batch.to(device
+00001fb0: 290a 2020 2060 6060 0a0a 312e 2052 6570  ).   ```..1. Rep
+00001fc0: 6c61 6365 2060 6c6f 7373 2e62 6163 6b77  lace `loss.backw
+00001fd0: 6172 6428 2960 2062 7920 6066 6162 7269  ard()` by `fabri
+00001fe0: 632e 6261 636b 7761 7264 286c 6f73 7329  c.backward(loss)
+00001ff0: 602e 0a0a 2020 2060 6060 6469 6666 0a20  `...   ```diff. 
+00002000: 2020 2d20 6c6f 7373 2e62 6163 6b77 6172    - loss.backwar
+00002010: 6428 290a 2020 202b 2066 6162 7269 632e  d().   + fabric.
+00002020: 6261 636b 7761 7264 286c 6f73 7329 0a20  backward(loss). 
+00002030: 2020 6060 600a 0a31 2e20 5275 6e20 7468    ```..1. Run th
+00002040: 6520 7363 7269 7074 2066 726f 6d20 7468  e script from th
+00002050: 6520 7465 726d 696e 616c 2077 6974 680a  e terminal with.
+00002060: 0a20 2020 6060 6062 6173 680a 2020 206c  .   ```bash.   l
+00002070: 6967 6874 6e69 6e67 2072 756e 206d 6f64  ightning run mod
+00002080: 656c 2070 6174 682f 746f 2f74 7261 696e  el path/to/train
+00002090: 2e70 790a 2020 2060 6060 0a0a 6f72 2075  .py.   ```..or u
+000020a0: 7365 2074 6865 206c 6175 6e63 6828 2920  se the launch() 
+000020b0: 6d65 7468 6f64 2069 6e20 6120 6e6f 7465  method in a note
+000020c0: 626f 6f6b 2e20 4c65 6172 6e20 6d6f 7265  book. Learn more
+000020d0: 2061 626f 7574 205b 6c61 756e 6368 696e   about [launchin
+000020e0: 6720 6469 7374 7269 6275 7465 6420 7472  g distributed tr
+000020f0: 6169 6e69 6e67 5d28 6874 7470 733a 2f2f  aining](https://
+00002100: 6c69 6768 746e 696e 672e 6169 2f64 6f63  lightning.ai/doc
+00002110: 732f 6661 6272 6963 2f73 7461 626c 652f  s/fabric/stable/
+00002120: 6675 6e64 616d 656e 7461 6c73 2f6c 6175  fundamentals/lau
+00002130: 6e63 682e 6874 6d6c 292e 0a0a 5f5f 5f5f  nch.html)...____
+00002140: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002150: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002160: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002170: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002180: 5f5f 0a0a 2320 4641 510a 0a23 2320 5768  __..# FAQ..## Wh
+00002190: 656e 2074 6f20 7573 6520 4661 6272 6963  en to use Fabric
+000021a0: 3f0a 0a2d 202a 2a4d 696e 696d 756d 2063  ?..- **Minimum c
+000021b0: 6f64 6520 6368 616e 6765 732a 2a2d 2059  ode changes**- Y
+000021c0: 6f75 2077 616e 7420 746f 2073 6361 6c65  ou want to scale
+000021d0: 2079 6f75 7220 5079 546f 7263 6820 6d6f   your PyTorch mo
+000021e0: 6465 6c20 746f 2075 7365 206d 756c 7469  del to use multi
+000021f0: 2d47 5055 206f 7220 7573 6520 6164 7661  -GPU or use adva
+00002200: 6e63 6564 2073 7472 6174 6567 6965 7320  nced strategies 
+00002210: 6c69 6b65 2044 6565 7053 7065 6564 2077  like DeepSpeed w
+00002220: 6974 686f 7574 2068 6176 696e 6720 746f  ithout having to
+00002230: 2072 6566 6163 746f 722e 2059 6f75 2064   refactor. You d
+00002240: 6f6e e280 9974 2063 6172 6520 6162 6f75  on...t care abou
+00002250: 7420 7374 7275 6374 7572 696e 6720 796f  t structuring yo
+00002260: 7572 2063 6f64 652d 2079 6f75 206a 7573  ur code- you jus
+00002270: 7420 7761 6e74 2074 6f20 7363 616c 6520  t want to scale 
+00002280: 6974 2061 7320 6661 7374 2061 7320 706f  it as fast as po
+00002290: 7373 6962 6c65 2e0a 2d20 2a2a 4d61 786d  ssible..- **Maxm
+000022a0: 6975 6d20 636f 6e74 726f 6c2a 2a2d 2057  ium control**- W
+000022b0: 7269 7465 2079 6f75 7220 6f77 6e20 7472  rite your own tr
+000022c0: 6169 6e69 6e67 2061 6e64 2f6f 7220 696e  aining and/or in
+000022d0: 6665 7265 6e63 6520 6c6f 6769 6320 646f  ference logic do
+000022e0: 776e 2074 6f20 7468 6520 696e 6469 7669  wn to the indivi
+000022f0: 6475 616c 206f 7074 696d 697a 6572 2063  dual optimizer c
+00002300: 616c 6c73 2e20 596f 7520 6172 656e e280  alls. You aren..
+00002310: 9974 2066 6f72 6365 6420 746f 2063 6f6e  .t forced to con
+00002320: 666f 726d 2074 6f20 6120 7374 616e 6461  form to a standa
+00002330: 7264 697a 6564 2065 706f 6368 2d62 6173  rdized epoch-bas
+00002340: 6564 2074 7261 696e 696e 6720 6c6f 6f70  ed training loop
+00002350: 206c 696b 6520 7468 6520 6f6e 6520 696e   like the one in
+00002360: 204c 6967 6874 6e69 6e67 2054 7261 696e   Lightning Train
+00002370: 6572 2e20 596f 7520 6361 6e20 646f 2066  er. You can do f
+00002380: 6c65 7869 626c 6520 6974 6572 6174 696f  lexible iteratio
+00002390: 6e20 6261 7365 6420 7472 6169 6e69 6e67  n based training
+000023a0: 2c20 6d65 7461 2d6c 6561 726e 696e 672c  , meta-learning,
+000023b0: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
+000023c0: 6e20 616e 6420 6f74 6865 7220 7479 7065  n and other type
+000023d0: 7320 6f66 206f 7074 696d 697a 6174 696f  s of optimizatio
+000023e0: 6e20 616c 676f 7269 7468 6d73 2077 6974  n algorithms wit
+000023f0: 686f 7574 2064 6967 6769 6e67 2069 6e74  hout digging int
+00002400: 6f20 6672 616d 6577 6f72 6b20 696e 7465  o framework inte
+00002410: 726e 616c 732e 2054 6869 7320 616c 736f  rnals. This also
+00002420: 206d 616b 6573 2069 7420 7375 7065 7220   makes it super 
+00002430: 6561 7379 2074 6f20 6164 6f70 7420 4661  easy to adopt Fa
+00002440: 6272 6963 2069 6e20 6578 6973 7469 6e67  bric in existing
+00002450: 2050 7954 6f72 6368 2070 726f 6a65 6374   PyTorch project
+00002460: 7320 746f 2073 7065 6564 2d75 7020 616e  s to speed-up an
+00002470: 6420 7363 616c 6520 796f 7572 206d 6f64  d scale your mod
+00002480: 656c 7320 7769 7468 6f75 7420 7468 6520  els without the 
+00002490: 636f 6d70 726f 6d69 7365 206f 6e20 6c61  compromise on la
+000024a0: 7267 6520 7265 6661 6374 6f72 732e 204a  rge refactors. J
+000024b0: 7573 7420 7265 6d65 6d62 6572 3a20 5769  ust remember: Wi
+000024c0: 7468 2067 7265 6174 2070 6f77 6572 2063  th great power c
+000024d0: 6f6d 6573 2061 2067 7265 6174 2072 6573  omes a great res
+000024e0: 706f 6e73 6962 696c 6974 792e 0a2d 202a  ponsibility..- *
+000024f0: 2a4d 6178 6d69 756d 2066 6c65 7869 6269  *Maxmium flexibi
+00002500: 6c69 7479 2a2a 2d20 596f 7520 7761 6e74  lity**- You want
+00002510: 2074 6f20 6861 7665 2066 756c 6c20 636f   to have full co
+00002520: 6e74 726f 6c20 6f76 6572 2079 6f75 7220  ntrol over your 
+00002530: 656e 7469 7265 2074 7261 696e 696e 672d  entire training-
+00002540: 2069 6e20 4661 6272 6963 2061 6c6c 2066   in Fabric all f
+00002550: 6561 7475 7265 7320 6172 6520 6f70 742d  eatures are opt-
+00002560: 696e 2c20 616e 6420 6974 2070 726f 7669  in, and it provi
+00002570: 6465 7320 796f 7520 7769 7468 2061 2074  des you with a t
+00002580: 6f6f 6c20 626f 7820 6f66 2070 7269 6d69  ool box of primi
+00002590: 7469 7665 7320 736f 2079 6f75 2063 616e  tives so you can
+000025a0: 2062 7569 6c64 2079 6f75 7220 6f77 6e20   build your own 
+000025b0: 5472 6169 6e65 722e 0a0a 2323 2057 6865  Trainer...## Whe
+000025c0: 6e20 746f 2075 7365 2074 6865 205b 4c69  n to use the [Li
+000025d0: 6768 746e 696e 6720 5472 6169 6e65 725d  ghtning Trainer]
+000025e0: 2868 7474 7073 3a2f 2f6c 6967 6874 6e69  (https://lightni
+000025f0: 6e67 2e61 692f 646f 6373 2f70 7974 6f72  ng.ai/docs/pytor
+00002600: 6368 2f73 7461 626c 652f 636f 6d6d 6f6e  ch/stable/common
+00002610: 2f74 7261 696e 6572 2e68 746d 6c29 3f0a  /trainer.html)?.
+00002620: 0a2d 2059 6f75 2077 616e 7420 746f 2068  .- You want to h
+00002630: 6176 6520 616c 6c20 7468 6520 656e 6769  ave all the engi
+00002640: 6e65 6572 696e 6720 626f 696c 6572 706c  neering boilerpl
+00002650: 6174 6520 6861 6e64 6c65 6420 666f 7220  ate handled for 
+00002660: 796f 7520 2d20 646f 7a65 6e73 206f 6620  you - dozens of 
+00002670: 6665 6174 7572 6573 206c 696b 6520 6368  features like ch
+00002680: 6563 6b70 6f69 6e74 696e 672c 206c 6f67  eckpointing, log
+00002690: 6769 6e67 2061 6e64 2065 6172 6c79 2073  ging and early s
+000026a0: 746f 7070 696e 6720 6f75 7420 6f66 2074  topping out of t
+000026b0: 6865 2062 6f78 2e20 4c65 7373 2068 6173  he box. Less has
+000026c0: 736c 652c 206c 6573 7320 6572 726f 7220  sle, less error 
+000026d0: 7072 6f6e 652c 2065 6173 7920 746f 2074  prone, easy to t
+000026e0: 7279 2064 6966 6665 7265 6e74 2074 6563  ry different tec
+000026f0: 686e 6971 7565 7320 616e 6420 6665 6174  hniques and feat
+00002700: 7572 6573 2e0a 2d20 596f 7520 7761 6e74  ures..- You want
+00002710: 2074 6f20 6861 7665 2067 6f6f 6420 6465   to have good de
+00002720: 6661 756c 7473 2063 686f 7365 6e20 666f  faults chosen fo
+00002730: 7220 796f 7520 2d20 736f 2079 6f75 2063  r you - so you c
+00002740: 616e 2068 6176 6520 6120 6265 7474 6572  an have a better
+00002750: 2073 7461 7274 696e 6720 706f 696e 742e   starting point.
+00002760: 0a2d 2059 6f75 2077 616e 7420 796f 7572  .- You want your
+00002770: 2063 6f64 6520 746f 2062 6520 6d6f 6475   code to be modu
+00002780: 6c61 722c 2072 6561 6461 626c 6520 616e  lar, readable an
+00002790: 6420 7765 6c6c 2073 7472 7563 7475 7265  d well structure
+000027a0: 6420 2d20 6561 7379 2074 6f20 7368 6172  d - easy to shar
+000027b0: 6520 6265 7477 6565 6e20 7072 6f6a 6563  e between projec
+000027c0: 7473 2061 6e64 2077 6974 6820 636f 6c6c  ts and with coll
+000027d0: 6162 6f72 6174 6f72 732e 0a0a 2323 2043  aborators...## C
+000027e0: 616e 2049 2075 7365 2046 6162 7269 6320  an I use Fabric 
+000027f0: 7769 7468 206d 7920 4c69 6768 746e 696e  with my Lightnin
+00002800: 674d 6f64 756c 6520 6f72 204c 6967 6874  gModule or Light
+00002810: 6e69 6e67 2043 616c 6c62 6163 6b3f 0a0a  ning Callback?..
+00002820: 5965 7320 3a29 2046 6162 7269 6320 776f  Yes :) Fabric wo
+00002830: 726b 7320 7769 7468 2050 7954 6f72 6368  rks with PyTorch
+00002840: 204c 6967 6874 6e69 6e67 4d6f 6475 6c65   LightningModule
+00002850: 7320 616e 6420 4361 6c6c 6261 636b 732c  s and Callbacks,
+00002860: 2073 6f20 796f 7520 6361 6e20 6368 6f6f   so you can choo
+00002870: 7365 2068 6f77 2074 6f20 7374 7275 6374  se how to struct
+00002880: 7572 6520 796f 7572 2063 6f64 6520 616e  ure your code an
+00002890: 6420 7265 7573 6520 6578 6973 7469 6e67  d reuse existing
+000028a0: 206d 6f64 656c 7320 616e 6420 6361 6c6c   models and call
+000028b0: 6261 636b 7320 6173 2079 6f75 2077 6973  backs as you wis
+000028c0: 682e 2052 6561 6420 6d6f 7265 205b 6865  h. Read more [he
+000028d0: 7265 5d28 6874 7470 733a 2f2f 6c69 6768  re](https://ligh
+000028e0: 746e 696e 672e 6169 2f64 6f63 732f 6661  tning.ai/docs/fa
+000028f0: 6272 6963 2f73 7461 626c 652f 6675 6e64  bric/stable/fund
+00002900: 616d 656e 7461 6c73 2f63 6f64 655f 7374  amentals/code_st
+00002910: 7275 6374 7572 652e 6874 6d6c 292e 0a0a  ructure.html)...
+00002920: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00002930: 2f2f 706c 2d70 7562 6c69 632d 6461 7461  //pl-public-data
+00002940: 2e73 332e 616d 617a 6f6e 6177 732e 636f  .s3.amazonaws.co
+00002950: 6d2f 6173 7365 7473 5f6c 6967 6874 6e69  m/assets_lightni
+00002960: 6e67 2f63 6f6e 7469 6e75 756d 2e70 6e67  ng/continuum.png
+00002970: 2220 7769 6474 683d 2238 3030 7078 223e  " width="800px">
+00002980: 0a0a 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ..______________
+00002990: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000029a0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000029b0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000029c0: 5f5f 5f5f 5f5f 5f5f 0a0a 2320 4578 616d  ________..# Exam
+000029d0: 706c 6573 0a0a 2d20 5b47 414e 5d28 6874  ples..- [GAN](ht
+000029e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000029f0: 2f4c 6967 6874 6e69 6e67 2d41 492f 6c69  /Lightning-AI/li
+00002a00: 6768 746e 696e 672f 7472 6565 2f6d 6173  ghtning/tree/mas
+00002a10: 7465 722f 6578 616d 706c 6573 2f66 6162  ter/examples/fab
+00002a20: 7269 632f 6463 6761 6e29 0a2d 205b 4d65  ric/dcgan).- [Me
+00002a30: 7461 206c 6561 726e 696e 675d 2868 7474  ta learning](htt
+00002a40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002a50: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
+00002a60: 6874 6e69 6e67 2f74 7265 652f 6d61 7374  htning/tree/mast
+00002a70: 6572 2f65 7861 6d70 6c65 732f 6661 6272  er/examples/fabr
+00002a80: 6963 2f6d 6574 615f 6c65 6172 6e69 6e67  ic/meta_learning
+00002a90: 290a 2d20 5b52 6569 6e66 6f72 6365 6d65  ).- [Reinforceme
+00002aa0: 6e74 206c 6561 726e 696e 675d 2868 7474  nt learning](htt
+00002ab0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002ac0: 4c69 6768 746e 696e 672d 4149 2f6c 6967  Lightning-AI/lig
+00002ad0: 6874 6e69 6e67 2f74 7265 652f 6d61 7374  htning/tree/mast
+00002ae0: 6572 2f65 7861 6d70 6c65 732f 6661 6272  er/examples/fabr
+00002af0: 6963 2f72 6569 6e66 6f72 6365 6d65 6e74  ic/reinforcement
+00002b00: 5f6c 6561 726e 696e 6729 0a2d 205b 4b2d  _learning).- [K-
+00002b10: 466f 6c64 2063 726f 7373 2076 616c 6964  Fold cross valid
+00002b20: 6174 696f 6e5d 2868 7474 7073 3a2f 2f67  ation](https://g
+00002b30: 6974 6875 622e 636f 6d2f 4c69 6768 746e  ithub.com/Lightn
+00002b40: 696e 672d 4149 2f6c 6967 6874 6e69 6e67  ing-AI/lightning
+00002b50: 2f74 7265 652f 6d61 7374 6572 2f65 7861  /tree/master/exa
+00002b60: 6d70 6c65 732f 6661 6272 6963 2f6b 666f  mples/fabric/kfo
+00002b70: 6c64 5f63 7629 0a0a 5f5f 5f5f 5f5f 5f5f  ld_cv)..________
+00002b80: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002b90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002ba0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00002bb0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0a0a  ______________..
+00002bc0: 2323 2041 736b 696e 6720 666f 7220 6865  ## Asking for he
+00002bd0: 6c70 0a0a 4966 2079 6f75 2068 6176 6520  lp..If you have 
+00002be0: 616e 7920 7175 6573 7469 6f6e 7320 706c  any questions pl
+00002bf0: 6561 7365 3a0a 0a31 2e20 5b52 6561 6420  ease:..1. [Read 
+00002c00: 7468 6520 646f 6373 5d28 6874 7470 733a  the docs](https:
+00002c10: 2f2f 6c69 6768 746e 696e 672e 6169 2f64  //lightning.ai/d
+00002c20: 6f63 732f 6661 6272 6963 292e 0a31 2e20  ocs/fabric)..1. 
+00002c30: 5b41 736b 2061 2071 7565 7374 696f 6e20  [Ask a question 
+00002c40: 696e 206f 7572 2066 6f72 756d 5d28 6874  in our forum](ht
+00002c50: 7470 733a 2f2f 6c69 6768 746e 696e 672e  tps://lightning.
+00002c60: 6169 2f66 6f72 756d 732f 292e 0a31 2e20  ai/forums/)..1. 
+00002c70: 5b4a 6f69 6e20 6f75 7220 6469 7363 6f72  [Join our discor
+00002c80: 6420 636f 6d6d 756e 6974 795d 2868 7474  d community](htt
+00002c90: 7073 3a2f 2f64 6973 636f 7264 2e63 6f6d  ps://discord.com
+00002ca0: 2f69 6e76 6974 652f 7466 5846 6574 455a  /invite/tfXFetEZ
+00002cb0: 7876 292e 0a0a 0a                        xv)....
```

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/SOURCES.txt` & `lightning-fabric-2.0.2/src/lightning_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.1.post0/src/lightning_fabric.egg-info/requires.txt` & `lightning-fabric-2.0.2/src/lightning_fabric.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 deepspeed>=0.6.0
 
 [dev]
 torchvision>=0.10.0
 torchmetrics>=0.10.0
 lightning-utilities>=0.8.0
 coverage==6.5.0
-codecov==2.1.12
 pytest==7.2.0
 pytest-cov==4.0.0
 pytest-rerunfailures==10.3
 click==8.1.3
 tensorboardX>=2.2
 
 [dev:platform_system != "Windows"]
@@ -41,13 +40,12 @@
 [strategies]
 
 [strategies:platform_system != "Windows"]
 deepspeed>=0.6.0
 
 [test]
 coverage==6.5.0
-codecov==2.1.12
 pytest==7.2.0
 pytest-cov==4.0.0
 pytest-rerunfailures==10.3
 click==8.1.3
 tensorboardX>=2.2
```

