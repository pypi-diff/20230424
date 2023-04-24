# Comparing `tmp/nerfacc-0.5.1.tar.gz` & `tmp/nerfacc-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nerfacc/nerfacc/dist/.tmp-xeko1dq4/nerfacc-0.5.1.tar", last modified: Sun Apr  9 10:22:38 2023, max compression
+gzip compressed data, was "/home/runner/work/nerfacc/nerfacc/dist/.tmp-0kkb42ub/nerfacc-0.5.2.tar", last modified: Mon Apr 24 08:00:56 2023, max compression
```

## Comparing `nerfacc-0.5.1.tar` & `nerfacc-0.5.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-09 10:22:20.000000 nerfacc-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-09 10:22:20.000000 nerfacc-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 10:22:38.000000 nerfacc-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-09 10:22:31.000000 nerfacc-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cameras2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/camera.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16208 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/grid.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec_packed.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_camera.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_contraction.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_grid.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    38908 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_math.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_scan.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/nerfacc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/pdf.cu
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/scan.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/data_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/occ_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/prop_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21810 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/volrend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-09 10:22:38.000000 nerfacc-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-09 10:22:20.000000 nerfacc-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-24 08:00:36.000000 nerfacc-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 08:00:36.000000 nerfacc-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 08:00:56.000000 nerfacc-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-24 08:00:48.000000 nerfacc-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cameras2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/camera.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/grid.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/data_spec.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/data_spec_packed.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_camera.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_contraction.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_grid.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    38908 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_math.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_scan.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/nerfacc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/pdf.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/cuda/csrc/scan.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/data_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/occ_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/estimators/prop_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-04-24 08:00:37.000000 nerfacc-0.5.2/nerfacc/volrend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 08:00:56.000000 nerfacc-0.5.2/nerfacc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 08:00:56.000000 nerfacc-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-24 08:00:37.000000 nerfacc-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:00:56.000000 nerfacc-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-24 08:00:37.000000 nerfacc-0.5.2/tests/test_scan.py
```

### Comparing `nerfacc-0.5.1/LICENSE` & `nerfacc-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/README.md` & `nerfacc-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/__init__.py` & `nerfacc-0.5.2/nerfacc/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cameras.py` & `nerfacc-0.5.2/nerfacc/cameras.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cameras2.py` & `nerfacc-0.5.2/nerfacc/cameras2.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/__init__.py` & `nerfacc-0.5.2/nerfacc/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/_backend.py` & `nerfacc-0.5.2/nerfacc/cuda/_backend.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/camera.cu` & `nerfacc-0.5.2/nerfacc/cuda/csrc/camera.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/grid.cu` & `nerfacc-0.5.2/nerfacc/cuda/csrc/grid.cu`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
             //     "[traverse init], delta=(%f, %f, %f), step_index=(%d, %d, %d)\n",
             //     delta.x, delta.y, delta.z, step_index.x, step_index.y, step_index.z
             // );
 
             const int3 overflow_index = final_index + step_index;
             while (true) {
                 float t_traverse = min(tdist.x, min(tdist.y, tdist.z));
+                t_traverse = fminf(t_traverse, this_tmax);
                 int64_t cell_id = (
                     current_index.x * resolution.y * resolution.z
                     + current_index.y * resolution.z
                     + current_index.z
                     + level * resolution.x * resolution.y * resolution.z
                 );
```

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec.hpp` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/data_spec.hpp`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec_packed.cuh` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/data_spec_packed.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_camera.cuh` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_camera.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_contraction.cuh` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_contraction.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_cuda.cuh` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_cuda.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_grid.cuh` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_grid.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_math.cuh` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_math.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_scan.cuh` & `nerfacc-0.5.2/nerfacc/cuda/csrc/include/utils_scan.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/nerfacc.cpp` & `nerfacc-0.5.2/nerfacc/cuda/csrc/nerfacc.cpp`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/pdf.cu` & `nerfacc-0.5.2/nerfacc/cuda/csrc/pdf.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/cuda/csrc/scan.cu` & `nerfacc-0.5.2/nerfacc/cuda/csrc/scan.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/data_specs.py` & `nerfacc-0.5.2/nerfacc/data_specs.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/estimators/base.py` & `nerfacc-0.5.2/nerfacc/estimators/base.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/estimators/occ_grid.py` & `nerfacc-0.5.2/nerfacc/estimators/occ_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         rays_o: Tensor,  # [n_rays, 3]
         rays_d: Tensor,  # [n_rays, 3]
         # sigma/alpha function for skipping invisible space
         sigma_fn: Optional[Callable] = None,
         alpha_fn: Optional[Callable] = None,
         near_plane: float = 0.0,
         far_plane: float = 1e10,
+        t_min: Optional[Tensor] = None,  # [n_rays]
+        t_max: Optional[Tensor] = None,  # [n_rays]
         # rendering options
         render_step_size: float = 1e-3,
         early_stop_eps: float = 1e-4,
         alpha_thre: float = 0.0,
         stratified: bool = False,
         cone_angle: float = 0.0,
     ) -> Tuple[Tensor, Tensor, Tensor]:
@@ -116,14 +118,18 @@
             alpha_fn: Optional. If provided, the marching will skip the invisible space
                 by evaluating the density along the ray with `alpha_fn`. It should be a
                 function that takes in samples {t_starts (N,), t_ends (N,),
                 ray indices (N,)} and returns the post-activation opacity values (N,).
                 You should only provide either `sigma_fn` or `alpha_fn`.
             near_plane: Optional. Near plane distance. Default: 0.0.
             far_plane: Optional. Far plane distance. Default: 1e10.
+            t_min: Optional. Per-ray minimum distance. Tensor with shape (n_rays).
+                If profided, the marching will start from maximum of t_min and near_plane.
+            t_max: Optional. Per-ray maximum distance. Tensor with shape (n_rays).
+                If profided, the marching will stop by minimum of t_max and far_plane.
             render_step_size: Step size for marching. Default: 1e-3.
             early_stop_eps: Early stop threshold for skipping invisible space. Default: 1e-4.
             alpha_thre: Alpha threshold for skipping empty space. Default: 0.0.
             stratified: Whether to use stratified sampling. Default: False.
             cone_angle: Cone angle for linearly-increased step size. 0. means
                 constant step size. Default: 0.0.
 
@@ -143,14 +149,20 @@
             >>> t_mid = (t_starts + t_ends) / 2.0
             >>> sample_locs = rays_o[ray_indices] + t_mid * rays_d[ray_indices]
 
         """
 
         near_planes = torch.full_like(rays_o[..., 0], fill_value=near_plane)
         far_planes = torch.full_like(rays_o[..., 0], fill_value=far_plane)
+
+        if t_min is not None:
+            near_planes = torch.clamp(near_planes, min=t_min)
+        if t_max is not None:
+            far_planes = torch.clamp(far_planes, max=t_max)
+
         if stratified:
             near_planes += torch.rand_like(near_planes) * render_step_size
         intervals, samples = traverse_grids(
             rays_o,
             rays_d,
             self.binaries,
             self.aabbs,
```

