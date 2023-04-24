# Comparing `tmp/generand-0.0.5.tar.gz` & `tmp/generand-2.15.5.tar.gz`

## Comparing `generand-0.0.5.tar` & `generand-2.15.5.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 generand-0.0.5/Python.gitignore
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 generand-0.0.5/Tests.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 generand-0.0.5/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/bernoulli.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/binomial.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/exponential.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/poisson.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/triangular.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/uniform.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 generand-0.0.5/src/generand/weibull.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 generand-0.0.5/LICENSE
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 generand-0.0.5/README.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 generand-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 generand-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 generand-2.15.5/.DS_Store
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 generand-2.15.5/Tests.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 generand-2.15.5/.vscode/launch.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 generand-2.15.5/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/bernoulli.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/binomial.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/erlang.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/exponential.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/geometric.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/normal.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/poisson.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/triangular.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/uniform.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 generand-2.15.5/src/generand/weibull.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 generand-2.15.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 generand-2.15.5/LICENSE
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 generand-2.15.5/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 generand-2.15.5/pyproject.toml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 generand-2.15.5/PKG-INFO
```

### Comparing `generand-0.0.5/Python.gitignore` & `generand-2.15.5/.gitignore`

 * *Files identical despite different names*

### Comparing `generand-0.0.5/src/generand/poisson.py` & `generand-2.15.5/src/generand/poisson.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 from .uniform import Uniform
 import time
 import math
 class Poisson:
 
     """Generates pseudo poisson random numbers using A-R method"""
-    # def generate(self, alpha= 1 , count= 1):
-    #     poisson = []
-    #     for i in range(count):
-    #         x = -1
-    #         p = 1
-    #         while p >= math.exp(-alpha):
-    #             u = Uniform(time.perf_counter_ns()).generate()
-    #             x+=1
-    #             p = u[0]*p
-    #         poisson.append(x)
-    #     return poisson
 
-    def generate(self, alpha= 1 , count= 1):
+    def __init__(self,alpha=0.1):
+        self.alpha = alpha
+
+    def generate(self, n= 1):
         poisson = []
-        for _ in range(count):
+        for _ in range(n):
             
             x = 0
             p = 1
             i= 0
-            u = Uniform(time.perf_counter_ns()).generate(5*alpha)
-            while p >= math.exp(-alpha):
+            u = Uniform(time.perf_counter_ns()).generate(n=5*self.alpha)
+            while p >= math.exp(-self.alpha):
                 
                 x+=1
                 p = u[i]*p
                 i+=1
             poisson.append(x)
         return poisson
```

### Comparing `generand-0.0.5/LICENSE` & `generand-2.15.5/LICENSE`

 * *Files identical despite different names*

### Comparing `generand-0.0.5/pyproject.toml` & `generand-2.15.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "generand"
-version = "0.0.5"
+version = "2.15.5"
 authors = [
   { name="rajat maheshwari", email="rajt.maheshwari30@gmail.com" },
 ]
 description = "A package to generate random numbers from various distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `generand-0.0.5/PKG-INFO` & `generand-2.15.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generand
-Version: 0.0.5
+Version: 2.15.5
 Summary: A package to generate random numbers from various distributions
 Project-URL: Homepage, https://github.com/pypa/generand
 Project-URL: Bug Tracker, https://github.com/pypa/generand/issues
 Author-email: rajat maheshwari <rajt.maheshwari30@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

