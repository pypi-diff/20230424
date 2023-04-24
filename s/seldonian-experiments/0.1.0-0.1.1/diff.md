# Comparing `tmp/seldonian_experiments-0.1.0.tar.gz` & `tmp/seldonian_experiments-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldonian_experiments-0.1.0.tar", last modified: Tue Mar 28 17:07:13 2023, max compression
+gzip compressed data, was "seldonian_experiments-0.1.1.tar", last modified: Mon Apr 24 16:32:29 2023, max compression
```

## Comparing `seldonian_experiments-0.1.0.tar` & `seldonian_experiments-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-03-28 17:07:13.276654 seldonian_experiments-0.1.0/
--rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.1.0/LICENSE
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-03-28 17:07:13.276489 seldonian_experiments-0.1.0/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.1.0/README.md
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-03-28 17:07:13.272020 seldonian_experiments-0.1.0/examples/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.1.0/examples/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.1.0/examples/run_examples.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-03-28 17:07:13.274528 seldonian_experiments-0.1.0/experiments/
--rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.1.0/experiments/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4058 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.0/experiments/base_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    46934 2023-03-27 18:09:43.000000 seldonian_experiments-0.1.0/experiments/experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)    38348 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.0/experiments/generate_plots.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3384 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.0/experiments/headless_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    17185 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.0/experiments/headless_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.0/experiments/headless_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     9342 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.0/experiments/utils.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-03-28 17:07:13.275358 seldonian_experiments-0.1.0/seldonian_experiments.egg-info/
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-03-28 17:07:13.000000 seldonian_experiments-0.1.0/seldonian_experiments.egg-info/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      615 2023-03-28 17:07:13.000000 seldonian_experiments-0.1.0/seldonian_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-03-28 17:07:13.000000 seldonian_experiments-0.1.0/seldonian_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-03-28 17:07:13.000000 seldonian_experiments-0.1.0/seldonian_experiments.egg-info/requires.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-03-28 17:07:13.000000 seldonian_experiments-0.1.0/seldonian_experiments.egg-info/top_level.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-03-28 17:07:13.276709 seldonian_experiments-0.1.0/setup.cfg
--rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-03-28 17:06:52.000000 seldonian_experiments-0.1.0/setup.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-03-28 17:07:13.276180 seldonian_experiments-0.1.0/tests/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.1.0/tests/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4257 2023-01-09 18:12:54.000000 seldonian_experiments-0.1.0/tests/conftest.py
--rw-r--r--   0 ahoag      (501) staff       (20)      713 2022-09-27 22:42:46.000000 seldonian_experiments-0.1.0/tests/test_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)    15160 2023-01-09 18:12:57.000000 seldonian_experiments-0.1.0/tests/test_generate_plots.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.216580 seldonian_experiments-0.1.1/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.1.1/LICENSE
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-04-24 16:32:29.216421 seldonian_experiments-0.1.1/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.1.1/README.md
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.211504 seldonian_experiments-0.1.1/examples/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.1.1/examples/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.1.1/examples/run_examples.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.214419 seldonian_experiments-0.1.1/experiments/
+-rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.1.1/experiments/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4058 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/base_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    46934 2023-03-27 18:09:43.000000 seldonian_experiments-0.1.1/experiments/experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    38683 2023-04-24 16:30:24.000000 seldonian_experiments-0.1.1/experiments/generate_plots.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3357 2023-04-24 16:25:04.000000 seldonian_experiments-0.1.1/experiments/headless_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    17185 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/headless_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/headless_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     9342 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/utils.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.215300 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      615 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/requires.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/top_level.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-04-24 16:32:29.216623 seldonian_experiments-0.1.1/setup.cfg
+-rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-04-24 16:32:18.000000 seldonian_experiments-0.1.1/setup.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.216085 seldonian_experiments-0.1.1/tests/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.1.1/tests/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4257 2023-01-09 18:12:54.000000 seldonian_experiments-0.1.1/tests/conftest.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      713 2022-09-27 22:42:46.000000 seldonian_experiments-0.1.1/tests/test_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    15190 2023-04-13 15:54:44.000000 seldonian_experiments-0.1.1/tests/test_generate_plots.py
```

### Comparing `seldonian_experiments-0.1.0/LICENSE` & `seldonian_experiments-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/PKG-INFO` & `seldonian_experiments-0.1.1/seldonian_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seldonian_experiments
-Version: 0.1.0
+Name: seldonian-experiments
+Version: 0.1.1
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.1.0/examples/run_examples.py` & `seldonian_experiments-0.1.1/examples/run_examples.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/experiments/base_example.py` & `seldonian_experiments-0.1.1/experiments/base_example.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/experiments/experiments.py` & `seldonian_experiments-0.1.1/experiments/experiments.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/experiments/generate_plots.py` & `seldonian_experiments-0.1.1/experiments/generate_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,18 @@
         :param savename: If not None, the filename path to which the plot
                 will be saved on disk.
         :type savename: str, defaults to None
         """
         plt.style.use("bmh")
         # plt.style.use('grayscale')
         regime = self.spec.dataset.regime
-        tot_data_size = self.spec.dataset.num_datapoints
+        if regime == "supervised_learning":
+            tot_data_size = self.spec.dataset.num_datapoints
+        else:
+            tot_data_size = self.hyperparameter_and_setting_dict['num_episodes']
 
         # Read in constraints
         parse_trees = self.spec.parse_trees
 
         constraint_dict = {}
         for pt_ii, pt in enumerate(parse_trees):
             delta = pt.delta
@@ -311,16 +314,16 @@
                 ).mean()["performance"]
                 baseline_std_performance = df_baseline_valid.groupby("data_frac").std()[
                     "performance"
                 ]
                 baseline_ste_performance = baseline_std_performance / np.sqrt(n_trials)
                 X_valid_baseline = this_baseline_dict["X_valid"]
                 (pl,) = ax_performance.plot(
-                    X_valid_baseline,
-                    baseline_mean_performance,
+                    X_valid_baseline.to_numpy(),
+                    baseline_mean_performance.to_numpy(),
                     color=baseline_color,
                     label=baseline,
                 )
                 legend_handles.append(pl)
                 if baseline in model_label_dict:
                     legend_labels.append(model_label_dict[baseline])
                 else:
@@ -336,29 +339,30 @@
                     X_valid_baseline,
                     baseline_mean_performance - baseline_ste_performance,
                     baseline_mean_performance + baseline_ste_performance,
                     color=baseline_color,
                     alpha=0.5,
                 )
 
+            # Seldonian performance
             for seldonian_i, seldonian_model in enumerate(seldonian_models):
                 this_seldonian_dict = seldonian_dict[seldonian_model]
                 seldonian_color = plot_colormap(seldonian_i)
                 df_seldonian_passed = this_seldonian_dict["df_seldonian_passed"]
                 mean_performance = df_seldonian_passed.groupby("data_frac").mean()[
                     "performance"
-                ]
+                ].to_numpy()
                 std_performance = df_seldonian_passed.groupby("data_frac").std()[
                     "performance"
-                ]
+                ].to_numpy()
                 n_passed = df_seldonian_passed.groupby("data_frac").count()[
                     "performance"
-                ]
+                ].to_numpy()
                 ste_performance = std_performance / np.sqrt(n_passed)
-                X_passed_seldonian = this_seldonian_dict["X_passed"]
+                X_passed_seldonian = this_seldonian_dict["X_passed"].to_numpy()
                 (pl,) = ax_performance.plot(
                     X_passed_seldonian,
                     mean_performance,
                     color=seldonian_color,
                     linestyle="--",
                 )
                 legend_handles.append(pl)
@@ -389,23 +393,22 @@
             ##########################
 
             # Plot baseline solution rate
             # (sometimes it doesn't return a solution due to not having enough training data
             # to run model.fit() )
             for baseline_i, baseline in enumerate(baselines):
                 this_baseline_dict = baseline_dict[baseline]
-                X_all_baseline = this_baseline_dict["X_all"]
                 baseline_color = plot_colormap(baseline_i + len(seldonian_models))
                 df_baseline = this_baseline_dict["df_baseline"]
                 n_trials = df_baseline["trial_i"].max() + 1
-                mean_sr = df_baseline.groupby("data_frac").mean()["solution_returned"]
-                std_sr = df_baseline.groupby("data_frac").std()["solution_returned"]
+                mean_sr = df_baseline.groupby("data_frac").mean()["solution_returned"].to_numpy()
+                std_sr = df_baseline.groupby("data_frac").std()["solution_returned"].to_numpy()
                 ste_sr = std_sr / np.sqrt(n_trials)
 
-                X_all_baseline = this_baseline_dict["X_all"]
+                X_all_baseline = this_baseline_dict["X_all"].to_numpy()
 
                 ax_sr.plot(
                     X_all_baseline, mean_sr, color=baseline_color, label=baseline
                 )
                 ax_sr.scatter(
                     X_all_baseline,
                     mean_sr,
@@ -417,24 +420,25 @@
                     X_all_baseline,
                     mean_sr - ste_sr,
                     mean_sr + ste_sr,
                     color=baseline_color,
                     alpha=0.5,
                 )
 
+            # Seldonian solution rate
             for seldonian_i, seldonian_model in enumerate(seldonian_models):
                 this_seldonian_dict = seldonian_dict[seldonian_model]
                 seldonian_color = plot_colormap(seldonian_i)
                 df_seldonian = this_seldonian_dict["df_seldonian"]
                 n_trials = df_seldonian["trial_i"].max() + 1
-                mean_sr = df_seldonian.groupby("data_frac").mean()["passed_safety"]
-                std_sr = df_seldonian.groupby("data_frac").std()["passed_safety"]
+                mean_sr = df_seldonian.groupby("data_frac").mean()["passed_safety"].to_numpy()
+                std_sr = df_seldonian.groupby("data_frac").std()["passed_safety"].to_numpy()
                 ste_sr = std_sr / np.sqrt(n_trials)
 
-                X_all_seldonian = this_seldonian_dict["X_all"]
+                X_all_seldonian = this_seldonian_dict["X_all"].to_numpy()
 
                 ax_sr.plot(
                     X_all_seldonian,
                     mean_sr,
                     color=seldonian_color,
                     linestyle="--",
                     label="QSA",
@@ -457,29 +461,28 @@
             ax_sr.set_ylim(-0.05, 1.05)
 
             ##########################
             ### FAILURE RATE PLOT ###
             ##########################
 
             # Baseline failure rate
-            
             for baseline_i, baseline in enumerate(baselines):
                 baseline_color = plot_colormap(baseline_i + len(seldonian_models))
                 # Baseline performance
                 this_baseline_dict = baseline_dict[baseline]
                 df_baseline_valid = this_baseline_dict["df_baseline_valid"]
                 n_trials = df_baseline_valid["trial_i"].max() + 1
 
                 baseline_mean_fr = df_baseline_valid.groupby("data_frac").mean()[
                     "failed"
-                ]
-                baseline_std_fr = df_baseline_valid.groupby("data_frac").std()["failed"]
+                ].to_numpy()
+                baseline_std_fr = df_baseline_valid.groupby("data_frac").std()["failed"].to_numpy()
                 baseline_ste_fr = baseline_std_fr / np.sqrt(n_trials)
 
-                X_valid_baseline = this_baseline_dict["X_valid"]
+                X_valid_baseline = this_baseline_dict["X_valid"].to_numpy()
 
                 ax_fr.plot(
                     X_valid_baseline,
                     baseline_mean_fr,
                     color=baseline_color,
                     label=baseline,
                 )
@@ -494,24 +497,25 @@
                     X_valid_baseline,
                     baseline_mean_fr - baseline_ste_fr,
                     baseline_mean_fr + baseline_ste_fr,
                     color=baseline_color,
                     alpha=0.5,
                 )
 
+            # Seldonian failure rate
             for seldonian_i, seldonian_model in enumerate(seldonian_models):
                 this_seldonian_dict = seldonian_dict[seldonian_model]
                 seldonian_color = plot_colormap(seldonian_i)
                 df_seldonian = this_seldonian_dict["df_seldonian"]
                 n_trials = df_seldonian["trial_i"].max() + 1
-                mean_fr = df_seldonian.groupby("data_frac").mean()["failed"]
-                std_fr = df_seldonian.groupby("data_frac").std()["failed"]
+                mean_fr = df_seldonian.groupby("data_frac").mean()["failed"].to_numpy()
+                std_fr = df_seldonian.groupby("data_frac").std()["failed"].to_numpy()
                 ste_fr = std_fr / np.sqrt(n_trials)
 
-                X_all_seldonian = this_seldonian_dict["X_all"]
+                X_all_seldonian = this_seldonian_dict["X_all"].to_numpy()
                 
                 ax_fr.plot(
                     X_all_seldonian,
                     mean_fr,
                     color=seldonian_color,
                     linestyle="--",
                     label="QSA",
@@ -545,16 +549,15 @@
                 legend_labels[::-1],
                 bbox_to_anchor=(0.5, 0.15),
                 loc="upper center",
                 ncol=ncol,
             )
 
         if savename:
-            # plt.savefig(savename,format=save_format,dpi=600)
-            plt.savefig(savename, format=save_format)
+            plt.savefig(savename, format=save_format,bbox_inches="tight")
             print(f"Saved {savename}")
         else:
             plt.show()
 
 
 class SupervisedPlotGenerator(PlotGenerator):
     def __init__(
```

### Comparing `seldonian_experiments-0.1.0/experiments/headless_example.py` & `seldonian_experiments-0.1.1/experiments/headless_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from .base_example import BaseExample
 
 
 class HeadlessExample(BaseExample):
     def __init__(self, spec):
         """Class for running headless experiments"""
         super().__init__(spec=spec)
-        print(self.regime)
         assert self.regime == "supervised_learning","Headless examples are only supported for supervised learning"
 
     def run(
         self,
         full_pretraining_model,
         headless_pretraining_model,
         head_layer_names,
```

### Comparing `seldonian_experiments-0.1.0/experiments/headless_experiments.py` & `seldonian_experiments-0.1.1/experiments/headless_experiments.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/experiments/headless_utils.py` & `seldonian_experiments-0.1.1/experiments/headless_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/experiments/utils.py` & `seldonian_experiments-0.1.1/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/seldonian_experiments.egg-info/PKG-INFO` & `seldonian_experiments-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seldonian-experiments
-Version: 0.1.0
+Name: seldonian_experiments
+Version: 0.1.1
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.1.0/seldonian_experiments.egg-info/SOURCES.txt` & `seldonian_experiments-0.1.1/seldonian_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/setup.py` & `seldonian_experiments-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seldonian_experiments",
-    version="0.1.0",
+    version="0.1.1",
     author="Austin Hoag",
     author_email="austinthomashoag@gmail.com",
     description="Library for running experiments with Seldonian algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="",
```

### Comparing `seldonian_experiments-0.1.0/tests/conftest.py` & `seldonian_experiments-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/tests/test_experiments.py` & `seldonian_experiments-0.1.1/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.0/tests/test_generate_plots.py` & `seldonian_experiments-0.1.1/tests/test_generate_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,15 @@
 	df_trial0 = pd.read_csv(trial_file_0)
 	assert len(df_trial0) == 1
 
 	# Now make plot
 	savename = os.path.join(results_dir,"test_gpa_classification_plot.png")
 	spg.make_plots(fontsize=12,legend_fontsize=8,
 		performance_label='Accuracy',
+		save_format="png",
 		savename=savename)
 	# Make sure it was saved
 	assert os.path.exists(savename)
 
 @pytest.mark.parametrize('experiment', ["./tests/static/results"], indirect=True)
 def test_too_few_datapoints(gpa_regression_spec,experiment):
 	""" Test that too small of a data_frac resulting in < 1
@@ -483,14 +484,15 @@
 
 	# Make sure the trial files have the right format
 	trial_file_0 = os.path.join(trial_dir,trial_files[0])
 	df_trial0 = pd.read_csv(trial_file_0)
 	assert len(df_trial0) == 1
 
 	# Now make plot
-	# savename = os.path.join(results_dir,"test_gridworld_plot.png")
-	# spg.make_plots(fontsize=12,legend_fontsize=8,
-	# 	performance_label='-IS_estimate',
-	# 	savename=savename)
-	# # Make sure it was saved
-	# assert os.path.exists(savename)
+	savename = os.path.join(results_dir,"test_gridworld_plot.png")
+	spg.make_plots(fontsize=12,legend_fontsize=8,
+		performance_label='-IS_estimate',
+		save_format="png",
+		savename=savename)
+	# Make sure it was saved
+	assert os.path.exists(savename)
```

