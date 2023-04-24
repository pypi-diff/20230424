# Comparing `tmp/funman_demo-1.4.0.tar.gz` & `tmp/funman_demo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funman_demo-1.4.0.tar", last modified: Fri Feb  3 17:05:51 2023, max compression
+gzip compressed data, was "funman_demo-1.5.0.tar", last modified: Mon Apr 24 15:10:17 2023, max compression
```

## Comparing `funman_demo-1.4.0.tar` & `funman_demo-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:51.132064 funman_demo-1.4.0/
--rw-r--r--   0 danbryce   (501) dialout     (20)      276 2023-02-03 17:05:51.130682 funman_demo-1.4.0/PKG-INFO
--rw-r--r--   0 danbryce   (501) dialout     (20)       51 2022-12-23 20:09:23.000000 funman_demo-1.4.0/README.md
--rw-r--r--   0 danbryce   (501) dialout     (20)      177 2022-12-23 20:09:23.000000 funman_demo-1.4.0/pyproject.toml
--rw-r--r--   0 danbryce   (501) dialout     (20)       38 2023-02-03 17:05:51.132777 funman_demo-1.4.0/setup.cfg
--rw-r--r--   0 danbryce   (501) dialout     (20)      844 2022-12-31 21:23:10.000000 funman_demo-1.4.0/setup.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:51.021802 funman_demo-1.4.0/src/
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:51.066235 funman_demo-1.4.0/src/funman_demo/
--rw-r--r--   0 danbryce   (501) dialout     (20)       34 2022-12-23 20:09:23.000000 funman_demo-1.4.0/src/funman_demo/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      127 2023-02-03 17:05:41.000000 funman_demo-1.4.0/src/funman_demo/_version.py
--rw-r--r--   0 danbryce   (501) dialout     (20)    12199 2023-02-01 21:25:58.000000 funman_demo-1.4.0/src/funman_demo/box_plotter.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:51.121652 funman_demo-1.4.0/src/funman_demo/example/
--rw-r--r--   0 danbryce   (501) dialout     (20)     1770 2023-01-20 22:15:58.000000 funman_demo-1.4.0/src/funman_demo/example/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     2921 2023-01-20 22:15:58.000000 funman_demo-1.4.0/src/funman_demo/example/bilayer.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     9453 2022-12-31 21:23:10.000000 funman_demo-1.4.0/src/funman_demo/example/chime.py
--rw-r--r--   0 danbryce   (501) dialout     (20)    36939 2023-01-20 22:15:58.000000 funman_demo-1.4.0/src/funman_demo/example/demo120822.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     3387 2023-02-01 21:25:19.000000 funman_demo-1.4.0/src/funman_demo/handlers.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     2245 2023-02-01 13:26:43.000000 funman_demo-1.4.0/src/funman_demo/plot.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:51.103126 funman_demo-1.4.0/src/funman_demo.egg-info/
--rw-r--r--   0 danbryce   (501) dialout     (20)      276 2023-02-03 17:05:50.000000 funman_demo-1.4.0/src/funman_demo.egg-info/PKG-INFO
--rw-r--r--   0 danbryce   (501) dialout     (20)      577 2023-02-03 17:05:51.000000 funman_demo-1.4.0/src/funman_demo.egg-info/SOURCES.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)        1 2023-02-03 17:05:50.000000 funman_demo-1.4.0/src/funman_demo.egg-info/dependency_links.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)        1 2022-11-09 17:37:37.000000 funman_demo-1.4.0/src/funman_demo.egg-info/not-zip-safe
--rw-r--r--   0 danbryce   (501) dialout     (20)       26 2023-02-03 17:05:50.000000 funman_demo-1.4.0/src/funman_demo.egg-info/requires.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)       12 2023-02-03 17:05:50.000000 funman_demo-1.4.0/src/funman_demo.egg-info/top_level.txt
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:51.126457 funman_demo-1.4.0/test/
--rw-r--r--   0 danbryce   (501) dialout     (20)     1974 2023-01-30 14:42:47.000000 funman_demo-1.4.0/test/test_chime_param_synth.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:17.542117 funman_demo-1.5.0/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      276 2023-04-24 15:10:17.541118 funman_demo-1.5.0/PKG-INFO
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       51 2023-04-24 14:35:12.000000 funman_demo-1.5.0/README.md
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      177 2023-04-24 14:35:12.000000 funman_demo-1.5.0/pyproject.toml
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       38 2023-04-24 15:10:17.542117 funman_demo-1.5.0/setup.cfg
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      844 2023-04-24 14:35:12.000000 funman_demo-1.5.0/setup.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:17.539117 funman_demo-1.5.0/src/
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:17.540117 funman_demo-1.5.0/src/funman_demo/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       34 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      127 2023-04-24 15:10:08.000000 funman_demo-1.5.0/src/funman_demo/_version.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    12199 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/box_plotter.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:17.541118 funman_demo-1.5.0/src/funman_demo/example/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1770 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/example/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2921 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/example/bilayer.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     9451 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/example/chime.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    36937 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/example/demo120822.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     3387 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/handlers.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2245 2023-04-24 14:35:12.000000 funman_demo-1.5.0/src/funman_demo/plot.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:17.541118 funman_demo-1.5.0/src/funman_demo.egg-info/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      276 2023-04-24 15:10:17.000000 funman_demo-1.5.0/src/funman_demo.egg-info/PKG-INFO
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      577 2023-04-24 15:10:17.000000 funman_demo-1.5.0/src/funman_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        1 2023-04-24 15:10:17.000000 funman_demo-1.5.0/src/funman_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        1 2022-12-21 17:24:38.000000 funman_demo-1.5.0/src/funman_demo.egg-info/not-zip-safe
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       26 2023-04-24 15:10:17.000000 funman_demo-1.5.0/src/funman_demo.egg-info/requires.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       12 2023-04-24 15:10:17.000000 funman_demo-1.5.0/src/funman_demo.egg-info/top_level.txt
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:17.541118 funman_demo-1.5.0/test/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1974 2023-04-24 14:35:12.000000 funman_demo-1.5.0/test/test_chime_param_synth.py
```

### Comparing `funman_demo-1.4.0/setup.py` & `funman_demo-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `funman_demo-1.4.0/src/funman_demo/box_plotter.py` & `funman_demo-1.5.0/src/funman_demo/box_plotter.py`

 * *Files identical despite different names*

