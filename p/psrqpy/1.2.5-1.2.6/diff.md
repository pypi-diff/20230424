# Comparing `tmp/psrqpy-1.2.5.tar.gz` & `tmp/psrqpy-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/psrqpy/psrqpy/dist/.tmp-sknj_pqg/psrqpy-1.2.5.tar", last modified: Mon Jan 16 10:08:41 2023, max compression
+gzip compressed data, was "/home/runner/work/psrqpy/psrqpy/dist/.tmp-a_9xzl3o/psrqpy-1.2.6.tar", last modified: Mon Apr 24 16:27:02 2023, max compression
```

## Comparing `psrqpy-1.2.5.tar` & `psrqpy-1.2.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-16 10:08:27.000000 psrqpy-1.2.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-16 10:08:27.000000 psrqpy-1.2.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-16 10:08:27.000000 psrqpy-1.2.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-16 10:08:27.000000 psrqpy-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-16 10:08:27.000000 psrqpy-1.2.5/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-16 10:08:27.000000 psrqpy-1.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-01-16 10:08:27.000000 psrqpy-1.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-01-16 10:08:27.000000 psrqpy-1.2.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-16 10:08:27.000000 psrqpy-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-01-16 10:08:41.000000 psrqpy-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-01-16 10:08:27.000000 psrqpy-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   187239 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/images/PvsPdot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/images/ppdot.png
--rw-r--r--   0 runner    (1001) docker     (123)    18282 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/pulsar.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/query.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-16 10:08:27.000000 psrqpy-1.2.5/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-16 10:08:27.000000 psrqpy-1.2.5/paper/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-16 10:08:27.000000 psrqpy-1.2.5/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-16 10:08:27.000000 psrqpy-1.2.5/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-01-16 10:08:27.000000 psrqpy-1.2.5/paper/paper.tex
--rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-01-16 10:08:27.000000 psrqpy-1.2.5/paper/ppdot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (123)   122264 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/tests/derived_catalogue.db
--rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/tests/query_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/tests/test_catalogue.db
--rw-r--r--   0 runner    (1001) docker     (123)    76429 2023-01-16 10:08:27.000000 psrqpy-1.2.5/psrqpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-16 10:08:41.000000 psrqpy-1.2.5/psrqpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-16 10:08:27.000000 psrqpy-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-16 10:08:27.000000 psrqpy-1.2.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-16 10:08:41.000000 psrqpy-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-16 10:08:27.000000 psrqpy-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 16:26:51.000000 psrqpy-1.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-24 16:26:51.000000 psrqpy-1.2.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 16:26:51.000000 psrqpy-1.2.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 16:26:51.000000 psrqpy-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-04-24 16:27:02.000000 psrqpy-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-04-24 16:26:51.000000 psrqpy-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   187239 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/images/PvsPdot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/images/ppdot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18282 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/pulsar.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/query.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 16:26:51.000000 psrqpy-1.2.6/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/paper.tex
+-rw-r--r--   0 runner    (1001) docker     (123)   141497 2023-04-24 16:26:51.000000 psrqpy-1.2.6/paper/ppdot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122264 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/derived_catalogue.db
+-rw-r--r--   0 runner    (1001) docker     (123)    28442 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/query_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/tests/test_catalogue.db
+-rw-r--r--   0 runner    (1001) docker     (123)    76496 2023-04-24 16:26:51.000000 psrqpy-1.2.6/psrqpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:27:02.000000 psrqpy-1.2.6/psrqpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 16:26:51.000000 psrqpy-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 16:26:51.000000 psrqpy-1.2.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-24 16:27:02.000000 psrqpy-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 16:26:51.000000 psrqpy-1.2.6/setup.py
```

### Comparing `psrqpy-1.2.5/.github/workflows/build.yml` & `psrqpy-1.2.6/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 name: build
 
 on:
   push:
-    branches: [ master ]
+    branches: [ main ]
   pull_request:
-    branches: [ master ]
+    branches: [ main ]
   schedule:
     - cron: "0 0 * * *"
 
 jobs:
   build:
     strategy:
       matrix:
         os: [ubuntu-20.04]
