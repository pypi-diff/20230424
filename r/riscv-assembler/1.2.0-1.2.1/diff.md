# Comparing `tmp/riscv-assembler-1.2.0.tar.gz` & `tmp/riscv-assembler-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riscv-assembler-1.2.0.tar", last modified: Wed Apr 12 05:51:07 2023, max compression
+gzip compressed data, was "riscv-assembler-1.2.1.tar", last modified: Mon Apr 24 20:47:57 2023, max compression
```

## Comparing `riscv-assembler-1.2.0.tar` & `riscv-assembler-1.2.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1610 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/references/
--rw-r--r--   0 runner    (1001) docker     (123)   289093 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/references/mdimg.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/riscv_assembler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/riscv_assembler/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/data/instr_data.dat
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/data/reg_map.dat
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/instr_arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/src/riscv_assembler/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 05:51:07.000000 riscv-assembler-1.2.0/src/riscv_assembler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.139420 riscv-assembler-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/tests/assembly/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:07.143420 riscv-assembler-1.2.0/tests/assembly/prjtest1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/argmax.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/classify.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/dot.s
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/main.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/matmul.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     3421 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/read_matrix.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/relu.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/utils.s
--rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/prjtest1/write_matrix.s
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test0.s
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test1.s
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test2.s
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test3.s
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test4.s
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test5.s
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test6.s
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/assembly/test7.s
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-12 05:50:59.000000 riscv-assembler-1.2.0/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.874914 riscv-assembler-1.2.1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.874914 riscv-assembler-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.874914 riscv-assembler-1.2.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1610 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.874914 riscv-assembler-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.874914 riscv-assembler-1.2.1/references/
+-rw-r--r--   0 runner    (1001) docker     (123)   289093 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/references/mdimg.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.874914 riscv-assembler-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.874914 riscv-assembler-1.2.1/src/riscv_assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/src/riscv_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/src/riscv_assembler/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/src/riscv_assembler/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/src/riscv_assembler/data/instr_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/src/riscv_assembler/data/reg_map.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/src/riscv_assembler/instr_arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/src/riscv_assembler/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/src/riscv_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-24 20:47:57.000000 riscv-assembler-1.2.1/src/riscv_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-24 20:47:57.000000 riscv-assembler-1.2.1/src/riscv_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:47:57.000000 riscv-assembler-1.2.1/src/riscv_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 20:47:57.000000 riscv-assembler-1.2.1/src/riscv_assembler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 20:47:57.000000 riscv-assembler-1.2.1/src/riscv_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 20:47:57.000000 riscv-assembler-1.2.1/src/riscv_assembler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/tests/assembly/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:47:57.878914 riscv-assembler-1.2.1/tests/assembly/prjtest1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/argmax.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/classify.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/dot.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/main.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/matmul.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3421 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/read_matrix.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/relu.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/utils.s
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/prjtest1/write_matrix.s
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test0.s
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test1.s
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test2.s
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test3.s
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test4.s
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test5.s
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test6.s
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test7.s
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/assembly/test8.s
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-24 20:47:50.000000 riscv-assembler-1.2.1/tests/test_class.py
```

### Comparing `riscv-assembler-1.2.0/.circleci/config.yml` & `riscv-assembler-1.2.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/.github/scripts/release.py` & `riscv-assembler-1.2.1/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/LICENSE` & `riscv-assembler-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/PKG-INFO` & `riscv-assembler-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: riscv-assembler
-Version: 1.2.0
+Version: 1.2.1
 Summary: RISC-V Assembly code assembler package for Python.
