# Comparing `tmp/remin-0.0.2.tar.gz` & `tmp/remin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remin-0.0.2.tar", last modified: Mon Apr 17 01:48:48 2023, max compression
+gzip compressed data, was "remin-0.0.3.tar", last modified: Mon Apr 24 20:59:40 2023, max compression
```

## Comparing `remin-0.0.2.tar` & `remin-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.423377 remin-0.0.2/
--rw-rw-r--   0 salih     (1000) salih     (1000)     1828 2023-04-15 00:41:42.000000 remin-0.0.2/.gitignore
--rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.0.2/LICENSE
--rw-rw-r--   0 salih     (1000) salih     (1000)      311 2023-04-17 01:44:50.000000 remin-0.0.2/Makefile
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-17 01:48:48.423377 remin-0.0.2/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.0.2/README.md
--rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-04-17 01:41:56.000000 remin-0.0.2/pyproject.toml
--rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.0.2/requirements.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-04-17 01:48:48.423377 remin-0.0.2/setup.cfg
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.419377 remin-0.0.2/src/
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.423377 remin-0.0.2/src/remin/
--rw-rw-r--   0 salih     (1000) salih     (1000)      120 2023-04-17 01:36:46.000000 remin-0.0.2/src/remin/__init__.py
--rw-rw-r--   0 salih     (1000) salih     (1000)       29 2023-04-14 23:42:16.000000 remin-0.0.2/src/remin/domain.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      809 2023-04-17 01:46:30.000000 remin-0.0.2/src/remin/func.py
--rw-rw-r--   0 salih     (1000) salih     (1000)      488 2023-04-17 01:44:59.000000 remin-0.0.2/src/remin/residual.py
--rw-rw-r--   0 salih     (1000) salih     (1000)     1720 2023-04-17 01:44:59.000000 remin-0.0.2/src/remin/solver.py
-drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-17 01:48:48.423377 remin-0.0.2/src/remin.egg-info/
--rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/PKG-INFO
--rw-rw-r--   0 salih     (1000) salih     (1000)      335 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/SOURCES.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/dependency_links.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/requires.txt
--rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-04-17 01:48:48.000000 remin-0.0.2/src/remin.egg-info/top_level.txt
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1828 2023-04-15 00:41:42.000000 remin-0.0.3/.gitignore
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1072 2023-04-14 21:12:20.000000 remin-0.0.3/LICENSE
+-rw-rw-r--   0 salih     (1000) salih     (1000)      349 2023-04-17 09:36:47.000000 remin-0.0.3/Makefile
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-24 20:59:40.413460 remin-0.0.3/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)     2625 2023-04-17 01:40:58.000000 remin-0.0.3/README.md
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/examples/
+-rw-rw-r--   0 salih     (1000) salih     (1000)    78602 2023-04-17 09:08:31.000000 remin-0.0.3/examples/example_heat_problem.ipynb
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1255 2023-04-24 20:59:14.000000 remin-0.0.3/pyproject.toml
+-rw-rw-r--   0 salih     (1000) salih     (1000)       28 2023-04-14 23:01:53.000000 remin-0.0.3/requirements.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       38 2023-04-24 20:59:40.413460 remin-0.0.3/setup.cfg
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/src/
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/src/remin/
+-rw-rw-r--   0 salih     (1000) salih     (1000)       22 2023-04-24 20:59:06.000000 remin-0.0.3/src/remin/__init__.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     1180 2023-04-24 20:56:05.000000 remin-0.0.3/src/remin/domain.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)      809 2023-04-17 01:46:30.000000 remin-0.0.3/src/remin/func.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3548 2023-04-24 20:56:05.000000 remin-0.0.3/src/remin/residual.py
+-rw-rw-r--   0 salih     (1000) salih     (1000)     4336 2023-04-24 20:56:05.000000 remin-0.0.3/src/remin/solver.py
+drwxrwxr-x   0 salih     (1000) salih     (1000)        0 2023-04-24 20:59:40.413460 remin-0.0.3/src/remin.egg-info/
+-rw-rw-r--   0 salih     (1000) salih     (1000)     3164 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/PKG-INFO
+-rw-rw-r--   0 salih     (1000) salih     (1000)      371 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/SOURCES.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        1 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/dependency_links.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)       80 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/requires.txt
+-rw-rw-r--   0 salih     (1000) salih     (1000)        6 2023-04-24 20:59:40.000000 remin-0.0.3/src/remin.egg-info/top_level.txt
```

### Comparing `remin-0.0.2/.gitignore` & `remin-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `remin-0.0.2/LICENSE` & `remin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remin-0.0.2/PKG-INFO` & `remin-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.0.2
+Version: 0.0.3
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `remin-0.0.2/README.md` & `remin-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `remin-0.0.2/pyproject.toml` & `remin-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "remin"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Salih Taşdelen", email="salih.tasdelen@hotmail.com"},
 ]
 description = "PINN solver implemented in Pytorch"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `remin-0.0.2/src/remin/func.py` & `remin-0.0.3/src/remin/func.py`

 * *Files identical despite different names*

### Comparing `remin-0.0.2/src/remin.egg-info/PKG-INFO` & `remin-0.0.3/src/remin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remin
-Version: 0.0.2
+Version: 0.0.3
 Summary: PINN solver implemented in Pytorch
 Author-email: Salih Taşdelen <salih.tasdelen@hotmail.com>
 Project-URL: Homepage, https://github.com/SalihTasdelen/remin
 Project-URL: Bug Tracker, https://github.com/SalihTasdelen/remin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

