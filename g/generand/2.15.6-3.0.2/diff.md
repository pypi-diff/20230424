# Comparing `tmp/generand-2.15.6.tar.gz` & `tmp/generand-3.0.2.tar.gz`

## Comparing `generand-2.15.6.tar` & `generand-3.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 generand-2.15.6/.DS_Store
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 generand-2.15.6/Tests.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 generand-2.15.6/.vscode/launch.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 generand-2.15.6/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/bernoulli.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/binomial.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/erlang.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/exponential.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/geometric.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/normal.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/poisson.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/triangular.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/uniform.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 generand-2.15.6/src/generand/weibull.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 generand-2.15.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 generand-2.15.6/LICENSE
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 generand-2.15.6/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 generand-2.15.6/pyproject.toml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 generand-2.15.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 generand-3.0.2/.DS_Store
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 generand-3.0.2/Tests.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 generand-3.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 generand-3.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/bernoulli.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/binomial.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/erlang.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/exponential.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/geometric.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/normal.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/poisson.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/triangular.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/uniform.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 generand-3.0.2/src/generand/weibull.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 generand-3.0.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 generand-3.0.2/LICENSE
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 generand-3.0.2/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 generand-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 generand-3.0.2/PKG-INFO
```

### Comparing `generand-2.15.6/.DS_Store` & `generand-3.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `generand-2.15.6/src/generand/binomial.py` & `generand-3.0.2/src/generand/binomial.py`

 * *Files identical despite different names*

### Comparing `generand-2.15.6/src/generand/triangular.py` & `generand-3.0.2/src/generand/triangular.py`

 * *Files identical despite different names*

### Comparing `generand-2.15.6/src/generand/uniform.py` & `generand-3.0.2/src/generand/uniform.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,13 +9,13 @@
         self.seed = seed
         self.a = a
         self.b = b
 
     def generate(self, n=1):
         u = []
         temp = (self.__a*self.seed)%self.__mod
-        u.append(temp/self.__mod)
+        u.append(self.a+(self.b-self.a)*(temp/self.__mod))
         for i in range(1,n):
             temp = (self.__a*temp)%self.__mod
             u.append(self.a+(self.b-self.a)*(temp/self.__mod))
 
         return u
```

### Comparing `generand-2.15.6/.gitignore` & `generand-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `generand-2.15.6/LICENSE` & `generand-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `generand-2.15.6/pyproject.toml` & `generand-3.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "generand"
-version = "2.15.6"
+version = "3.0.2"
 authors = [
   { name="rajat maheshwari", email="rajat.maheshwari30@gmail.com" },
+  { name="shanthan kesharaju", email="shanthan.kesharaju@gmail.com" }
 ]
 description = "A package to generate random numbers from various distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `generand-2.15.6/PKG-INFO` & `generand-3.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: generand
-Version: 2.15.6
+Version: 3.0.2
 Summary: A package to generate random numbers from various distributions
 Project-URL: Homepage, https://github.com/pypa/generand
 Project-URL: Bug Tracker, https://github.com/pypa/generand/issues
-Author-email: rajat maheshwari <rajat.maheshwari30@gmail.com>
+Author-email: rajat maheshwari <rajat.maheshwari30@gmail.com>, shanthan kesharaju <shanthan.kesharaju@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