### Comparing `funman_demo-1.4.0/src/funman_demo/example/__init__.py` & `funman_demo-1.5.0/src/funman_demo/example/__init__.py`

 * *Files identical despite different names*

### Comparing `funman_demo-1.4.0/src/funman_demo/example/bilayer.py` & `funman_demo-1.5.0/src/funman_demo/example/bilayer.py`

 * *Files identical despite different names*

### Comparing `funman_demo-1.4.0/src/funman_demo/example/chime.py` & `funman_demo-1.5.0/src/funman_demo/example/chime.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
             betas,
             gamma,
             n,
             delta,
         )
 
     def make_dynamics_s1(self, *vars):
-
         (
             susceptible,
             infected,
             recovered,
             susceptible_n,
             infected_n,
             recovered_n,
@@ -263,15 +262,14 @@
                         self.make_dynamics_s3(*vars, epoch_idx, t),
                     )
                 )
 
         return parameters, init, dynamics
 
     def make_chime_query(self, infected, n, num_timepoints, threshold):
-
         # I_t <= n * threshold, threshold is proportion (0, 1]
         query = [
             LT(infected[t], Times(n, Real(threshold)))
             for t in range(num_timepoints + 1)
         ]
         return query
```

### Comparing `funman_demo-1.4.0/src/funman_demo/example/demo120822.py` & `funman_demo-1.5.0/src/funman_demo/example/demo120822.py`

 * *Files 0% similar despite different names*

```diff
@@ -795,15 +795,14 @@
             self.query = QueryLE(
                 self.config["query_variable"],
                 self.config["query_threshold"],
                 at_end=True,
             )
 
     def to_md(self, model):
-
         model.measurements.to_dot().render(
             filename="measurement", format="png"
         )
         model.bilayer.to_dot().render(filename="bilayer", format="png")
 
         init_values_md = "\n".join(
             {f"- ## {k}: {v}" for k, v in model.init_values.items()}
@@ -860,15 +859,14 @@
                 f"vaccination_increase must be a list of the form [lb, ub]"
             )
 
         results = {}
         for model_name, model in self.models[
             "intervention_vaccination"
         ].items():
-
             lb = model.parameter_bounds["v_r"][0] * (
                 1.0 + vaccination_increase[0]
             )
             ub = model.parameter_bounds["v_r"][1] * (
                 1.0 + vaccination_increase[1]
             )
             model.parameter_bounds["v_r"] = [lb, ub]
```

### Comparing `funman_demo-1.4.0/src/funman_demo/handlers.py` & `funman_demo-1.5.0/src/funman_demo/handlers.py`

 * *Files identical despite different names*

### Comparing `funman_demo-1.4.0/src/funman_demo/plot.py` & `funman_demo-1.5.0/src/funman_demo/plot.py`

 * *Files identical despite different names*

### Comparing `funman_demo-1.4.0/src/funman_demo.egg-info/SOURCES.txt` & `funman_demo-1.5.0/src/funman_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funman_demo-1.4.0/test/test_chime_param_synth.py` & `funman_demo-1.5.0/test/test_chime_param_synth.py`

 * *Files identical despite different names*

