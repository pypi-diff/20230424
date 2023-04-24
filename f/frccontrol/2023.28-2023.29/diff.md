# Comparing `tmp/frccontrol-2023.28.tar.gz` & `tmp/frccontrol-2023.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frccontrol-2023.28.tar", last modified: Tue Mar 28 17:22:30 2023, max compression
+gzip compressed data, was "frccontrol-2023.29.tar", last modified: Mon Apr 24 20:43:42 2023, max compression
```

## Comparing `frccontrol-2023.28.tar` & `frccontrol-2023.29.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-03-28 17:22:30.932726 frccontrol-2023.28/
--rw-r--r--   0 tav       (1000) users      (100)     1457 2018-07-14 03:19:56.000000 frccontrol-2023.28/LICENSE
--rw-r--r--   0 tav       (1000) users      (100)     1115 2023-03-28 17:22:30.932726 frccontrol-2023.28/PKG-INFO
--rw-r--r--   0 tav       (1000) users      (100)      383 2022-11-10 21:45:34.000000 frccontrol-2023.28/README.rst
-drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-03-28 17:22:30.929393 frccontrol-2023.28/frccontrol/
--rw-r--r--   0 tav       (1000) users      (100)      401 2023-03-28 17:22:28.000000 frccontrol-2023.28/frccontrol/__init__.py
--rw-r--r--   0 tav       (1000) users      (100)     1865 2023-03-17 22:26:57.000000 frccontrol-2023.28/frccontrol/ctrlutil.py
--rw-r--r--   0 tav       (1000) users      (100)     2240 2023-03-19 21:39:39.000000 frccontrol-2023.28/frccontrol/discretization.py
--rw-r--r--   0 tav       (1000) users      (100)     4252 2023-03-26 17:19:21.000000 frccontrol-2023.28/frccontrol/extended_kalman_filter.py
--rw-r--r--   0 tav       (1000) users      (100)     2587 2023-03-17 22:26:57.000000 frccontrol-2023.28/frccontrol/kalman_filter.py
--rw-r--r--   0 tav       (1000) users      (100)     1484 2023-03-17 22:26:57.000000 frccontrol-2023.28/frccontrol/linear_plant_inversion_feedforward.py
--rw-r--r--   0 tav       (1000) users      (100)     2797 2023-03-17 22:26:57.000000 frccontrol-2023.28/frccontrol/linear_quadratic_regulator.py
--rw-r--r--   0 tav       (1000) users      (100)     6150 2023-03-26 01:10:05.000000 frccontrol-2023.28/frccontrol/models.py
--rw-r--r--   0 tav       (1000) users      (100)     3980 2023-03-26 22:28:18.000000 frccontrol-2023.28/frccontrol/numerical_integration.py
--rw-r--r--   0 tav       (1000) users      (100)     1518 2023-03-15 05:59:43.000000 frccontrol-2023.28/frccontrol/numerical_jacobian.py
--rw-r--r--   0 tav       (1000) users      (100)     3193 2023-03-28 17:13:23.000000 frccontrol-2023.28/frccontrol/plotutil.py
--rw-r--r--   0 tav       (1000) users      (100)     4462 2023-03-15 06:00:03.000000 frccontrol-2023.28/frccontrol/profiles.py
-drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-03-28 17:22:30.932726 frccontrol-2023.28/frccontrol/test/
--rw-r--r--   0 tav       (1000) users      (100)        0 2022-10-01 04:59:40.000000 frccontrol-2023.28/frccontrol/test/__init__.py
--rw-r--r--   0 tav       (1000) users      (100)      654 2022-10-01 05:01:04.000000 frccontrol-2023.28/frccontrol/test/test_numerical_jacobian.py
--rw-r--r--   0 tav       (1000) users      (100)       51 2023-03-28 17:22:30.000000 frccontrol-2023.28/frccontrol/version.py
-drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-03-28 17:22:30.932726 frccontrol-2023.28/frccontrol.egg-info/
--rw-r--r--   0 tav       (1000) users      (100)     1115 2023-03-28 17:22:30.000000 frccontrol-2023.28/frccontrol.egg-info/PKG-INFO
--rw-r--r--   0 tav       (1000) users      (100)      694 2023-03-28 17:22:30.000000 frccontrol-2023.28/frccontrol.egg-info/SOURCES.txt
--rw-r--r--   0 tav       (1000) users      (100)        1 2023-03-28 17:22:30.000000 frccontrol-2023.28/frccontrol.egg-info/dependency_links.txt
--rw-r--r--   0 tav       (1000) users      (100)       23 2023-03-28 17:22:30.000000 frccontrol-2023.28/frccontrol.egg-info/requires.txt
--rw-r--r--   0 tav       (1000) users      (100)       11 2023-03-28 17:22:30.000000 frccontrol-2023.28/frccontrol.egg-info/top_level.txt
--rw-r--r--   0 tav       (1000) users      (100)        1 2018-07-14 02:44:51.000000 frccontrol-2023.28/frccontrol.egg-info/zip-safe
--rw-r--r--   0 tav       (1000) users      (100)       63 2023-03-28 17:22:30.932726 frccontrol-2023.28/setup.cfg
--rw-r--r--   0 tav       (1000) users      (100)     2692 2022-10-01 06:42:46.000000 frccontrol-2023.28/setup.py
+drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-04-24 20:43:42.328099 frccontrol-2023.29/
+-rw-r--r--   0 tav       (1000) users      (100)     1457 2018-07-14 03:19:56.000000 frccontrol-2023.29/LICENSE
+-rw-r--r--   0 tav       (1000) users      (100)     1115 2023-04-24 20:43:42.328099 frccontrol-2023.29/PKG-INFO
+-rw-r--r--   0 tav       (1000) users      (100)      383 2022-11-10 21:45:34.000000 frccontrol-2023.29/README.rst
+drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-04-24 20:43:42.328099 frccontrol-2023.29/frccontrol/
+-rw-r--r--   0 tav       (1000) users      (100)      427 2023-04-24 20:42:51.000000 frccontrol-2023.29/frccontrol/__init__.py
+-rw-r--r--   0 tav       (1000) users      (100)     1865 2023-03-17 22:26:57.000000 frccontrol-2023.29/frccontrol/ctrlutil.py
+-rw-r--r--   0 tav       (1000) users      (100)     2240 2023-03-19 21:39:39.000000 frccontrol-2023.29/frccontrol/discretization.py
+-rw-r--r--   0 tav       (1000) users      (100)     4252 2023-03-26 17:19:21.000000 frccontrol-2023.29/frccontrol/extended_kalman_filter.py
+-rw-r--r--   0 tav       (1000) users      (100)     2587 2023-03-17 22:26:57.000000 frccontrol-2023.29/frccontrol/kalman_filter.py
+-rw-r--r--   0 tav       (1000) users      (100)     1484 2023-03-17 22:26:57.000000 frccontrol-2023.29/frccontrol/linear_plant_inversion_feedforward.py
+-rw-r--r--   0 tav       (1000) users      (100)     2797 2023-03-17 22:26:57.000000 frccontrol-2023.29/frccontrol/linear_quadratic_regulator.py
+-rw-r--r--   0 tav       (1000) users      (100)     6150 2023-03-26 01:10:05.000000 frccontrol-2023.29/frccontrol/models.py
+-rw-r--r--   0 tav       (1000) users      (100)     3980 2023-03-26 22:28:18.000000 frccontrol-2023.29/frccontrol/numerical_integration.py
+-rw-r--r--   0 tav       (1000) users      (100)     1518 2023-03-15 05:59:43.000000 frccontrol-2023.29/frccontrol/numerical_jacobian.py
+-rw-r--r--   0 tav       (1000) users      (100)     3193 2023-03-28 17:13:23.000000 frccontrol-2023.29/frccontrol/plotutil.py
+-rw-r--r--   0 tav       (1000) users      (100)     4462 2023-03-15 06:00:03.000000 frccontrol-2023.29/frccontrol/profiles.py
+drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-04-24 20:43:42.328099 frccontrol-2023.29/frccontrol/test/
+-rw-r--r--   0 tav       (1000) users      (100)        0 2022-10-01 04:59:40.000000 frccontrol-2023.29/frccontrol/test/__init__.py
+-rw-r--r--   0 tav       (1000) users      (100)      654 2022-10-01 05:01:04.000000 frccontrol-2023.29/frccontrol/test/test_numerical_jacobian.py
+-rw-r--r--   0 tav       (1000) users      (100)     8039 2023-04-24 20:42:51.000000 frccontrol-2023.29/frccontrol/trajectory.py
+-rw-r--r--   0 tav       (1000) users      (100)       51 2023-04-24 20:43:42.000000 frccontrol-2023.29/frccontrol/version.py
+drwxr-xr-x   0 tav       (1000) users      (100)        0 2023-04-24 20:43:42.328099 frccontrol-2023.29/frccontrol.egg-info/
+-rw-r--r--   0 tav       (1000) users      (100)     1115 2023-04-24 20:43:42.000000 frccontrol-2023.29/frccontrol.egg-info/PKG-INFO
+-rw-r--r--   0 tav       (1000) users      (100)      719 2023-04-24 20:43:42.000000 frccontrol-2023.29/frccontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 tav       (1000) users      (100)        1 2023-04-24 20:43:42.000000 frccontrol-2023.29/frccontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 tav       (1000) users      (100)       23 2023-04-24 20:43:42.000000 frccontrol-2023.29/frccontrol.egg-info/requires.txt
+-rw-r--r--   0 tav       (1000) users      (100)       11 2023-04-24 20:43:42.000000 frccontrol-2023.29/frccontrol.egg-info/top_level.txt
+-rw-r--r--   0 tav       (1000) users      (100)        1 2018-07-14 02:44:51.000000 frccontrol-2023.29/frccontrol.egg-info/zip-safe
+-rw-r--r--   0 tav       (1000) users      (100)       63 2023-04-24 20:43:42.328099 frccontrol-2023.29/setup.cfg
+-rw-r--r--   0 tav       (1000) users      (100)     2692 2022-10-01 06:42:46.000000 frccontrol-2023.29/setup.py
```

### Comparing `frccontrol-2023.28/LICENSE` & `frccontrol-2023.29/LICENSE`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/PKG-INFO` & `frccontrol-2023.29/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frccontrol
-Version: 2023.28
+Version: 2023.29
 Summary: Wrappers around Python Control for making development of state-space models for the FIRST Robotics Competition easier
 Home-page: https://github.com/calcmogul/frccontrol
 Author: Tyler Veness
 Maintainer: Tyler Veness
 Maintainer-email: calcmogul@gmail.com
 License: BSD License
 Keywords: frc first robotics control
```