-Home-page: https://github.com/kcelebi/riscv-assembler
+Home-page: https://github.com/celebi-pkg/riscv-assembler
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
-Project-URL: Bug Tracker, https://github.com/kcelebi/riscv-assembler/issues
-Project-URL: Changelog, https://github.com/kcelebi/riscv-assembler/releases
+Project-URL: Bug Tracker, https://github.com/celebi-pkg/riscv-assembler/issues
+Project-URL: Changelog, https://github.com/celebi-pkg/riscv-assembler/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `riscv-assembler-1.2.0/README.md` & `riscv-assembler-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/references/mdimg.png` & `riscv-assembler-1.2.1/references/mdimg.png`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/setup.cfg` & `riscv-assembler-1.2.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = riscv-assembler
 author = Kaya Celebi
 author_email = kayacelebi17@gmail.com
 description = RISC-V Assembly code assembler package for Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/kcelebi/riscv-assembler
+url = https://github.com/celebi-pkg/riscv-assembler
 project_urls = 
-	Bug Tracker = https://github.com/kcelebi/riscv-assembler/issues
-	Changelog = https://github.com/kcelebi/riscv-assembler/releases
+	Bug Tracker = https://github.com/celebi-pkg/riscv-assembler/issues
+	Changelog = https://github.com/celebi-pkg/riscv-assembler/releases
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Developers
 
 [options]
 package_dir =
```

### Comparing `riscv-assembler-1.2.0/src/riscv_assembler/convert.py` & `riscv-assembler-1.2.1/src/riscv_assembler/convert.py`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/src/riscv_assembler/data/instr_data.dat` & `riscv-assembler-1.2.1/src/riscv_assembler/data/instr_data.dat`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/src/riscv_assembler/instr_arr.py` & `riscv-assembler-1.2.1/src/riscv_assembler/instr_arr.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,16 +180,16 @@
 		return self.organize(*args)
 
 	@staticmethod
 	def JUMP(tk : str, line_num : int, code: list) -> int:
 		try:
 			index, skip_labels = code.index(tk + ":"), 0
 		except:
-			raise Exception('''Address not found! Provided assembly code could
-				 be faulty, branch is expressed but not found in code.''')
+			raise Exception('''Address not found for {}! Provided assembly code could 
+				be faulty, branch is expressed but not found in code.'''.format(tk))
 
 		pos = 1
 		if index > line_num: # forward search:
 			skip_labels = sum([1 for i in range(line_num, index) if code[i][-1] == ":"])
 		else: # backwards search
 			skip_labels = -1 * sum([1 for i in range(index, line_num) if code[i][-1] == ":"])
 
@@ -294,28 +294,35 @@
 
 	def __str__(self):
 		return "Pseudo Parser"
 
 	def organize(self, tokens):
 		# better way to organize, express, abstract pseudo?
 		instr = tokens[0]
+		line_num, code = tokens[-2], tokens[-1]
 		if instr == 'nop':
 			rs1, imm, rd = reg_map["x0"], 0, reg_map["x0"]
 			return I("addi", rs1, imm, rd)
 		elif instr == "mv":
 			rs1, imm, rd = reg_map[tokens[2]], 0, reg_map[tokens[1]]
 			return I("addi", rs1, imm, rd)
 		elif instr == "not":
 			rs1, imm, rd = reg_map[tokens[2]], -1, reg_map[tokens[1]]
 			return I("xori", rs1, imm, rd)
 		elif instr == "neg":
 			rs1, rs2, rd = reg_map["x0"], reg_map[tokens[2]], reg_map[tokens[1]]
 			return R("sub", rs1, rs2, rd)
+		elif instr == "j":
+			return UJ("jal", super().JUMP(tokens[1], line_num, code), "x0")
+		elif instr == "li":
+			# This is missing addi rd rd -273
+			return U("lui", tokens[2], reg_map[tokens[1]])
+			# I("addi", reg_map[tokens[1]], reg_map[tokens[1]], tokens[2])
 
-		raise Exception("Bad Instruction provided, this does not exist or has not been implemented here yet.")
+		raise Exception("Bad Instruction provided, {} does not exist or has not been implemented here yet.".format(instr))
 
 
 def register_map():
 	path = Path(__file__).parent / "data/reg_map.dat"
 	rmap = {}
 
 	f = open(path, "r")
