# Comparing `tmp/dune_harmonizer-0.5.1.tar.gz` & `tmp/dune_harmonizer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_harmonizer-0.5.1.tar", max compression
+gzip compressed data, was "dune_harmonizer-0.6.0.tar", max compression
```

## Comparing `dune_harmonizer-0.5.1.tar` & `dune_harmonizer-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1061 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/LICENSE
--rw-r--r--   0        0        0     2378 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/README.md
--rw-r--r--   0        0        0      440 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/dune/harmonizer/__init__.py
--rw-r--r--   0        0        0      849 2023-04-21 12:10:53.099273 dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19435 2023-04-21 12:10:53.103273 dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
--rw-r--r--   0        0        0      630 2023-04-21 12:10:53.107273 dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     3103 2023-04-21 12:10:53.103273 dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
--rw-r--r--   0        0        0     3544 2023-04-21 12:10:53.103273 dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/dune/harmonizer/constants.py
--rw-r--r--   0        0        0    16901 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/dune/harmonizer/custom_transforms.py
--rw-r--r--   0        0        0     2359 2023-04-21 12:10:53.107273 dune_harmonizer-0.5.1/dune/harmonizer/dialects/__pycache__/dunesql.cpython-311.pyc
--rw-r--r--   0        0        0     1061 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/dune/harmonizer/dialects/dunesql.py
--rw-r--r--   0        0        0      105 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/dune/harmonizer/errors.py
--rw-r--r--   0        0        0     2018 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/dune/harmonizer/table_replacements.py
--rw-r--r--   0        0        0     2916 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/dune/harmonizer/translate.py
--rw-r--r--   0        0        0      570 2023-04-21 12:10:34.067320 dune_harmonizer-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2378 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/README.md
+-rw-r--r--   0        0        0      440 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/__init__.py
+-rw-r--r--   0        0        0      849 2023-04-24 08:27:37.515846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    19435 2023-04-24 08:27:37.519846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
+-rw-r--r--   0        0        0      630 2023-04-24 08:27:37.523846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     3103 2023-04-24 08:27:37.519846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
+-rw-r--r--   0        0        0     3544 2023-04-24 08:27:37.515846 dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/constants.py
+-rw-r--r--   0        0        0    16901 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/custom_transforms.py
+-rw-r--r--   0        0        0     4082 2023-04-24 08:27:37.519846 dune_harmonizer-0.6.0/dune/harmonizer/dialects/__pycache__/dunesql.cpython-311.pyc
+-rw-r--r--   0        0        0     2715 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/dialects/dunesql.py
+-rw-r--r--   0        0        0      105 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-24 08:27:11.287844 dune_harmonizer-0.6.0/dune/harmonizer/table_replacements.py
+-rw-r--r--   0        0        0     2916 2023-04-24 08:27:11.291843 dune_harmonizer-0.6.0/dune/harmonizer/translate.py
+-rw-r--r--   0        0        0      570 2023-04-24 08:27:11.291843 dune_harmonizer-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.6.0/PKG-INFO
```

### Comparing `dune_harmonizer-0.5.1/LICENSE` & `dune_harmonizer-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.5.1/README.md` & `dune_harmonizer-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/__init__.cpython-311.pyc` & `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3a7d4264 (Fri Apr 21 12:10:34 2023 UTC)
+moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
 files sz: 440
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc` & `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3a7d4264 (Fri Apr 21 12:10:34 2023 UTC)
+moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
 files sz: 16901
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/errors.cpython-311.pyc` & `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3a7d4264 (Fri Apr 21 12:10:34 2023 UTC)
+moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
 files sz: 105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc` & `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3a7d4264 (Fri Apr 21 12:10:34 2023 UTC)
+moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
 files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/__pycache__/translate.cpython-311.pyc` & `dune_harmonizer-0.6.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3a7d4264 (Fri Apr 21 12:10:34 2023 UTC)
+moddate:  0x5f3d4664 (Mon Apr 24 08:27:11 2023 UTC)
 files sz: 2916
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/custom_transforms.py` & `dune_harmonizer-0.6.0/dune/harmonizer/custom_transforms.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/table_replacements.py` & `dune_harmonizer-0.6.0/dune/harmonizer/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.5.1/dune/harmonizer/translate.py` & `dune_harmonizer-0.6.0/dune/harmonizer/translate.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.5.1/pyproject.toml` & `dune_harmonizer-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dune-harmonizer"
-version = "0.5.1"
+version = "0.6.0"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dune_harmonizer-0.5.1/PKG-INFO` & `dune_harmonizer-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-harmonizer
-Version: 0.5.1
+Version: 0.6.0
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.5.5,<12.0.0)
```

