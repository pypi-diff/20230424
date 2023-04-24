# Comparing `tmp/pip-package-template-docker-2023.4.23.tar.gz` & `tmp/pip-package-template-docker-2023.4.23.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-package-template-docker-2023.4.23.tar", last modified: Sun Apr 23 22:45:25 2023, max compression
+gzip compressed data, was "pip-package-template-docker-2023.4.23.post1.tar", last modified: Mon Apr 24 02:15:57 2023, max compression
```

## Comparing `pip-package-template-docker-2023.4.23.tar` & `pip-package-template-docker-2023.4.23.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:45:25.256129 pip-package-template-docker-2023.4.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-23 22:45:15.000000 pip-package-template-docker-2023.4.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-23 22:45:25.256129 pip-package-template-docker-2023.4.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-23 22:45:15.000000 pip-package-template-docker-2023.4.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:45:25.256129 pip-package-template-docker-2023.4.23/pip_package_template_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-23 22:45:09.000000 pip-package-template-docker-2023.4.23/pip_package_template_docker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:45:25.256129 pip-package-template-docker-2023.4.23/pip_package_template_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-23 22:45:25.000000 pip-package-template-docker-2023.4.23/pip_package_template_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-23 22:45:25.000000 pip-package-template-docker-2023.4.23/pip_package_template_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:45:25.000000 pip-package-template-docker-2023.4.23/pip_package_template_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-23 22:45:25.000000 pip-package-template-docker-2023.4.23/pip_package_template_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 22:45:25.000000 pip-package-template-docker-2023.4.23/pip_package_template_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 22:45:25.256129 pip-package-template-docker-2023.4.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-23 22:45:09.000000 pip-package-template-docker-2023.4.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:45:25.256129 pip-package-template-docker-2023.4.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-23 22:45:09.000000 pip-package-template-docker-2023.4.23/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:15:57.941348 pip-package-template-docker-2023.4.23.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-24 02:15:49.000000 pip-package-template-docker-2023.4.23.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-24 02:15:57.941348 pip-package-template-docker-2023.4.23.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-24 02:15:49.000000 pip-package-template-docker-2023.4.23.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:15:57.941348 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 02:15:41.000000 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:15:57.941348 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-24 02:15:57.000000 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 02:15:57.000000 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 02:15:57.000000 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 02:15:57.000000 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 02:15:57.000000 pip-package-template-docker-2023.4.23.post1/pip_package_template_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 02:15:57.941348 pip-package-template-docker-2023.4.23.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-24 02:15:41.000000 pip-package-template-docker-2023.4.23.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 02:15:57.941348 pip-package-template-docker-2023.4.23.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 02:15:41.000000 pip-package-template-docker-2023.4.23.post1/tests/test_placeholder.py
```

### Comparing `pip-package-template-docker-2023.4.23/LICENSE` & `pip-package-template-docker-2023.4.23.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-package-template-docker-2023.4.23/README.md` & `pip-package-template-docker-2023.4.23.post1/README.md`

 * *Files identical despite different names*

### Comparing `pip-package-template-docker-2023.4.23/setup.py` & `pip-package-template-docker-2023.4.23.post1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from pathlib import Path
+
 from setuptools import setup, find_packages
 
 from pip_package_template_docker import __version__
 
+project_dir = Path(__file__).parent
+
 deps = ()
 
 extra_flake8 = (
     'flake8',
     'flake8-commas',
     'flake8-quotes',
     'flake8-multiline-containers',
@@ -32,14 +36,15 @@
     version=__version__,
     packages=find_packages(exclude=['tests', 'tests.*']),
     url='https://github.com/MichaelKim0407/pip-package-template-docker',
     license='MIT',
     author='Zheng Jin',
     author_email='mkim0407@gmail.com',
     description='Project template for Dockerized pip package development.',
+    long_description=(project_dir / 'README.md').read_text(),
     long_description_content_type='text/markdown',
 
     install_requires=deps,
     extras_require={
         'dev': extra_dev,
         'ci': extra_ci,
     },
```

