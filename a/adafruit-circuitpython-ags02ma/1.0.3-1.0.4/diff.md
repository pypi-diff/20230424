# Comparing `tmp/adafruit-circuitpython-ags02ma-1.0.3.tar.gz` & `tmp/adafruit-circuitpython-ags02ma-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ags02ma-1.0.3.tar", last modified: Thu Aug 25 19:30:41 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ags02ma-1.0.4.tar", last modified: Mon Apr 24 14:44:38 2023, max compression
```

## Comparing `adafruit-circuitpython-ags02ma-1.0.3.tar` & `adafruit-circuitpython-ags02ma-1.0.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.384304 adafruit-circuitpython-ags02ma-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.380303 adafruit-circuitpython-ags02ma-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.380303 adafruit-circuitpython-ags02ma-1.0.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.380303 adafruit-circuitpython-ags02ma-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.380303 adafruit-circuitpython-ags02ma-1.0.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-08-25 19:30:41.384304 adafruit-circuitpython-ags02ma-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-08-25 19:30:33.000000 adafruit-circuitpython-ags02ma-1.0.3/adafruit_ags02ma.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.384304 adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-08-25 19:30:41.000000 adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-25 19:30:41.000000 adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 19:30:41.000000 adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-25 19:30:41.000000 adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-25 19:30:41.000000 adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.384304 adafruit-circuitpython-ags02ma-1.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.384304 adafruit-circuitpython-ags02ma-1.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5979 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:30:41.384304 adafruit-circuitpython-ags02ma-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-08-25 19:30:33.000000 adafruit-circuitpython-ags02ma-1.0.3/examples/ags02ma_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-08-25 19:30:33.000000 adafruit-circuitpython-ags02ma-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-08-25 19:30:26.000000 adafruit-circuitpython-ags02ma-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-25 19:30:41.384304 adafruit-circuitpython-ags02ma-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.604179 adafruit-circuitpython-ags02ma-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-24 14:44:29.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_ags02ma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 14:44:29.000000 adafruit-circuitpython-ags02ma-1.0.4/examples/ags02ma_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-24 14:44:29.000000 adafruit-circuitpython-ags02ma-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/setup.cfg
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ags02ma-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/.gitignore` & `adafruit-circuitpython-ags02ma-1.0.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/.pre-commit-config.yaml` & `adafruit-circuitpython-ags02ma-1.0.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/.pylintrc` & `adafruit-circuitpython-ags02ma-1.0.4/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ags02ma-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/LICENSE` & `adafruit-circuitpython-ags02ma-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ags02ma-1.0.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/LICENSES/MIT.txt` & `adafruit-circuitpython-ags02ma-1.0.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ags02ma-1.0.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/PKG-INFO` & `adafruit-circuitpython-ags02ma-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ags02ma
-Version: 1.0.3
+Version: 1.0.4
 Summary: CircuitPython / Python library for AGS02MA gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AGS02MA
 Keywords: adafruit,blinka,circuitpython,micropython,ags02ma,tvoc,gas,resistance,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/README.rst` & `adafruit-circuitpython-ags02ma-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO` & `adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ags02ma
-Version: 1.0.3
+Version: 1.0.4
 Summary: CircuitPython / Python library for AGS02MA gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AGS02MA
 Keywords: adafruit,blinka,circuitpython,micropython,ags02ma,tvoc,gas,resistance,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt` & `adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_ags02ma.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ags02ma.egg-info/PKG-INFO
 adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt
 adafruit_circuitpython_ags02ma.egg-info/dependency_links.txt
 adafruit_circuitpython_ags02ma.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/docs/_static/favicon.ico` & `adafruit-circuitpython-ags02ma-1.0.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/docs/conf.py` & `adafruit-circuitpython-ags02ma-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/docs/index.rst` & `adafruit-circuitpython-ags02ma-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/examples/ags02ma_simpletest.py` & `adafruit-circuitpython-ags02ma-1.0.4/examples/ags02ma_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.3/pyproject.toml` & `adafruit-circuitpython-ags02ma-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ags02ma"
 description = "CircuitPython / Python library for AGS02MA gas sensor"
-version = "1.0.3"
+version = "1.0.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AGS02MA"}
 keywords = [
     "adafruit",
```

