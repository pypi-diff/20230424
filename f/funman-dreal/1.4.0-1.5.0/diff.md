# Comparing `tmp/funman_dreal-1.4.0.tar.gz` & `tmp/funman_dreal-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funman_dreal-1.4.0.tar", last modified: Fri Feb  3 17:05:57 2023, max compression
+gzip compressed data, was "funman_dreal-1.5.0.tar", last modified: Mon Apr 24 15:10:24 2023, max compression
```

## Comparing `funman_dreal-1.4.0.tar` & `funman_dreal-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:57.131063 funman_dreal-1.4.0/
--rw-r--r--   0 danbryce   (501) dialout     (20)      303 2023-02-03 17:05:57.129670 funman_dreal-1.4.0/PKG-INFO
--rw-r--r--   0 danbryce   (501) dialout     (20)       54 2022-12-23 20:09:23.000000 funman_dreal-1.4.0/README.md
--rw-r--r--   0 danbryce   (501) dialout     (20)      177 2022-12-23 20:09:23.000000 funman_dreal-1.4.0/pyproject.toml
--rw-r--r--   0 danbryce   (501) dialout     (20)       38 2023-02-03 17:05:57.131908 funman_dreal-1.4.0/setup.cfg
--rw-r--r--   0 danbryce   (501) dialout     (20)      898 2023-01-19 19:06:07.000000 funman_dreal-1.4.0/setup.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:57.035235 funman_dreal-1.4.0/src/
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:57.070623 funman_dreal-1.4.0/src/funman_dreal/
--rw-r--r--   0 danbryce   (501) dialout     (20)      103 2023-01-20 22:15:58.000000 funman_dreal-1.4.0/src/funman_dreal/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      127 2023-02-03 17:05:41.000000 funman_dreal-1.4.0/src/funman_dreal/_version.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     6209 2023-01-30 14:42:47.000000 funman_dreal-1.4.0/src/funman_dreal/converter.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:57.108721 funman_dreal-1.4.0/src/funman_dreal/example/
--rw-r--r--   0 danbryce   (501) dialout     (20)        1 2022-12-23 20:09:23.000000 funman_dreal-1.4.0/src/funman_dreal/example/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)    16722 2023-02-02 04:37:36.000000 funman_dreal-1.4.0/src/funman_dreal/solver.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:57.104191 funman_dreal-1.4.0/src/funman_dreal.egg-info/
--rw-r--r--   0 danbryce   (501) dialout     (20)      303 2023-02-03 17:05:57.000000 funman_dreal-1.4.0/src/funman_dreal.egg-info/PKG-INFO
--rw-r--r--   0 danbryce   (501) dialout     (20)      517 2023-02-03 17:05:57.000000 funman_dreal-1.4.0/src/funman_dreal.egg-info/SOURCES.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)        1 2023-02-03 17:05:57.000000 funman_dreal-1.4.0/src/funman_dreal.egg-info/dependency_links.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)        1 2022-11-07 17:48:22.000000 funman_dreal-1.4.0/src/funman_dreal.egg-info/not-zip-safe
--rw-r--r--   0 danbryce   (501) dialout     (20)       48 2023-02-03 17:05:57.000000 funman_dreal-1.4.0/src/funman_dreal.egg-info/requires.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)       13 2023-02-03 17:05:57.000000 funman_dreal-1.4.0/src/funman_dreal.egg-info/top_level.txt
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:57.125948 funman_dreal-1.4.0/test/
--rw-r--r--   0 danbryce   (501) dialout     (20)     6051 2023-01-20 22:15:58.000000 funman_dreal-1.4.0/test/test_chime_bilayer_solve.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     2265 2022-12-31 21:23:10.000000 funman_dreal-1.4.0/test/test_file_io.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     4729 2022-12-31 21:23:10.000000 funman_dreal-1.4.0/test/test_socket.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     5598 2023-01-20 22:15:58.000000 funman_dreal-1.4.0/test/test_solver.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:24.023919 funman_dreal-1.5.0/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      303 2023-04-24 15:10:24.023919 funman_dreal-1.5.0/PKG-INFO
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       54 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/README.md
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      177 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/pyproject.toml
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       38 2023-04-24 15:10:24.023919 funman_dreal-1.5.0/setup.cfg
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      898 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/setup.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:24.021919 funman_dreal-1.5.0/src/
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:24.022919 funman_dreal-1.5.0/src/funman_dreal/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      103 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/src/funman_dreal/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      127 2023-04-24 15:10:08.000000 funman_dreal-1.5.0/src/funman_dreal/_version.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     6209 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/src/funman_dreal/converter.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:24.022919 funman_dreal-1.5.0/src/funman_dreal/example/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        1 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/src/funman_dreal/example/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    17445 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/src/funman_dreal/solver.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:24.022919 funman_dreal-1.5.0/src/funman_dreal.egg-info/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      303 2023-04-24 15:10:24.000000 funman_dreal-1.5.0/src/funman_dreal.egg-info/PKG-INFO
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      517 2023-04-24 15:10:24.000000 funman_dreal-1.5.0/src/funman_dreal.egg-info/SOURCES.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        1 2023-04-24 15:10:24.000000 funman_dreal-1.5.0/src/funman_dreal.egg-info/dependency_links.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        1 2022-12-21 17:24:40.000000 funman_dreal-1.5.0/src/funman_dreal.egg-info/not-zip-safe
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       48 2023-04-24 15:10:24.000000 funman_dreal-1.5.0/src/funman_dreal.egg-info/requires.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       13 2023-04-24 15:10:24.000000 funman_dreal-1.5.0/src/funman_dreal.egg-info/top_level.txt
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:24.023919 funman_dreal-1.5.0/test/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     6050 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/test/test_chime_bilayer_solve.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2265 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/test/test_file_io.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     4729 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/test/test_socket.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     5598 2023-04-24 14:35:12.000000 funman_dreal-1.5.0/test/test_solver.py
```

### Comparing `funman_dreal-1.4.0/setup.py` & `funman_dreal-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `funman_dreal-1.4.0/src/funman_dreal/converter.py` & `funman_dreal-1.5.0/src/funman_dreal/converter.py`

 * *Files identical despite different names*

