# Comparing `tmp/turingpoint-0.0.2.tar.gz` & `tmp/turingpoint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turingpoint-0.0.2.tar", last modified: Sat Jan 21 15:37:54 2023, max compression
+gzip compressed data, was "turingpoint-0.0.3.tar", last modified: Mon Apr 24 11:56:15 2023, max compression
```

## Comparing `turingpoint-0.0.2.tar` & `turingpoint-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-01-21 15:37:54.700000 turingpoint-0.0.2/
--rw-r--r--   0 oren      (1000) oren      (1000)     6927 2023-01-21 15:37:54.700000 turingpoint-0.0.2/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)     6137 2023-01-21 14:31:35.000000 turingpoint-0.0.2/README.md
--rw-r--r--   0 oren      (1000) oren      (1000)      103 2023-01-21 13:37:50.000000 turingpoint-0.0.2/pyproject.toml
--rw-r--r--   0 oren      (1000) oren      (1000)     1044 2023-01-21 15:37:54.700000 turingpoint-0.0.2/setup.cfg
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-01-21 15:37:54.700000 turingpoint-0.0.2/turingpoint/
--rw-r--r--   0 oren      (1000) oren      (1000)       82 2023-01-21 15:37:08.000000 turingpoint-0.0.2/turingpoint/__init__.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1448 2023-01-21 14:08:54.000000 turingpoint-0.0.2/turingpoint/assembly.py
--rw-r--r--   0 oren      (1000) oren      (1000)      476 2023-01-20 16:18:22.000000 turingpoint-0.0.2/turingpoint/definitions.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1809 2023-01-21 12:28:20.000000 turingpoint-0.0.2/turingpoint/gym_utils.py
--rw-r--r--   0 oren      (1000) oren      (1000)      138 2023-01-21 12:14:23.000000 turingpoint-0.0.2/turingpoint/utils.py
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-01-21 15:37:54.700000 turingpoint-0.0.2/turingpoint.egg-info/
--rw-r--r--   0 oren      (1000) oren      (1000)     6927 2023-01-21 15:37:54.000000 turingpoint-0.0.2/turingpoint.egg-info/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)      359 2023-01-21 15:37:54.000000 turingpoint-0.0.2/turingpoint.egg-info/SOURCES.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-01-21 15:37:54.000000 turingpoint-0.0.2/turingpoint.egg-info/dependency_links.txt
--rw-r--r--   0 oren      (1000) oren      (1000)       68 2023-01-21 15:37:54.000000 turingpoint-0.0.2/turingpoint.egg-info/requires.txt
--rw-r--r--   0 oren      (1000) oren      (1000)       12 2023-01-21 15:37:54.000000 turingpoint-0.0.2/turingpoint.egg-info/top_level.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-01-21 13:51:35.000000 turingpoint-0.0.2/turingpoint.egg-info/zip-safe
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-04-24 11:56:15.292458 turingpoint-0.0.3/
+-rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-04-24 11:56:15.292458 turingpoint-0.0.3/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)     6233 2023-02-25 19:46:15.000000 turingpoint-0.0.3/README.md
+-rw-r--r--   0 oren      (1000) oren      (1000)      103 2023-01-21 13:37:50.000000 turingpoint-0.0.3/pyproject.toml
+-rw-r--r--   0 oren      (1000) oren      (1000)     1185 2023-04-24 11:56:15.292458 turingpoint-0.0.3/setup.cfg
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-04-24 11:56:15.292458 turingpoint-0.0.3/turingpoint/
+-rw-r--r--   0 oren      (1000) oren      (1000)      136 2023-04-24 11:12:09.000000 turingpoint-0.0.3/turingpoint/__init__.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1448 2023-01-21 14:08:54.000000 turingpoint-0.0.3/turingpoint/assembly.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      476 2023-01-20 16:18:22.000000 turingpoint-0.0.3/turingpoint/definitions.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1433 2023-04-24 11:08:57.000000 turingpoint-0.0.3/turingpoint/gymnasium_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      435 2023-04-24 11:09:05.000000 turingpoint-0.0.3/turingpoint/sb3_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1778 2023-02-10 15:09:28.000000 turingpoint-0.0.3/turingpoint/self_play.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      862 2023-04-24 10:31:58.000000 turingpoint-0.0.3/turingpoint/utils.py
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-04-24 11:56:15.292458 turingpoint-0.0.3/turingpoint.egg-info/
+-rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)      415 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)      146 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/requires.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)       12 2023-04-24 11:56:15.000000 turingpoint-0.0.3/turingpoint.egg-info/top_level.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-01-21 13:51:35.000000 turingpoint-0.0.3/turingpoint.egg-info/zip-safe
```

### Comparing `turingpoint-0.0.2/PKG-INFO` & `turingpoint-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turingpoint
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reinforcement Learning (RL) library
 Home-page: https://github.com/zbenmo/turingpoint
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 Keywords: Reinforcement Learning,Framework,Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,26 +16,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 
 # turingpoint
 
