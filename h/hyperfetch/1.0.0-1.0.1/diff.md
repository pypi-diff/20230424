# Comparing `tmp/hyperfetch-1.0.0.tar.gz` & `tmp/hyperfetch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfetch-1.0.0.tar", last modified: Mon Apr 17 09:59:37 2023, max compression
+gzip compressed data, was "hyperfetch-1.0.1.tar", last modified: Mon Apr 24 12:53:43 2023, max compression
```

## Comparing `hyperfetch-1.0.0.tar` & `hyperfetch-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:37.101065 hyperfetch-1.0.0/
--rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    10283 2023-04-17 09:59:37.101065 hyperfetch-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7860 2023-04-16 23:07:53.000000 hyperfetch-1.0.0/README.md
--rw-rw-rw-   0        0        0     4782 2023-04-16 23:02:22.000000 hyperfetch-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 09:59:37.101065 hyperfetch-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:37.034459 hyperfetch-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:37.073137 hyperfetch-1.0.0/src/hyperfetch/
--rw-rw-rw-   0        0        0        0 2023-04-16 16:06:24.000000 hyperfetch-1.0.0/src/hyperfetch/__init__.py
--rw-rw-rw-   0        0        0    10569 2023-04-15 07:49:41.000000 hyperfetch-1.0.0/src/hyperfetch/alg_samplers.py
--rw-rw-rw-   0        0        0      654 2023-04-16 21:41:06.000000 hyperfetch-1.0.0/src/hyperfetch/auth_connection.py
--rw-rw-rw-   0        0        0     2118 2023-04-13 19:35:11.000000 hyperfetch-1.0.0/src/hyperfetch/callbacks.py
--rw-rw-rw-   0        0        0    33062 2023-04-17 09:32:09.000000 hyperfetch-1.0.0/src/hyperfetch/manager.py
--rw-rw-rw-   0        0        0     4901 2023-04-16 22:22:27.000000 hyperfetch-1.0.0/src/hyperfetch/tuning.py
--rw-rw-rw-   0        0        0      825 2023-04-16 16:50:23.000000 hyperfetch-1.0.0/src/hyperfetch/util.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:59:37.099081 hyperfetch-1.0.0/src/hyperfetch.egg-info/
--rw-rw-rw-   0        0        0    10283 2023-04-17 09:59:37.000000 hyperfetch-1.0.0/src/hyperfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-17 09:59:37.000000 hyperfetch-1.0.0/src/hyperfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:59:37.000000 hyperfetch-1.0.0/src/hyperfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-17 09:59:37.000000 hyperfetch-1.0.0/src/hyperfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     2238 2023-04-17 09:59:37.000000 hyperfetch-1.0.0/src/hyperfetch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 09:59:37.000000 hyperfetch-1.0.0/src/hyperfetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 12:53:43.980290 hyperfetch-1.0.1/
+-rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    10284 2023-04-24 12:53:43.979295 hyperfetch-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7860 2023-04-17 10:07:09.000000 hyperfetch-1.0.1/README.md
+-rw-rw-rw-   0        0        0     4783 2023-04-17 10:03:34.000000 hyperfetch-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:53:43.980290 hyperfetch-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 12:53:43.932903 hyperfetch-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 12:53:43.949729 hyperfetch-1.0.1/src/hyperfetch/
+-rw-rw-rw-   0        0        0        0 2023-04-16 16:06:24.000000 hyperfetch-1.0.1/src/hyperfetch/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-04-15 07:49:41.000000 hyperfetch-1.0.1/src/hyperfetch/alg_samplers.py
+-rw-rw-rw-   0        0        0      654 2023-04-16 21:41:06.000000 hyperfetch-1.0.1/src/hyperfetch/auth_connection.py
+-rw-rw-rw-   0        0        0     2118 2023-04-13 19:35:11.000000 hyperfetch-1.0.1/src/hyperfetch/callbacks.py
+-rw-rw-rw-   0        0        0    33242 2023-04-24 12:09:42.000000 hyperfetch-1.0.1/src/hyperfetch/manager.py
+-rw-rw-rw-   0        0        0     4996 2023-04-24 11:58:31.000000 hyperfetch-1.0.1/src/hyperfetch/tuning.py
+-rw-rw-rw-   0        0        0      825 2023-04-16 16:50:23.000000 hyperfetch-1.0.1/src/hyperfetch/util.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:53:43.978306 hyperfetch-1.0.1/src/hyperfetch.egg-info/
+-rw-rw-rw-   0        0        0    10284 2023-04-24 12:53:43.000000 hyperfetch-1.0.1/src/hyperfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-24 12:53:43.000000 hyperfetch-1.0.1/src/hyperfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:53:43.000000 hyperfetch-1.0.1/src/hyperfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-24 12:53:43.000000 hyperfetch-1.0.1/src/hyperfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     2238 2023-04-24 12:53:43.000000 hyperfetch-1.0.1/src/hyperfetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 12:53:43.000000 hyperfetch-1.0.1/src/hyperfetch.egg-info/top_level.txt
```

### Comparing `hyperfetch-1.0.0/LICENSE` & `hyperfetch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.0/PKG-INFO` & `hyperfetch-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.0
+Version: 1.0.1
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
-Author-email: Karoline Sund Wahl <karolies.wahl@gmail.com>
+Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, 
            this list of conditions and the following disclaimer.
```

### Comparing `hyperfetch-1.0.0/README.md` & `hyperfetch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.0/pyproject.toml` & `hyperfetch-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["hyperfetch"]
 
 [project]
 name = "hyperfetch"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