```

### Comparing `riscv-assembler-1.2.0/src/riscv_assembler/parse.py` & `riscv-assembler-1.2.1/src/riscv_assembler/parse.py`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/src/riscv_assembler.egg-info/PKG-INFO` & `riscv-assembler-1.2.1/src/riscv_assembler.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: riscv-assembler
-Version: 1.2.0
+Version: 1.2.1
 Summary: RISC-V Assembly code assembler package for Python.
-Home-page: https://github.com/kcelebi/riscv-assembler
+Home-page: https://github.com/celebi-pkg/riscv-assembler
 Author: Kaya Celebi
 Author-email: kayacelebi17@gmail.com
-Project-URL: Bug Tracker, https://github.com/kcelebi/riscv-assembler/issues
-Project-URL: Changelog, https://github.com/kcelebi/riscv-assembler/releases
+Project-URL: Bug Tracker, https://github.com/celebi-pkg/riscv-assembler/issues
+Project-URL: Changelog, https://github.com/celebi-pkg/riscv-assembler/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `riscv-assembler-1.2.0/src/riscv_assembler.egg-info/SOURCES.txt` & `riscv-assembler-1.2.1/src/riscv_assembler.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 tests/assembly/test1.s
 tests/assembly/test2.s
 tests/assembly/test3.s
 tests/assembly/test4.s
 tests/assembly/test5.s
 tests/assembly/test6.s
 tests/assembly/test7.s
+tests/assembly/test8.s
 tests/assembly/prjtest1/argmax.s
 tests/assembly/prjtest1/classify.s
 tests/assembly/prjtest1/dot.s
 tests/assembly/prjtest1/main.s
 tests/assembly/prjtest1/matmul.s
 tests/assembly/prjtest1/read_matrix.s
 tests/assembly/prjtest1/relu.s
```

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/argmax.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/argmax.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/classify.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/classify.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/dot.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/dot.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/matmul.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/matmul.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/read_matrix.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/read_matrix.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/relu.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/relu.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/utils.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/utils.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/assembly/prjtest1/write_matrix.s` & `riscv-assembler-1.2.1/tests/assembly/prjtest1/write_matrix.s`

 * *Files identical despite different names*

### Comparing `riscv-assembler-1.2.0/tests/test_class.py` & `riscv-assembler-1.2.1/tests/test_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from pathlib import Path
 from os.path import exists
 from riscv_assembler.convert import AssemblyConverter as AC
 from riscv_assembler.instr_arr import *
 from riscv_assembler.parse import Parser
 
-num_test_files = 8
+num_test_files = 9
 num_questions = 15
 
 def SUITE():
 	# 0. convert directly from file to array
 	# 1. convert directly from file to print (return nothing)
 	# 2. convert directly from file to txt file
 	# 3. convert directly from file to bin file
@@ -81,23 +81,26 @@
 		cnv(code, dump_path + '/arr{}.bin'.format(i))
 		results[13] += ['arr{}.bin'.format(i)] #**
 		results[14] += [cnv.output_mode]
 
 
 	return results
 
