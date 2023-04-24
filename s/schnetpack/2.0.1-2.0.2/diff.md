# Comparing `tmp/schnetpack-2.0.1.tar.gz` & `tmp/schnetpack-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schnetpack-2.0.1.tar", last modified: Tue Mar  7 18:21:37 2023, max compression
+gzip compressed data, was "schnetpack-2.0.2.tar", last modified: Mon Apr 24 09:40:30 2023, max compression
```

## Comparing `schnetpack-2.0.1.tar` & `schnetpack-2.0.2.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.982693 schnetpack-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-07 18:21:28.000000 schnetpack-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-07 18:21:28.000000 schnetpack-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-07 18:21:37.982693 schnetpack-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-03-07 18:21:28.000000 schnetpack-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 18:21:37.982693 schnetpack-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-07 18:21:28.000000 schnetpack-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.942694 schnetpack-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.946694 schnetpack-2.0.1/src/schnetpack/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.946694 schnetpack-2.0.1/src/schnetpack/atomistic/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/atomwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/electrostatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/external_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/nuclear_repulsion.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/atomistic/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.946694 schnetpack-2.0.1/src/schnetpack/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.946694 schnetpack-2.0.1/src/schnetpack/configs/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/callbacks/checkpoint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/callbacks/earlystopping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/callbacks/ema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/callbacks/lrmonitor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.946694 schnetpack-2.0.1/src/schnetpack/configs/data/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/ani1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/custom.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/iso17.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/materials_project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/md17.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/md22.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/omdb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/qm9.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/data/rmd17.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/experiment/md17.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/experiment/qm9_atomwise.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/experiment/qm9_dipole.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/experiment/response.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/globals/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/globals/default_globals.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/logger/aim.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/logger/csv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/logger/tensorboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/model/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/model/nnp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/model/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/model/representation/field_schnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/model/representation/painn.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/model/representation/radial_basis/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/model/representation/radial_basis/bessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/model/representation/radial_basis/gaussian.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/model/representation/schnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/model/representation/so3net.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/predict.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/run/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/run/default_run.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.950693 schnetpack-2.0.1/src/schnetpack/configs/task/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/task/default_task.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.954693 schnetpack-2.0.1/src/schnetpack/configs/task/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/task/optimizer/adabelief.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/task/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/task/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.954693 schnetpack-2.0.1/src/schnetpack/configs/task/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/task/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/train.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.954693 schnetpack-2.0.1/src/schnetpack/configs/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/trainer/ddp_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/trainer/ddp_trainer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/trainer/debug_trainer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/configs/trainer/default_trainer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.954693 schnetpack-2.0.1/src/schnetpack/data/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/data/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/data/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/data/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.958693 schnetpack-2.0.1/src/schnetpack/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/ani1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/iso17.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/md17.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/md22.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/omdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/qm9.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/datasets/rmd17.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.958693 schnetpack-2.0.1/src/schnetpack/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/interfaces/ase_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/interfaces/batchwise_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.958693 schnetpack-2.0.1/src/schnetpack/md/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.962693 schnetpack-2.0.1/src/schnetpack/md/calculators/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/calculators/base_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/calculators/ensemble_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/calculators/lj_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/calculators/orca_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/calculators/schnetpack_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.962693 schnetpack-2.0.1/src/schnetpack/md/data/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/data/hdf5_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/data/spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.962693 schnetpack-2.0.1/src/schnetpack/md/md_configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.962693 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/lj.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.962693 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/neighbor_list/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/neighbor_list/ase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/neighbor_list/matscipy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/neighbor_list/torch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/orca.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/spk.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/calculator/spk_ensemble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.962693 schnetpack-2.0.1/src/schnetpack/md/md_configs/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/callbacks/checkpoint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/callbacks/hdf5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/callbacks/tensorboard.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.966693 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.966693 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/barostat/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/barostat/nhc_aniso.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/barostat/nhc_iso.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/barostat/pile_rpmd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.966693 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/integrator/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/integrator/md.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/integrator/rpmd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.966693 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/berendsen.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/gle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/langevin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/nhc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/pi_gle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_global.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/piglet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/pile_global.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/pile_local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/dynamics/thermostat/trpmd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.970693 schnetpack-2.0.1/src/schnetpack/md/md_configs/system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.970693 schnetpack-2.0.1/src/schnetpack/md/md_configs/system/initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/system/initializer/maxwell_boltzmann.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/system/initializer/uniform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/md_configs/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/neighborlist_md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.970693 schnetpack-2.0.1/src/schnetpack/md/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27148 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/parsers/orca_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.970693 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/barostats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/barostats_rpmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/basic_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/callback_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/thermostats.py
--rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25557 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.970693 schnetpack-2.0.1/src/schnetpack/md/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/utils/md_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/utils/normal_model_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/md/utils/thermostat_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.970693 schnetpack-2.0.1/src/schnetpack/model/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.974693 schnetpack-2.0.1/src/schnetpack/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/equivariant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.974693 schnetpack-2.0.1/src/schnetpack/nn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/ops/so3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/radial.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/so3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.978693 schnetpack-2.0.1/src/schnetpack/representation/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/representation/field_schnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/representation/painn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/representation/schnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/representation/so3net.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.978693 schnetpack-2.0.1/src/schnetpack/train/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/train/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/train/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/train/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.978693 schnetpack-2.0.1/src/schnetpack/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/transform/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/transform/casting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24697 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/transform/neighborlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/transform/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.978693 schnetpack-2.0.1/src/schnetpack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/schnetpack/utils/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.946694 schnetpack-2.0.1/src/schnetpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-07 18:21:37.000000 schnetpack-2.0.1/src/schnetpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-03-07 18:21:37.000000 schnetpack-2.0.1/src/schnetpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 18:21:37.000000 schnetpack-2.0.1/src/schnetpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-07 18:21:37.000000 schnetpack-2.0.1/src/schnetpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-07 18:21:37.000000 schnetpack-2.0.1/src/schnetpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:21:37.978693 schnetpack-2.0.1/src/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/scripts/spkconvert
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/scripts/spkdeploy
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/scripts/spkmd
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/scripts/spkpredict
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-07 18:21:28.000000 schnetpack-2.0.1/src/scripts/spktrain
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 09:40:20.000000 schnetpack-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 09:40:20.000000 schnetpack-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 09:40:30.381232 schnetpack-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-04-24 09:40:20.000000 schnetpack-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:40:30.381232 schnetpack-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 09:40:20.000000 schnetpack-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/atomistic/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/atomwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/electrostatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/external_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/nuclear_repulsion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/atomistic/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack/configs/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/checkpoint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/earlystopping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/ema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/callbacks/lrmonitor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/ani1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/custom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/iso17.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/materials_project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/md17.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/md22.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/omdb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/qm9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/data/rmd17.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/md17.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_atomwise.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_dipole.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/experiment/response.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/globals/default_globals.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/logger/aim.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/logger/csv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/logger/tensorboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/nnp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/model/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/field_schnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/painn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/model/representation/radial_basis/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/radial_basis/bessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/radial_basis/gaussian.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/schnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/model/representation/so3net.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/predict.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/run/default_run.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/default_task.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/adabelief.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/task/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/task/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/train.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/configs/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/ddp_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/ddp_trainer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/debug_trainer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/configs/trainer/default_trainer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.369232 schnetpack-2.0.2/src/schnetpack/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/data/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/ani1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/iso17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/md17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/md22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/omdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/qm9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/datasets/rmd17.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/interfaces/ase_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28296 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/interfaces/batchwise_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/calculators/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/base_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/ensemble_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/lj_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/orca_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/calculators/schnetpack_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/data/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/data/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/md_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/lj.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.373232 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/ase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/matscipy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/neighbor_list/torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/orca.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/spk.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/calculator/spk_ensemble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/checkpoint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/hdf5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/callbacks/tensorboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/nhc_aniso.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/nhc_iso.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/barostat/pile_rpmd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/integrator/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/integrator/md.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/integrator/rpmd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/berendsen.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/gle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/langevin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/nhc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pi_gle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_global.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pi_nhc_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/piglet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pile_global.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/pile_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/dynamics/thermostat/trpmd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/initializer/maxwell_boltzmann.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/initializer/uniform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/md_configs/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/neighborlist_md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27148 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/parsers/orca_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats_rpmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/basic_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31159 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/callback_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25557 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/md/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/md_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/normal_model_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/md/utils/thermostat_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.377232 schnetpack-2.0.2/src/schnetpack/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/equivariant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/nn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/ops/so3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/radial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/so3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/field_schnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/painn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/schnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/representation/so3net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/train/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/train/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/casting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/neighborlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/transform/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/schnetpack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/schnetpack/utils/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.365232 schnetpack-2.0.2/src/schnetpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 09:40:30.000000 schnetpack-2.0.2/src/schnetpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:40:30.381232 schnetpack-2.0.2/src/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkconvert
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkdeploy
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkmd
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spkpredict
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 09:40:20.000000 schnetpack-2.0.2/src/scripts/spktrain
```

### Comparing `schnetpack-2.0.1/LICENSE` & `schnetpack-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/PKG-INFO` & `schnetpack-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schnetpack
-Version: 2.0.1
+Version: 2.0.2
 Summary: SchNetPack - Deep Neural Networks for Atomistic Systems
 Home-page: https://github.com/atomistic-machine-learning/schnetpack
 Author: Kristof T. Schuett, Michael Gastegger, Stefaan Hessmann, Niklas Gebauer, Jonas Lederer
 License: MIT
 Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `schnetpack-2.0.1/README.md` & `schnetpack-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/setup.py` & `schnetpack-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with io.open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="schnetpack",
-    version="2.0.1",
+    version="2.0.2",
     author="Kristof T. Schuett, Michael Gastegger, Stefaan Hessmann, Niklas Gebauer, Jonas Lederer",
     url="https://github.com/atomistic-machine-learning/schnetpack",
     packages=find_packages("src"),
     scripts=[
         "src/scripts/spkconvert",
         "src/scripts/spktrain",
         "src/scripts/spkpredict",
@@ -28,15 +28,15 @@
         "numpy",
         "sympy",
         "ase>=3.21",
         "h5py",
         "pyyaml",
         "hydra-core>=1.1.0",
         "torch>=1.9",
-        "pytorch_lightning>=1.9.0",
+        "pytorch_lightning>=2.0.0",
         "torchmetrics",
         "hydra-colorlog>=1.1.0",
         "rich",
         "fasteners",
         "dirsync",
         "torch-ema",
         "matscipy",
```

