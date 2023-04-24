# Comparing `tmp/heflow-1.3.0.tar.gz` & `tmp/heflow-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heflow-1.3.0.tar", last modified: Wed Mar 22 09:05:05 2023, max compression
+gzip compressed data, was "heflow-1.3.1.tar", last modified: Mon Apr 24 14:57:00 2023, max compression
```

## Comparing `heflow-1.3.0.tar` & `heflow-1.3.1.tar`

### file list

```diff
@@ -1,53 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.711063 heflow-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.711063 heflow-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-22 09:04:56.000000 heflow-1.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-22 09:04:56.000000 heflow-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-22 09:04:56.000000 heflow-1.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-22 09:05:05.715063 heflow-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-03-22 09:04:56.000000 heflow-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.711063 heflow-1.3.0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   383186 2023-03-22 09:04:56.000000 heflow-1.3.0/assets/heflow-ppmlops.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.711063 heflow-1.3.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-22 09:04:56.000000 heflow-1.3.0/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-22 09:04:56.000000 heflow-1.3.0/docker/dev.Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.711063 heflow-1.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.711063 heflow-1.3.0/examples/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-22 09:04:56.000000 heflow-1.3.0/examples/sklearn/MLproject
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 09:04:56.000000 heflow-1.3.0/examples/sklearn/python_env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-22 09:04:56.000000 heflow-1.3.0/examples/sklearn/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/heflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/heflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/cli/keygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/heflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/plugins/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/plugins/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/heflow/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/sklearn/linear_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/heflow/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/heflow/tensorflow/keras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/tensorflow/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/tensorflow/keras/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-03-22 09:04:56.000000 heflow-1.3.0/heflow/tensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 09:05:05.715063 heflow-1.3.0/heflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-22 09:05:05.000000 heflow-1.3.0/heflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-22 09:05:05.000000 heflow-1.3.0/heflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 09:05:05.000000 heflow-1.3.0/heflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-22 09:05:05.000000 heflow-1.3.0/heflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-22 09:05:05.000000 heflow-1.3.0/heflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 09:05:05.000000 heflow-1.3.0/heflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-22 09:04:56.000000 heflow-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-22 09:04:56.000000 heflow-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 09:04:56.000000 heflow-1.3.0/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 09:05:05.715063 heflow-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-22 09:04:56.000000 heflow-1.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-22 09:04:56.000000 heflow-1.3.0/start
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.159975 heflow-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-24 14:56:50.000000 heflow-1.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-24 14:56:50.000000 heflow-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 14:56:50.000000 heflow-1.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-24 14:57:00.175976 heflow-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-24 14:56:50.000000 heflow-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   383186 2023-04-24 14:56:50.000000 heflow-1.3.1/assets/heflow-ppmlops.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.159975 heflow-1.3.1/charts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/charts/heflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/Chart.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/charts/heflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/secret.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/values.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.167976 heflow-1.3.1/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 14:56:50.000000 heflow-1.3.1/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 14:56:50.000000 heflow-1.3.1/docker/dev.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.159975 heflow-1.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.167976 heflow-1.3.1/examples/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 14:56:50.000000 heflow-1.3.1/examples/sklearn/MLproject
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 14:56:50.000000 heflow-1.3.1/examples/sklearn/python_env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-24 14:56:50.000000 heflow-1.3.1/examples/sklearn/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.167976 heflow-1.3.1/heflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.171976 heflow-1.3.1/heflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/cli/keygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.171976 heflow-1.3.1/heflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/plugins/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/plugins/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/sklearn/linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/tensorflow/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensorflow/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensorflow/keras/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.171976 heflow-1.3.1/heflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 14:56:50.000000 heflow-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 14:56:50.000000 heflow-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 14:56:50.000000 heflow-1.3.1/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:57:00.175976 heflow-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-24 14:56:50.000000 heflow-1.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 14:56:50.000000 heflow-1.3.1/start
```

### Comparing `heflow-1.3.0/.github/workflows/release.yml` & `heflow-1.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heflow-1.3.0/LICENSE` & `heflow-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heflow-1.3.0/PKG-INFO` & `heflow-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflow
-Version: 1.3.0
+Version: 1.3.1
 Summary: HEflow: A platform for the privacy-preserving machine learning lifecycle
 Home-page: https://github.com/inaccel/heflow
 Author: InAccel
 Author-email: info@inaccel.com
 License: Apache-2.0
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 [Seldon MLServer](https://github.com/SeldonIO/MLServer) and
 [OpenMined TenSEAL](https://github.com/OpenMined/TenSEAL), HEflow offers a set
 of lightweight homomorphic encryption APIs that can be used with any existing
 machine learning application or library (scikit-learn, Keras, TensorFlow,
 PyTorch, etc), wherever you currently run ML code (e.g. in notebooks, standalone
 applications, or the cloud).
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://gesis.mybinder.org/v2/gh/inaccel/heflow/master)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/inaccel/heflow/master)
 [![PyPI version](https://badge.fury.io/py/heflow.svg)](https://badge.fury.io/py/heflow)
 
 ## Homomorphic Encryption (HE)
 
 Homomorphic encryption differs from typical encryption methods in that it allows
 computation to be performed directly on encrypted data without requiring access
 to a secret key. The result of such a computation remains in encrypted form, and
```

### Comparing `heflow-1.3.0/README.md` & `heflow-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [Seldon MLServer](https://github.com/SeldonIO/MLServer) and
 [OpenMined TenSEAL](https://github.com/OpenMined/TenSEAL), HEflow offers a set
 of lightweight homomorphic encryption APIs that can be used with any existing
 machine learning application or library (scikit-learn, Keras, TensorFlow,
 PyTorch, etc), wherever you currently run ML code (e.g. in notebooks, standalone
 applications, or the cloud).
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://gesis.mybinder.org/v2/gh/inaccel/heflow/master)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/inaccel/heflow/master)
 [![PyPI version](https://badge.fury.io/py/heflow.svg)](https://badge.fury.io/py/heflow)
 
 ## Homomorphic Encryption (HE)
 
 Homomorphic encryption differs from typical encryption methods in that it allows
 computation to be performed directly on encrypted data without requiring access
 to a secret key. The result of such a computation remains in encrypted form, and
```

### Comparing `heflow-1.3.0/assets/heflow-ppmlops.svg` & `heflow-1.3.1/assets/heflow-ppmlops.svg`

 * *Files identical despite different names*

### Comparing `heflow-1.3.0/examples/sklearn/train.py` & `heflow-1.3.1/examples/sklearn/train.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.0/heflow/cli/keygen.py` & `heflow-1.3.1/heflow/cli/keygen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import click
-import heflow
 import heflow.keys
 import json
 import pathlib
 
 
 def jsondict(ctx, param, value):
     if isinstance(value, tuple):
```

### Comparing `heflow-1.3.0/heflow/codecs.py` & `heflow-1.3.1/heflow/codecs.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.0/heflow/contexts.py` & `heflow-1.3.1/heflow/contexts.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,14 @@
     def in_context(self):
         try:
             self.key()
         except Exception:
             return False
         return True
 
+    @classmethod
     @functools.lru_cache
-    def key(self):
+    def key(cls):
         return heflow.load_key(os.getenv('HEFLOW_CKKS', 'id_ckks'))
 
     def tags(self):
         return {'heflow.ckks_key.fingerprint': self.key().fingerprint()}
-
-
-@functools.lru_cache
-def ckks_context():
-    return CKKSContext()
```

### Comparing `heflow-1.3.0/heflow/keys.py` & `heflow-1.3.1/heflow/keys.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from mlflow.store.artifact.mlflow_artifacts_repo import MlflowArtifactsRepository
 
 import base64
 import functools
 import hashlib
+import joblib
 import mlflow
+import tempfile
 import tenseal
 import urllib.parse
 
 
 class CKKSKey:
 
     def __getstate__(self):
@@ -74,7 +76,35 @@
 
 def ckks_key(*,
              coeff_modulus_bit_sizes=[52, 52, 52, 52, 52, 52, 52],
              poly_modulus_degree=16384,
              scale_bit_size=52):
     return CKKSKey(coeff_modulus_bit_sizes, poly_modulus_degree,
                    scale_bit_size)
+
+
+@functools.singledispatch
+def load_key(path):
+    return joblib.load(path)
+
+
+@load_key.register
+def _(key_uri: str):
+    with tempfile.TemporaryDirectory() as tmp:
+        return joblib.load(
+            mlflow.artifacts.download_artifacts(key_uri, dst_path=tmp))
+
+
+def log_key(key):
+    with tempfile.TemporaryDirectory() as tmp:
+        if isinstance(key, CKKSKey):
+            path = f'{tmp}/id_ckks.pub'
+        else:
+            raise mlflow.MlflowException(
+                f'`key` must be a subclass of `CKKSKey`. Instead, found an object of type: {type(key)}',
+                mlflow.exceptions.INVALID_PARAMETER_VALUE)
+        save_key(path, key.public_key())
+        KeysRepository(f'keys:/{key.fingerprint()}').log_artifact(path)
+
+
+def save_key(path, key):
+    joblib.dump(key, path)
```

### Comparing `heflow-1.3.0/heflow/sklearn/__init__.py` & `heflow-1.3.1/heflow/sklearn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-import heflow
 import heflow.sklearn.linear_model
 import sklearn.linear_model
 
 
 def log_model(model,
               *,
               registered_model_name=None,
               await_registration_for=300):
     if isinstance(model, sklearn.linear_model.LogisticRegression):
-        return heflow.log_model(
-            heflow.sklearn.linear_model.LogisticRegression(model),
-            registered_model_name=registered_model_name,
-            await_registration_for=await_registration_for)
+        model = heflow.sklearn.linear_model.LogisticRegression(model)
     else:
         raise TypeError(f'invalid model instance: {type(model)}')
 
+    return heflow.log_model(model,
+                            registered_model_name=registered_model_name,
+                            await_registration_for=await_registration_for)
+
 
 def save_model(path, model):
     if isinstance(model, sklearn.linear_model.LogisticRegression):
-        heflow.save_model(
-            path, heflow.sklearn.linear_model.LogisticRegression(model))
+        model = heflow.sklearn.linear_model.LogisticRegression(model)
     else:
         raise TypeError(f'invalid model instance: {type(model)}')
+
+    heflow.save_model(path, model)
```

### Comparing `heflow-1.3.0/heflow/sklearn/linear_model.py` & `heflow-1.3.1/heflow/sklearn/linear_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-import heflow.models
-import heflow.tensors
+import heflow
 import numpy
 
 
-@heflow.models.ckks_model('he_decision_function')
+@heflow.ckks_model('he_decision_function')
 class LogisticRegression:
 
     def __init__(self, model):
         self.classes_ = model.classes_
-        self.he_coef_ = heflow.tensors.ckks_tensor(model.coef_).transpose_()
-        self.he_intercept_ = heflow.tensors.ckks_tensor(model.intercept_)
+        self.he_coef_ = heflow.ckks_tensor(model.coef_).transpose_()
+        self.he_intercept_ = heflow.ckks_tensor(model.intercept_)
 
     def he_decision_function(self, he_X):
         he_scores = he_X.dot_(self.he_coef_).add_(self.he_intercept_)
         return he_scores.reshape_(
             (he_scores.shape[0], )) if he_scores.shape[1] == 1 else he_scores
 
     def predict(self, X):
-        he_X = heflow.tensors.ckks_tensor(X)
+        he_X = heflow.ckks_tensor(X)
         he_scores = self.he_decision_function(he_X)
         scores = he_scores.numpy()
         if len(scores.shape) == 1:
             indices = (scores > 0).astype(int)
         else:
             indices = numpy.argmax(scores, axis=1)
         return numpy.take(self.classes_, indices, axis=0)
```

### Comparing `heflow-1.3.0/heflow/tensors.py` & `heflow-1.3.1/heflow/tensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import functools
 import heflow.contexts
 import numpy
 import tenseal
 
 
 class CKKSTensor:
-    key = heflow.contexts.ckks_context().key()
 
     def __getstate__(self):
         return {'data': self.backend.serialize()}
 
     @functools.singledispatchmethod
     def __init__(self, data):
-        self.backend = tenseal.ckks_tensor(self.key.backend, data)
+        key = heflow.contexts.CKKSContext.key()
+
+        self.backend = tenseal.ckks_tensor(key.backend, data)
 
     @__init__.register
     def _(self, backend: tenseal.CKKSTensor):
         self.backend = backend
 
     def __setstate__(self, state):
-        self.backend = tenseal.ckks_tensor_from(self.key.backend,
-                                                state['data'])
+        key = heflow.contexts.CKKSContext.key()
+
+        self.backend = tenseal.ckks_tensor_from(key.backend, state['data'])
 
     def add(self, other):
         if isinstance(other, CKKSTensor):
             other = other.backend
 
         return CKKSTensor(self.backend.add(other))
```

### Comparing `heflow-1.3.0/heflow.egg-info/PKG-INFO` & `heflow-1.3.1/heflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflow
-Version: 1.3.0
+Version: 1.3.1
 Summary: HEflow: A platform for the privacy-preserving machine learning lifecycle
 Home-page: https://github.com/inaccel/heflow
 Author: InAccel
 Author-email: info@inaccel.com
 License: Apache-2.0
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 [Seldon MLServer](https://github.com/SeldonIO/MLServer) and
 [OpenMined TenSEAL](https://github.com/OpenMined/TenSEAL), HEflow offers a set
 of lightweight homomorphic encryption APIs that can be used with any existing
 machine learning application or library (scikit-learn, Keras, TensorFlow,
 PyTorch, etc), wherever you currently run ML code (e.g. in notebooks, standalone
 applications, or the cloud).
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://gesis.mybinder.org/v2/gh/inaccel/heflow/master)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/inaccel/heflow/master)
 [![PyPI version](https://badge.fury.io/py/heflow.svg)](https://badge.fury.io/py/heflow)
 
 ## Homomorphic Encryption (HE)
 
 Homomorphic encryption differs from typical encryption methods in that it allows
 computation to be performed directly on encrypted data without requiring access
 to a secret key. The result of such a computation remains in encrypted form, and
```

### Comparing `heflow-1.3.0/setup.py` & `heflow-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,22 @@
         'Linux',
     ],
     install_requires=requirements(),
     entry_points={
         'console_scripts': [
             'heflow-keygen = heflow.cli.keygen:command',
         ],
+        'mlflow.app': [
+            'heflow = heflow.ui:app',
+        ],
         'mlflow.artifact_repository': [
             'keys = heflow.plugins.keys:KeysRepository',
         ],
         'mlflow.run_context_provider': [
-            'heflow-ckks = heflow.plugins.contexts:ckks_context',
+            'heflow-ckks = heflow.plugins.contexts:CKKSContext',
         ],
     },
     extras_require={
         'extras': [
             'psycopg2',
         ],
     },
```