### Comparing `nerfacc-0.5.1/nerfacc/estimators/prop_net.py` & `nerfacc-0.5.2/nerfacc/estimators/prop_net.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/grid.py` & `nerfacc-0.5.2/nerfacc/grid.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/pack.py` & `nerfacc-0.5.2/nerfacc/pack.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/pdf.py` & `nerfacc-0.5.2/nerfacc/pdf.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/scan.py` & `nerfacc-0.5.2/nerfacc/scan.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/nerfacc/volrend.py` & `nerfacc-0.5.2/nerfacc/volrend.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 
 
 def render_transmittance_from_alpha(
     alphas: Tensor,
     packed_info: Optional[Tensor] = None,
     ray_indices: Optional[Tensor] = None,
     n_rays: Optional[int] = None,
+    prefix_trans: Optional[Tensor] = None,
 ) -> Tensor:
     """Compute transmittance :math:`T_i` from alpha :math:`\\alpha_i`.
 
     .. math::
         T_i = \\prod_{j=1}^{i-1}(1-\\alpha_j)
 
     This function supports both batched and flattened input tensor. For flattened input tensor, either
@@ -167,14 +168,15 @@
     Args:
         alphas: The opacity values of the samples. Tensor with shape (all_samples,) or (n_rays, n_samples).
         packed_info: A tensor of shape (n_rays, 2) that specifies the start and count
             of each chunk in the flattened samples, with in total n_rays chunks.
             Useful for flattened input.
         ray_indices: Ray indices of the flattened samples. LongTensor with shape (all_samples).
         n_rays: Number of rays. Only useful when `ray_indices` is provided.
+        prefix_trans: The pre-computed transmittance of the samples. Tensor with shape (all_samples,).
 
     Returns:
         The rendering transmittance with the same shape as `alphas`.
 
     Examples:
 
     .. code-block:: python
@@ -187,24 +189,27 @@
     # FIXME Try not to use exclusive_prod because:
     # 1. torch.cumprod is much slower than torch.cumsum
     # 2. exclusive_prod gradient on input == 0 is not correct.
     if ray_indices is not None and packed_info is None:
         packed_info = pack_info(ray_indices, n_rays)
 
     trans = exclusive_prod(1 - alphas, packed_info)
+    if prefix_trans is not None:
+        trans *= prefix_trans
     return trans
 
 
 def render_transmittance_from_density(
     t_starts: Tensor,
     t_ends: Tensor,
     sigmas: Tensor,
     packed_info: Optional[Tensor] = None,
     ray_indices: Optional[Tensor] = None,
     n_rays: Optional[int] = None,
+    prefix_trans: Optional[Tensor] = None,
 ) -> Tuple[Tensor, Tensor]:
     """Compute transmittance :math:`T_i` from density :math:`\\sigma_i`.
 
     .. math::
         T_i = exp(-\\sum_{j=1}^{i-1}\\sigma_j\delta_j)
     
     This function supports both batched and flattened input tensor. For flattened input tensor, either