-        python-version: [3.7, 3.8, 3.9, 3.10]
+        python-version: [3.7, 3.8, 3.9, "3.10"]
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `psrqpy-1.2.5/.github/workflows/pypi.yml` & `psrqpy-1.2.6/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/CHANGELOG.md` & `psrqpy-1.2.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Notable changes between versions
 
+## [1.2.6] 2023-04-24]
+
+- Make the `NAME` attribute default to using the PSRB name if available to be consistent with `psrcat`. See [#122](https://github.com/mattpitkin/psrqpy/pull/122).
+- Fix parsing of the glitch catalogue table. See [#121](https://github.com/mattpitkin/psrqpy/pull/121).
+
 ## [1.2.5] 2023-01-16
 
 - Update `get_gc_catalogue` for parsing the [Globular Cluster pulsar catalogue](https://www.naic.edu/~pfreire/GCpsr.txt) to allow the "Offset" value to have an associated error value.
 
 ## [1.2.4] 2022-11-22
 
 - Allow references to be extracted for a given ATNF catalogue version. See [#115](https://github.com/mattpitkin/psrqpy/pull/115).
```

### Comparing `psrqpy-1.2.5/Dockerfile` & `psrqpy-1.2.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/LICENSE` & `psrqpy-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/PKG-INFO` & `psrqpy-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrqpy
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python module for querying the ATNF pulsar catalogue
 Home-page: https://github.com/mattpitkin/psrqpy
 Author: Matthew Pitkin
 Author-email: matthew.pitkin@ligo.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -168,15 +168,15 @@
 from psrqpy import QueryATNF
 query = QueryATNF(params=['P0', 'P1', 'ASSOC', 'BINARY', 'TYPE', 'P1_I'])
 query.ppdot(showSNRs=True, showtypes='all')
 ```
 
 gives
 
-![PPdot](../master/docs/source/images/ppdot.png)
+![PPdot](../main/docs/source/images/ppdot.png)
 
 ## Development and Support
 
 Code development is done via the package's [GitHib repository](https://github.com/mattpitkin/psrqpy).
 Any contributions can be made via a [fork and pull request](https://help.github.com/articles/creating-a-pull-request-from-a-fork/) model
 from that repository, and must adhere to the [MIT license](#License). Any problems with the code
 or support requests can be submitted via the repository's [Issue tracker](https://github.com/mattpitkin/psrqpy/issues).
```

### Comparing `psrqpy-1.2.5/README.md` & `psrqpy-1.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 from psrqpy import QueryATNF
 query = QueryATNF(params=['P0', 'P1', 'ASSOC', 'BINARY', 'TYPE', 'P1_I'])
 query.ppdot(showSNRs=True, showtypes='all')
 ```
 
 gives
 
-![PPdot](../master/docs/source/images/ppdot.png)
+![PPdot](../main/docs/source/images/ppdot.png)
 
 ## Development and Support
 
 Code development is done via the package's [GitHib repository](https://github.com/mattpitkin/psrqpy).
 Any contributions can be made via a [fork and pull request](https://help.github.com/articles/creating-a-pull-request-from-a-fork/) model
 from that repository, and must adhere to the [MIT license](#License). Any problems with the code
 or support requests can be submitted via the repository's [Issue tracker](https://github.com/mattpitkin/psrqpy/issues).
```

### Comparing `psrqpy-1.2.5/docs/Makefile` & `psrqpy-1.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/docs/source/CHANGELOG.md` & `psrqpy-1.2.6/docs/source/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Notable changes between versions
 
