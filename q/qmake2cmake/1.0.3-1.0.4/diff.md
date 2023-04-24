# Comparing `tmp/qmake2cmake-1.0.3.tar.gz` & `tmp/qmake2cmake-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmake2cmake-1.0.3.tar", last modified: Thu Mar 16 08:26:05 2023, max compression
+gzip compressed data, was "qmake2cmake-1.0.4.tar", last modified: Mon Apr 24 10:32:40 2023, max compression
```

## Comparing `qmake2cmake-1.0.3.tar` & `qmake2cmake-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-03-16 08:26:05.403773 qmake2cmake-1.0.3/
--rw-r--r--   0 jobor     (1000) jobor     (1000)     5268 2023-03-16 08:26:05.407773 qmake2cmake-1.0.3/PKG-INFO
--rw-r--r--   0 jobor     (1000) jobor     (1000)     4327 2022-06-22 14:12:02.000000 qmake2cmake-1.0.3/README.md
--rw-r--r--   0 jobor     (1000) jobor     (1000)      223 2022-04-06 06:09:46.000000 qmake2cmake-1.0.3/pyproject.toml
--rw-r--r--   0 jobor     (1000) jobor     (1000)     1412 2023-03-16 08:26:05.407773 qmake2cmake-1.0.3/setup.cfg
--rw-r--r--   0 jobor     (1000) jobor     (1000)       38 2022-06-29 12:36:52.000000 qmake2cmake-1.0.3/setup.py
-drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-03-16 08:26:05.403773 qmake2cmake-1.0.3/src/
-drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-03-16 08:26:05.403773 qmake2cmake-1.0.3/src/qmake2cmake/
--rw-r--r--   0 jobor     (1000) jobor     (1000)        0 2022-06-29 12:36:52.000000 qmake2cmake-1.0.3/src/qmake2cmake/__init__.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)     8055 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/src/qmake2cmake/condition_simplifier.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)     5199 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/src/qmake2cmake/condition_simplifier_cache.py
--rw-r--r--   0 jobor     (1000) jobor     (1000)    35371 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/src/qmake2cmake/helper.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)   183009 2023-03-16 08:24:19.000000 qmake2cmake-1.0.3/src/qmake2cmake/pro2cmake.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)     7018 2023-03-16 08:24:19.000000 qmake2cmake-1.0.3/src/qmake2cmake/pro_conversion_rate.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)    16464 2023-03-16 08:24:19.000000 qmake2cmake-1.0.3/src/qmake2cmake/qmake_parser.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)     9878 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/src/qmake2cmake/run_pro2cmake.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)    15121 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/src/qmake2cmake/special_case_helper.py
-drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-03-16 08:26:05.403773 qmake2cmake-1.0.3/src/qmake2cmake.egg-info/
--rw-r--r--   0 jobor     (1000) jobor     (1000)     5268 2023-03-16 08:26:05.000000 qmake2cmake-1.0.3/src/qmake2cmake.egg-info/PKG-INFO
--rw-r--r--   0 jobor     (1000) jobor     (1000)      743 2023-03-16 08:26:05.000000 qmake2cmake-1.0.3/src/qmake2cmake.egg-info/SOURCES.txt
--rw-r--r--   0 jobor     (1000) jobor     (1000)        1 2023-03-16 08:26:05.000000 qmake2cmake-1.0.3/src/qmake2cmake.egg-info/dependency_links.txt
--rw-r--r--   0 jobor     (1000) jobor     (1000)      108 2023-03-16 08:26:05.000000 qmake2cmake-1.0.3/src/qmake2cmake.egg-info/entry_points.txt
--rw-r--r--   0 jobor     (1000) jobor     (1000)       89 2023-03-16 08:26:05.000000 qmake2cmake-1.0.3/src/qmake2cmake.egg-info/requires.txt
--rw-r--r--   0 jobor     (1000) jobor     (1000)       12 2023-03-16 08:26:05.000000 qmake2cmake-1.0.3/src/qmake2cmake.egg-info/top_level.txt
-drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-03-16 08:26:05.403773 qmake2cmake-1.0.3/tests/
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)     8321 2023-03-16 08:24:19.000000 qmake2cmake-1.0.3/tests/test_conversion.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)      600 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/tests/test_lc_fixup.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)     4187 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/tests/test_logic_mapping.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)      984 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/tests/test_operations.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)    10508 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/tests/test_parsing.py
--rwxr-xr-x   0 jobor     (1000) jobor     (1000)    10857 2022-07-05 06:04:44.000000 qmake2cmake-1.0.3/tests/test_scope_handling.py
+drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-04-24 10:32:40.207246 qmake2cmake-1.0.4/
+-rw-r--r--   0 jobor     (1000) jobor     (1000)     5074 2023-04-24 10:32:40.207246 qmake2cmake-1.0.4/PKG-INFO
+-rw-r--r--   0 jobor     (1000) jobor     (1000)     4038 2023-04-19 12:59:05.000000 qmake2cmake-1.0.4/README.md
+-rw-r--r--   0 jobor     (1000) jobor     (1000)      223 2022-05-02 10:44:13.000000 qmake2cmake-1.0.4/pyproject.toml
+-rw-r--r--   0 jobor     (1000) jobor     (1000)     1372 2023-04-24 10:32:40.207246 qmake2cmake-1.0.4/setup.cfg
+-rw-r--r--   0 jobor     (1000) jobor     (1000)       38 2022-05-02 10:44:13.000000 qmake2cmake-1.0.4/setup.py
+drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-04-24 10:32:40.203246 qmake2cmake-1.0.4/src/
+drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-04-24 10:32:40.207246 qmake2cmake-1.0.4/src/qmake2cmake/
+-rw-r--r--   0 jobor     (1000) jobor     (1000)        0 2022-05-02 10:44:13.000000 qmake2cmake-1.0.4/src/qmake2cmake/__init__.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)     8055 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/src/qmake2cmake/condition_simplifier.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)     5184 2023-03-20 14:25:08.000000 qmake2cmake-1.0.4/src/qmake2cmake/condition_simplifier_cache.py
+-rw-r--r--   0 jobor     (1000) jobor     (1000)    35371 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/src/qmake2cmake/helper.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)   183009 2023-03-17 12:37:25.000000 qmake2cmake-1.0.4/src/qmake2cmake/pro2cmake.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)     7018 2023-02-24 16:43:40.000000 qmake2cmake-1.0.4/src/qmake2cmake/pro_conversion_rate.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)    16464 2023-02-24 16:35:51.000000 qmake2cmake-1.0.4/src/qmake2cmake/qmake_parser.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)     9878 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/src/qmake2cmake/run_pro2cmake.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)    15121 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/src/qmake2cmake/special_case_helper.py
+drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-04-24 10:32:40.207246 qmake2cmake-1.0.4/src/qmake2cmake.egg-info/
+-rw-r--r--   0 jobor     (1000) jobor     (1000)     5074 2023-04-24 10:32:40.000000 qmake2cmake-1.0.4/src/qmake2cmake.egg-info/PKG-INFO
+-rw-r--r--   0 jobor     (1000) jobor     (1000)      743 2023-04-24 10:32:40.000000 qmake2cmake-1.0.4/src/qmake2cmake.egg-info/SOURCES.txt
+-rw-r--r--   0 jobor     (1000) jobor     (1000)        1 2023-04-24 10:32:40.000000 qmake2cmake-1.0.4/src/qmake2cmake.egg-info/dependency_links.txt
+-rw-r--r--   0 jobor     (1000) jobor     (1000)      108 2023-04-24 10:32:40.000000 qmake2cmake-1.0.4/src/qmake2cmake.egg-info/entry_points.txt
+-rw-r--r--   0 jobor     (1000) jobor     (1000)       89 2023-04-24 10:32:40.000000 qmake2cmake-1.0.4/src/qmake2cmake.egg-info/requires.txt
+-rw-r--r--   0 jobor     (1000) jobor     (1000)       12 2023-04-24 10:32:40.000000 qmake2cmake-1.0.4/src/qmake2cmake.egg-info/top_level.txt
+drwxr-xr-x   0 jobor     (1000) jobor     (1000)        0 2023-04-24 10:32:40.207246 qmake2cmake-1.0.4/tests/
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)     8321 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/tests/test_conversion.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)      600 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/tests/test_lc_fixup.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)     4187 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/tests/test_logic_mapping.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)      984 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/tests/test_operations.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)    10508 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/tests/test_parsing.py
+-rwxr-xr-x   0 jobor     (1000) jobor     (1000)    10857 2023-02-24 12:59:50.000000 qmake2cmake-1.0.4/tests/test_scope_handling.py
```

### Comparing `qmake2cmake-1.0.3/PKG-INFO` & `qmake2cmake-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: qmake2cmake
-Version: 1.0.3
+Version: 1.0.4
 Summary: QMake to CMake project file converter
 Home-page: https://wiki.qt.io/qmake2cmake