@@ -217,14 +222,15 @@
             shape (all_samples,) or (n_rays, n_samples).
         sigmas: The density values of the samples. Tensor with shape (all_samples,) or (n_rays, n_samples).
         packed_info: A tensor of shape (n_rays, 2) that specifies the start and count
             of each chunk in the flattened samples, with in total n_rays chunks.
             Useful for flattened input.
         ray_indices: Ray indices of the flattened samples. LongTensor with shape (all_samples).
         n_rays: Number of rays. Only useful when `ray_indices` is provided.
+        prefix_trans: The pre-computed transmittance of the samples. Tensor with shape (all_samples,).
 
     Returns:
         The rendering transmittance and opacities, both with the same shape as `sigmas`.
 
     Examples:
     
     .. code-block:: python
@@ -241,22 +247,25 @@
     """
     if ray_indices is not None and packed_info is None:
         packed_info = pack_info(ray_indices, n_rays)
 
     sigmas_dt = sigmas * (t_ends - t_starts)
     alphas = 1.0 - torch.exp(-sigmas_dt)
     trans = torch.exp(-exclusive_sum(sigmas_dt, packed_info))
+    if prefix_trans is not None:
+        trans *= prefix_trans
     return trans, alphas
 
 
 def render_weight_from_alpha(
     alphas: Tensor,
     packed_info: Optional[Tensor] = None,
     ray_indices: Optional[Tensor] = None,
     n_rays: Optional[int] = None,
+    prefix_trans: Optional[Tensor] = None,
 ) -> Tuple[Tensor, Tensor]:
     """Compute rendering weights :math:`w_i` from opacity :math:`\\alpha_i`.
 
     .. math::
         w_i = T_i\\alpha_i, \\quad\\textrm{where}\\quad T_i = \\prod_{j=1}^{i-1}(1-\\alpha_j)
 
     This function supports both batched and flattened input tensor. For flattened input tensor, either
@@ -265,14 +274,15 @@
     Args:
         alphas: The opacity values of the samples. Tensor with shape (all_samples,) or (n_rays, n_samples).
         packed_info: A tensor of shape (n_rays, 2) that specifies the start and count
             of each chunk in the flattened samples, with in total n_rays chunks.
             Useful for flattened input.
         ray_indices: Ray indices of the flattened samples. LongTensor with shape (all_samples).
         n_rays: Number of rays. Only useful when `ray_indices` is provided.