### Comparing `schnetpack-2.0.1/src/schnetpack/atomistic/aggregation.py` & `schnetpack-2.0.2/src/schnetpack/atomistic/aggregation.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/atomistic/atomwise.py` & `schnetpack-2.0.2/src/schnetpack/atomistic/atomwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             n_layers: number of layers.
             aggregation_mode: one of {sum, avg} (default: sum)
             output_key: the key under which the result will be stored
             per_atom_output_key: If not None, the key under which the per-atom result will be stored
         """
         super(Atomwise, self).__init__()
         self.output_key = output_key
-        self.model_outputs = [output_key]
+        self.model_outputs = [output_key, per_atom_output_key]
         self.per_atom_output_key = per_atom_output_key
         self.n_out = n_out
 
         if aggregation_mode is None and self.per_atom_output_key is None:
             raise ValueError(
                 "If `aggregation_mode` is None, `per_atom_output_key` needs to be set,"
                 + " since no accumulated output will be returned!"
@@ -64,14 +64,18 @@
         )
         self.aggregation_mode = aggregation_mode
 
     def forward(self, inputs: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         # predict atomwise contributions
         y = self.outnet(inputs["scalar_representation"])
 
+        # accumulate the per-atom output if necessary
+        if self.per_atom_output_key is not None:
+            inputs[self.per_atom_output_key] = y
+
         # aggregate
         if self.aggregation_mode is not None:
             idx_m = inputs[properties.idx_m]
             maxm = int(idx_m[-1]) + 1
             y = snn.scatter_add(y, idx_m, dim_size=maxm)
             y = torch.squeeze(y, -1)
```

### Comparing `schnetpack-2.0.1/src/schnetpack/atomistic/distances.py` & `schnetpack-2.0.2/src/schnetpack/atomistic/distances.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/atomistic/electrostatic.py` & `schnetpack-2.0.2/src/schnetpack/atomistic/electrostatic.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/atomistic/external_fields.py` & `schnetpack-2.0.2/src/schnetpack/atomistic/external_fields.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/atomistic/nuclear_repulsion.py` & `schnetpack-2.0.2/src/schnetpack/atomistic/nuclear_repulsion.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/atomistic/response.py` & `schnetpack-2.0.2/src/schnetpack/atomistic/response.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/cli.py` & `schnetpack-2.0.2/src/schnetpack/cli.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/configs/experiment/md17.yaml` & `schnetpack-2.0.2/src/schnetpack/configs/experiment/md17.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/configs/experiment/qm9_atomwise.yaml` & `schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_atomwise.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/configs/experiment/qm9_dipole.yaml` & `schnetpack-2.0.2/src/schnetpack/configs/experiment/qm9_dipole.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/configs/experiment/response.yaml` & `schnetpack-2.0.2/src/schnetpack/configs/experiment/response.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/configs/predict.yaml` & `schnetpack-2.0.2/src/schnetpack/configs/predict.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/configs/train.yaml` & `schnetpack-2.0.2/src/schnetpack/configs/train.yaml`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/data/atoms.py` & `schnetpack-2.0.2/src/schnetpack/data/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         transforms: Optional[List[Transform]] = None,
         subset_idx: Optional[List[int]] = None,
     ):
         """
         Args:
             load_properties: Set of properties to be loaded and returned.
                 If None, all properties in the ASE dB will be returned.
-            load_properties: If True, load structure properties.
+            load_structure: If True, load structure properties.
             transforms: preprocessing transforms (see schnetpack.data.transforms)
             subset: List of data indices.
         """
         self._transform_module = None
         self.load_properties = load_properties
         self.load_structure = load_structure
         self.transforms = transforms
@@ -116,15 +116,18 @@
     def units(self) -> Dict[str, str]:
         """Property to unit dict"""
         pass
 
     @property
     def load_properties(self) -> List[str]:
         """Properties to be loaded"""
-        return self._load_properties or self.available_properties
+        if self._load_properties is None:
+            return self.available_properties
+        else:
+            return self._load_properties
 
     @load_properties.setter
     def load_properties(self, val: List[str]):
         if val is not None:
             props = self.available_properties
             assert all(
                 [p in props for p in val]
@@ -198,15 +201,15 @@
         distance_unit: Optional[str] = None,
     ):
         """
         Args:
             datapath: Path to ASE DB.
             load_properties: Set of properties to be loaded and returned.
                 If None, all properties in the ASE dB will be returned.
-            load_properties: If True, load structure properties.
+            load_structure: If True, load structure properties.
             transforms: preprocessing torch.nn.Module (see schnetpack.data.transforms)
             subset_idx: List of data indices.
             units: property-> unit string dictionary that overwrites the native units
                 of the dataset. Units are converted automatically during loading.
         """
         self.datapath = datapath
 
@@ -299,15 +302,16 @@
             load_properties (sequence or None): subset of available properties to load
             load_structure: load and return structure
 
         Returns:
             properties (dict): dictionary with molecular properties
 
         """
-        load_properties = load_properties or self.load_properties
+        if load_properties is None:
+            load_properties = self.load_properties
         load_structure = load_structure or self.load_structure
 
         if self.subset_idx:
             if indices is None:
                 indices = self.subset_idx
             elif type(indices) is int:
                 indices = [self.subset_idx[indices]]
```

### Comparing `schnetpack-2.0.1/src/schnetpack/data/datamodule.py` & `schnetpack-2.0.2/src/schnetpack/data/datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Optional, List, Dict, Tuple, Union
 
 
 import numpy as np
 import fasteners
 
 import pytorch_lightning as pl