### Comparing `frccontrol-2023.28/frccontrol/ctrlutil.py` & `frccontrol-2023.29/frccontrol/ctrlutil.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/discretization.py` & `frccontrol-2023.29/frccontrol/discretization.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/extended_kalman_filter.py` & `frccontrol-2023.29/frccontrol/extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/kalman_filter.py` & `frccontrol-2023.29/frccontrol/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/linear_plant_inversion_feedforward.py` & `frccontrol-2023.29/frccontrol/linear_plant_inversion_feedforward.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/linear_quadratic_regulator.py` & `frccontrol-2023.29/frccontrol/linear_quadratic_regulator.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/models.py` & `frccontrol-2023.29/frccontrol/models.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/numerical_integration.py` & `frccontrol-2023.29/frccontrol/numerical_integration.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/numerical_jacobian.py` & `frccontrol-2023.29/frccontrol/numerical_jacobian.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/plotutil.py` & `frccontrol-2023.29/frccontrol/plotutil.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/profiles.py` & `frccontrol-2023.29/frccontrol/profiles.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol/test/test_numerical_jacobian.py` & `frccontrol-2023.29/frccontrol/test/test_numerical_jacobian.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2023.28/frccontrol.egg-info/PKG-INFO` & `frccontrol-2023.29/frccontrol.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frccontrol
-Version: 2023.28
+Version: 2023.29
 Summary: Wrappers around Python Control for making development of state-space models for the FIRST Robotics Competition easier
 Home-page: https://github.com/calcmogul/frccontrol
 Author: Tyler Veness
 Maintainer: Tyler Veness
 Maintainer-email: calcmogul@gmail.com
 License: BSD License
 Keywords: frc first robotics control
```

### Comparing `frccontrol-2023.28/frccontrol.egg-info/SOURCES.txt` & `frccontrol-2023.29/frccontrol.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 frccontrol/linear_plant_inversion_feedforward.py
 frccontrol/linear_quadratic_regulator.py
 frccontrol/models.py
 frccontrol/numerical_integration.py
 frccontrol/numerical_jacobian.py
 frccontrol/plotutil.py
 frccontrol/profiles.py
+frccontrol/trajectory.py
 frccontrol/version.py
 frccontrol.egg-info/PKG-INFO
 frccontrol.egg-info/SOURCES.txt
 frccontrol.egg-info/dependency_links.txt
 frccontrol.egg-info/requires.txt
 frccontrol.egg-info/top_level.txt
 frccontrol.egg-info/zip-safe
```

### Comparing `frccontrol-2023.28/setup.py` & `frccontrol-2023.29/setup.py`

 * *Files identical despite different names*