+        prefix_trans: The pre-computed transmittance of the samples. Tensor with shape (all_samples,).
 
     Returns:
         The rendering weights and transmittance, both with the same shape as `alphas`.
 
     Examples:
 
     .. code-block:: python
@@ -281,27 +291,28 @@
         >>> ray_indices = torch.tensor([0, 0, 0, 1, 1, 2, 2], device="cuda")
         >>> weights, transmittance = render_weight_from_alpha(alphas, ray_indices=ray_indices)
         weights: [0.4, 0.48, 0.012, 0.8, 0.02, 0.0, 0.9])
         transmittance: [1.00, 0.60, 0.12, 1.00, 0.20, 1.00, 1.00]
 
     """
     trans = render_transmittance_from_alpha(
-        alphas, packed_info, ray_indices, n_rays
+        alphas, packed_info, ray_indices, n_rays, prefix_trans
     )
     weights = trans * alphas
     return weights, trans
 
 
 def render_weight_from_density(
     t_starts: Tensor,
     t_ends: Tensor,
     sigmas: Tensor,
     packed_info: Optional[Tensor] = None,
     ray_indices: Optional[Tensor] = None,
     n_rays: Optional[int] = None,
+    prefix_trans: Optional[Tensor] = None,
 ) -> Tuple[Tensor, Tensor, Tensor]:
     """Compute rendering weights :math:`w_i` from density :math:`\\sigma_i` and interval :math:`\\delta_i`.
 
     .. math::
         w_i = T_i(1 - exp(-\\sigma_i\delta_i)), \\quad\\textrm{where}\\quad T_i = exp(-\\sum_{j=1}^{i-1}\\sigma_j\delta_j)
 
     This function supports both batched and flattened input tensor. For flattened input tensor, either
@@ -312,14 +323,15 @@
         t_ends: The end time of the samples. Tensor with shape (all_samples,) or (n_rays, n_samples).
         sigmas: The density values of the samples. Tensor with shape (all_samples,) or (n_rays, n_samples).
         packed_info: A tensor of shape (n_rays, 2) that specifies the start and count
             of each chunk in the flattened samples, with in total n_rays chunks.
             Useful for flattened input.
         ray_indices: Ray indices of the flattened samples. LongTensor with shape (all_samples).
         n_rays: Number of rays. Only useful when `ray_indices` is provided.
+        prefix_trans: The pre-computed transmittance of the samples. Tensor with shape (all_samples,).
 
     Returns:
         The rendering weights, transmittance and opacities, both with the same shape as `sigmas`.
 
     Examples:
 
     .. code-block:: python
@@ -332,28 +344,29 @@
         >>>     t_starts, t_ends, sigmas, ray_indices=ray_indices)
         weights: [0.33, 0.37, 0.03, 0.55, 0.04, 0.00, 0.59]
         transmittance: [1.00, 0.67, 0.30, 1.00, 0.45, 1.00, 1.00]
         alphas: [0.33, 0.55, 0.095, 0.55, 0.095, 0.00, 0.59]
 
     """
     trans, alphas = render_transmittance_from_density(
-        t_starts, t_ends, sigmas, packed_info, ray_indices, n_rays
+        t_starts, t_ends, sigmas, packed_info, ray_indices, n_rays, prefix_trans
     )
     weights = trans * alphas
     return weights, trans, alphas
 
 
 @torch.no_grad()
 def render_visibility_from_alpha(
     alphas: Tensor,
     packed_info: Optional[Tensor] = None,
     ray_indices: Optional[Tensor] = None,
     n_rays: Optional[int] = None,
     early_stop_eps: float = 1e-4,
     alpha_thre: float = 0.0,
+    prefix_trans: Optional[Tensor] = None,
 ) -> Tensor:
     """Compute visibility from opacity :math:`\\alpha_i`.
 
     In this function, we first compute the transmittance from the sample opacity. The
     transmittance is then used to filter out occluded samples. And opacity is used to
     filter out transparent samples. The function returns a boolean tensor indicating
     which samples are visible (`transmittance > early_stop_eps` and `opacity > alpha_thre`).