-  { name="Karoline Sund Wahl", email="karolies.wahl@gmail.com" },
+  { name="Karoline Sund Wahl", email="karolines.wahl@gmail.com" },
 ]
 description = "HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["reinforcement learning", "hyperparameters", "replication"]
```

### Comparing `hyperfetch-1.0.0/src/hyperfetch/alg_samplers.py` & `hyperfetch-1.0.1/src/hyperfetch/alg_samplers.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.0/src/hyperfetch/auth_connection.py` & `hyperfetch-1.0.1/src/hyperfetch/auth_connection.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.0/src/hyperfetch/callbacks.py` & `hyperfetch-1.0.1/src/hyperfetch/callbacks.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.0/src/hyperfetch/manager.py` & `hyperfetch-1.0.1/src/hyperfetch/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from optuna.samplers import RandomSampler, TPESampler, CmaEsSampler, NSGAIISampler
 from optuna.trial import FrozenTrial
 from stable_baselines3 import PPO, DQN, A2C, TD3, SAC
 from stable_baselines3.common.env_util import make_vec_env
 from stable_baselines3.common.preprocessing import is_image_space, is_image_space_channels_first
 from stable_baselines3.common.vec_env import VecTransposeImage, is_vecenv_wrapped
 from stable_baselines3.common.vec_env.vec_frame_stack import VecFrameStack
-from .util import *
-from .alg_samplers import ALG_HP_SAMPLER
-from .callbacks import TrialEvalCallback, ThresholdExceeded
+from util import *  # todo
+from alg_samplers import ALG_HP_SAMPLER  # todo
+from callbacks import TrialEvalCallback, ThresholdExceeded  # todo
 
 
 def _select_model(alg, **kwargs):
     if alg == "ppo":
         return PPO(**kwargs)
     elif alg == "dqn":
         return DQN(**kwargs)
@@ -257,15 +257,15 @@
 
         if 'project_name' not in data.keys():
             logger.error("The name of the project 'project_name' must be specified in config at path %s",
                          path_to_config, stack_info=True)
             logger.info("If you are using HyperFetch with no correlation to a Git-proejct, "
                         "simply give the parameter an empty string as value. ")
 
-        if 'policy' not in data.keys() :
+        if 'policy' not in data.keys():
             logger.info('No policy was specified. Config value "policy" set to "MlpPolicy". '
                         'Policies available: "MlpPolicy", "CnnPolicy", "MultiInputPolicy"')
             data.update({'policy': 'MlpPolicy'})
             with open(path_to_config, "w") as writer:
                 yaml.safe_dump(data, writer)
 
         if 'reward_threshold' not in data.keys():
@@ -674,14 +674,16 @@
                'gpu_model': gpu_model,
                'CO2_emissions': emissions,
                'alg': self.alg,
                'env': self.env,
                'git_link': self.git_link,
                'project_name': self.project_name,
                'total_time': duration,
+               'sampler': self.sampler,
+               'pruner': self.pruner,
                'reward': trial.value}
 
         print("Posting...")
 
         await my_client[db][collection].insert_one(run)
         print("Posted!")
         print("\n\nTo filter-search for your run on the website, use the run ID:\n ", run_id + "\n")
@@ -699,14 +701,16 @@
         print("Preparing config hyperparameters for persistance...")
 
         run = {'_id': run_id,
                'trial': hyperparameters,
                'alg': self.alg,
                'env': self.env,
                'git_link': self.git_link,
+               'sampler': self.sampler,
+               'pruner': self.pruner,
                'project_name': self.project_name}
 
         # Add energy consumed to run
         if 'energy_consumed' not in config_dict.keys():
             run['energy_consumed'] = None
         else:
             run['energy_consumed'] = config_dict['energy_consumed']
```

### Comparing `hyperfetch-1.0.0/src/hyperfetch/tuning.py` & `hyperfetch-1.0.1/src/hyperfetch/tuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
-from .manager import Manager
+from manager import Manager #todo
 from codecarbon import EmissionsTracker
 import asyncio
 from motor.motor_asyncio import AsyncIOMotorClient
-from .auth_connection import MONGODB_URL, MONGO_DB, MONGO_COLLECTION
+from auth_connection import MONGODB_URL, MONGO_DB, MONGO_COLLECTION #todo
 
 client = AsyncIOMotorClient(MONGODB_URL)
 
 # Tracks emissions (writes to emissions.csv)
 tracker = EmissionsTracker()
 
 
@@ -107,7 +107,10 @@
                                                  'tuned in HyperFetch.')
     parser.add_argument('config_path', type=str, help='The path to the config file (.yaml). Can be a new file or t'
                                                       'he same as for the tuning() method.')
 
     args = parser.parse_args()
     manager = Manager(config_path=args.config_path)
     asyncio.run(manager.save_custom(client=MONGODB_URL, db=MONGO_DB, collection=MONGO_COLLECTION))
+
+if __name__ == '__main__':
+    tune(config_path="../config/tuning_parameters.yml")
```

### Comparing `hyperfetch-1.0.0/src/hyperfetch/util.py` & `hyperfetch-1.0.1/src/hyperfetch/util.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.0.0/src/hyperfetch.egg-info/PKG-INFO` & `hyperfetch-1.0.1/src/hyperfetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.0.0
+Version: 1.0.1
 Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application.
-Author-email: Karoline Sund Wahl <karolies.wahl@gmail.com>
+Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, 
            this list of conditions and the following disclaimer.
```

### Comparing `hyperfetch-1.0.0/src/hyperfetch.egg-info/requires.txt` & `hyperfetch-1.0.1/src/hyperfetch.egg-info/requires.txt`

 * *Files identical despite different names*

