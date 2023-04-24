# Comparing `tmp/lambda_repl-1.1.0.tar.gz` & `tmp/lambda_repl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_repl-1.1.0.tar", last modified: Sun Sep 11 18:23:30 2022, max compression
+gzip compressed data, was "lambda_repl-1.2.0.tar", last modified: Mon Apr 24 17:23:26 2023, max compression
```

## Comparing `lambda_repl-1.1.0.tar` & `lambda_repl-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 18:23:30.721201 lambda_repl-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-09-11 18:23:30.721201 lambda_repl-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 18:23:30.717201 lambda_repl-1.1.0/lambda_repl/
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/lambda_repl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/lambda_repl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/lambda_repl/aliases.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/lambda_repl/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/lambda_repl/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/lambda_repl/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/lambda_repl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-11 18:23:30.721201 lambda_repl-1.1.0/lambda_repl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-09-11 18:23:30.000000 lambda_repl-1.1.0/lambda_repl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-11 18:23:30.000000 lambda_repl-1.1.0/lambda_repl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-11 18:23:30.000000 lambda_repl-1.1.0/lambda_repl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-11 18:23:30.000000 lambda_repl-1.1.0/lambda_repl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-11 18:23:30.000000 lambda_repl-1.1.0/lambda_repl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-11 18:23:30.000000 lambda_repl-1.1.0/lambda_repl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-09-11 18:23:13.000000 lambda_repl-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-11 18:23:30.721201 lambda_repl-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:23:26.560632 lambda_repl-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 17:23:26.560632 lambda_repl-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:23:26.556632 lambda_repl-1.2.0/lambda_repl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/lambda_repl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/lambda_repl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/lambda_repl/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/lambda_repl/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/lambda_repl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/lambda_repl/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/lambda_repl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:23:26.556632 lambda_repl-1.2.0/lambda_repl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 17:23:26.000000 lambda_repl-1.2.0/lambda_repl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-24 17:23:26.000000 lambda_repl-1.2.0/lambda_repl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:23:26.000000 lambda_repl-1.2.0/lambda_repl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 17:23:26.000000 lambda_repl-1.2.0/lambda_repl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 17:23:26.000000 lambda_repl-1.2.0/lambda_repl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 17:23:26.000000 lambda_repl-1.2.0/lambda_repl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:23:26.560632 lambda_repl-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:23:26.556632 lambda_repl-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/tests/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-24 17:23:15.000000 lambda_repl-1.2.0/tests/test_repl.py
```

### Comparing `lambda_repl-1.1.0/LICENSE` & `lambda_repl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda_repl-1.1.0/PKG-INFO` & `lambda_repl-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda_repl
-Version: 1.1.0
+Version: 1.2.0
 Summary: REPL for the lambda calculus
 Author-email: Eric Niklas Wolf <eric_niklas.wolf@mailbox.tu-dresden.de>
 Project-URL: Repository, https://github.com/Deric-W/lambda_repl
 Project-URL: Bugtracker, https://github.com/Deric-W/lambda_repl/issues
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,37 +17,41 @@
 License-File: LICENSE
 
 # lambda_repl
 
 ![Tests](https://github.com/Deric-W/lambda_repl/actions/workflows/Tests.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/Deric-W/lambda_repl/branch/main/graph/badge.svg?token=SU3982mC17)](https://codecov.io/gh/Deric-W/lambda_repl)
 
-The `lambda_repl` package contains a [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop) for the [lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus).
+The `lambda_repl` package contains a [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop)
+for the [lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus).
 
 To use it, execute `lambda-repl` or `python3 -m lambda_repl` and enter commands.
 
 ## Requirements
 
-Python >= 3.10 and the `lambda_calculus` package are required to use this package.
+Python >= 3.10 and the packages [`lambda_calculus`](https://github.com/Deric-W/lambda_calculus)
+and [`lark`](https://github.com/lark-parser/lark) are required to use this package.
 
 ## Installation
 
 ```sh
 python3 -m pip install lambda-repl
 ```
 
 ## Examples
 
 ```
 python3 -m lambda_repl
 Welcome to the the Lambda REPL, type 'help' for help
 λ alias I = \x.x
 λ alias K = λx.λy.x
+λ import SUCC = lambda_calculus.terms.arithmetic.SUCCESSOR
 λ aliases
 I = (λx.x)
 K = (λx.(λy.x))
+SUCC = (λn.(λf.(λx.(f ((n f) x)))))
 λ trace K a b
 β ((λy.a) b)
 β a
 λ exit
 Exiting REPL...
 ```
```

### Comparing `lambda_repl-1.1.0/lambda_repl/aliases.py` & `lambda_repl-1.2.0/lambda_repl/aliases.py`

 * *Files identical despite different names*

### Comparing `lambda_repl-1.1.0/lambda_repl/main.py` & `lambda_repl-1.2.0/lambda_repl/main.py`

 * *Files identical despite different names*

### Comparing `lambda_repl-1.1.0/lambda_repl/parsing.py` & `lambda_repl-1.2.0/lambda_repl/parsing.py`

 * *Files identical despite different names*

### Comparing `lambda_repl-1.1.0/lambda_repl.egg-info/PKG-INFO` & `lambda_repl-1.2.0/lambda_repl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-repl
-Version: 1.1.0
+Version: 1.2.0
 Summary: REPL for the lambda calculus
 Author-email: Eric Niklas Wolf <eric_niklas.wolf@mailbox.tu-dresden.de>
 Project-URL: Repository, https://github.com/Deric-W/lambda_repl
 Project-URL: Bugtracker, https://github.com/Deric-W/lambda_repl/issues
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,37 +17,41 @@
 License-File: LICENSE
 
 # lambda_repl
 
 ![Tests](https://github.com/Deric-W/lambda_repl/actions/workflows/Tests.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/Deric-W/lambda_repl/branch/main/graph/badge.svg?token=SU3982mC17)](https://codecov.io/gh/Deric-W/lambda_repl)
 
-The `lambda_repl` package contains a [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop) for the [lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus).
+The `lambda_repl` package contains a [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop)
+for the [lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus).
 
 To use it, execute `lambda-repl` or `python3 -m lambda_repl` and enter commands.
 
 ## Requirements
 
-Python >= 3.10 and the `lambda_calculus` package are required to use this package.
+Python >= 3.10 and the packages [`lambda_calculus`](https://github.com/Deric-W/lambda_calculus)
+and [`lark`](https://github.com/lark-parser/lark) are required to use this package.
 
 ## Installation
 
 ```sh
 python3 -m pip install lambda-repl
 ```
 
 ## Examples
 
 ```
 python3 -m lambda_repl
 Welcome to the the Lambda REPL, type 'help' for help
 λ alias I = \x.x
 λ alias K = λx.λy.x
+λ import SUCC = lambda_calculus.terms.arithmetic.SUCCESSOR
 λ aliases
 I = (λx.x)
 K = (λx.(λy.x))
+SUCC = (λn.(λf.(λx.(f ((n f) x)))))
 λ trace K a b
 β ((λy.a) b)
 β a
 λ exit
 Exiting REPL...
 ```
```

### Comparing `lambda_repl-1.1.0/pyproject.toml` & `lambda_repl-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lambda_repl"
-version = "1.1.0"
+version = "1.2.0"
 description = "REPL for the lambda calculus"
 requires-python = ">=3.10"
 keywords = []
 classifiers = [
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