-Turing point is a Reinforcement Learning (RL) library.
+Turing point is a Reinforcement Learning (RL) library. It adds the missing duck tape.
 It allows for multiple (hetrogenous) agents seamlessly. Per-agent partial observation is natural with Turing point.
 Different agents can act in differnet frequencies.
-You may opt to continue using also the libraries that you're currently using, such as Gym, Stable-Baselines3, RLLib, etc.
+You may opt to continue using also the environment and the agent libraries that you're currently using, for the such as Gym/Gymnasium, Stable-Baselines3, Tianshou, RLLib, etc.
 Turing point integrates easily with existing RL libraries and your own custom code.
 Integration of RL agents in the target applications should be significantly easier with Turing point.
 
 The main concept in Turing point is that there are multiple participants and each gets its turn.
 The participants communicate by a parcel that is passed among them. The agent and the environment are both participants in that sense. No more confusion which of those should call which. Reward's logic, for example,
 can be addressed where you believe is most suitable.
 
-Turing point may be helpful with parallel or distributed training, yet it does not address those implicitly. On the contrary; with Turing point the flow is sequential between the participants. As far as we can tell Turing point at least does not hinder the use of parallel and / or parallel training.
+Turing point may be helpful with parallel or distributed training, yet Turing point does not address those explicitly. On the contrary; with Turing point the flow is sequential among the participants. As far as we can tell Turing point at least does not hinder the use of parallel and / or distributed training.
 
 Participants can be added and / or removed dynamically (ex. a new "monster" enters or then "disappears").
 
 Consider a Gym/SB3 training realm:
 
 ```python
 import gym
```

### Comparing `turingpoint-0.0.2/README.md` & `turingpoint-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # turingpoint
 
-Turing point is a Reinforcement Learning (RL) library.
+Turing point is a Reinforcement Learning (RL) library. It adds the missing duck tape.
 It allows for multiple (hetrogenous) agents seamlessly. Per-agent partial observation is natural with Turing point.
 Different agents can act in differnet frequencies.
-You may opt to continue using also the libraries that you're currently using, such as Gym, Stable-Baselines3, RLLib, etc.
+You may opt to continue using also the environment and the agent libraries that you're currently using, for the such as Gym/Gymnasium, Stable-Baselines3, Tianshou, RLLib, etc.
 Turing point integrates easily with existing RL libraries and your own custom code.
 Integration of RL agents in the target applications should be significantly easier with Turing point.
 
 The main concept in Turing point is that there are multiple participants and each gets its turn.
 The participants communicate by a parcel that is passed among them. The agent and the environment are both participants in that sense. No more confusion which of those should call which. Reward's logic, for example,
 can be addressed where you believe is most suitable.
 
-Turing point may be helpful with parallel or distributed training, yet it does not address those implicitly. On the contrary; with Turing point the flow is sequential between the participants. As far as we can tell Turing point at least does not hinder the use of parallel and / or parallel training.
+Turing point may be helpful with parallel or distributed training, yet Turing point does not address those explicitly. On the contrary; with Turing point the flow is sequential among the participants. As far as we can tell Turing point at least does not hinder the use of parallel and / or distributed training.
 
 Participants can be added and / or removed dynamically (ex. a new "monster" enters or then "disappears").
 
 Consider a Gym/SB3 training realm:
 
 ```python
 import gym
```

### Comparing `turingpoint-0.0.2/setup.cfg` & `turingpoint-0.0.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -21,20 +21,23 @@
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
-	tqdm
+	tqdm # not really, just don't know how to leave it empty
 
 [options.extras_require]
 examples = 
-	gym >= 0.21, < 0.22
-	stable-baselines3 >= 1.6.2, < 1.7
+	gymnasium >= 0.28.1, < 0.29
+	stable-baselines3[extra] >= 2.0.0a5, < 2.1
+	pettingzoo[classic] >= 1.22.3, < 1.23
+	tianshou >= 0.5.0, < 0.6
+	numpy
 	tqdm
 
 [options.package_data]
 * = README.md
 
 [egg_info]
 tag_build =
