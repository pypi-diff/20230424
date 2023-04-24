# Comparing `tmp/pysparkler-0.6.dev1682027344.tar.gz` & `tmp/pysparkler-0.7.dev1682352964.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.6.dev1682027344.tar", max compression
+gzip compressed data, was "pysparkler-0.7.dev1682352964.tar", max compression
```

## Comparing `pysparkler-0.6.dev1682027344.tar` & `pysparkler-0.7.dev1682352964.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     9874 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/README.md
--rw-r--r--   0        0        0     1203 2023-04-20 21:49:04.926683 pysparkler-0.6.dev1682027344/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/__init__.py
--rw-r--r--   0        0        0     5294 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/api.py
--rw-r--r--   0        0        0     7372 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/base.py
--rw-r--r--   0        0        0     6398 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2206 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10561 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4550 2023-04-20 21:48:55.914674 pysparkler-0.6.dev1682027344/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0    10753 1970-01-01 00:00:00.000000 pysparkler-0.6.dev1682027344/PKG-INFO
+-rw-r--r--   0        0        0    12161 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/README.md
+-rw-r--r--   0        0        0     1203 2023-04-24 16:16:04.661523 pysparkler-0.7.dev1682352964/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/__init__.py
+-rw-r--r--   0        0        0     5294 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/api.py
+-rw-r--r--   0        0        0     7372 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/base.py
+-rw-r--r--   0        0        0     6398 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2206 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10561 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4550 2023-04-24 16:15:55.481405 pysparkler-0.7.dev1682352964/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0    13040 1970-01-01 00:00:00.000000 pysparkler-0.7.dev1682352964/PKG-INFO
```

### Comparing `pysparkler-0.6.dev1682027344/README.md` & `pysparkler-0.7.dev1682352964/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,63 @@
 # PySparkler
 
 [![PyPI version](https://badge.fury.io/py/pysparkler.svg)](https://badge.fury.io/py/pysparkler)
 [![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 PySparkler is a tool that upgrades your PySpark scripts to latest Spark version. It is a command line tool that takes a
-PySpark script as input and outputs a latest Spark version compatible script. It is written in Python and uses the
+PySpark script as input and outputs latest Spark version compatible script. It is written in Python and uses the
 [LibCST](https://github.com/Instagram/LibCST) module to parse the input script and generate the output script.
 
-## Basic Usage
+## Installation
 
-Install from PyPI:
+We recommend installing PySparkler from PyPI using [pipx](https://pypa.github.io/pipx) which allows us to install and 
+run Python Applications in Isolated Environments. To install pipx on your system, follow the instructions 
+[here](https://pypa.github.io/pipx/installation/#install-pipx). Once pipx is installed, you can install PySparkler using:
 
 ```bash
-pip install pysparkler
+pipx install pysparkler
 ```
 
+That's it! You are now ready to use PySparkler.
+
+```bash
+pysparkler --help
+```
+
+## Getting Started
+
 Provide the path to the script you want to upgrade:
 
 ```bash
 pysparkler upgrade --input-file /path/to/script.py
 ```
 
+PySparkler parses the code and can perform either of the following actions:
+
+1. **Code Transformations** - These are modifications that are performed on the code to make it compatible with the
+latest Spark version. For example, if you are upgrading from Spark 2.4 to 3.0, PySparkler will alphabetically sort the
+keyword arguments in the `Row` constructor to preserve backwards compatible behavior. This action will also add a
+comment to the end of statement line being modified to indicate that the code was modified by PySparkler, explaining 
+why.
+
+2. **Code Hints** - Python is a dynamically-typed language, so there are situations wherein PySparkler cannot, with
+100% accuracy, determine if the code is eligible for a transformation. In such situations, PySparkler adds code hints to
+guide the end-user to make an appropriate change if needed. Code hints are comments that are added to the end of a 
+statement line to suggest changes that may be needed it to make it compatible with the latest Spark version. 
+For example, if you are upgrading from Spark 2.4 to 3.0 and PySparkler detects `spark.sql.execution.arrow.enabled` is
+set to `True` in your code, it will add a code hint to the end of the line to suggest setting 
+`spark.sql.execution.pandas.convertToArrowArraySafely` to `True` in case you want to raise errors in case of Integer 
+overflow or Floating point truncation, instead of silent allows. As you can see the suggestion is pretty contextual and 
+may not be applicable in all cases. In cases where not applicable, the end-user can choose to ignore the code hint.
+
+**NOTE**: PySparkler tries to keep the code formatting intact as much as possible. However, it is possible that the
+statement lines it takes actions on may fail the linting checks post changes. In such situations, the end-user will have 
+to fix the linting errors manually.
+
+
 ## PySpark Upgrades Supported
 
 This tool follows the [Apache Spark Migration guide for PySpark](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html)
 to upgrade your PySpark scripts. In the latest stable version it supports the following upgrades from the migration guide:
 
 | Migration                                       | Supported | Details                                                                                                                                      |
 |-------------------------------------------------|-----------|----------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `pysparkler-0.6.dev1682027344/pyproject.toml` & `pysparkler-0.7.dev1682352964/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.6.dev1682027344"
+version = "0.7.dev1682352964"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/__init__.py` & `pysparkler-0.7.dev1682352964/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/api.py` & `pysparkler-0.7.dev1682352964/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/base.py` & `pysparkler-0.7.dev1682352964/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/cli.py` & `pysparkler-0.7.dev1682352964/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.7.dev1682352964/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.7.dev1682352964/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.7.dev1682352964/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.7.dev1682352964/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.7.dev1682352964/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.6.dev1682027344/PKG-INFO` & `pysparkler-0.7.dev1682352964/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.6.dev1682027344
+Version: 0.7.dev1682352964
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
@@ -22,31 +22,64 @@
 
 # PySparkler
 
 [![PyPI version](https://badge.fury.io/py/pysparkler.svg)](https://badge.fury.io/py/pysparkler)
 [![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 PySparkler is a tool that upgrades your PySpark scripts to latest Spark version. It is a command line tool that takes a
-PySpark script as input and outputs a latest Spark version compatible script. It is written in Python and uses the
+PySpark script as input and outputs latest Spark version compatible script. It is written in Python and uses the
 [LibCST](https://github.com/Instagram/LibCST) module to parse the input script and generate the output script.
 
-## Basic Usage
+## Installation
 
-Install from PyPI:
+We recommend installing PySparkler from PyPI using [pipx](https://pypa.github.io/pipx) which allows us to install and 
+run Python Applications in Isolated Environments. To install pipx on your system, follow the instructions 
+[here](https://pypa.github.io/pipx/installation/#install-pipx). Once pipx is installed, you can install PySparkler using:
 
 ```bash
-pip install pysparkler
+pipx install pysparkler
 ```
 
+That's it! You are now ready to use PySparkler.
+
+```bash
+pysparkler --help
+```
+
+## Getting Started
+
 Provide the path to the script you want to upgrade:
 
 ```bash
 pysparkler upgrade --input-file /path/to/script.py
 ```
 
+PySparkler parses the code and can perform either of the following actions:
+
+1. **Code Transformations** - These are modifications that are performed on the code to make it compatible with the
+latest Spark version. For example, if you are upgrading from Spark 2.4 to 3.0, PySparkler will alphabetically sort the
+keyword arguments in the `Row` constructor to preserve backwards compatible behavior. This action will also add a
+comment to the end of statement line being modified to indicate that the code was modified by PySparkler, explaining 
+why.
+
+2. **Code Hints** - Python is a dynamically-typed language, so there are situations wherein PySparkler cannot, with
+100% accuracy, determine if the code is eligible for a transformation. In such situations, PySparkler adds code hints to
+guide the end-user to make an appropriate change if needed. Code hints are comments that are added to the end of a 
+statement line to suggest changes that may be needed it to make it compatible with the latest Spark version. 
+For example, if you are upgrading from Spark 2.4 to 3.0 and PySparkler detects `spark.sql.execution.arrow.enabled` is
+set to `True` in your code, it will add a code hint to the end of the line to suggest setting 
+`spark.sql.execution.pandas.convertToArrowArraySafely` to `True` in case you want to raise errors in case of Integer 
+overflow or Floating point truncation, instead of silent allows. As you can see the suggestion is pretty contextual and 
+may not be applicable in all cases. In cases where not applicable, the end-user can choose to ignore the code hint.
+
+**NOTE**: PySparkler tries to keep the code formatting intact as much as possible. However, it is possible that the
+statement lines it takes actions on may fail the linting checks post changes. In such situations, the end-user will have 
+to fix the linting errors manually.
+
+
 ## PySpark Upgrades Supported
 
 This tool follows the [Apache Spark Migration guide for PySpark](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html)
 to upgrade your PySpark scripts. In the latest stable version it supports the following upgrades from the migration guide:
 
 | Migration                                       | Supported | Details                                                                                                                                      |
 |-------------------------------------------------|-----------|----------------------------------------------------------------------------------------------------------------------------------------------|
```

