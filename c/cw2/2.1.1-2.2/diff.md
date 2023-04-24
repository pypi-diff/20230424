# Comparing `tmp/cw2-2.1.1.tar.gz` & `tmp/cw2-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cw2-2.1.1.tar", last modified: Wed Feb 22 09:19:40 2023, max compression
+gzip compressed data, was "cw2-2.2.tar", last modified: Mon Apr 24 13:12:53 2023, max compression
```

## Comparing `cw2-2.1.1.tar` & `cw2-2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:40.735229 cw2-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-22 09:19:25.000000 cw2-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-22 09:19:40.735229 cw2-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-22 09:19:25.000000 cw2-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:40.731229 cw2-2.1.1/cw2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/alternative_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cluster_work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:40.735229 cw2-2.1.1/cw2/cw_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_config/conf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_config/conf_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_config/conf_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_config/conf_unfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_config/cw_conf_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_config/cw_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:40.735229 cw2-2.1.1/cw2/cw_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_data/cw_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_data/cw_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_data/cw_pd_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_data/cw_wandb_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:40.735229 cw2-2.1.1/cw2/cw_slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_slurm/cw_slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/cw_slurm/cw_slurm_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/default_sbatch.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-02-22 09:19:25.000000 cw2-2.1.1/cw2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:40.731229 cw2-2.1.1/cw2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-22 09:19:40.000000 cw2-2.1.1/cw2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-22 09:19:40.000000 cw2-2.1.1/cw2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:19:40.000000 cw2-2.1.1/cw2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-22 09:19:40.000000 cw2-2.1.1/cw2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 09:19:40.000000 cw2-2.1.1/cw2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-22 09:19:25.000000 cw2-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:19:40.735229 cw2-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-02-22 09:19:25.000000 cw2-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:19:40.735229 cw2-2.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-02-22 09:19:25.000000 cw2-2.1.1/test/test_cw_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.947887 cw2-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-24 13:12:39.000000 cw2-2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-24 13:12:53.947887 cw2-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-24 13:12:39.000000 cw2-2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-24 13:12:39.000000 cw2-2.2/cw2/alternative_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cluster_work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/cw_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/conf_unfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/cw_conf_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_config/cw_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/cw_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_pd_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_data/cw_wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2/cw_slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_slurm/cw_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 13:12:39.000000 cw2-2.2/cw2/cw_slurm/cw_slurm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 13:12:39.000000 cw2-2.2/cw2/default_sbatch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-24 13:12:39.000000 cw2-2.2/cw2/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-24 13:12:39.000000 cw2-2.2/cw2/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14026 2023-04-24 13:12:39.000000 cw2-2.2/cw2/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-24 13:12:39.000000 cw2-2.2/cw2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/cw2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 13:12:53.000000 cw2-2.2/cw2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 13:12:39.000000 cw2-2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:12:53.947887 cw2-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 13:12:39.000000 cw2-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:12:53.943887 cw2-2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-24 13:12:39.000000 cw2-2.2/test/test_cw_config.py
```

### Comparing `cw2-2.1.1/LICENSE` & `cw2-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/PKG-INFO` & `cw2-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cw2
-Version: 2.1.1
+Version: 2.2
 Summary: A reengineered framework to run experiments on a computing cluster.
 Home-page: https://github.com/ALRhub/cw2
 Author: Maximilian Li
 Author-email: maximilian.xiling.li@gmail.com
 License: MIT
 Keywords: scientific,experiments,distributed computing,mpi,research
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cw2-2.1.1/README.md` & `cw2-2.2/README.md`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/alternative_schedulers.py` & `cw2-2.2/cw2/alternative_schedulers.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cli_parser.py` & `cw2-2.2/cw2/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cluster_work.py` & `cw2-2.2/cw2/cluster_work.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             s = scheduler.SlurmScheduler(self.config)
         else:
             # Do Local execution
             if sch is None:
                 if scheduler.GPUDistributingLocalScheduler.use_distributed_gpu_scheduling(self.config):
                     scheduler_cls = scheduler.get_gpu_scheduler_cls(self.config.slurm_config.get("scheduler", "mp"))
                     s = scheduler_cls(self.config)
+
+                elif scheduler.CpuDistributingLocalScheduler.use_distributed_cpu_scheduling(self.config):
+                    s = scheduler.CpuDistributingLocalScheduler(self.config)
+
                 else:
                     s = scheduler.LocalScheduler()
             else:
                 s = sch
 
         self._run_scheduler(s, root_dir)
```

### Comparing `cw2-2.1.1/cw2/cw_config/conf_io.py` & `cw2-2.2/cw2/cw_config/conf_io.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_config/conf_path.py` & `cw2-2.2/cw2/cw_config/conf_path.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_config/conf_resolver.py` & `cw2-2.2/cw2/cw_config/conf_resolver.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_config/conf_unfolder.py` & `cw2-2.2/cw2/cw_config/conf_unfolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
             config[KEY.i_BASIC_PATH] = config.get(KEY.PATH)
         # save name argument from YML for grid modification
         if KEY.i_EXP_NAME not in config:
             config[KEY.i_EXP_NAME] = config.get(KEY.NAME)
         # add empty string for parent DIR in case of grid
         if KEY.i_NEST_DIR not in config:
             config[KEY.i_NEST_DIR] = ''
