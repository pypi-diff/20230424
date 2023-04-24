# Comparing `tmp/chardetng_py-0.1.0.tar.gz` & `tmp/chardetng_py-0.1.1.tar.gz`

## Comparing `chardetng_py-0.1.0.tar` & `chardetng_py-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 chardetng_py-0.1.0/Cargo.toml
--rw-rw-r--   0     1000     1000     2809 2023-04-23 03:38:01.000000 chardetng_py-0.1.0/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      685 2023-04-23 03:38:01.000000 chardetng_py-0.1.0/.gitignore
--rw-rw-r--   0     1000     1000     2095 2023-04-24 19:15:16.000000 chardetng_py-0.1.0/bench/bench.py
--rw-rw-r--   0     1000     1000     2395 2023-04-24 19:15:08.000000 chardetng_py-0.1.0/bench/compare.py
--rw-rw-r--   0     1000     1000      374 2023-04-24 18:10:51.000000 chardetng_py-0.1.0/pyproject.toml
--rw-rw-r--   0     1000     1000      615 2023-04-24 18:09:44.000000 chardetng_py-0.1.0/src/lib.rs
--rw-rw-r--   0     1000     1000     8353 2023-04-24 18:11:28.000000 chardetng_py-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 chardetng_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 chardetng_py-0.1.1/Cargo.toml
+-rw-rw-r--   0     1000     1000     2809 2023-04-23 03:38:01.000000 chardetng_py-0.1.1/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      685 2023-04-23 03:38:01.000000 chardetng_py-0.1.1/.gitignore
+-rw-rw-r--   0     1000     1000      849 2023-04-24 19:34:57.000000 chardetng_py-0.1.1/README.md
+-rw-rw-r--   0     1000     1000     2095 2023-04-24 19:15:16.000000 chardetng_py-0.1.1/bench/bench.py
+-rw-rw-r--   0     1000     1000     2395 2023-04-24 19:15:08.000000 chardetng_py-0.1.1/bench/compare.py
+-rw-rw-r--   0     1000     1000      510 2023-04-24 19:36:17.000000 chardetng_py-0.1.1/pyproject.toml
+-rw-rw-r--   0     1000     1000      615 2023-04-24 18:09:44.000000 chardetng_py-0.1.1/src/lib.rs
+-rw-rw-r--   0     1000     1000     8353 2023-04-24 19:37:10.000000 chardetng_py-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 chardetng_py-0.1.1/PKG-INFO
```

### Comparing `chardetng_py-0.1.0/.github/workflows/CI.yml` & `chardetng_py-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `chardetng_py-0.1.0/.gitignore` & `chardetng_py-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `chardetng_py-0.1.0/bench/bench.py` & `chardetng_py-0.1.1/bench/bench.py`

 * *Files identical despite different names*

### Comparing `chardetng_py-0.1.0/bench/compare.py` & `chardetng_py-0.1.1/bench/compare.py`

 * *Files identical despite different names*

### Comparing `chardetng_py-0.1.0/src/lib.rs` & `chardetng_py-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chardetng_py-0.1.0/Cargo.lock` & `chardetng_py-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  "cfg-if",
  "encoding_rs",
  "memchr",
 ]
 
 [[package]]
 name = "chardetng_py"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "chardetng",
  "encoding_rs",
  "pyo3",
 ]
 
 [[package]]
```