-from pytorch_lightning.accelerators import GPUAccelerator
 import torch
 
 from schnetpack.data import (
     AtomsDataFormat,
     resolve_format,
     load_dataset,
     BaseAtomsData,
@@ -113,16 +112,20 @@
         self.num_val = num_val
         self.num_test = num_test
         self.splitting = splitting or RandomSplit()
         self.split_file = split_file
         self.datapath, self.format = resolve_format(datapath, format)
         self.load_properties = load_properties
         self.num_workers = num_workers
-        self.num_val_workers = num_val_workers or self.num_workers
-        self.num_test_workers = num_test_workers or self.num_workers
+        self.num_val_workers = self.num_workers
+        self.num_test_workers = self.num_workers
+        if num_val_workers is not None:
+            self.num_val_workers = num_val_workers
+        if num_test_workers is not None:
+            self.num_test_workers = num_test_workers
         self.property_units = property_units
         self.distance_unit = distance_unit
         self._stats = {}
         self._is_setup = False
         self.data_workdir = data_workdir
         self.cleanup_workdir_stage = cleanup_workdir_stage
         self._pin_memory = pin_memory
```

### Comparing `schnetpack-2.0.1/src/schnetpack/data/loader.py` & `schnetpack-2.0.2/src/schnetpack/data/loader.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/data/splitting.py` & `schnetpack-2.0.2/src/schnetpack/data/splitting.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/data/stats.py` & `schnetpack-2.0.2/src/schnetpack/data/stats.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/ani1.py` & `schnetpack-2.0.2/src/schnetpack/datasets/ani1.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/iso17.py` & `schnetpack-2.0.2/src/schnetpack/datasets/iso17.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/materials_project.py` & `schnetpack-2.0.2/src/schnetpack/datasets/materials_project.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/md17.py` & `schnetpack-2.0.2/src/schnetpack/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/md22.py` & `schnetpack-2.0.2/src/schnetpack/datasets/md22.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/omdb.py` & `schnetpack-2.0.2/src/schnetpack/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/qm9.py` & `schnetpack-2.0.2/src/schnetpack/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/datasets/rmd17.py` & `schnetpack-2.0.2/src/schnetpack/datasets/rmd17.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/interfaces/ase_interface.py` & `schnetpack-2.0.2/src/schnetpack/interfaces/ase_interface.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/interfaces/batchwise_optimizer.py` & `schnetpack-2.0.2/src/schnetpack/md/system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,712 +1,704 @@
+"""
+This module is used to store all information on the simulated atomistic systems.
+It includes functionality for loading molecules from files.
+All this functionality is encoded in the :obj:`schnetpack.md.System` class.
+"""
 import torch
-import pickle
-import time
-import numpy as np
-from math import sqrt
-from os.path import isfile
-
-from ase.optimize.optimize import Dynamics
-from ase.parallel import world, barrier
-from ase.io import write
+import torch.nn as nn
+
+from schnetpack.md.utils import NormalModeTransformer
 from ase import Atoms
 
-from schnetpack import properties
-from schnetpack.units import convert_units
+from typing import Union, List, OrderedDict
+
+from schnetpack import units as spk_units
+from schnetpack.md.utils import UninitializedMixin
+
+__all__ = ["System"]
 
 
-__all__ = ["ASEBatchwiseLBFGS"]
+class SystemException(Exception):
+    pass
 
 
-class BatchwiseDynamics(Dynamics):
-    """Base-class for batch-wise MD and structure optimization classes."""
+class SystemWarning(Warning):
+    pass
 
-    energy = "energy"
-    forces = "forces"
-    stress = "stress"
+
+class System(UninitializedMixin, nn.Module):
+    """
+    Container for all properties associated with the simulated molecular system
+    (masses, positions, momenta, ...). Uses MD unit system defined in `schnetpack.units` internally.
+
+    In order to simulate multiple systems efficiently dynamics properties
+    (positions, momenta, forces) are torch tensors with the following
+    dimensions:
+        n_replicas x (n_molecules * n_atoms) x 3
+
+    Here n_replicas is the number of copies for every molecule. In a normal
+    simulation, these are treated as independent molecules e.g. for sampling
+    purposes. In the case of ring polymer molecular dynamics (using the
+    RingPolymer integrator), these replicas correspond to the beads of the
+    polymer. n_molecules is the number of different molecules constituting
+    the system, these can e.g. be different initial configurations of the
+    same system (once again for sampling) or completely different molecules.
+    Atoms of multiple molecules are concatenated.
+
+    Static properties are stored in tensors of the shape:
+        n_atoms : n_molecules (the same for all replicas)
+        masses : 1 x (n_molecules * n_atoms) x 1 (the same for all replicas)
+        atom_types : (n_molecules * n_atoms)
+        index_m : (n_molecules * n_atoms)
+
+    `n_atoms` contains the number of atoms present in every molecule, `masses`
+    and `atom_types` contain the molcular masses and nuclear charges.
+    `index_m` is an index for mapping atoms to individual molecules.
+
+    Finally a dictionary properties stores the results of every calculator
+    call for easy access of e.g. energies and dipole moments.
+
+    Args:
+        device (str, torch.device): Computation device (default='cuda').
+        precision (int, torch.dtype): Precision used for floating point numbers (default=32).
+    """
+
+    # Property dictionary, updated during simulation
+    properties = {}
 
     def __init__(
+        self, normal_mode_transform: NormalModeTransformer = NormalModeTransformer
+    ):
+        super(System, self).__init__()
+
+        self._nm_transformer = normal_mode_transform
+        # For initialized nm transform
+        self.nm_transform = None
+
+        # Index for aggregation
+        self.register_uninitialized_buffer("index_m", dtype=torch.long)
+
+        # number of molecules, replicas of each and vector with the number of
+        # atoms in each molecule
+        self.n_replicas = None
+        self.n_molecules = None
+        self.total_n_atoms = None
+
+        # General static molecular properties
+        self.register_uninitialized_buffer("n_atoms", dtype=torch.long)
+        self.register_uninitialized_buffer("atom_types", dtype=torch.long)
+        self.register_uninitialized_buffer("masses")
+
+        # Dynamic properties updated during simulation
+        self.register_uninitialized_buffer("positions")
+        self.register_uninitialized_buffer("momenta")
+        self.register_uninitialized_buffer("forces")
+        self.register_uninitialized_buffer("energy")
+
+        # Properties for periodic boundary conditions and crystal cells
+        self.register_uninitialized_buffer("cells")
+        self.register_uninitialized_buffer("pbc")
+        self.register_uninitialized_buffer(
+            "stress"
+        )  # Used for the computation of the pressure
+
+        # Dummy tensor for device and dtype
+        self.register_buffer("_dd_dummy", torch.zeros(1))
+
+    @property
+    def device(self):
+        return self._dd_dummy.device
+
+    @property
+    def dtype(self):
+        return self._dd_dummy.dtype
+
+    def load_molecules(
         self,
-        model,
-        atoms,
-        converter,
-        logfile,
-        trajectory,
-        fixed_atoms_mask=None,
-        append_trajectory=False,
-        master=None,
-        energy_key="energy",
-        force_key="forces",
-        energy_unit="eV",
-        position_unit="Ang",
-        log_every_step=False,
+        molecules: Union[Atoms, List[Atoms]],
+        n_replicas: int = 1,
+        position_unit_input: Union[str, float] = "Angstrom",
+        mass_unit_input: Union[str, float] = 1.0,
     ):
-        """Structure dynamics object.
+        """
+        Initializes all required variables and tensors based on a list of ASE
+        atoms objects.
 
-        Parameters:
+        Args:
+            molecules (ase.Atoms, list(ase.Atoms)): List of ASE atoms objects containing
+                molecular structures and chemical elements.
+            n_replicas (int): Number of replicas (e.g. for RPMD)
+            position_unit_input (str, float): Position units of the input structures (default="Angstrom")
+            mass_unit_input (str, float): Units of masses passed in the ASE atoms. Assumed to be Dalton.
+        """
+        self.n_replicas = n_replicas
 
-        model: torch.nn.Module
-            The force field model used to calculate the respective atomic forces
+        # TODO: make cells/PBC False if not set?
 
-        atoms: list of Atoms objects
-            The Atoms objects to relax.
-
-        converter: schnetpack.interfaces.AtomsConverter
-            Class used to convert ase Atoms objects to schnetpack input
-
-        restart: str
-            Filename for restart file.  Default value is *None*.
-
-        logfile: file object or str
-            If *logfile* is a string, a file with that name will be opened.
-            Use '-' for stdout.
-
-        trajectory: Trajectory object or str
-            Attach trajectory object.  If *trajectory* is a string a
-            Trajectory will be constructed.  Use *None* for no
-            trajectory.
-
-        fixed_atoms list(int):
-            list of indices corresponding to atoms with positions fixed in space.
-
-        append_trajectory: boolean
-            Appended to the trajectory file instead of overwriting it.
-
-        master: boolean
-            Defaults to None, which causes only rank 0 to save files.  If
-            set to true,  this rank will save files.
-
-        energy_key: str
-            name of energies in model (default="energy")
-
-        force_key: str
-            name of forces in model (default="forces")
-
-        energy_unit: str, float
-            energy units used by model (default="eV")
-
-        position_unit: str, float
-            position units used by model (default="Angstrom")
-
-        log_every_step: bool
-            set to True to log Dynamics after each step (default=False)
-        """
-        super().__init__(None, logfile, trajectory, append_trajectory, master)
-
-        self.model = model
-        self.atoms = atoms
-        self.converter = converter
-        self.fixed_atoms_mask = fixed_atoms_mask
-        self.previous_pos = None
-        self.model_results = None
-        self.energy_key = energy_key
-        self.force_key = force_key
-        self.trajectory = trajectory
-        self.log_every_step = log_every_step
-
-        # set up basic conversion factors
-        self.energy_conversion = convert_units(energy_unit, "eV")
-        self.position_conversion = convert_units(position_unit, "Angstrom")
-
-        # Unit conversion to default ASE units
-        self.property_units = {
-            self.energy: self.energy_conversion,
-            self.forces: self.energy_conversion / self.position_conversion,
-            self.stress: self.energy_conversion / self.position_conversion**3,
-        }
-
-        # get initial model inputs and set device
-        self._update_model_inputs()
-        self.device = (
-            torch.device("cuda")
-            if self.model_inputs[properties.R].is_cuda
-            else torch.device("cpu")
-        )
-
-    def _update_model_inputs(self):
-        self.model_inputs = self.converter(self.atoms)
-
-    def _requires_calculation(self, property_keys):
-        if self.model_results is None or self.previous_pos is None:
-            return True
-        for name in property_keys:
-            if name not in self.model_results:
-                return True
-        return not np.array_equal(
-            self.previous_pos, self.model_inputs[properties.R].detach().cpu().numpy()
-        )
-
-    def _get_forces(self, inputs):
-        if self._requires_calculation(property_keys=[self.energy_key, self.force_key]):
-            self.model_results = self.model(inputs)
-            self.previous_pos = self.model_inputs[properties.R].detach().cpu().numpy()
-        f = (
-            self.model_results[self.force_key].detach().cpu().numpy()
-            * self.property_units[self.forces]
-        )
-        if self.fixed_atoms_mask is not None:
-            f[self.fixed_atoms_mask] *= 0.0
-        return f
-
-    def _get_potential_energy(self, inputs):
-        if self._requires_calculation(property_keys=[self.energy_key]):
-            self.model_results = self.model(inputs)
-        return (
-            self.model_results[self.energy_key].detach().cpu().numpy()
-            * self.property_units[self.energy]
-        )
-
-    def irun(self):
-        # compute initial structure and log the first step
-        self._get_forces(self.model_inputs)
-
-        # in the following we are assuming that index_m is sorted in ascending order
-        # this is required since the flat tensors are reshaped to tensors of dimension batch_size x n_atoms x 3
-        dev_from_sorted_index_m = (
-            self.model_inputs[properties.idx_m].sort()[0]
-            - self.model_inputs[properties.idx_m]
-        )
-        if abs(dev_from_sorted_index_m).sum() > 0.0:
-            raise ValueError(
-                "idx_m is assumed to be sorted in ascending order, this is not the case here!"
+        # Set up unit conversion
+        positions2internal = spk_units.unit2internal(position_unit_input)
+        mass2internal = spk_units.unit2internal(mass_unit_input)
+
+        # 0) Check if molecules is a single ase.Atoms object and wrap it in list.
+        if isinstance(molecules, Atoms):
+            molecules = [molecules]
+
+        # 1) Get number of molecules, number of replicas and number of
+        #    overall systems
+        self.n_molecules = len(molecules)
+
+        # 2) Construct array with number of atoms in each molecule
+        self.n_atoms = torch.zeros(self.n_molecules, dtype=torch.long)
+
+        for i in range(self.n_molecules):
+            self.n_atoms[i] = molecules[i].get_global_number_of_atoms()
+
+        # 3) Get total n_molecule x n_atom dimension
+        self.total_n_atoms = torch.sum(self.n_atoms).item()
+        # initialize index vector for aggregation
+        self.index_m = torch.zeros(self.total_n_atoms, dtype=torch.long)
+
+        # 3) Construct basic property arrays
+        self.atom_types = torch.zeros(self.total_n_atoms, dtype=torch.long)
+        self.masses = torch.ones(1, self.total_n_atoms, 1)
+
+        # Relevant for dynamic properties: positions, momenta, forces
+        self.positions = torch.zeros(self.n_replicas, self.total_n_atoms, 3)
+        self.momenta = torch.zeros(self.n_replicas, self.total_n_atoms, 3)
+        self.forces = torch.zeros(self.n_replicas, self.total_n_atoms, 3)
+
+        self.energy = torch.zeros(self.n_replicas, self.n_molecules, 1)
+
+        # Relevant for periodic boundary conditions and simulation cells
+        self.cells = torch.zeros(self.n_replicas, self.n_molecules, 3, 3)
+        self.stress = torch.zeros(self.n_replicas, self.n_molecules, 3, 3)
+        self.pbc = torch.zeros(1, self.n_molecules, 3)
+
+        # 5) Populate arrays according to the data provided in molecules
+        idx_c = 0
+        for i in range(self.n_molecules):
+            n_atoms = self.n_atoms[i]
+
+            # Aggregation array
+            self.index_m[idx_c : idx_c + n_atoms] = i
+
+            # Static properties
+            self.atom_types[idx_c : idx_c + n_atoms] = torch.from_numpy(
+                molecules[i].get_atomic_numbers()
+            ).long()
+            self.masses[0, idx_c : idx_c + n_atoms, 0] = torch.from_numpy(
+                molecules[i].get_masses() * mass2internal
             )
 
-        # yield the first time to inspect before logging
-        yield False
+            # Dynamic properties
+            self.positions[:, idx_c : idx_c + n_atoms, :] = torch.from_numpy(
+                molecules[i].positions * positions2internal
+            )
 
-        if self.nsteps == 0:
-            self.log()
-            pass
+            # Properties for cell simulations
+            self.cells[:, i, :, :] = torch.from_numpy(
+                molecules[i].cell.array * positions2internal
+            )
+            self.pbc[0, i, :] = torch.from_numpy(molecules[i].pbc)
 
-        # run the algorithm until converged or max_steps reached
-        while not self.converged() and self.nsteps < self.max_steps:
+            idx_c += n_atoms
 
-            # compute the next step
-            self.step()
-            self.nsteps += 1
+        # Convert periodic boundary conditions to Boolean tensor
+        self.pbc = self.pbc.bool()
 
-            # update the model inputs (needed to get new nbh list)
-            self._update_model_inputs()
+        # Check for cell/pbc stuff:
+        if torch.sum(torch.abs(self.cells)) == 0.0:
+            if torch.sum(self.pbc) > 0.0:
+                raise SystemException("Found periodic boundary conditions but no cell.")
 
-            # let the user inspect the step and change things before logging
-            # and predicting the next step
-            yield False
+        # Set normal mode transformer
+        self.nm_transform = self._nm_transformer(n_replicas)
 
-            # log the step
-            if self.log_every_step:
-                self.log()
+    def sum_atoms(self, x: torch.Tensor):
+        """
+        Auxiliary routine for summing atomic contributions for each molecule.
 
-        # log last step
-        self.log()
+        Args:
+            x (torch.Tensor): Input tensor of the shape ( : x (n_molecules * n_atoms) x ...)
 
-        # finally check if algorithm was converged
-        yield self.converged()
+        Returns:
+            torch.Tensor: Aggregated tensor of the shape ( : x n_molecules x ...)
+        """
+        x_shape = x.shape
+        x_tmp = torch.zeros(
+            x_shape[0], self.n_molecules, *x_shape[2:], device=x.device, dtype=x.dtype
+        )
+        return x_tmp.index_add(1, self.index_m, x)
 
-    def run(self):
-        """Run dynamics algorithm.
+    def _mean_atoms(self, x: torch.Tensor):
+        """
+        Auxiliary routine for computing mean over atomic contributions for each molecule.
 
-        This method will return when the forces on all individual
-        atoms are less than *fmax* or when the number of steps exceeds
-        *steps*."""
+        Args:
+            x (torch.Tensor): Input tensor of the shape ( : x (n_molecules * n_atoms) x ...)
 
-        for converged in BatchwiseDynamics.irun(self):
-            pass
-        return converged
+        Returns:
+            torch.Tensor: Aggregated tensor of the shape ( : x n_molecules x ...)
+        """
+        return self.sum_atoms(x) / self.n_atoms[None, :, None]
 
+    def expand_atoms(self, x: torch.Tensor):
+        """
+        Auxiliary routine for expanding molecular contributions over the corresponding atoms.
 
-class BatchwiseOptimizer(BatchwiseDynamics):
-    """Base-class for all structure optimization classes."""
+        Args:
+            x (torch.Tensor): Tensor of the shape ( : x n_molecules x ...)
 
-    # default maxstep for all optimizers
-    defaults = {"maxstep": 0.2}
+        Returns:
+            torch.Tensor: Tensor of the shape ( : x (n_molecules * n_atoms) x ...)
+        """
+        return x[:, self.index_m, ...]
 
-    def __init__(
-        self,
-        model,
-        atoms,
-        converter,
-        fixed_atoms_mask,
-        restart,
-        logfile,
-        trajectory,
-        master=None,
-        append_trajectory=False,
-        energy_key="energy",
-        force_key="forces",
-        energy_unit="eV",
-        position_unit="Ang",
-        log_every_step=False,
-    ):
-        """Structure optimizer object.
+    @property
+    def center_of_mass(self):
+        """
+        Compute the center of mass for each replica and molecule
 
-        Parameters:
+        Returns:
+            torch.Tensor: n_replicas x n_molecules x 3 tensor holding the
+                          center of mass.
+        """
+        # Compute center of mass
+        center_of_mass = self.sum_atoms(self.positions * self.masses) / self.sum_atoms(
+            self.masses
+        )
+        return center_of_mass
 
-        model: torch.nn.Module
-            The force field model used to calculate the respective atomic forces
+    def remove_center_of_mass(self):
+        """
+        Move all structures to their respective center of mass.
+        """
+        self.positions -= self.expand_atoms(self.center_of_mass)
 
-        atoms: list of Atoms objects
-            The Atoms objects to relax.
+    def remove_translation(self):
+        """
+        Remove all components in the current momenta associated with
+        translational motion.
+        """
+        self.momenta -= self.expand_atoms(self._mean_atoms(self.momenta))
 
-        converter: schnetpack.interfaces.AtomsConverter
-            Class used to convert ase Atoms objects to schnetpack input
+    def remove_com_rotation(self):
+        """
+        Remove all components in the current momenta associated with rotational
+        motion using Eckart conditions.
+        """
+        # Compute the moment of inertia tensor
+        moment_of_inertia = (
+            torch.sum(self.positions**2, dim=2, keepdim=True)[..., None]
+            * torch.eye(3, dtype=self.positions.dtype, device=self.positions.device)[
+                None, None, :, :
+            ]
+            - self.positions[..., :, None] * self.positions[..., None, :]
+        )
 
-        fixed_atoms list(int):
-            list of indices corresponding to atoms with positions fixed in space.
+        moment_of_inertia = self.sum_atoms(moment_of_inertia * self.masses[..., None])
 
-        restart: str
-            Filename for restart file.  Default value is *None*.
+        # Compute the angular momentum
+        angular_momentum = self.sum_atoms(torch.cross(self.positions, self.momenta, -1))
 
-        logfile: file object or str
-            If *logfile* is a string, a file with that name will be opened.
-            Use '-' for stdout.
+        # Compute the angular velocities
+        angular_velocities = torch.matmul(
+            angular_momentum[:, :, None, :], torch.inverse(moment_of_inertia)
+        ).squeeze(2)
+
+        # Compute individual atomic contributions
+        rotational_velocities = torch.cross(
+            self.expand_atoms(angular_velocities), self.positions, -1
+        )
 
-        trajectory: Trajectory object or str
-            Attach trajectory object.  If *trajectory* is a string a
-            Trajectory will be constructed.  Use *None* for no
-            trajectory.
+        # Subtract rotation from overall motion (apply atom mask)
+        self.momenta -= rotational_velocities * self.masses
 
-        master: boolean
-            Defaults to None, which causes only rank 0 to save files.  If
-            set to true,  this rank will save files.
+    def get_ase_atoms(self, position_unit_output="Angstrom"):
+        # TODO: make sensible unit conversion and update docs
+        """
+        Convert the stored molecular configurations into ASE Atoms objects. This is e.g. used for the
+        neighbor lists based on environment providers. All units are atomic units by default, as used in the calculator
 
-        append_trajectory: boolean
-            Appended to the trajectory file instead of overwriting it.
+        Args:
+            position_unit_output (str, float): Target units for position output.
 
-        energy_key: str
-            name of energies in model (default="energy")
+        Returns:
+            list(ase.Atoms): List of ASE Atoms objects, with the replica and molecule dimension flattened.
+        """
+        internal2positions = spk_units.convert_units(
+            spk_units.length, position_unit_output
+        )
 
-        force_key: str
-            name of forces in model (default="forces")
+        atoms = []
+        for idx_r in range(self.n_replicas):
+            idx_c = 0
+            for idx_m in range(self.n_molecules):
+                n_atoms = self.n_atoms[idx_m]
+
+                positions = (
+                    self.positions[idx_r, idx_c : idx_c + n_atoms]
+                    .cpu()
+                    .detach()
+                    .numpy()
+                ) * internal2positions
+
+                atom_types = (
+                    self.atom_types[idx_c : idx_c + n_atoms].cpu().detach().numpy()
+                )
+
+                cell = (
+                    self.cells[idx_r, idx_m].cpu().detach().numpy() * internal2positions
+                )
+                pbc = self.pbc[0, idx_m].cpu().detach().numpy()
 
-        energy_unit: str, float
-            energy units used by model (default="eV")
+                mol = Atoms(atom_types, positions, cell=cell, pbc=pbc)
+                atoms.append(mol)
 
-        position_unit: str, float
-            position units used by model (default="Angstrom")
+                idx_c += n_atoms
 
-        log_every_step: bool
-            set to True to log Dynamics after each step (default=False)
+        return atoms
+
+    @property
+    def velocities(self):
+        """
+        Convenience property to access molecular velocities instead of the
+        momenta (e.g for power spectra)
+
+        Returns:
+            torch.Tensor: Velocity tensor with the same shape as the momenta.
+        """
+        return self.momenta / self.masses
+
+    @property
+    def kinetic_energy(self) -> torch.tensor:
+        """
+        Convenience property for computing the kinetic energy associated with
+        each replica and molecule.
+
+        Returns:
+            torch.Tensor: Tensor of the kinetic energies (in Hartree) with
+                          the shape n_replicas x n_molecules x 1
         """
-        BatchwiseDynamics.__init__(
-            self,
-            model=model,
-            atoms=atoms,
-            converter=converter,
-            fixed_atoms_mask=fixed_atoms_mask,
-            logfile=logfile,
-            trajectory=trajectory,
-            master=master,
-            append_trajectory=append_trajectory,
-            energy_key=energy_key,
-            force_key=force_key,
-            energy_unit=energy_unit,
-            position_unit=position_unit,
-            log_every_step=log_every_step,
+        kinetic_energy = 0.5 * self.sum_atoms(
+            torch.sum(self.momenta**2, dim=2, keepdim=True) / self.masses
         )
+        return kinetic_energy
 
-        self.restart = restart
+    @property
+    def kinetic_energy_tensor(self):
+        """
+        Compute the kinetic energy tensor (outer product of momenta divided by masses) for pressure computation.
+        The standard kinetic energy is the trace of this tensor.
 
-        # initialize attribute
-        self.fmax = None
+        Returns:
+            torch.tensor: n_replicas x n_molecules x 3 x 3 tensor containing kinetic energy components.
 
-        if restart is None or not isfile(restart):
-            self.initialize()
-        else:
-            self.read()
-            barrier()
+        """
+        # Apply atom mask
+        kinetic_energy_tensor = 0.5 * self.sum_atoms(
+            self.momenta[..., None]
+            * self.momenta[:, :, None, :]
+            / self.masses[..., None]
+        )
+        return kinetic_energy_tensor
 
-    def todict(self):
-        description = {
-            "type": "optimization",
-            "optimizer": self.__class__.__name__,
-        }
-        return description
-
-    def initialize(self):
-        pass
-
-    def irun(self, fmax=0.05, steps=None):
-        """call Dynamics.irun and keep track of fmax"""
-        self.fmax = fmax
-        if steps:
-            self.max_steps = steps
-        return BatchwiseDynamics.irun(self)
-
-    def run(self, fmax=0.05, steps=None):
-        """call Dynamics.run and keep track of fmax"""
-        self.fmax = fmax
-        if steps:
-            self.max_steps = steps
-        return BatchwiseDynamics.run(self)
-
-    def converged(self, forces=None):
-        """Did the optimization converge?"""
-        if forces is None:
-            forces = self._get_forces(self.model_inputs)
-        return (forces**2).sum(axis=1).max() < self.fmax**2
-
-    def log(self, forces=None):
-        if forces is None:
-            forces = self._get_forces(self.model_inputs)
-        fmax = sqrt((forces**2).sum(axis=1).max())
-        T = time.localtime()
-        if self.logfile is not None:
-            name = self.__class__.__name__
-            if self.nsteps == 0:
-                args = (" " * len(name), "Step", "Time", "fmax")
-                msg = "%s  %4s %8s %12s\n" % args
-                self.logfile.write(msg)
-
-            args = (name, self.nsteps, T[3], T[4], T[5], fmax)
-            msg = "%s:  %3d %02d:%02d:%02d %12.4f\n" % args
-            self.logfile.write(msg)
-
-            self.logfile.flush()
-
-        if self.trajectory is not None:
-            for struc_idx, at in enumerate(self.atoms):
-                # store in trajectory
-                write(
-                    self.trajectory + "_{}.xyz".format(struc_idx),
-                    at,
-                    format="extxyz",
-                    append=False if self.nsteps == 0 else True,
-                )
+    @property
+    def temperature(self):
+        """
+        Convenience property for accessing the instantaneous temperatures of
+        each replica and molecule.
 
-    def get_relaxation_results(self):
-        self._get_forces(self.model_inputs)
-        return self.atoms, self.model_results
-
-    def dump(self, data):
-        if world.rank == 0 and self.restart is not None:
-            with open(self.restart, "wb") as fd:
-                pickle.dump(data, fd, protocol=2)
-
-    def load(self):
-        with open(self.restart, "rb") as fd:
-            return pickle.load(fd)
-
-
-class ASEBatchwiseLBFGS(BatchwiseOptimizer):
-    """Limited memory BFGS optimizer.
-
-    LBFGS optimizer that allows for relaxation of multiple structures in parallel. This optimizer is an
-    extension/adaptation of the ase.optimize.LBFGS optimizer particularly designed for batch-wise relaxation
-    of atomic structures. The inverse Hessian is approximated for each sample separately, which allows for
-    optimizing batches of different structures/compositions.
+        Returns:
+            torch.Tensor: Tensor of the instantaneous temperatures (in
+                          Kelvin) with the shape n_replicas x n_molecules x 1
+        """
+        temperature = (
+            2.0
+            / (3.0 * self.n_atoms[None, :, None] * spk_units.kB)
+            * self.kinetic_energy
+        )
+        return temperature
 
-    """
+    @property
+    def potential_energy(self):
+        """
+        Property for accessing potential energy pf system. The energy array is only populated if a `energy_key` is
+        given in the calculator, energies will be 0 otherwise.
 
-    def __init__(
-        self,
-        model,
-        atoms,
-        converter,
-        fixed_atoms_mask=None,
-        restart=None,
-        logfile="-",
-        trajectory=None,
-        maxstep=None,
-        memory=100,
-        damping=1.0,
-        alpha=70.0,
-        use_line_search=False,
-        master=None,
-        energy_key="energy",
-        force_key="forces",
-        energy_unit="eV",
-        position_unit="Ang",
-        log_every_step=False,
-    ):
+        Returns:
+            torch.tensor: Potential energy, if requested in the calculator
+        """
+        return self.energy
+
+    @potential_energy.setter
+    def potential_energy(self, energy: torch.tensor):
+        """
+        Setter for the potential energy.
+
+        Args:
+            energy (torch.tensor): Potential energy.
+        """
+        self.energy = energy
+
+    @property
+    def momenta_normal(self):
+        """
+        Property for normal mode representation of momenta (e.g. for RPMD)
+
+        Returns:
+            torch.tensor: momenta in normal mode representation.
+        """
+        return self.nm_transform.beads2normal(self.momenta)
+
+    @momenta_normal.setter
+    def momenta_normal(self, momenta_normal):
+        """
+        Use momenta in normal mode representation to set system momenta.
+
+        Args:
+            momenta_normal (torch.tensor): momenta in normal mode representation
+        """
+        self.momenta = self.nm_transform.normal2beads(momenta_normal)
+
+    @property
+    def positions_normal(self):
+        """
+        Property for normal mode representation of positions (e.g. for RPMD)
+
+        Returns:
+            torch.tensor: positions in normal mode representation.
+        """
+        return self.nm_transform.beads2normal(self.positions)
+
+    @positions_normal.setter
+    def positions_normal(self, positions_normal):
+        """
+        Use positions in normal mode representation to set system positions.
+
+        Args:
+            positions_normal (torch.tensor): positions in normal mode representation
+        """
+        self.positions = self.nm_transform.normal2beads(positions_normal)
 
-        """Parameters:
+    @property
+    def centroid_positions(self):
+        """
+        Convenience property to access the positions of the centroid during
+        ring polymer molecular dynamics. Does not make sense during a
+        standard dynamics setup.
+
+        Returns:
+            torch.Tensor: Tensor of the shape 1 x (n_molecules * n_atoms) x 3
+            holding the centroid positions.
+        """
+        return torch.mean(self.positions, dim=0, keepdim=True)
 
-        model: torch.nn.Module
-            The force field model used to calculate the respective atomic forces
+    @property
+    def centroid_momenta(self):
+        """
+        Convenience property to access the centroid momenta during ring
+        polymer molecular dynamics. Does not make sense during a standard
+        dynamics setup.
+
+        Returns:
+            torch.Tensor: Tensor of the shape 1 x (n_molecules * n_atoms) x 3
+                          holding the centroid momenta.
+        """
+        return torch.mean(self.momenta, dim=0, keepdim=True)
 
-        atoms: list of Atoms objects
-            The Atoms objects to relax.
+    @property
+    def centroid_velocities(self):
+        """
+        Convenience property to access the velocities of the centroid during
+        ring polymer molecular dynamics (e.g. for computing power spectra).
+        Does not make sense during a standard dynamics setup.
+
+        Returns:
+            torch.Tensor: Tensor of the shape (1 x n_molecules * n_atoms) x 3
+            holding the centroid velocities.
+        """
+        return self.centroid_momenta / self.masses
 
-        converter: schnetpack.interfaces.AtomsConverter
-            Class used to convert ase Atoms objects to schnetpack input
-
-        fixed_atoms list(int):
-            list of indices corresponding to atoms with positions fixed in space.
-
-        restart: string
-            Pickle file used to store vectors for updating the inverse of
-            Hessian matrix. If set, file with such a name will be searched
-            and information stored will be used, if the file exists.
-
-        logfile: file object or str
-            If *logfile* is a string, a file with that name will be opened.
-            Use '-' for stdout.
-
-        trajectory: string
-            Pickle file used to store trajectory of atomic movement.
-
-        maxstep: float
-            How far is a single atom allowed to move. This is useful for DFT
-            calculations where wavefunctions can be reused if steps are small.
-            Default is 0.2 Angstrom.
-
-        memory: int
-            Number of steps to be stored. Default value is 100. Three numpy
-            arrays of this length containing floats are stored.
-
-        damping: float
-            The calculated step is multiplied with this number before added to
-            the positions.
-
-        alpha: float
-            Initial guess for the Hessian (curvature of energy surface). A
-            conservative value of 70.0 is the default, but number of needed
-            steps to converge might be less if a lower value is used. However,
-            a lower value also means risk of instability.
-
-        master: boolean
-            Defaults to None, which causes only rank 0 to save files.  If
-            set to true, this rank will save files.
-
-        energy_key: str
-            name of energies in model (default="energy")
-
-        force_key: str
-            name of forces in model (default="forces")
-
-        energy_unit: str, float
-            energy units used by model (default="eV")
-
-        position_unit: str, float
-            position units used by model (default="Angstrom")
-
-        log_every_step: bool
-            set to True to log Dynamics after each step (default=False)
-        """
-
-        BatchwiseOptimizer.__init__(
-            self,
-            model=model,
-            atoms=atoms,
-            converter=converter,
-            fixed_atoms_mask=fixed_atoms_mask,
-            restart=restart,
-            logfile=logfile,
-            trajectory=trajectory,
-            master=master,
-            energy_key=energy_key,
-            force_key=force_key,
-            energy_unit=energy_unit,
-            position_unit=position_unit,
-            log_every_step=log_every_step,
+    @property
+    def centroid_kinetic_energy(self):
+        """
+        Convenience property for computing the kinetic energy associated with
+        the centroid of each molecule. Only sensible in the context of ring
+        polymer molecular dynamics.
+
+        Returns:
+            torch.Tensor: Tensor of the centroid kinetic energies (in
+                          Hartree) with the shape 1 x n_molecules x 1
+        """
+        kinetic_energy = 0.5 * self.sum_atoms(
+            torch.sum(self.centroid_momenta**2, dim=2, keepdim=True) / self.masses
         )
+        return kinetic_energy
 
-        if maxstep is not None:
-            self.maxstep = maxstep
-        else:
-            self.maxstep = self.defaults["maxstep"]
+    @property
+    def centroid_temperature(self):
+        """
+        Convenience property for accessing the instantaneous temperatures of
+        the centroid of each molecule. Only makes sense in the context of
+        ring polymer molecular dynamics.
+
+        Returns:
+            torch.Tensor: Tensor of the instantaneous centroid temperatures (
+                          in Kelvin) with the shape 1 x n_molecules x 1
+        """
+        temperature = (
+            2.0
+            / (3.0 * spk_units.kB * self.n_atoms[None, :, None])
+            * self.centroid_kinetic_energy
+        )
+        return temperature
 
-        if self.maxstep > 1.0:
-            raise ValueError(
-                "You are using a much too large value for "
-                + "the maximum step size: %.1f Angstrom" % maxstep
-            )
+    @property
+    def centroid_potential_energy(self):
+        """
+        Get the centroid potential energy.
+
+        Returns:
+            torch.tensor: Centroid potential energy
+        """
+        return torch.mean(self.energy, dim=0, keepdim=True)
 
-        self.memory = memory
-        # Initial approximation of inverse Hessian 1./70. is to emulate the
-        # behaviour of BFGS. Note that this is never changed!
-        self.H0 = 1.0 / alpha
-        self.damping = damping
-        self.use_line_search = use_line_search
-        self.p = None
-        self.function_calls = 0
-        self.force_calls = 0
-        self.n_configs = None
-
-        if use_line_search:
-            raise NotImplementedError("Lines search has not been implemented yet")
-
-    def initialize(self):
-        """Initialize everything so no checks have to be done in step"""
-        self.iteration = 0
-        self.s = []
-        self.y = []
-        # Store also rho, to avoid calculating the dot product again and
-        # again.
-        self.rho = []
-
-        self.r0 = None
-        self.f0 = None
-        self.e0 = None
-        self.task = "START"
-        self.load_restart = False
-
-    def read(self):
-        """Load saved arrays to reconstruct the Hessian"""
-        (
-            self.iteration,
-            self.s,
-            self.y,
-            self.rho,
-            self.r0,
-            self.f0,
-            self.e0,
-            self.task,
-        ) = self.load()
-        self.load_restart = True
-
-    def step(self, f=None):
-        """Take a single step
-
-        Use the given forces, update the history and calculate the next step --
-        then take it"""
-
-        self.n_configs = self.model_inputs[properties.n_atoms].shape[0]
-
-        if f is None:
-            f = self._get_forces(self.model_inputs)
-
-        # check if updates for respective structures are required
-        q_euclidean = -f.reshape(self.n_configs, -1, 3)
-        squared_max_forces = (q_euclidean**2).sum(axis=-1).max(axis=-1)
-        configs_mask = squared_max_forces < self.fmax**2
-        mask = (
-            configs_mask[:, None]
-            .repeat(q_euclidean.shape[1], 0)
-            .repeat(q_euclidean.shape[2], 1)
-        )
-
-        r = self.model_inputs[properties.R].detach().cpu().numpy()
-
-        self.update(r, f, self.r0, self.f0, configs_mask)
-
-        s = self.s
-        y = self.y
-        rho = self.rho
-        H0 = self.H0
-
-        loopmax = np.min([self.memory, self.iteration])
-        a = np.empty(
-            (
-                loopmax,
-                self.n_configs,
-                1,
-                1,
-            ),
-            dtype=np.float64,
-        )
-
-        # ## The algorithm itself:
-        q = -f.reshape(self.n_configs, 1, -1)
-        for i in range(loopmax - 1, -1, -1):
-            a[i] = rho[i] * np.matmul(s[i], np.transpose(q, axes=(0, 2, 1)))
-            q -= a[i] * y[i]
-
-        z = H0 * q
-
-        for i in range(loopmax):
-            b = rho[i] * np.matmul(y[i], np.transpose(z, axes=(0, 2, 1)))
-            z += s[i] * (a[i] - b)
-
-        p = -z.reshape((-1, 3))
-        self.p = np.where(mask, np.zeros_like(p), p)
-        # ##
-
-        g = -f
-        if self.use_line_search is True:
-            e = self.func(r)
-            self.line_search(r, g, e)
-            dr = (self.alpha_k * self.p).reshape(
-                self.model_inputs[properties.n_atoms].item(), -1
+    @property
+    def volume(self):
+        """
+        Compute the cell volumes if cells are present.
+
+        Returns:
+            torch.tensor: n_replicas x n_molecules x 1 containing the volumes.
+        """
+        volume = torch.sum(
+            self.cells[:, :, 0]
+            * torch.cross(self.cells[:, :, 1], self.cells[:, :, 2], dim=2),
+            dim=2,
+            keepdim=True,
+        )
+        return volume
+
+    def compute_pressure(self, tensor: bool = False, kinetic_component: bool = False):
+        """
+        Compute the pressure (tensor) based on the stress tensor of the systems.
+
+        Args:
+            tensor (bool): Instead of a scalar pressure, return the full pressure tensor. (Required for
+                           anisotropic cell deformation.)
+            kinetic_component (bool): Include the kinetic energy component during the computation of the
+                                      pressure (default=False).
+
+        Returns:
+            torch.Tensor: Depending on the tensor-flag, returns a tensor containing the pressure with dimensions
+                          n_replicas x n_molecules x 1 (False) or n_replicas x n_molecules x 3 x 3 (True).
+        """
+        volume = self.volume
+
+        if torch.any(volume == 0.0):
+            raise SystemError(
+                "Non-zero volume simulation cell required for computation of the instantaneous pressure."
             )
+
+        pressure = -self.stress
+
+        if tensor:
+            if kinetic_component:
+                pressure += 2 * self.kinetic_energy_tensor / self.volume[..., None]
         else:
-            self.force_calls += 1
-            self.function_calls += 1
-            dr = self.determine_step(self.p) * self.damping
-
-        # update positions
-        pos_updated = self.model_inputs[properties.R].detach().cpu().numpy() + dr
-
-        # store in ase Atoms object
-        ats = []
-        indices_m = self.model_inputs[properties.idx_m].detach().cpu().numpy()
-        for struc_idx, previous_at in enumerate(self.atoms):
-            # get atom positions for respective structure
-            pos_updated_m = pos_updated[indices_m == struc_idx]
-            # update ase Atoms object
-            at = Atoms(
-                positions=pos_updated_m, numbers=previous_at.get_atomic_numbers()
+            pressure = torch.einsum("abii->ab", pressure)[..., None] / 3.0
+            if kinetic_component:
+                pressure += 2.0 * self.kinetic_energy / self.volume / 3.0
+
+        return pressure
+
+    def compute_centroid_pressure(
+        self, tensor: bool = False, kinetic_component: bool = False
+    ):
+        """
+        Compute the pressure (tensor) of the ring polymer centroid based on the stress tensor of the systems.
+
+        Args:
+            tensor (bool): Instead of a scalar pressure, return the full pressure tensor. (Required for
+                           anisotropic cell deformation.)
+            kinetic_component (bool): Include the kinetic energy component during the computation of the
+                                      pressure (default=False).
+
+        Returns:
+            torch.Tensor: Depending on the tensor-flag, returns a tensor containing the pressure with dimensions
+                          n_replicas x n_molecules x 1 (False) or n_replicas x n_molecules x 3 x 3 (True).
+        """
+        volume = torch.mean(self.volume, dim=0, keepdim=True)
+
+        if torch.any(volume == 0.0):
+            raise SystemError(
+                "Non-zero volume simulation cell required for computation of the instantaneous pressure."
             )
-            at.pbc = previous_at.pbc
-            at.cell = previous_at.cell
-            ats.append(at)
-        # store
-        self.atoms = ats
-
-        self.iteration += 1
-        self.r0 = r
-        self.f0 = -g
-        self.dump(
-            (
-                self.iteration,
-                self.s,
-                self.y,
-                self.rho,
-                self.r0,
-                self.f0,
-                self.e0,
-                self.task,
+
+        # Compute centroid pressure
+        pressure = -torch.mean(self.stress, dim=0, keepdim=True)
+
+        if tensor:
+            if kinetic_component:
+                pressure += 2 * self._mean_atoms(self.kinetic_energy_tensor) / volume
+        else:
+            pressure = torch.einsum("abii->ab", pressure)[..., None] / 3.0
+            if kinetic_component:
+                pressure += 2.0 * self.centroid_kinetic_energy / volume / 3.0
+
+        return pressure
+
+    def wrap_positions(self, eps=1e-6):
+        """
+        Move atoms outside the box back into the box for all dimensions with periodic boundary
+        conditions.
+
+        Args:
+            eps (float): Small offset for numerical stability
+        """
+        if torch.any(self.volume == 0.0):
+            raise SystemWarning("Simulation cell required for wrapping of positions.")
+        else:
+            pbc_atomic = self.expand_atoms(self.pbc)
+
+            # Compute fractional coordinates
+            inverse_cell = torch.inverse(self.cells)
+            inverse_cell = self.expand_atoms(inverse_cell)
+            inv_positions = torch.sum(self.positions[..., None] * inverse_cell, dim=2)
+
+            # Get periodic coordinates
+            periodic = torch.masked_select(inv_positions, pbc_atomic)
+
+            # Apply periodic boundary conditions (with small buffer)
+            periodic = periodic + eps
+            periodic = periodic % 1.0
+            periodic = periodic - eps
+
+            # Update fractional coordinates
+            inv_positions.masked_scatter_(pbc_atomic, periodic)
+
+            # Convert to positions
+            self.positions = torch.sum(
+                inv_positions[..., None] * self.expand_atoms(self.cells), dim=2
             )
-        )
 
-    def determine_step(self, dr):
-        """Determine step to take according to maxstep
+    def load_system_state(self, state_dict: OrderedDict[str, torch.Tensor]):
+        """
+        Routine for restoring the state of a system specified in a previously
+        stored state dict. Used to restart molecular dynamics simulations.
 
-        Normalize all steps as the largest step. This way
-        we still move along the eigendirection.
+        Args:
+            state_dict (dict): State dict of the system state.
         """
-        steplengths = (dr**2).sum(1) ** 0.5
-        # check if any step in entire batch is greater than maxstep
-        if np.max(steplengths) >= self.maxstep:
-            # rescale steps for each config separately
-            for idx_m in range(self.n_configs):
-                longest_step = np.max(
-                    steplengths[
-                        self.model_inputs[properties.idx_m].detach().cpu() == idx_m
-                    ]
-                )
-                if longest_step >= self.maxstep:
-                    print("normalized integration step")
-                    dr[self.model_inputs[properties.idx_m].detach().cpu() == idx_m] *= (
-                        self.maxstep / longest_step
-                    )
-        return dr
-
-    def update(self, r, f, r0, f0, configs_mask):
-        """Update everything that is kept in memory
-
-        This function is mostly here to allow for replay_trajectory.
-        """
-        if self.iteration > 0:
-            s0 = r.reshape(self.n_configs, 1, -1) - r0.reshape(self.n_configs, 1, -1)
-            self.s.append(s0)
-
-            # We use the gradient which is minus the force!
-            y0 = f0.reshape(self.n_configs, 1, -1) - f.reshape(self.n_configs, 1, -1)
-            self.y.append(y0)
-
-            ys0 = np.matmul(y0, np.transpose(s0, axes=(0, 2, 1))) + 1e-10
-            rho0 = np.where(configs_mask[:, None, None], np.ones_like(ys0), 1.0 / ys0)
-            self.rho.append(rho0)
-
-        if self.iteration > self.memory:
-            self.s.pop(0)
-            self.y.pop(0)
-            self.rho.pop(0)
-
-    def func(self, x):
-        """Objective function for use of the optimizers"""
-        raise NotImplementedError("func not implemented yet")
-
-    def line_search(self, r, g, e):
-        self.alpha_k = None
-        raise NotImplementedError("LineSearch not implemented yet")
+        self.load_state_dict(state_dict, strict=False)
+
+        # Set PBC to bool for periodic boundary conditions
+        self.pbc = self.pbc.bool()
+
+        # Set derived properties for restarting
+        self.n_replicas = self.positions.shape[0]
+        self.total_n_atoms = self.positions.shape[1]
+        self.n_molecules = self.n_atoms.shape[0]
+
+        # Set normal mode transformer
+        self.nm_transform = self._nm_transformer(self.n_replicas)
```

### Comparing `schnetpack-2.0.1/src/schnetpack/md/calculators/base_calculator.py` & `schnetpack-2.0.2/src/schnetpack/md/calculators/base_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/calculators/ensemble_calculator.py` & `schnetpack-2.0.2/src/schnetpack/md/calculators/ensemble_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/calculators/lj_calculator.py` & `schnetpack-2.0.2/src/schnetpack/md/calculators/lj_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/calculators/orca_calculator.py` & `schnetpack-2.0.2/src/schnetpack/md/calculators/orca_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/calculators/schnetpack_calculator.py` & `schnetpack-2.0.2/src/schnetpack/md/calculators/schnetpack_calculator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/cli.py` & `schnetpack-2.0.2/src/schnetpack/md/cli.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/data/hdf5_data.py` & `schnetpack-2.0.2/src/schnetpack/md/data/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/data/spectra.py` & `schnetpack-2.0.2/src/schnetpack/md/data/spectra.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/initial_conditions.py` & `schnetpack-2.0.2/src/schnetpack/md/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/integrators.py` & `schnetpack-2.0.2/src/schnetpack/md/integrators.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/neighborlist_md.py` & `schnetpack-2.0.2/src/schnetpack/md/neighborlist_md.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/parsers/orca_parser.py` & `schnetpack-2.0.2/src/schnetpack/md/parsers/orca_parser.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/barostats.py` & `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/barostats_rpmd.py` & `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/barostats_rpmd.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/basic_hooks.py` & `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/basic_hooks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/callback_hooks.py` & `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/callback_hooks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/thermostats.py` & `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py` & `schnetpack-2.0.2/src/schnetpack/md/simulation_hooks/thermostats_rpmd.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/simulator.py` & `schnetpack-2.0.2/src/schnetpack/md/simulator.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/utils/__init__.py` & `schnetpack-2.0.2/src/schnetpack/md/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/utils/md_config.py` & `schnetpack-2.0.2/src/schnetpack/md/utils/md_config.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/utils/normal_model_transformation.py` & `schnetpack-2.0.2/src/schnetpack/md/utils/normal_model_transformation.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/md/utils/thermostat_utils.py` & `schnetpack-2.0.2/src/schnetpack/md/utils/thermostat_utils.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/model/base.py` & `schnetpack-2.0.2/src/schnetpack/model/base.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/activations.py` & `schnetpack-2.0.2/src/schnetpack/nn/activations.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/base.py` & `schnetpack-2.0.2/src/schnetpack/nn/base.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/blocks.py` & `schnetpack-2.0.2/src/schnetpack/nn/blocks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/cutoff.py` & `schnetpack-2.0.2/src/schnetpack/nn/cutoff.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/equivariant.py` & `schnetpack-2.0.2/src/schnetpack/nn/equivariant.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/ops/so3.py` & `schnetpack-2.0.2/src/schnetpack/nn/ops/so3.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/radial.py` & `schnetpack-2.0.2/src/schnetpack/nn/radial.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/scatter.py` & `schnetpack-2.0.2/src/schnetpack/nn/scatter.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/so3.py` & `schnetpack-2.0.2/src/schnetpack/nn/so3.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/nn/utils.py` & `schnetpack-2.0.2/src/schnetpack/nn/utils.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/properties.py` & `schnetpack-2.0.2/src/schnetpack/properties.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/representation/field_schnet.py` & `schnetpack-2.0.2/src/schnetpack/representation/field_schnet.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/representation/painn.py` & `schnetpack-2.0.2/src/schnetpack/representation/painn.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/representation/schnet.py` & `schnetpack-2.0.2/src/schnetpack/representation/schnet.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/representation/so3net.py` & `schnetpack-2.0.2/src/schnetpack/representation/so3net.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/task.py` & `schnetpack-2.0.2/src/schnetpack/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,19 +264,15 @@
             return optimizer
 
     def optimizer_step(
         self,
         epoch: int = None,
         batch_idx: int = None,
         optimizer=None,
-        optimizer_idx: int = None,
         optimizer_closure=None,
-        on_tpu: bool = None,
-        using_native_amp: bool = None,
-        using_lbfgs: bool = None,
     ):
         if self.global_step < self.warmup_steps:
             lr_scale = min(1.0, float(self.trainer.global_step + 1) / self.warmup_steps)
             for pg in optimizer.param_groups:
                 pg["lr"] = lr_scale * self.lr
 
         # update params
```

### Comparing `schnetpack-2.0.1/src/schnetpack/train/callbacks.py` & `schnetpack-2.0.2/src/schnetpack/train/callbacks.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/train/lr_scheduler.py` & `schnetpack-2.0.2/src/schnetpack/train/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/train/metrics.py` & `schnetpack-2.0.2/src/schnetpack/train/metrics.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/transform/__init__.py` & `schnetpack-2.0.2/src/schnetpack/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/transform/atomistic.py` & `schnetpack-2.0.2/src/schnetpack/transform/atomistic.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/transform/base.py` & `schnetpack-2.0.2/src/schnetpack/transform/base.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/transform/casting.py` & `schnetpack-2.0.2/src/schnetpack/transform/casting.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/transform/neighborlist.py` & `schnetpack-2.0.2/src/schnetpack/transform/neighborlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,22 +271,17 @@
     ):
         """
         Args:
             neighbor_list: the neighbor list to use
             nbh_transforms: transforms for manipulating the neighbor lists
                 provided by neighbor_list
             cutoff_skin: float
-                If no atom has moved more than the skin-distance since the neighbor list
-                    has been updated the last time, then the neighbor list is reused.
-                    This will save some expensive rebuilds of the list.
-
-        Note:
-            Please choose a sufficiently large cutoff_skin value to ensure that between
-            two subsequent samples no atom can penetrate through the skin into the
-            cutoff sphere of another atom if it is not in the neighbor list of that atom.
+                If no atom has moved more than cutoff_skin/2 since the neighbor list
+                has been updated the last time, then the neighbor list is reused.
+                This will save some expensive rebuilds of the list.
         """
 
         super().__init__()
 
         self.neighbor_list = neighbor_list
         self.cutoff = neighbor_list._cutoff
         self.cutoff_skin = cutoff_skin
@@ -357,21 +352,21 @@
                 (previous_pbc == pbc.numpy()).any()
                 and (previous_cell == cell.numpy()).any()
                 and ((previous_positions - positions.numpy()) ** 2).sum(1).max()
                 < 0.25 * self.cutoff_skin**2
             ):
                 # reuse previous neighbor list
                 inputs[properties.idx_i] = (
-                    previous_inputs[properties.idx_i].detach().clone()
+                    previous_inputs[properties.idx_i].clone()
                 )
                 inputs[properties.idx_j] = (
-                    previous_inputs[properties.idx_j].detach().clone()
+                    previous_inputs[properties.idx_j].clone()
                 )
                 inputs[properties.offsets] = (
-                    previous_inputs[properties.offsets].detach().clone()
+                    previous_inputs[properties.offsets].clone()
                 )
                 return False, inputs
 
         # build new neighbor list
         inputs = self._build(inputs)
         return True, inputs
 
