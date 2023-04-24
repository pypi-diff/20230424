# Comparing `tmp/jnb2py-0.0.1.tar.gz` & `tmp/jnb2py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jnb2py-0.0.1.tar", last modified: Mon Apr 24 06:25:14 2023, max compression
+gzip compressed data, was "jnb2py-0.0.2.tar", last modified: Mon Apr 24 09:27:48 2023, max compression
```

## Comparing `jnb2py-0.0.1.tar` & `jnb2py-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:25:14.978629 jnb2py-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-23 19:52:55.000000 jnb2py-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1049 2023-04-24 06:25:14.978629 jnb2py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-04-24 06:24:52.000000 jnb2py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 06:25:14.931815 jnb2py-0.0.1/jnb2py/
-drwxrwxrwx   0        0        0        0 2023-04-24 06:25:14.963010 jnb2py-0.0.1/jnb2py/jnb2py.egg-info/
--rw-rw-rw-   0        0        0     1049 2023-04-24 06:25:14.000000 jnb2py-0.0.1/jnb2py/jnb2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-04-24 06:25:14.000000 jnb2py-0.0.1/jnb2py/jnb2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:25:14.000000 jnb2py-0.0.1/jnb2py/jnb2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-24 06:25:14.000000 jnb2py-0.0.1/jnb2py/jnb2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 06:25:14.000000 jnb2py-0.0.1/jnb2py/jnb2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 06:25:14.978629 jnb2py-0.0.1/jnb2py/models/
--rw-rw-rw-   0        0        0       30 2023-04-24 05:58:19.000000 jnb2py-0.0.1/jnb2py/models/__init__.py
--rw-rw-rw-   0        0        0      247 2023-04-23 20:47:26.000000 jnb2py-0.0.1/jnb2py/models/cell_model.py
--rw-rw-rw-   0        0        0       76 2023-04-23 20:55:03.000000 jnb2py-0.0.1/jnb2py/models/notebook_model.py
--rw-rw-rw-   0        0        0       42 2023-04-24 06:25:14.978629 jnb2py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-04-24 06:24:51.000000 jnb2py-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:48.730321 jnb2py-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-24 09:27:39.000000 jnb2py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-24 09:27:48.730321 jnb2py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-24 09:27:39.000000 jnb2py-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:48.726321 jnb2py-0.0.2/jnb2py/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 09:27:39.000000 jnb2py-0.0.2/jnb2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:48.730321 jnb2py-0.0.2/jnb2py/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 09:27:39.000000 jnb2py-0.0.2/jnb2py/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-24 09:27:39.000000 jnb2py-0.0.2/jnb2py/models/cell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 09:27:39.000000 jnb2py-0.0.2/jnb2py/models/notebook_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-24 09:27:39.000000 jnb2py-0.0.2/jnb2py/nbconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 09:27:39.000000 jnb2py-0.0.2/jnb2py/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:48.726321 jnb2py-0.0.2/jnb2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-24 09:27:48.000000 jnb2py-0.0.2/jnb2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 09:27:48.000000 jnb2py-0.0.2/jnb2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:27:48.000000 jnb2py-0.0.2/jnb2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 09:27:48.000000 jnb2py-0.0.2/jnb2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 09:27:48.000000 jnb2py-0.0.2/jnb2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:27:48.730321 jnb2py-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 09:27:39.000000 jnb2py-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:48.730321 jnb2py-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:27:39.000000 jnb2py-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-24 09:27:39.000000 jnb2py-0.0.2/tests/test_nbconverter.py
```

### Comparing `jnb2py-0.0.1/setup.py` & `jnb2py-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from setuptools import find_packages, setup
-
-with open("README.md", "r") as f:
-    long_description = f.read()
-
-setup(
-    name="jnb2py",
-    version="0.0.1",
-    description="Converts .ipynb files to .py files.",
-    package_dir={"": "jnb2py"},
-    packages=find_packages(where="jnb2py"),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/subhranil2605/nb2py",
-    author="Subhranil Sarkar",
-    author_email="subhranil2605@gmail.com",
-    license="MIT",
-    classifiers=[
-        "Programming Language :: Python :: 3.10",
-        "Operating System :: OS Independent"
-    ],
-    extras_require={
-        "dev": ["pytest>=7.0", "twine>=4.0.2"],
-    },
-    python_requires=">=3.10"
-)
+from setuptools import find_packages, setup
+
+with open("README.md", "r") as f:
+    long_description = f.read()
+
+setup(
+    name="jnb2py",
+    version="0.0.2",
+    description="Converts .ipynb files to .py files.",
+    packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/subhranil2605/nb2py",
+    author="Subhranil Sarkar",
+    author_email="subhranil2605@gmail.com",
+    license="MIT",
+    classifiers=[
+        "Programming Language :: Python :: 3.10",
+        "Operating System :: OS Independent"
+    ],
+    extras_require={
+        "dev": ["pytest>=7.0", "twine>=4.0.2"],
+    },
+    python_requires=">=3.10"
+)
```