### Comparing `funman_dreal-1.4.0/src/funman_dreal/solver.py` & `funman_dreal-1.5.0/src/funman_dreal/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,27 +419,45 @@
         self.converter = DRealConverter(environment)
         # self.options(self)
         # self.options.set_params(self)
         self.mgr = environment.formula_manager
         self.model = None
 
         # dreal specific attributes
-        self.context = dreal.Context()
-        self.context.SetLogic(dreal.Logic.QF_NRA)
-        self.context.config.precision = 0.05
+        self.config = dreal.Config()
+
+        if "dreal_precision" in options:
+            self.config.precision = options["solver_options"][
+                "dreal_precision"
+            ]
         # self.context.config.use_polytope = True
         # self.context.config.use_worklist_fixpoint = True
         self.model = None
-        # dreal.set_log_level(dreal.LogLevel.DEBUG)
-        # dreal.set_log_level(dreal.LogLevel.INFO)
+        if "dreal_log_level" in options["solver_options"]:
+            if options["solver_options"]["dreal_log_level"] == "debug":
+                dreal.set_log_level(dreal.LogLevel.DEBUG)
+            elif options["solver_options"]["dreal_log_level"] == "info":
+                dreal.set_log_level(dreal.LogLevel.INFO)
+
+        if (
+            "dreal_mcts" in options["solver_options"]
+            and options["solver_options"]["dreal_mcts"]
+        ):
+            self.config.mcts = True
+
+        self.context = dreal.Context(self.config)
+        self.context.SetLogic(dreal.Logic.QF_NRA)
 
         # self.to = self.environment.typeso
         self.LOGICS = DReal.LOGICS
         self.symbols = {}
 
+    def __del__(self):
+        self.context.Exit()
+
     @clear_pending_pop
     def add_assertion(self, formula, named=None):
         # print(f"Assert({formula})")
 
         f = self.converter.convert(formula)
 
         deps = formula.get_free_variables()
@@ -511,17 +529,21 @@
             s = self.symbols[sn][0]
             if s.is_term():
                 v = self.get_value(self.symbols[sn][1])
                 assignment[s] = v
         return EagerModel(assignment=assignment, environment=self.environment)
 
     def get_value(self, item):
+        # print(f"get_value() {item}: {self.model[item]}")
         return Real(self.model[item].lb())
 
     @clear_pending_pop
     def solve(self, assumptions=None):
         assert assumptions is None
-        ans = self.check_sat()
+        try:
+            ans = self.check_sat()
+        except Exception as e:
+            raise e
         return ans is not None
 
     def _exit(self):
         pass
```

### Comparing `funman_dreal-1.4.0/src/funman_dreal.egg-info/SOURCES.txt` & `funman_dreal-1.5.0/src/funman_dreal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funman_dreal-1.4.0/test/test_chime_bilayer_solve.py` & `funman_dreal-1.5.0/test/test_chime_bilayer_solve.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         assert result
 
         result.plot(logy=True)
         print(result.dataframe())
 
     # @unittest.skip("temporarily remove")
     def test_chime_bilayer_synthesize(self):
-
         model, query, encoder = self.setup(
             duration=10, transmission_reduction=[-0.05, 0.1]
         )
         model.init_values = {
             "S": 7438.567991,
             "I": 2261.927694,
             "R": 299.504315,
```

### Comparing `funman_dreal-1.4.0/test/test_file_io.py` & `funman_dreal-1.5.0/test/test_file_io.py`

 * *Files identical despite different names*

### Comparing `funman_dreal-1.4.0/test/test_socket.py` & `funman_dreal-1.5.0/test/test_socket.py`

 * *Files identical despite different names*

### Comparing `funman_dreal-1.4.0/test/test_solver.py` & `funman_dreal-1.5.0/test/test_solver.py`

 * *Files identical despite different names*

