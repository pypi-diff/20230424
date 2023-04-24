# Comparing `tmp/pyproject_pre_commit-0.0.7.tar.gz` & `tmp/pyproject_pre_commit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_pre_commit-0.0.7.tar", max compression
+gzip compressed data, was "pyproject_pre_commit-0.0.8.tar", max compression
```

## Comparing `pyproject_pre_commit-0.0.7.tar` & `pyproject_pre_commit-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11337 2023-04-17 01:02:26.086021 pyproject_pre_commit-0.0.7/LICENSE
--rw-r--r--   0        0        0     5374 2023-04-17 01:02:26.086021 pyproject_pre_commit-0.0.7/README.md
--rw-r--r--   0        0        0     2944 2023-04-17 01:02:26.770022 pyproject_pre_commit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      118 2023-04-17 01:02:26.770022 pyproject_pre_commit-0.0.7/src/pyproject_pre_commit/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-17 01:02:26.086021 pyproject_pre_commit-0.0.7/src/pyproject_pre_commit/pyproject_pre_commit.py
--rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-24 01:02:50.116757 pyproject_pre_commit-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5374 2023-04-24 01:02:50.116757 pyproject_pre_commit-0.0.8/README.md
+-rw-r--r--   0        0        0     2944 2023-04-24 01:02:51.068768 pyproject_pre_commit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-04-24 01:02:51.068768 pyproject_pre_commit-0.0.8/src/pyproject_pre_commit/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-24 01:02:50.116757 pyproject_pre_commit-0.0.8/src/pyproject_pre_commit/pyproject_pre_commit.py
+-rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.0.8/PKG-INFO
```

### Comparing `pyproject_pre_commit-0.0.7/LICENSE` & `pyproject_pre_commit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.7/README.md` & `pyproject_pre_commit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.7/pyproject.toml` & `pyproject_pre_commit-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyproject-pre-commit"
-version = "0.0.7"
+version = "0.0.8"
 description = "pre-commit hooks for python projects using pyproject.toml."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/pyproject-pre-commit"
 homepage = "https://github.com/rcmdnk/pyproject-pre-commit"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["pre-commit", "pyproject.toml", "poetry"]
@@ -33,15 +33,15 @@
 flake8-executable = "2.1.3"
 flake8-pep3101 = "^2.0.0"
 flake8-print = "5.0.0"
 flake8-rst-docstrings = "0.3.0"
 flake8-string-format = "0.3.0"
 pep8-naming = "0.13.3"
 pycodestyle = "2.10.0"
-autoflake = "2.0.2"
+autoflake = "2.1.1"
 autopep8 = "2.0.2"
 isort = "5.12.0"
 mypy = "1.2.0"
 bandit = {extras = ["toml"], version = "1.7.5"}
 shellcheck-py = "0.9.0.2"
 mdformat = "0.7.16"
 mdformat-gfm = "0.3.5"
```

### Comparing `pyproject_pre_commit-0.0.7/src/pyproject_pre_commit/pyproject_pre_commit.py` & `pyproject_pre_commit-0.0.8/src/pyproject_pre_commit/pyproject_pre_commit.py`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.0.7/PKG-INFO` & `pyproject_pre_commit-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-pre-commit
-Version: 0.0.7
+Version: 0.0.8
 Summary: pre-commit hooks for python projects using pyproject.toml.
 Home-page: https://github.com/rcmdnk/pyproject-pre-commit
 License: Apache-2.0
 Keywords: pre-commit,pyproject.toml,poetry
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.8.1,<3.12
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: autoflake (==2.0.2)
+Requires-Dist: autoflake (==2.1.1)
 Requires-Dist: autopep8 (==2.0.2)
 Requires-Dist: bandit[toml] (==1.7.5)
 Requires-Dist: black (==23.3.0)
 Requires-Dist: blacken-docs (==1.13.0)
 Requires-Dist: flake8-annotations-complexity (==0.0.7)
 Requires-Dist: flake8-bugbear (==23.3.23)
 Requires-Dist: flake8-builtins (==2.1.0)
```