+ans = ['0xfe810113','0x00812023','0x00912223','0x01212423','0x01312623','0x01412823','0x01512a23','0x00100f13','0x01e64863','0x01e6ca63','0x01e74863','0x0140006f','0x00500593','0xfcdff06f','0x00600593','0xfc5ff06f','0x00000413','0x00000293','0x00000313','0x00000393','0x00400e13','0x03c68a33','0x03c70ab3','0x0040006f','0x02c28263','0x00052483','0x0005a903','0x01450533','0x015585b3','0x032489b3','0x01340433','0x00128293','0xfe1ff06f','0x00040513','0x00012403','0x00412483','0x00812903','0x00c12983','0x01012a03','0x01412a83','0x01810113']
 ANSWERS = {
 	0: [['0x000000b3'], None, 'file0.txt', 'file0.bin', ['0x000000b3'], None, 'str0.txt', 'str0.bin', ['0x000000b3'], 'a', None, 'p', 'arr0.txt', 'arr0.bin', 'f'],
 	1: [['0x02040293'], None, 'file1.txt', 'file1.bin',['0x02040293'], None, 'str1.txt', 'str1.bin',['0x02040293'], 'a', None, 'p', 'arr1.txt', 'arr1.bin', 'f'],
 	2: [['0x00a00413', '0x00a00493', '0x00848263', '0xfe040493'], None, 'file2.txt', 'file2.bin', ['0x00a00413', '0x00a00493', '0x00848263', '0xfe040493'], None, 'str2.txt', 'str2.bin', ['0x00a00413', '0x00a00493', '0x00848263', '0xfe040493'], 'a', None, 'p', 'arr2.txt', 'arr2.bin', 'f'],
 	3: [['0x00812023'], None, 'file3.txt', 'file3.bin', ['0x00812023'], None, 'str3.txt', 'str3.bin', ['0x00812023'], 'a', None, 'p', 'arr3.txt', 'arr3.bin', 'f'],
 	4: [['0x000000b3', '0x02040293', '0x02040293','0x00812023'], None, 'file4.txt', 'file4.bin',['0x000000b3', '0x02040293', '0x02040293','0x00812023'], None, 'str4.txt', 'str4.bin',['0x000000b3', '0x02040293', '0x02040293','0x00812023'], 'a', None, 'p', 'arr4.txt', 'arr4.bin', 'f'],
 	5: [['0x00a00413','0x00a00493','0xfff00493','0x00048463','0xfe000ce3','0xfe040493'], None, 'file5.txt', 'file5.bin', ['0x00a00413','0x00a00493','0xfff00493','0x00048463','0xfe000ce3','0xfe040493'], None, 'str5.txt', 'str5.bin', ['0x00a00413','0x00a00493','0xfff00493','0x00048463','0xfe000ce3','0xfe040493'], 'a', None, 'p', 'arr5.txt', 'arr5.bin', 'f'],
 	6: [['0x00a00093','0xfec00113','0x00000663','0x00123023','0x00023083','0xfff00093','0x00123023','0x00023083','0xfe02c6e3'], None, 'file6.txt', 'file6.bin', ['0x00a00093','0xfec00113','0x00000663','0x00123023','0x00023083','0xfff00093','0x00123023','0x00023083','0xfe02c6e3'], None, 'str6.txt', 'str6.bin', ['0x00a00093','0xfec00113','0x00000663','0x00123023','0x00023083','0xfff00093','0x00123023','0x00023083','0xfe02c6e3'], 'a', None, 'p', 'arr6.txt', 'arr6.bin', 'f'],
-	7: [['0x00318233','0x002080b3','0x00708093','0x00123023','0x00023083'], None, 'file7.txt', 'file7.bin', ['0x00318233','0x002080b3','0x00708093','0x00123023','0x00023083'], None, 'str7.txt', 'str7.bin', ['0x00318233','0x002080b3','0x00708093','0x00123023','0x00023083'], 'a', None, 'p', 'arr7.txt', 'arr7.bin', 'f']}
+	7: [['0x00318233','0x002080b3','0x00708093','0x00123023','0x00023083'], None, 'file7.txt', 'file7.bin', ['0x00318233','0x002080b3','0x00708093','0x00123023','0x00023083'], None, 'str7.txt', 'str7.bin', ['0x00318233','0x002080b3','0x00708093','0x00123023','0x00023083'], 'a', None, 'p', 'arr7.txt', 'arr7.bin', 'f'],
+	8: [ans, None, 'file8.txt', 'file8.bin', ans, None, 'str8.txt', 'str8.bin', ans, 'a', None, 'p', 'arr8.txt', 'arr8.bin', 'f']}
+
 RESULTS = SUITE()
 
 def error_label(q, test):
 	return "Question {q} Failed for Test {test}".format(q = q, test = test)
 
 test_data = []
 for q in range(num_questions):
```

