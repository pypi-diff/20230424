# Comparing `tmp/quadcube-0.1.0.tar.gz` & `tmp/quadcube-1.0.0.tar.gz`

## Comparing `quadcube-0.1.0.tar` & `quadcube-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 quadcube-0.1.0/Cargo.toml
--rw-r--r--   0      503       20     2785 2023-03-28 11:21:52.000000 quadcube-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      503       20      685 2023-03-28 11:21:52.000000 quadcube-0.1.0/.gitignore
--rw-r--r--   0      503       20      472 2023-03-29 13:02:00.000000 quadcube-0.1.0/pyproject.toml
--rw-r--r--   0      503       20     7802 2023-03-29 13:20:15.000000 quadcube-0.1.0/src/lib.rs
--rw-r--r--   0      503       20     2211 2023-03-29 13:00:44.000000 quadcube-0.1.0/tests/test_pix2vec.py
--rw-r--r--   0      503       20    16244 2023-03-28 11:24:35.000000 quadcube-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      414 1970-01-01 00:00:00.000000 quadcube-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 quadcube-1.0.0/Cargo.toml
+-rw-rw-r--   0   249026   192705     2785 2023-04-24 07:56:52.000000 quadcube-1.0.0/.github/workflows/CI.yml
+-rw-rw-r--   0   249026   192705      685 2023-04-24 07:56:52.000000 quadcube-1.0.0/.gitignore
+-rw-rw-r--   0   249026   192705    35149 2023-04-24 07:56:52.000000 quadcube-1.0.0/LICENSE
+-rw-rw-r--   0   249026   192705      909 2023-04-24 07:56:52.000000 quadcube-1.0.0/README.md
+-rw-rw-r--   0   249026   192705      472 2023-04-24 07:56:52.000000 quadcube-1.0.0/pyproject.toml
+-rw-rw-r--   0   249026   192705     7802 2023-04-24 08:20:43.000000 quadcube-1.0.0/src/lib.rs
+-rw-rw-r--   0   249026   192705     2211 2023-04-24 07:56:52.000000 quadcube-1.0.0/tests/test_pix2vec.py
+-rw-rw-r--   0   249026   192705    16244 2023-04-24 08:30:06.000000 quadcube-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 quadcube-1.0.0/PKG-INFO
```

### Comparing `quadcube-0.1.0/.github/workflows/CI.yml` & `quadcube-1.0.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `quadcube-0.1.0/.gitignore` & `quadcube-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quadcube-0.1.0/src/lib.rs` & `quadcube-1.0.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
         match n_face {
             0 => [-eta * norm, x_i * norm, norm],
             1 => [norm, x_i * norm, eta * norm],
             2 => [-x_i * norm, norm, eta * norm],
             3 => [-norm, -x_i * norm, eta * norm],
             4 => [x_i * norm, -norm, eta * norm],
-            5 => [eta * norm, -x_i * norm, norm],
+            5 => [eta * norm, x_i * norm, -norm],
             _ => panic!("Invalid face number: {}", n_face),
         }
     }
 
     fn deproject_face(a: f64, b: f64) -> f64 {
         let a_squared = a * a;
         let b_squared = b * b;
```

### Comparing `quadcube-0.1.0/tests/test_pix2vec.py` & `quadcube-1.0.0/tests/test_pix2vec.py`

 * *Files identical despite different names*

### Comparing `quadcube-0.1.0/Cargo.lock` & `quadcube-1.0.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quadcube"
-version = "0.1.0"
+version = "1.0.0"
 dependencies = [
  "cached",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
```

