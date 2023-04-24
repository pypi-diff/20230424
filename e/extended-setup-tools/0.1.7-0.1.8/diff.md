# Comparing `tmp/extended-setup-tools-0.1.7.tar.gz` & `tmp/extended-setup-tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extended-setup-tools-0.1.7.tar", last modified: Mon Jan 10 20:39:21 2022, max compression
+gzip compressed data, was "extended-setup-tools-0.1.8.tar", last modified: Mon Apr 24 15:26:57 2023, max compression
```

## Comparing `extended-setup-tools-0.1.7.tar` & `extended-setup-tools-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-10 20:39:21.216881 extended-setup-tools-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1318 2022-01-10 20:39:08.000000 extended-setup-tools-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3022 2022-01-10 20:39:21.216881 extended-setup-tools-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1982 2022-01-10 20:39:08.000000 extended-setup-tools-0.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)    15084 2022-01-10 20:39:08.000000 extended-setup-tools-0.1.7/extended_setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-10 20:39:21.216881 extended-setup-tools-0.1.7/extended_setup_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3022 2022-01-10 20:39:20.000000 extended-setup-tools-0.1.7/extended_setup_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      263 2022-01-10 20:39:20.000000 extended-setup-tools-0.1.7/extended_setup_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-10 20:39:20.000000 extended-setup-tools-0.1.7/extended_setup_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2022-01-10 20:39:20.000000 extended-setup-tools-0.1.7/extended_setup_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-01-10 20:39:20.000000 extended-setup-tools-0.1.7/extended_setup_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-10 20:39:21.216881 extended-setup-tools-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      888 2022-01-10 20:39:08.000000 extended-setup-tools-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 15:26:57.350431 extended-setup-tools-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-04-24 15:26:42.000000 extended-setup-tools-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-04-24 15:26:57.345848 extended-setup-tools-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-04-24 15:26:42.000000 extended-setup-tools-0.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    35628 2023-04-24 15:26:42.000000 extended-setup-tools-0.1.8/extended_setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 15:26:57.345848 extended-setup-tools-0.1.8/extended_setup_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-04-24 15:26:57.000000 extended-setup-tools-0.1.8/extended_setup_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-24 15:26:57.000000 extended-setup-tools-0.1.8/extended_setup_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 15:26:57.000000 extended-setup-tools-0.1.8/extended_setup_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-24 15:26:57.000000 extended-setup-tools-0.1.8/extended_setup_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-24 15:26:57.000000 extended-setup-tools-0.1.8/extended_setup_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 15:26:57.350431 extended-setup-tools-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-04-24 15:26:42.000000 extended-setup-tools-0.1.8/setup.py
```

### Comparing `extended-setup-tools-0.1.7/LICENSE` & `extended-setup-tools-0.1.8/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2021, Peter Zaitcev
+Copyright (c) 2021-2023, Peter Zaitcev
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `extended-setup-tools-0.1.7/PKG-INFO` & `extended-setup-tools-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: extended-setup-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python tool for helping making shorter and smarter setup.py scripts
 Home-page: https://gitlab.com/Hares-Lab/tools/extended-setup-tools
 Author: Peter Zaitcev / USSX Hares
 Maintainer: Peter Zaitcev / USSX Hares
 License: BSD 2-clause
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 # Extended SetupTools
-Python tool for helping making shorter and smarter `setup.py` scripts.
+Python tool for helping in making shorter and smarter `setup.py` scripts.
 
 ### Features
  - Automatically extracts application meta-info from the root `__init__.py` file:
    * Name
    * Version
    * License
  - Automatically finds packages
  - Finds and attaches ReadMe file
- - Handles requirements files and maps the to the respective `requires` setup arguments:
+ - Handles requirements files and maps to the respective `requires` setup arguments:
    * `setup_requires`: `setup-requirements.txt` and `requirements/setup-requirements.txt`
    * `install_requires`: `requirements.txt` and `requirements/requirements.txt`
    * `tests_require`: `test-requirements.txt` and `requirements/test-requirements.txt`
    * `extras_require`: `requirements/requirements-*.txt`
    * Also creates extras `all` that contains all available features
  - Creates test runner with HTML reports
  - Inserts link to the repository as the homepage
@@ -86,9 +87,7 @@
 from extended_setup import ExtendedSetupManager
 ExtendedSetupManager('python_package_name').setup \
 (
     short_description = "Some short description",
     classifiers = [ 'Programming Language :: Python :: 3.7' ],
 )
 ```
-
-
```

### Comparing `extended-setup-tools-0.1.7/README.md` & `extended-setup-tools-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Extended SetupTools
-Python tool for helping making shorter and smarter `setup.py` scripts.
+Python tool for helping in making shorter and smarter `setup.py` scripts.
 
 ### Features
  - Automatically extracts application meta-info from the root `__init__.py` file:
    * Name
    * Version
    * License
  - Automatically finds packages
  - Finds and attaches ReadMe file
- - Handles requirements files and maps the to the respective `requires` setup arguments:
+ - Handles requirements files and maps to the respective `requires` setup arguments:
    * `setup_requires`: `setup-requirements.txt` and `requirements/setup-requirements.txt`
    * `install_requires`: `requirements.txt` and `requirements/requirements.txt`
    * `tests_require`: `test-requirements.txt` and `requirements/test-requirements.txt`
    * `extras_require`: `requirements/requirements-*.txt`
    * Also creates extras `all` that contains all available features
  - Creates test runner with HTML reports
  - Inserts link to the repository as the homepage
```

### Comparing `extended-setup-tools-0.1.7/extended_setup_tools.egg-info/PKG-INFO` & `extended-setup-tools-0.1.8/extended_setup_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: extended-setup-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python tool for helping making shorter and smarter setup.py scripts
 Home-page: https://gitlab.com/Hares-Lab/tools/extended-setup-tools
 Author: Peter Zaitcev / USSX Hares
 Maintainer: Peter Zaitcev / USSX Hares
 License: BSD 2-clause
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 # Extended SetupTools
-Python tool for helping making shorter and smarter `setup.py` scripts.
+Python tool for helping in making shorter and smarter `setup.py` scripts.
 
 ### Features
  - Automatically extracts application meta-info from the root `__init__.py` file:
    * Name
    * Version
    * License
  - Automatically finds packages
  - Finds and attaches ReadMe file
- - Handles requirements files and maps the to the respective `requires` setup arguments:
+ - Handles requirements files and maps to the respective `requires` setup arguments:
    * `setup_requires`: `setup-requirements.txt` and `requirements/setup-requirements.txt`
    * `install_requires`: `requirements.txt` and `requirements/requirements.txt`
    * `tests_require`: `test-requirements.txt` and `requirements/test-requirements.txt`
    * `extras_require`: `requirements/requirements-*.txt`
    * Also creates extras `all` that contains all available features
  - Creates test runner with HTML reports
  - Inserts link to the repository as the homepage
@@ -86,9 +87,7 @@
 from extended_setup import ExtendedSetupManager
 ExtendedSetupManager('python_package_name').setup \
 (
     short_description = "Some short description",
     classifiers = [ 'Programming Language :: Python :: 3.7' ],
 )
 ```
-
-
```