+        # set debug flag
+        config[KEY.i_DEBUG_FLAG] = (debug or debug_all)
 
         # In-Between Step to solve grid AND list combinations
         if all(k in config for k in (KEY.GRID, KEY.LIST)):
             iter_func = zip
             key = KEY.LIST
 
             expansion = params_combine(config, key, iter_func)
```

### Comparing `cw2-2.1.1/cw2/cw_config/cw_conf_keys.py` & `cw2-2.2/cw2/cw_config/cw_conf_keys.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 LIST = "list"
 ABLATIVE = "ablative"
 
 # INTERNAL
 i_BASIC_PATH = "_basic_path"
 i_EXP_NAME = "_experiment_name"
 i_NEST_DIR = "_nested_dir"
-
+i_DEBUG_FLAG = "_debug"
 # INTERNAL REP
 i_REP_IDX = "_rep_idx"
 i_REP_LOG_PATH = "_rep_log_path"
 
 # INTERNAL IMPORT ARCHIVE
 i_IMPORT_PATH_ARCHIVE = "_import_path_archive"
 i_IMPORT_EXP_ARCHIVE = "_import_exp_archive"
```

### Comparing `cw2-2.1.1/cw2/cw_config/cw_config.py` & `cw2-2.2/cw2/cw_config/cw_config.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_data/cw_loading.py` & `cw2-2.2/cw2/cw_data/cw_loading.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_data/cw_logging.py` & `cw2-2.2/cw2/cw_data/cw_logging.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_data/cw_pd_logger.py` & `cw2-2.2/cw2/cw_data/cw_pd_logger.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_data/cw_wandb_logger.py` & `cw2-2.2/cw2/cw_data/cw_wandb_logger.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_error.py` & `cw2-2.2/cw2/cw_error.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/cw_slurm/cw_slurm.py` & `cw2-2.2/cw2/cw_slurm/cw_slurm.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/default_sbatch.sh` & `cw2-2.2/cw2/default_sbatch.sh`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/experiment.py` & `cw2-2.2/cw2/experiment.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/job.py` & `cw2-2.2/cw2/job.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2/scheduler.py` & `cw2-2.2/cw2/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,37 +37,40 @@
 
 
 class GPUDistributingLocalScheduler(AbstractScheduler):
 
     def __init__(self, conf: cw_config.Config = None):
 
         super(GPUDistributingLocalScheduler, self).__init__(conf=conf)
-        self._total_num_gpus = int(conf.slurm_config['sbatch_args']['gres'][4:])
+        self._total_num_gpus = int(conf.slurm_config["sbatch_args"]["gres"].rsplit(":", 1)[1])
         self._gpus_per_rep = conf.slurm_config['gpus_per_rep']
         self._queue_elements = int(self._total_num_gpus / self._gpus_per_rep)
 
         print("GPUDistributingLocalScheduler: {} GPUs available, {} GPUs per rep, {} queue elements".format(
             self._total_num_gpus, self._gpus_per_rep, self._queue_elements))
 
         if self._gpus_per_rep >= 1.0:
             assert self._gpus_per_rep == int(self._gpus_per_rep), "gpus_per_rep must be integer"
 
-
-
     @staticmethod
     def use_distributed_gpu_scheduling(conf: cw_config.Config) -> bool:
         if conf.slurm_config is None:
             return False
         # Use if
         # 1.) GPUs Requested
         # 2.) Number of GPUs per rep specified
         # 3.) Number of GPUs per rep != total number of gpus requested
         gpus_requested = "gres" in conf.slurm_config.get("sbatch_args", "DUMMY_DEFAULT")
         gpus_per_rep_specified = "gpus_per_rep" in conf.slurm_config
-        num_gpus_requested = int(conf.slurm_config["sbatch_args"]["gres"][4:]) if gpus_requested else 0
+
+        if gpus_requested:
+            num_gpus_requested = int(conf.slurm_config["sbatch_args"]["gres"].rsplit(":", 1)[1])
+            # e.g. gres=gpu:4 or gres=gpu:full:4
+        else:
+            num_gpus_requested = 0
 
         use_distributed_gpu_scheduling = \
             gpus_requested and gpus_per_rep_specified and num_gpus_requested != conf.slurm_config["gpus_per_rep"]
 
         if not use_distributed_gpu_scheduling:
             on_horeka_gpu = "hkn" in socket.gethostname() and conf.slurm_config["partition"] == "accelerated"
             if on_horeka_gpu:
@@ -79,15 +82,15 @@
     @staticmethod
     def get_gpu_str(queue_idx: int, gpus_per_rep: float) -> str:
         if gpus_per_rep >= 1:
             assert int(gpus_per_rep) == gpus_per_rep, "gpus_per_rep must be integer if >= 1"
             gpus_per_rep = int(gpus_per_rep)
             return ("{}," * gpus_per_rep).format(*[queue_idx * gpus_per_rep + i for i in range(gpus_per_rep)])[:-1]
         else:
-            return str(int(queue_idx * gpus_per_rep))
+            return str(int(queue_idx * gpus_per_rep) + 0.01)
 
 
 class MPGPUDistributingLocalScheduler(GPUDistributingLocalScheduler):
 
     def run(self, overwrite: bool = False):
         num_parallel = self.joblist[0].n_parallel
         for j in self.joblist:
@@ -247,14 +250,74 @@
         return HOREKAAffinityGPUDistributingLocalScheduler
     elif scheduler == "kluster":
         return KlusterThreadLimitingScheduler
     else:
         raise NotImplementedError
 
 
+class CpuDistributingLocalScheduler(AbstractScheduler):
+    def __init__(self, conf: cw_config.Config = None):
+        super(CpuDistributingLocalScheduler, self).__init__(conf=conf)
+        self._total_num_cpus = conf.slurm_config['cpus-per-task'] * conf.slurm_config['ntasks']
+        self._cpus_per_rep = conf.slurm_config['cpus_per_rep']
+        assert self._cpus_per_rep == int(self._cpus_per_rep), "cpus_per_rep must be integer"
+        self._queue_elements = int(self._total_num_cpus / self._cpus_per_rep)
+        print("CPUDistributingLocalScheduler: {} CPUs available, {} CPUs per rep, {} queue elements".format(
+            self._total_num_cpus, self._cpus_per_rep, self._queue_elements))
+
+    def run(self, overwrite: bool = False):
+        print("Seeing CPUs:", os.sched_getaffinity(0))
+        num_parallel = self.joblist[0].n_parallel
+        for j in self.joblist:
+            assert j.n_parallel == num_parallel, "All jobs in list must have same n_parallel"
+            assert j.n_parallel == self._queue_elements, "Mismatch between CPUs Queue Elements and Jobs executed in" \
+                                                         "parallel. Fix for optimal resource usage!!"
+
+        with concurrent.futures.ProcessPoolExecutor(max_workers=num_parallel,
+                                                    ) as pool:
+            # setup gpu resource queue
+            m = multiprocessing.Manager()
+            cpu_queue = m.Queue(maxsize=self._queue_elements)
+            for i in range(self._queue_elements):
+                cpu_queue.put(i)
+
+            for j in self.joblist:
+                for c in j.tasks:
+                    pool.submit(
+                        CpuDistributingLocalScheduler._execute_task,
+                        j, c, cpu_queue, self._cpus_per_rep,
+                        overwrite)
+
+    @staticmethod
+    def _execute_task(j: job.Job,
+                      c: dict,
+                      q: multiprocessing.Queue,
+                      cpus_per_rep: int,
+                      overwrite: bool = False):
+        print("Seeing CPUs:", os.sched_getaffinity(0))
+        queue_idx = q.get()
+        cpus = set(range(queue_idx * cpus_per_rep, (queue_idx + 1) * cpus_per_rep))
+        print("Job {}: Using CPUs: {}".format(queue_idx, cpus))
+        try:
+            os.sched_setaffinity(0, cpus)
+            c[KEYS.i_CPU_CORES] = cpus
+            j.run_task(c, overwrite)
+        except cw_error.ExperimentSurrender as _:
+            return
+        finally:
+            q.put(queue_idx)
+
+    @staticmethod
+    def use_distributed_cpu_scheduling(conf: cw_config.Config) -> bool:
+        if conf.slurm_config is None:
+            return False
+        else:
+            scheduler = conf.slurm_config.get('scheduler', None)
+            return scheduler == 'cpu_distribute'
+
 class LocalScheduler(AbstractScheduler):
     def run(self, overwrite: bool = False):
         for j in self.joblist:
             Parallel(n_jobs=j.n_parallel)(delayed(self.execute_task)(j, c, overwrite)
                                           for c in j.tasks)
 
     def execute_task(self, j: job.Job, c: dict, overwrite: bool = False):
```

### Comparing `cw2-2.1.1/cw2/util.py` & `cw2-2.2/cw2/util.py`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/cw2.egg-info/PKG-INFO` & `cw2-2.2/cw2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cw2
-Version: 2.1.1
+Version: 2.2
 Summary: A reengineered framework to run experiments on a computing cluster.
 Home-page: https://github.com/ALRhub/cw2
 Author: Maximilian Li
 Author-email: maximilian.xiling.li@gmail.com
 License: MIT
 Keywords: scientific,experiments,distributed computing,mpi,research
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cw2-2.1.1/cw2.egg-info/SOURCES.txt` & `cw2-2.2/cw2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cw2-2.1.1/setup.py` & `cw2-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='cw2',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.1.1',
+    version='2.2',
 
     description='A reengineered framework to run experiments on a computing cluster.',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/ALRhub/cw2',
```

### Comparing `cw2-2.1.1/test/test_cw_config.py` & `cw2-2.2/test/test_cw_config.py`

 * *Files identical despite different names*