-Download-URL: https://download.qt.io/
 Author: The Qt Company
 License: GPLv3
+Project-URL: Bug Tracker, https://bugreports.qt.io
+Project-URL: Source, https://codereview.qt-project.org/admin/repos/qt/qmake2cmake
 Keywords: qmake,cmake,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -45,51 +46,42 @@
 - extra compilers
 - extra targets
 - installation rules
 
 # Requirements
 
 * [Python 3.7](https://www.python.org/downloads/),
-* `pipenv` or `pip` to manage the modules.
+* `pip` to manage Python packages.
 
-## Python modules
-
-Since Python has many ways of handling projects, you have a couple of options to
-install the dependencies of the scripts:
+# Installation
 
-### Using `pipenv`
+You can install the `qmake2cmake` package directly via `pip install
+qmake2cmake`.
 
-The dependencies are specified on the `Pipfile`, so you just need to run
-`pipenv install` and that will automatically create a virtual environment
-that you can activate with a `pipenv shell`.
+In case you are developing a new feature or want to install the latest
+repository version, do an editable build by running `pip install -e .`
 
-### Using `pip`
+# Installation for contributors
 
-It's highly recommended to use a [virtual
+For developers who want to contribute to `qmake2cmake`, we recommend
+using a [virtual
 environment](https://docs.python.org/3/library/venv.html) to avoid
 conflicts with other packages that are already installed.
 
 * Create an environment: `python3 -m venv env --prompt qmake2cmake`,
 * Activate the environment: `source env/bin/activate`
   (on Windows: `env\Scripts\activate.bat`)
 * Install the requirements: `pip install -r requirements.txt`
 
 If the `pip install` command above doesn't work, try:
 
 ```
 python3.7 -m pip install -r requirements.txt
 ```
 
-# Installation
-
-You can install the package directly via `pip install qmake2cmake`.
-
-In case you are developing a new feature or want to install the latest
-repository version, do an editable build by running `pip install -e .`
-
 # Usage
 
 After installing the `qmake2cmake` package, two scripts will be
 available in your bin/ directory of your Python environment:
 `qmake2cmake` and `qmake2cmake_all`.
 
 The following call converts a single QMake project file to CMake:
```

### Comparing `qmake2cmake-1.0.3/README.md` & `qmake2cmake-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,51 +20,42 @@
 - extra compilers
 - extra targets
 - installation rules
 
 # Requirements
 
 * [Python 3.7](https://www.python.org/downloads/),
-* `pipenv` or `pip` to manage the modules.
+* `pip` to manage Python packages.
 
-## Python modules
-
-Since Python has many ways of handling projects, you have a couple of options to
-install the dependencies of the scripts:
+# Installation
 
-### Using `pipenv`
+You can install the `qmake2cmake` package directly via `pip install
+qmake2cmake`.
 
-The dependencies are specified on the `Pipfile`, so you just need to run
-`pipenv install` and that will automatically create a virtual environment
-that you can activate with a `pipenv shell`.
+In case you are developing a new feature or want to install the latest
+repository version, do an editable build by running `pip install -e .`
 
-### Using `pip`
+# Installation for contributors
 
-It's highly recommended to use a [virtual
+For developers who want to contribute to `qmake2cmake`, we recommend
+using a [virtual
 environment](https://docs.python.org/3/library/venv.html) to avoid
 conflicts with other packages that are already installed.
 
 * Create an environment: `python3 -m venv env --prompt qmake2cmake`,
 * Activate the environment: `source env/bin/activate`
   (on Windows: `env\Scripts\activate.bat`)
 * Install the requirements: `pip install -r requirements.txt`
 
 If the `pip install` command above doesn't work, try:
 
 ```
 python3.7 -m pip install -r requirements.txt
 ```
 
-# Installation
-
-You can install the package directly via `pip install qmake2cmake`.
-
-In case you are developing a new feature or want to install the latest
-repository version, do an editable build by running `pip install -e .`
-
 # Usage
 
 After installing the `qmake2cmake` package, two scripts will be
 available in your bin/ directory of your Python environment:
 `qmake2cmake` and `qmake2cmake_all`.
 
 The following call converts a single QMake project file to CMake:
```

### Comparing `qmake2cmake-1.0.3/setup.cfg` & `qmake2cmake-1.0.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [metadata]
 name = qmake2cmake
-version = 1.0.3
+version = 1.0.4
 description = QMake to CMake project file converter
 url = https://wiki.qt.io/qmake2cmake
-download_url = https://download.qt.io/
 license = GPLv3
 license_files = LICENSE.GPL3
 author = The Qt Company
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = qmake, cmake, development
 ext_modules = None
-projects_urls = 
+project_urls = 
 	Bug Tracker = https://bugreports.qt.io
 	Source = https://codereview.qt-project.org/admin/repos/qt/qmake2cmake
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Topic :: Software Development :: Build Tools
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/condition_simplifier.py` & `qmake2cmake-1.0.4/src/qmake2cmake/condition_simplifier.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/condition_simplifier_cache.py` & `qmake2cmake-1.0.4/src/qmake2cmake/condition_simplifier_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import atexit
 import hashlib
 import json
 import os
 import sys
 import time
+import platformdirs
 
 from typing import Any, Callable, Dict
 
 condition_simplifier_cache_enabled = True
 
 
 def set_condition_simplified_cache_enabled(value: bool):
@@ -25,17 +26,16 @@
     except NameError:
         this_file = sys.argv[0]
     this_file = os.path.abspath(this_file)
     return this_file
 
 
 def get_cache_location() -> str:
-    this_file = get_current_file_path()
-    dir_path = os.path.dirname(this_file)
-    cache_path = os.path.join(dir_path, ".pro2cmake_cache", "cache.json")
+    temp_path = platformdirs.user_cache_dir()
+    cache_path = os.path.join(temp_path, ".pro2cmake_cache", "cache.json")
     return cache_path
 
 
 def get_file_checksum(file_path: str) -> str:
     try:
         with open(file_path, "r") as content_file:
             content = content_file.read()
```

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/helper.py` & `qmake2cmake-1.0.4/src/qmake2cmake/helper.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/pro2cmake.py` & `qmake2cmake-1.0.4/src/qmake2cmake/pro2cmake.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/pro_conversion_rate.py` & `qmake2cmake-1.0.4/src/qmake2cmake/pro_conversion_rate.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/qmake_parser.py` & `qmake2cmake-1.0.4/src/qmake2cmake/qmake_parser.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/run_pro2cmake.py` & `qmake2cmake-1.0.4/src/qmake2cmake/run_pro2cmake.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake/special_case_helper.py` & `qmake2cmake-1.0.4/src/qmake2cmake/special_case_helper.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake.egg-info/PKG-INFO` & `qmake2cmake-1.0.4/src/qmake2cmake.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: qmake2cmake
-Version: 1.0.3
+Version: 1.0.4
 Summary: QMake to CMake project file converter
 Home-page: https://wiki.qt.io/qmake2cmake
-Download-URL: https://download.qt.io/
 Author: The Qt Company
 License: GPLv3
+Project-URL: Bug Tracker, https://bugreports.qt.io
+Project-URL: Source, https://codereview.qt-project.org/admin/repos/qt/qmake2cmake
 Keywords: qmake,cmake,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -45,51 +46,42 @@
 - extra compilers
 - extra targets
 - installation rules
 
 # Requirements
 
 * [Python 3.7](https://www.python.org/downloads/),
-* `pipenv` or `pip` to manage the modules.
+* `pip` to manage Python packages.
 
-## Python modules
-
-Since Python has many ways of handling projects, you have a couple of options to
-install the dependencies of the scripts:
+# Installation
 
-### Using `pipenv`
+You can install the `qmake2cmake` package directly via `pip install
+qmake2cmake`.
 
-The dependencies are specified on the `Pipfile`, so you just need to run
-`pipenv install` and that will automatically create a virtual environment
-that you can activate with a `pipenv shell`.
+In case you are developing a new feature or want to install the latest
+repository version, do an editable build by running `pip install -e .`
 
-### Using `pip`
+# Installation for contributors
 
-It's highly recommended to use a [virtual
+For developers who want to contribute to `qmake2cmake`, we recommend
+using a [virtual
 environment](https://docs.python.org/3/library/venv.html) to avoid
 conflicts with other packages that are already installed.
 
 * Create an environment: `python3 -m venv env --prompt qmake2cmake`,
 * Activate the environment: `source env/bin/activate`
   (on Windows: `env\Scripts\activate.bat`)
 * Install the requirements: `pip install -r requirements.txt`
 
 If the `pip install` command above doesn't work, try:
 
 ```
 python3.7 -m pip install -r requirements.txt
 ```
 
-# Installation
-
-You can install the package directly via `pip install qmake2cmake`.
-
-In case you are developing a new feature or want to install the latest
-repository version, do an editable build by running `pip install -e .`
-
 # Usage
 
 After installing the `qmake2cmake` package, two scripts will be
 available in your bin/ directory of your Python environment:
 `qmake2cmake` and `qmake2cmake_all`.
 
 The following call converts a single QMake project file to CMake:
```

### Comparing `qmake2cmake-1.0.3/src/qmake2cmake.egg-info/SOURCES.txt` & `qmake2cmake-1.0.4/src/qmake2cmake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/tests/test_conversion.py` & `qmake2cmake-1.0.4/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/tests/test_lc_fixup.py` & `qmake2cmake-1.0.4/tests/test_lc_fixup.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/tests/test_logic_mapping.py` & `qmake2cmake-1.0.4/tests/test_logic_mapping.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/tests/test_operations.py` & `qmake2cmake-1.0.4/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/tests/test_parsing.py` & `qmake2cmake-1.0.4/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `qmake2cmake-1.0.3/tests/test_scope_handling.py` & `qmake2cmake-1.0.4/tests/test_scope_handling.py`

 * *Files identical despite different names*

