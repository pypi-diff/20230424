# Comparing `tmp/light_the_torch-0.7.2.tar.gz` & `tmp/light_the_torch-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/light-the-torch/light-the-torch/dist/.tmp-5cqc9o2t/light_the_torch-0.7.2.tar", last modified: Tue Mar 21 09:14:13 2023, max compression
+gzip compressed data, was "/home/runner/work/light-the-torch/light-the-torch/dist/.tmp-bltslpod/light_the_torch-0.7.3.tar", last modified: Mon Apr 24 08:54:45 2023, max compression
```

## Comparing `light_the_torch-0.7.2.tar` & `light_the_torch-0.7.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/light_the_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/light_the_torch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/light_the_torch/_cb.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/light_the_torch/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/light_the_torch/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/light_the_torch/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/light_the_torch/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/light_the_torch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/local-project-stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/local-project-stubs/pep517-setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/local-project-stubs/pep517-setuptools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/local-project-stubs/pep517-setuptools/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-21 09:13:40.000000 light_the_torch-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-21 09:14:13.000000 light_the_torch-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/light_the_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/light_the_torch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/light_the_torch/_cb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/light_the_torch/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/light_the_torch/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/light_the_torch/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/light_the_torch/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/light_the_torch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/local-project-stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/local-project-stubs/pep517-setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/local-project-stubs/pep517-setuptools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/local-project-stubs/pep517-setuptools/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-24 08:53:59.000000 light_the_torch-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:54:45.000000 light_the_torch-0.7.3/setup.cfg
```

### Comparing `light_the_torch-0.7.2/CONTRIBUTING.md` & `light_the_torch-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.2/LICENSE` & `light_the_torch-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.2/PKG-INFO` & `light_the_torch-0.7.3/light_the_torch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
-Name: light_the_torch
-Version: 0.7.2
+Name: light-the-torch
+Version: 0.7.3
 Summary: Install PyTorch distributions with computation backend auto-detection
-Home-page: https://github.com/pmeier/light-the-torch
-Author: Philip Meier
-Author-email: github.pmeier@posteo.de
+Author-email: Philip Meier <github.pmeier@posteo.de>
 License: BSD-3-Clause
-Project-URL: Source, https://github.com/pmeier/light-the-torch
 Project-URL: Tracker, https://github.com/pmeier/light-the-torch/issues
+Project-URL: Source, https://github.com/pmeier/light-the-torch
 Keywords: pytorch,cuda,pip,install
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `light-the-torch`
 
 [![BSD-3-Clause License](https://img.shields.io/github/license/pmeier/light-the-torch)](https://opensource.org/licenses/BSD-3-Clause)
 [![Project Status: WIP](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![Code coverage via codecov.io](https://codecov.io/gh/pmeier/light-the-torch/branch/main/graph/badge.svg)](https://codecov.io/gh/pmeier/light-the-torch)
```

### Comparing `light_the_torch-0.7.2/README.md` & `light_the_torch-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.2/light_the_torch/_cb.py` & `light_the_torch-0.7.3/light_the_torch/_cb.py`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.2/light_the_torch/_patch.py` & `light_the_torch-0.7.3/light_the_torch/_patch.py`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.2/light_the_torch/_utils.py` & `light_the_torch-0.7.3/light_the_torch/_utils.py`

 * *Files identical despite different names*

### Comparing `light_the_torch-0.7.2/light_the_torch.egg-info/PKG-INFO` & `light_the_torch-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
-Name: light-the-torch
-Version: 0.7.2
+Name: light_the_torch
+Version: 0.7.3
 Summary: Install PyTorch distributions with computation backend auto-detection
-Home-page: https://github.com/pmeier/light-the-torch
-Author: Philip Meier
-Author-email: github.pmeier@posteo.de
+Author-email: Philip Meier <github.pmeier@posteo.de>
 License: BSD-3-Clause
-Project-URL: Source, https://github.com/pmeier/light-the-torch
 Project-URL: Tracker, https://github.com/pmeier/light-the-torch/issues
+Project-URL: Source, https://github.com/pmeier/light-the-torch
 Keywords: pytorch,cuda,pip,install
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `light-the-torch`
 
 [![BSD-3-Clause License](https://img.shields.io/github/license/pmeier/light-the-torch)](https://opensource.org/licenses/BSD-3-Clause)
 [![Project Status: WIP](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![Code coverage via codecov.io](https://codecov.io/gh/pmeier/light-the-torch/branch/main/graph/badge.svg)](https://codecov.io/gh/pmeier/light-the-torch)
```

### Comparing `light_the_torch-0.7.2/light_the_torch.egg-info/SOURCES.txt` & `light_the_torch-0.7.3/light_the_torch.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .prettierignore
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 light_the_torch/__init__.py
 light_the_torch/__main__.py
 light_the_torch/_cb.py
 light_the_torch/_cli.py
 light_the_torch/_compat.py
 light_the_torch/_patch.py
 light_the_torch/_utils.py
```

