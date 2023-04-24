# Comparing `tmp/pyecotrend-ista-1.0.9.tar.gz` & `tmp/pyecotrend-ista-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecotrend-ista-1.0.9.tar", last modified: Sat Apr 16 22:00:53 2022, max compression
+gzip compressed data, was "pyecotrend-ista-2.0.0.tar", last modified: Mon Apr 24 08:31:11 2023, max compression
```

## Comparing `pyecotrend-ista-1.0.9.tar` & `pyecotrend-ista-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 22:00:53.418550 pyecotrend-ista-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-04-16 22:00:36.000000 pyecotrend-ista-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-04-16 22:00:53.418550 pyecotrend-ista-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-04-16 22:00:36.000000 pyecotrend-ista-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 22:00:53.414550 pyecotrend-ista-1.0.9/pyecotrend_ista/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-16 22:00:36.000000 pyecotrend-ista-1.0.9/pyecotrend_ista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-04-16 22:00:36.000000 pyecotrend-ista-1.0.9/pyecotrend_ista/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     8956 2022-04-16 22:00:36.000000 pyecotrend-ista-1.0.9/pyecotrend_ista/pyecotrend_ista.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 22:00:53.418550 pyecotrend-ista-1.0.9/pyecotrend_ista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-04-16 22:00:53.000000 pyecotrend-ista-1.0.9/pyecotrend_ista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-04-16 22:00:53.000000 pyecotrend-ista-1.0.9/pyecotrend_ista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-16 22:00:53.000000 pyecotrend-ista-1.0.9/pyecotrend_ista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-16 22:00:53.000000 pyecotrend-ista-1.0.9/pyecotrend_ista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-16 22:00:53.000000 pyecotrend-ista-1.0.9/pyecotrend_ista.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-16 22:00:53.418550 pyecotrend-ista-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-04-16 22:00:36.000000 pyecotrend-ista-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.481258 pyecotrend-ista-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/src/pyecotrend_ista/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/helper_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/ista_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/pyecotrend_ista.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/top_level.txt
```

### Comparing `pyecotrend-ista-1.0.9/LICENSE` & `pyecotrend-ista-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-1.0.9/setup.py` & `pyecotrend-ista-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import setuptools
 import configparser
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.0.0"
-
-with open("./pyecotrend_ista/const.py") as f:
-    config_string = '[dummy_section]\n' + f.read()
+with open("./src/pyecotrend_ista/const.py") as f:
+    config_string = "[dummy_section]\n" + f.read()
     config = configparser.ConfigParser(allow_no_value=True)
     config.read_string(config_string)
-    version = config['dummy_section']['VERSION'].strip('"')
+    version = config["dummy_section"]["VERSION"].strip('"')
 
 setuptools.setup(
     name="pyecotrend-ista",
     version=version,
     author="Ludy87",
     author_email="android@astra-g.org",
     description="Python ecotrend-ista Api",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ludy87/pyecotrend-ista",
-    packages=setuptools.find_packages(),
+    project_urls={
+        "Bug Tracker": "https://github.com/Ludy87/pyecotrend-ista/issues",
+    },
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "Topic :: Utilities",
         "Topic :: Home Automation",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="python api ecotrend ista",
     install_requires=["aiohttp==3.8.1"],
+    python_requires=">=3.6",
 )
```