@@ -366,14 +379,15 @@
         packed_info: A tensor of shape (n_rays, 2) that specifies the start and count
             of each chunk in the flattened samples, with in total n_rays chunks.
             Useful for flattened input.
         ray_indices: Ray indices of the flattened samples. LongTensor with shape (all_samples).
         n_rays: Number of rays. Only useful when `ray_indices` is provided.
         early_stop_eps: The early stopping threshold on transmittance.
         alpha_thre: The threshold on opacity.
+        prefix_trans: The pre-computed transmittance of the samples. Tensor with shape (all_samples,).
 
     Returns:
         A boolean tensor indicating which samples are visible. Same shape as `alphas`.
 
     Examples:
 
     .. code-block:: python
@@ -384,15 +398,15 @@
         tensor([1.0, 0.6, 0.12, 1.0, 0.2, 1.0, 1.0])
         >>> visibility = render_visibility_from_alpha(
         >>>     alphas, ray_indices=ray_indices, early_stop_eps=0.3, alpha_thre=0.2)
         tensor([True,  True, False,  True, False, False,  True])
 
     """
     trans = render_transmittance_from_alpha(
-        alphas, packed_info, ray_indices, n_rays
+        alphas, packed_info, ray_indices, n_rays, prefix_trans
     )
     vis = trans >= early_stop_eps
     if alpha_thre > 0:
         vis = vis & (alphas >= alpha_thre)
     return vis
 
 
@@ -402,14 +416,15 @@
     t_ends: Tensor,
     sigmas: Tensor,
     packed_info: Optional[Tensor] = None,
     ray_indices: Optional[Tensor] = None,
     n_rays: Optional[int] = None,
     early_stop_eps: float = 1e-4,
     alpha_thre: float = 0.0,
+    prefix_trans: Optional[Tensor] = None,
 ) -> Tensor:
     """Compute visibility from density :math:`\\sigma_i` and interval :math:`\\delta_i`.
 
     In this function, we first compute the transmittance and opacity from the sample density. The
     transmittance is then used to filter out occluded samples. And opacity is used to
     filter out transparent samples. The function returns a boolean tensor indicating
     which samples are visible (`transmittance > early_stop_eps` and `opacity > alpha_thre`).
@@ -422,14 +437,15 @@
         packed_info: A tensor of shape (n_rays, 2) that specifies the start and count
             of each chunk in the flattened samples, with in total n_rays chunks.
             Useful for flattened input.
         ray_indices: Ray indices of the flattened samples. LongTensor with shape (all_samples).
         n_rays: Number of rays. Only useful when `ray_indices` is provided.
         early_stop_eps: The early stopping threshold on transmittance.
         alpha_thre: The threshold on opacity.
+        prefix_trans: The pre-computed transmittance of the samples. Tensor with shape (all_samples,).
 
     Returns:
         A boolean tensor indicating which samples are visible. Same shape as `alphas`.
 
     Examples:
 
     .. code-block:: python
@@ -444,15 +460,15 @@
         alphas: [0.33, 0.55, 0.095, 0.55, 0.095, 0.00, 0.59]
         >>> visibility = render_visibility_from_density(
         >>>     t_starts, t_ends, sigmas, ray_indices=ray_indices, early_stop_eps=0.3, alpha_thre=0.2)
         tensor([True,  True, False,  True, False, False,  True])
 
     """
     trans, alphas = render_transmittance_from_density(
-        t_starts, t_ends, sigmas, packed_info, ray_indices, n_rays
+        t_starts, t_ends, sigmas, packed_info, ray_indices, n_rays, prefix_trans
     )
     vis = trans >= early_stop_eps
     if alpha_thre > 0:
         vis = vis & (alphas >= alpha_thre)
     return vis
```

### Comparing `nerfacc-0.5.1/nerfacc.egg-info/SOURCES.txt` & `nerfacc-0.5.2/nerfacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/setup.py` & `nerfacc-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/tests/test_camera.py` & `nerfacc-0.5.2/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/tests/test_pack.py` & `nerfacc-0.5.2/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/tests/test_pdf.py` & `nerfacc-0.5.2/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/tests/test_rendering.py` & `nerfacc-0.5.2/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.1/tests/test_scan.py` & `nerfacc-0.5.2/tests/test_scan.py`

 * *Files identical despite different names*