+## [1.2.6] 2023-04-24]
+
+- Make the `NAME` attribute default to using the PSRB name if available to be consistent with `psrcat`. See [#122](https://github.com/mattpitkin/psrqpy/pull/122).
+- Fix parsing of the glitch catalogue table. See [#121](https://github.com/mattpitkin/psrqpy/pull/121).
+
 ## [1.2.5] 2023-01-16
 
 - Update `get_gc_catalogue` for parsing the [Globular Cluster pulsar catalogue](https://www.naic.edu/~pfreire/GCpsr.txt) to allow the "Offset" value to have an associated error value.
 
 ## [1.2.4] 2022-11-22
 
 - Allow references to be extracted for a given ATNF catalogue version. See [#115](https://github.com/mattpitkin/psrqpy/pull/115).
```

### Comparing `psrqpy-1.2.5/docs/source/conf.py` & `psrqpy-1.2.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/docs/source/images/PvsPdot.ipynb` & `psrqpy-1.2.6/docs/source/images/PvsPdot.ipynb`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/docs/source/images/ppdot.png` & `psrqpy-1.2.6/docs/source/images/ppdot.png`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/docs/source/index.rst` & `psrqpy-1.2.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/paper/Makefile` & `psrqpy-1.2.6/paper/Makefile`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/paper/paper.bib` & `psrqpy-1.2.6/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/paper/paper.md` & `psrqpy-1.2.6/paper/paper.md`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/paper/paper.tex` & `psrqpy-1.2.6/paper/paper.tex`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/paper/ppdot.png` & `psrqpy-1.2.6/paper/ppdot.png`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/psrqpy/__init__.py` & `psrqpy-1.2.6/psrqpy/__init__.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/psrqpy/config.py` & `psrqpy-1.2.6/psrqpy/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 URLs used for queries.
 """
 
 import itertools
 
 
 #: The ATNF pulsar catalogue base URL.
-ATNF_BASE_URL = r"http://www.atnf.csiro.au/people/pulsar/psrcat/"
+ATNF_BASE_URL = r"https://www.atnf.csiro.au/people/pulsar/psrcat/"
 
 #: The name of the tarball containing the entire catalogue database.
 ATNF_TARBALL = ATNF_BASE_URL + r"downloads/psrcat_pkg.tar.gz"
 
 # The name of the tarball containing the entire catalogue database (allowing version string to
 # be added).
 ATNF_VERSION_TARBALL = ATNF_BASE_URL + r"downloads/psrcat_pkg.v{}.tar.gz"
 
 #: The Jodrell Bank glitch catalogue table URL.
-GLITCH_URL = r"http://www.jb.man.ac.uk/pulsar/glitches/gTable.html"
+GLITCH_URL = r"https://www.jb.man.ac.uk/pulsar/glitches/gTable.html"
 
 #: Paolo Freire's globular cluster pulsar table URL
-GC_URL = r"http://www.naic.edu/~pfreire/GCpsr.txt"
+GC_URL = r"https://www.naic.edu/~pfreire/GCpsr.txt"
 
 #: Dunc Lorimer's MSP table URL
 MSP_URL = r"http://astro.phys.wvu.edu/GalacticMSPs/GalacticMSPs.txt"
 
 # Pulsar parameters (http://www.atnf.csiro.au/research/pulsar/psrcat/psrcat_help.html) that can be
 # queried. For each parameter there is a dictionary giving:
 #  - 'ref': True if the parameter can have an associated reference in the ATNF catalogue
```

### Comparing `psrqpy-1.2.5/psrqpy/pulsar.py` & `psrqpy-1.2.6/psrqpy/pulsar.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/psrqpy/search.py` & `psrqpy-1.2.6/psrqpy/search.py`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/psrqpy/tests/derived_catalogue.db` & `psrqpy-1.2.6/psrqpy/tests/derived_catalogue.db`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/psrqpy/tests/query_test.py` & `psrqpy-1.2.6/psrqpy/tests/query_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -999,7 +999,18 @@
 
     sort_key = 1.2  # non-string sort key
     with pytest.raises(ValueError):
         query.sort_key = sort_key
 
     # reset sort key
     query.sort_key = curkey
+
+def test_name(query):
+    """
+    Test that the PSRB name is used as default for NAME if it exists, else use PSRJ.
+    """
+
+    psr = query.get_pulsar("J0034-0721")  # This pulsar has a BName and a JName
+    assert psr["NAME"][0] == psr["BNAME"][0]
+
+    psr = query.get_pulsar("J1906+1854")  # This pulsar only has a JName
+    assert psr["NAME"][0] == psr["JNAME"][0]
```

### Comparing `psrqpy-1.2.5/psrqpy/tests/test_catalogue.db` & `psrqpy-1.2.6/psrqpy/tests/test_catalogue.db`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/psrqpy/utils.py` & `psrqpy-1.2.6/psrqpy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,28 +195,31 @@
     del psrlist[-1]  # Final breakstring comes at the end of the file
 
     # add RA and DEC in degs and JNAME/BNAME
     for i, psr in enumerate(list(psrlist)):
         # add 'JNAME', 'BNAME' and 'NAME'
         if "PSRJ" in psr.keys():
             psrlist[i]["JNAME"] = psr["PSRJ"]
-            psrlist[i]["NAME"] = psr["PSRJ"]
             if "PSRJ_REF" in psr.keys():
                 psrlist[i]["JNAME_REF"] = psr["PSRJ_REF"]
-                psrlist[i]["NAME_REF"] = psr["PSRJ_REF"]
 
         if "PSRB" in psr.keys():
             psrlist[i]["BNAME"] = psr["PSRB"]
             if "PSRB_REF" in psr.keys():
                 psrlist[i]["BNAME_REF"] = psr["PSRB_REF"]
 
-            if "NAME" not in psrlist[i].keys():
-                psrlist[i]["NAME"] = psr["PSRB"]
-                if "PSRB_REF" in psr.keys():
-                    psrlist[i]["NAME_REF"] = psr["PSRB_REF"]
+        if "PSRB" in psr.keys() and "PSRJ" in psr.keys():
+            psrlist[i]["NAME"] = psr["PSRB"]
+            if "PSRB_REF" in psr.keys():
+                psrlist[i]["NAME_REF"] = psr["PSRB_REF"]
+
+        else:
+            psrlist[i]["NAME"] = psr["PSRJ"]
+            if "PSRJ_REF" in psr.keys():
+                psrlist[i]["NAME_REF"] = psr["PSRJ_REF"]
 
         if "RAJ" in psr.keys() and "DECJ" in psr.keys():
             # check if the string can be converted to a float (there are a few
             # cases where the position is just a decimal value)
             try:
                 rad = float(psr["RAJ"])
                 ras = Angle(rad * aunits.hourangle)
@@ -500,15 +503,15 @@
                     "DeltaF/F_ERR",
                     "DeltaF1/F1",
                     "DeltaF1/F1_ERR",
                 ]
             ):
                 try:
                     val = float(tds[4 + j].contents[0].string)
-                except ValueError:
+                except (ValueError, TypeError):
                     val = np.nan
 
                 tabledict[pname].append(val)
 
             # get reference link if present
             try:
                 ref = tds[10].contents[0].a.attrs["href"]
```

### Comparing `psrqpy-1.2.5/psrqpy.egg-info/PKG-INFO` & `psrqpy-1.2.6/psrqpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrqpy
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python module for querying the ATNF pulsar catalogue
 Home-page: https://github.com/mattpitkin/psrqpy
 Author: Matthew Pitkin
 Author-email: matthew.pitkin@ligo.org
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -168,15 +168,15 @@
 from psrqpy import QueryATNF
 query = QueryATNF(params=['P0', 'P1', 'ASSOC', 'BINARY', 'TYPE', 'P1_I'])
 query.ppdot(showSNRs=True, showtypes='all')
 ```
 
 gives
 
-![PPdot](../master/docs/source/images/ppdot.png)
+![PPdot](../main/docs/source/images/ppdot.png)
 
 ## Development and Support
 
 Code development is done via the package's [GitHib repository](https://github.com/mattpitkin/psrqpy).
 Any contributions can be made via a [fork and pull request](https://help.github.com/articles/creating-a-pull-request-from-a-fork/) model
 from that repository, and must adhere to the [MIT license](#License). Any problems with the code
 or support requests can be submitted via the repository's [Issue tracker](https://github.com/mattpitkin/psrqpy/issues).
```

### Comparing `psrqpy-1.2.5/psrqpy.egg-info/SOURCES.txt` & `psrqpy-1.2.6/psrqpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psrqpy-1.2.5/setup.cfg` & `psrqpy-1.2.6/setup.cfg`

 * *Files identical despite different names*