```

### Comparing `turingpoint-0.0.2/turingpoint/assembly.py` & `turingpoint-0.0.3/turingpoint/assembly.py`

 * *Files identical despite different names*

### Comparing `turingpoint-0.0.2/turingpoint/gym_utils.py` & `turingpoint-0.0.3/turingpoint/gymnasium_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 from typing import Generator, List
-from turingpoint import Assembly
-from turingpoint.definitions import Participant
-import stable_baselines3.common
-import gym
-
-
-class AgentParticipant(Participant):
-  def __init__(self,
-               agent: stable_baselines3.common.base_class.BaseAlgorithm,
-               **kwargs):
-    self.agent = agent
-    self.kwargs = kwargs
-
-  def __call__(self, parcel: dict) -> None:
-    obs = parcel['obs']
-    action, _state = self.agent.predict(obs, **self.kwargs)
-    parcel['action'] = action
+from turingpoint import Assembly, Participant
+import gymnasium as gym
 
 
 class EnvironmentParticipant(Participant):
   def __init__(self, env: gym.Env, save_obs_as="obs"):
-    self.env = env
-    self.save_obs_as = save_obs_as
+    self._env = env
+    self._save_obs_as = save_obs_as
 
   def __call__(self, parcel: dict) -> None:
     action = parcel['action']
-    obs, reward, done, info = self.env.step(action)
-    # this version of gym is still with done (if you have terminate + truncated) modify it accordingly
-    parcel[self.save_obs_as] = obs
+    obs, reward, terminated, truncated, info = self._env.step(action)
+    parcel[self._save_obs_as] = obs
     parcel['reward'] = reward
-    parcel['done'] = done
+    parcel['terminated'] = terminated
+    parcel['truncated'] = truncated
     parcel['info'] = info
 
 
 class RenderParticipant(Participant):
   def __init__(self, env: gym.Env):
-    self.env = env
+    self._env = env
 
   def __call__(self, _: dict):
-    self.env.render()
+    self._env.render()
 
 
-class GymAssembly(Assembly):
+class GymnasiumAssembly(Assembly):
   def __init__(self, env: gym.Env, participants_list: List[Participant]):
-    self.env = env
-    self.participants_list = participants_list
+    self._env = env
+    self._participants_list = participants_list
 
   def create_initial_parcel(self) -> dict:
-    obs = self.env.reset()
+    obs, info = self._env.reset()
     parcel = {
-      'obs': obs
+      'obs': obs,
+      'info': info
     }
     return parcel
 
   def participants(self) -> Generator[Participant, None, None]:
     done = False
 
     def check_done(parcel: dict) -> None:
       "a helper participant for checking for 'done' in the parcel"
 
       nonlocal done
-      done = parcel.get('done', False)
+      done = parcel.get('terminated', False) or parcel.get('truncated', False)
 
     while not done:
-      yield from self.participants_list
+      yield from self._participants_list
       yield check_done
```

### Comparing `turingpoint-0.0.2/turingpoint.egg-info/PKG-INFO` & `turingpoint-0.0.3/turingpoint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turingpoint
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reinforcement Learning (RL) library
 Home-page: https://github.com/zbenmo/turingpoint
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 Keywords: Reinforcement Learning,Framework,Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,26 +16,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 
 # turingpoint
 
-Turing point is a Reinforcement Learning (RL) library.
+Turing point is a Reinforcement Learning (RL) library. It adds the missing duck tape.
 It allows for multiple (hetrogenous) agents seamlessly. Per-agent partial observation is natural with Turing point.
 Different agents can act in differnet frequencies.
-You may opt to continue using also the libraries that you're currently using, such as Gym, Stable-Baselines3, RLLib, etc.
+You may opt to continue using also the environment and the agent libraries that you're currently using, for the such as Gym/Gymnasium, Stable-Baselines3, Tianshou, RLLib, etc.
 Turing point integrates easily with existing RL libraries and your own custom code.
 Integration of RL agents in the target applications should be significantly easier with Turing point.
 
 The main concept in Turing point is that there are multiple participants and each gets its turn.
 The participants communicate by a parcel that is passed among them. The agent and the environment are both participants in that sense. No more confusion which of those should call which. Reward's logic, for example,
 can be addressed where you believe is most suitable.
 
-Turing point may be helpful with parallel or distributed training, yet it does not address those implicitly. On the contrary; with Turing point the flow is sequential between the participants. As far as we can tell Turing point at least does not hinder the use of parallel and / or parallel training.
+Turing point may be helpful with parallel or distributed training, yet Turing point does not address those explicitly. On the contrary; with Turing point the flow is sequential among the participants. As far as we can tell Turing point at least does not hinder the use of parallel and / or distributed training.
 
 Participants can be added and / or removed dynamically (ex. a new "monster" enters or then "disappears").
 
 Consider a Gym/SB3 training realm:
 
 ```python
 import gym
```