@@ -381,20 +376,20 @@
         inputs = self.neighbor_list(inputs)
         for nbh_transform in self.nbh_transforms:
             inputs = nbh_transform(inputs)
 
         # store new reference conformation and remove old one
         sample_idx = inputs[properties.idx].item()
         stored_inputs = {
-            properties.R: inputs[properties.R].clone(),
-            properties.cell: inputs[properties.cell].clone(),
-            properties.pbc: inputs[properties.pbc].clone(),
-            properties.idx_i: inputs[properties.idx_i].clone(),
-            properties.idx_j: inputs[properties.idx_j].clone(),
-            properties.offsets: inputs[properties.offsets].clone(),
+            properties.R: inputs[properties.R].detach().clone(),
+            properties.cell: inputs[properties.cell].detach().clone(),
+            properties.pbc: inputs[properties.pbc].detach().clone(),
+            properties.idx_i: inputs[properties.idx_i].detach().clone(),
+            properties.idx_j: inputs[properties.idx_j].detach().clone(),
+            properties.offsets: inputs[properties.offsets].detach().clone(),
         }
         self.previous_inputs.update({sample_idx: stored_inputs})
 
         return inputs
 
 
 class TorchNeighborList(NeighborListTransform):
```

### Comparing `schnetpack-2.0.1/src/schnetpack/transform/response.py` & `schnetpack-2.0.2/src/schnetpack/transform/response.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/units.py` & `schnetpack-2.0.2/src/schnetpack/units.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/utils/__init__.py` & `schnetpack-2.0.2/src/schnetpack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack/utils/script.py` & `schnetpack-2.0.2/src/schnetpack/utils/script.py`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/schnetpack.egg-info/PKG-INFO` & `schnetpack-2.0.2/src/schnetpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schnetpack
-Version: 2.0.1
+Version: 2.0.2
 Summary: SchNetPack - Deep Neural Networks for Atomistic Systems
 Home-page: https://github.com/atomistic-machine-learning/schnetpack
 Author: Kristof T. Schuett, Michael Gastegger, Stefaan Hessmann, Niklas Gebauer, Jonas Lederer
 License: MIT
 Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `schnetpack-2.0.1/src/schnetpack.egg-info/SOURCES.txt` & `schnetpack-2.0.2/src/schnetpack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 src/schnetpack/datasets/md17.py
 src/schnetpack/datasets/md22.py
 src/schnetpack/datasets/omdb.py
 src/schnetpack/datasets/qm9.py
 src/schnetpack/datasets/rmd17.py
 src/schnetpack/interfaces/__init__.py
 src/schnetpack/interfaces/ase_interface.py
-src/schnetpack/interfaces/batchwise_optimizer.py
+src/schnetpack/interfaces/batchwise_optimization.py
 src/schnetpack/md/__init__.py
 src/schnetpack/md/cli.py
 src/schnetpack/md/initial_conditions.py
 src/schnetpack/md/integrators.py
 src/schnetpack/md/neighborlist_md.py
 src/schnetpack/md/simulator.py
 src/schnetpack/md/system.py
```

### Comparing `schnetpack-2.0.1/src/scripts/spkconvert` & `schnetpack-2.0.2/src/scripts/spkconvert`

 * *Files identical despite different names*

### Comparing `schnetpack-2.0.1/src/scripts/spkdeploy` & `schnetpack-2.0.2/src/scripts/spkdeploy`

 * *Files identical despite different names*

