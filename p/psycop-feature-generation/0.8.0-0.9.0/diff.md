# Comparing `tmp/psycop_feature_generation-0.8.0.tar.gz` & `tmp/psycop_feature_generation-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycop_feature_generation-0.8.0.tar", max compression
+gzip compressed data, was "psycop_feature_generation-0.9.0.tar", max compression
```

## Comparing `psycop_feature_generation-0.8.0.tar` & `psycop_feature_generation-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     2002 2022-11-17 15:47:34.290040 psycop_feature_generation-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/__init__.py
--rw-r--r--   0        0        0        0 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/__init__.py
--rw-r--r--   0        0        0    15849 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/flattened/data_integrity.py
--rw-r--r--   0        0        0     7381 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/flattened/feature_describer.py
--rw-r--r--   0        0        0     7058 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/raw/check_predictor_lists.py
--rw-r--r--   0        0        0     6664 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/raw/check_raw_df.py
--rw-r--r--   0        0        0     7669 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/raw/validate_raw_data.py
--rw-r--r--   0        0        0     1575 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/utils.py
--rw-r--r--   0        0        0        0 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/featurizers/__init__.py
--rw-r--r--   0        0        0     3340 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/featurizers/tfidf.py
--rw-r--r--   0        0        0        0 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/__init__.py
--rw-r--r--   0        0        0       85 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/flattened/__init__.py
--rw-r--r--   0        0        0     3522 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/flattened/local_feature_loaders.py
--rw-r--r--   0        0        0     2093 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/non_numerical_coercer.py
--rw-r--r--   0        0        0      616 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/__init__.py
--rw-r--r--   0        0        0     3477 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_admissions.py
--rw-r--r--   0        0        0     9326 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_coercion.py
--rw-r--r--   0        0        0     1477 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_demographic.py
--rw-r--r--   0        0        0    18705 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_diagnoses.py
--rw-r--r--   0        0        0      708 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_ids.py
--rw-r--r--   0        0        0    18402 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_lab_results.py
--rw-r--r--   0        0        0    14210 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_medications.py
--rw-r--r--   0        0        0     4505 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_structured_sfi.py
--rw-r--r--   0        0        0     1529 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_t2d_outcomes.py
--rw-r--r--   0        0        0    15469 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_text.py
--rw-r--r--   0        0        0     4069 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_visits.py
--rw-r--r--   0        0        0     2288 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/sql_load.py
--rw-r--r--   0        0        0      670 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/t2d_loaders.py
--rw-r--r--   0        0        0     5626 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/utils.py
--rw-r--r--   0        0        0     2327 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/synth/raw/load_synth_data.py
--rw-r--r--   0        0        0      497 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/utils.py
--rw-r--r--   0        0        0       80 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/__init__.py
--rw-r--r--   0        0        0    11177 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/feature_spec_objects.py
--rw-r--r--   0        0        0    32837 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0        0        0        0 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/flattened_ds_cache.py
--rw-r--r--   0        0        0     2065 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0        0        0     3200 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/resolve_multiple_functions.py
--rw-r--r--   0        0        0     4479 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/utils.py
--rw-r--r--   0        0        0     4639 2022-11-17 15:47:33.522028 psycop_feature_generation-0.8.0/src/psycop_feature_generation/utils_for_testing.py
--rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 psycop_feature_generation-0.8.0/setup.py
--rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 psycop_feature_generation-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1984 2022-11-18 12:03:25.919831 psycop_feature_generation-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/__init__.py
+-rw-r--r--   0        0        0    15849 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/flattened/data_integrity.py
+-rw-r--r--   0        0        0     7381 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/flattened/feature_describer.py
+-rw-r--r--   0        0        0     7058 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/raw/check_predictor_lists.py
+-rw-r--r--   0        0        0     6664 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/raw/check_raw_df.py
+-rw-r--r--   0        0        0     7669 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/raw/validate_raw_data.py
+-rw-r--r--   0        0        0     1575 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/utils.py
+-rw-r--r--   0        0        0        0 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/featurizers/__init__.py
+-rw-r--r--   0        0        0     3340 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/featurizers/tfidf.py
+-rw-r--r--   0        0        0        0 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/__init__.py
+-rw-r--r--   0        0        0       85 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/flattened/__init__.py
+-rw-r--r--   0        0        0     3522 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/flattened/local_feature_loaders.py
+-rw-r--r--   0        0        0     2093 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/non_numerical_coercer.py
+-rw-r--r--   0        0        0      616 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/__init__.py
+-rw-r--r--   0        0        0     3477 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_admissions.py
+-rw-r--r--   0        0        0     9326 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_coercion.py
+-rw-r--r--   0        0        0     1477 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_demographic.py
+-rw-r--r--   0        0        0    18705 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_diagnoses.py
+-rw-r--r--   0        0        0      708 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_ids.py
+-rw-r--r--   0        0        0    18402 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_lab_results.py
+-rw-r--r--   0        0        0    14210 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_medications.py
+-rw-r--r--   0        0        0     4505 2022-11-18 12:03:24.947807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_structured_sfi.py
+-rw-r--r--   0        0        0     1529 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_t2d_outcomes.py
+-rw-r--r--   0        0        0    16180 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_text.py
+-rw-r--r--   0        0        0     4069 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_visits.py
+-rw-r--r--   0        0        0     2288 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/sql_load.py
+-rw-r--r--   0        0        0      670 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/t2d_loaders.py
+-rw-r--r--   0        0        0     5626 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/utils.py
+-rw-r--r--   0        0        0     2327 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/synth/raw/load_synth_data.py
+-rw-r--r--   0        0        0      497 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/utils.py
+-rw-r--r--   0        0        0       80 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/__init__.py
+-rw-r--r--   0        0        0    11982 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/feature_spec_objects.py
+-rw-r--r--   0        0        0    32837 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0        0        0        0 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/flattened_ds_cache.py
+-rw-r--r--   0        0        0     2065 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0        0        0     3200 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/resolve_multiple_functions.py
+-rw-r--r--   0        0        0     4479 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/utils.py
+-rw-r--r--   0        0        0     4639 2022-11-18 12:03:24.951807 psycop_feature_generation-0.9.0/src/psycop_feature_generation/utils_for_testing.py
+-rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 psycop_feature_generation-0.9.0/setup.py
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 psycop_feature_generation-0.9.0/PKG-INFO
```

### Comparing `psycop_feature_generation-0.8.0/pyproject.toml` & `psycop_feature_generation-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psycop_feature_generation"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
 scipy = ">=1.8.0,<1.9.4"
 wasabi = ">=0.9.1,<0.10.2"
@@ -17,15 +17,14 @@
 pyodbc = ">=4.0.34, <4.0.36"
 dask = ">=2022.9.0,<2022.12.0"
 pydantic = ">=1.9.0, <1.10.0"
 psutil = ">=5.9.1, <6.0.0"
 pandas = ">=1.4.0,<1.6.0"
 catalogue = ">=2.0.0, <2.1.0"
 numpy = ">=1.23.3,<1.23.5"
-torch = "^1.12.1"
 transformers = "^4.22.2"
 pyarrow = ">=9.0.0,<9.1.0"
 psycopmlutils = ">=0.2.4, <0.3.0"
 protobuf = "<=3.20.3" # Other versions give errors with pytest, super weird!
 frozendict = "^2.3.4"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/flattened/data_integrity.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/flattened/data_integrity.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/flattened/feature_describer.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/flattened/feature_describer.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/raw/check_predictor_lists.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/raw/check_predictor_lists.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/raw/check_raw_df.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/raw/check_raw_df.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/raw/validate_raw_data.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/raw/validate_raw_data.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/data_checks/utils.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/data_checks/utils.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/featurizers/tfidf.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/featurizers/tfidf.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/flattened/local_feature_loaders.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/flattened/local_feature_loaders.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/non_numerical_coercer.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/non_numerical_coercer.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/__init__.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_admissions.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_admissions.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_coercion.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_coercion.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_demographic.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_demographic.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_diagnoses.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_diagnoses.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_ids.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_ids.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_lab_results.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_lab_results.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_medications.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_medications.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_structured_sfi.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_structured_sfi.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_t2d_outcomes.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_t2d_outcomes.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_text.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,142 +1,143 @@
-"""Load text data from a database and featurise it using a tf-idf
-vectorizer."""
+# """Load text data from a database and featurise it using a tf-idf
+# vectorizer."""
 
-# pylint: disable=E0211,E0213,missing-function-docstring
+# # pylint: disable=E0211,E0213,missing-function-docstring
 
-from functools import partial
-from multiprocessing import Pool
-from pathlib import Path
-from typing import Optional, Union
-
-import dill as pkl
-import pandas as pd
-import torch
-from transformers import AutoModel, AutoTokenizer
-from transformers.modeling_outputs import BaseModelOutputWithPoolingAndCrossAttentions
-
-from psycop_feature_generation.loaders.raw.sql_load import sql_load
-from psycop_feature_generation.utils import PROJECT_ROOT, data_loaders
-
-
-def get_all_valid_note_types() -> set[str]:
-    """Returns a set of valid note types. Notice that 'Konklusion' is replaced
-    by 'Vurdering/konklusion' in 2020, so make sure to use both. 'Ordination'
-    was replaced by 'Ordination, Psykiatry' in 2022, but 'Ordination,
-    Psykiatri' is not included in the table. Use with caution.
-
-    Returns:
-        Set[str]: Set of valid note types
-    """
-    return {
-        "Observation af patient, Psykiatri",
-        "Samtale med behandlingssigte",
-        "Ordination",  # OBS replaced "Ordination, Psykiatri" in 01/02-22
-        # but is not included in this table. Use with caution
-        "Aktuelt psykisk",
-        "Aktuelt socialt, Psykiatri",
-        "Aftaler, Psykiatri",
-        "Medicin",
-        "Aktuelt somatisk, Psykiatri",
-        "Objektivt psykisk",
-        "Kontaktårsag",
-        "Telefonkonsultation",
-        "Journalnotat",
-        "Telefonnotat",
-        "Objektivt, somatisk",
-        "Plan",
-        "Semistruktureret diagnostisk interview",
-        "Vurdering/konklusion",
-    }
-
-
-def _load_notes_for_year(
-    note_types: Union[str, list[str]],
-    year: str,
-    view: Optional[str] = "FOR_SFI_fritekst_resultat_udfoert_i_psykiatrien_aendret",
-    n_rows: Optional[int] = None,
-) -> pd.DataFrame:
-    """Loads clinical notes from sql from a specified year and matching
-    specified note types.
-
-    Args:
-        note_names (Union[str, list[str]]): Which types of notes to load.
-        year (str): Which year to load
-        view (str, optional): Which table to load.
-            Defaults to "[FOR_SFI_fritekst_resultat_udfoert_i_psykiatrien_aendret".
-        n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
-
-    Returns:
-        pd.DataFrame: Dataframe with clinical notes
-    """
-
-    sql = (
-        "SELECT dw_ek_borger, datotid_senest_aendret_i_sfien, fritekst"
-        + f" FROM [fct].[{view}_{year}_inkl_2021_feb2022]"
-        + f" WHERE overskrift IN {note_types}"
-    )
-    return sql_load(
-        sql,
-        database="USR_PS_FORSK",
-        chunksize=None,
-        n_rows=n_rows,
-    )
-
-
-def _tfidf_featurize(
-    df: pd.DataFrame,
-    tfidf_path: Path,
-    text_col: str = "text",
-) -> pd.DataFrame:
-    """TF-IDF featurize text. Assumes `df` to have a column named `text`.
-
-    Args:
-        df (pd.DataFrame): Dataframe with text column
-        tfidf_path (Optional[Path]): Path to a sklearn tf-idf vectorizer
-        text_col (str, optional): Name of text column. Defaults to "text".
-
-    Returns:
-        pd.DataFrame: Original dataframe with tf-idf features appended
-    """
-    with open(tfidf_path, "rb") as f:
-        tfidf = pkl.load(f)
-
-    vocab = ["tfidf-" + word for word in tfidf.get_feature_names()]
-
-    text = df[text_col].values
-    df = df.drop(text_col, axis=1).reset_index(drop=True)
-
-    text = tfidf.transform(text)
-    text = pd.DataFrame(text.toarray(), columns=vocab)
-    return pd.concat([df, text], axis=1)
-
-
-def _mean_pooling(
-    model_output: BaseModelOutputWithPoolingAndCrossAttentions,
-    attention_mask: torch.Tensor,
-) -> torch.Tensor:
-    """Mean Pooling - take attention mask into account for correct averaging.
-
-    Args:
-        model_output (BaseModelOutputWithPoolingAndCrossAttentions): model output from pretrained Huggingface transformer
-        attention_mask (torch.Tensor): attention mask from from pretrained Hugginface tokenizer
-
-    Returns:
-        np.ndarray: numpy array with mean pooled embeddings
-    """
-    token_embeddings = model_output[
-        0
-    ]  # first element of model_output contains all token embeddings
-    input_mask_expanded = (
-        attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
-    )
-    return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(
-        input_mask_expanded.sum(1),
-        min=1e-9,
-    )
+# from functools import partial
+# from multiprocessing import Pool
+# from pathlib import Path
+# from typing import Optional, Union
+
+# import dill as pkl
+# import pandas as pd
+
+# # import torch
+# from transformers import AutoModel, AutoTokenizer
+# from transformers.modeling_outputs import BaseModelOutputWithPoolingAndCrossAttentions
+
+# from psycop_feature_generation.loaders.raw.sql_load import sql_load
+# from psycop_feature_generation.utils import PROJECT_ROOT, data_loaders
+
+
+# def get_all_valid_note_types() -> set[str]:
+#     """Returns a set of valid note types. Notice that 'Konklusion' is replaced
+#     by 'Vurdering/konklusion' in 2020, so make sure to use both. 'Ordination'
+#     was replaced by 'Ordination, Psykiatry' in 2022, but 'Ordination,
+#     Psykiatri' is not included in the table. Use with caution.
+
+#     Returns:
+#         Set[str]: Set of valid note types
+#     """
+#     return {
+#         "Observation af patient, Psykiatri",
+#         "Samtale med behandlingssigte",
+#         "Ordination",  # OBS replaced "Ordination, Psykiatri" in 01/02-22
+#         # but is not included in this table. Use with caution
+#         "Aktuelt psykisk",
+#         "Aktuelt socialt, Psykiatri",
+#         "Aftaler, Psykiatri",
+#         "Medicin",
+#         "Aktuelt somatisk, Psykiatri",
+#         "Objektivt psykisk",
+#         "Kontaktårsag",
+#         "Telefonkonsultation",
+#         "Journalnotat",
+#         "Telefonnotat",
+#         "Objektivt, somatisk",
+#         "Plan",
+#         "Semistruktureret diagnostisk interview",
+#         "Vurdering/konklusion",
+#     }
+
+
+# def _load_notes_for_year(
+#     note_types: Union[str, list[str]],
+#     year: str,
+#     view: Optional[str] = "FOR_SFI_fritekst_resultat_udfoert_i_psykiatrien_aendret",
+#     n_rows: Optional[int] = None,
+# ) -> pd.DataFrame:
+#     """Loads clinical notes from sql from a specified year and matching
+#     specified note types.
+
+#     Args:
+#         note_names (Union[str, list[str]]): Which types of notes to load.
+#         year (str): Which year to load
+#         view (str, optional): Which table to load.
+#             Defaults to "[FOR_SFI_fritekst_resultat_udfoert_i_psykiatrien_aendret".
+#         n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
+
+#     Returns:
+#         pd.DataFrame: Dataframe with clinical notes
+#     """
+
+#     sql = (
+#         "SELECT dw_ek_borger, datotid_senest_aendret_i_sfien, fritekst"
+#         + f" FROM [fct].[{view}_{year}_inkl_2021_feb2022]"
+#         + f" WHERE overskrift IN {note_types}"
+#     )
+#     return sql_load(
+#         sql,
+#         database="USR_PS_FORSK",
+#         chunksize=None,
+#         n_rows=n_rows,
+#     )
+
+
+# def _tfidf_featurize(
+#     df: pd.DataFrame,
+#     tfidf_path: Path,
+#     text_col: str = "text",
+# ) -> pd.DataFrame:
+#     """TF-IDF featurize text. Assumes `df` to have a column named `text`.
+
+#     Args:
+#         df (pd.DataFrame): Dataframe with text column
+#         tfidf_path (Optional[Path]): Path to a sklearn tf-idf vectorizer
+#         text_col (str, optional): Name of text column. Defaults to "text".
+
+#     Returns:
+#         pd.DataFrame: Original dataframe with tf-idf features appended
+#     """
+#     with open(tfidf_path, "rb") as f:
+#         tfidf = pkl.load(f)
+
+#     vocab = ["tfidf-" + word for word in tfidf.get_feature_names()]
+
+#     text = df[text_col].values
+#     df = df.drop(text_col, axis=1).reset_index(drop=True)
+
+#     text = tfidf.transform(text)
+#     text = pd.DataFrame(text.toarray(), columns=vocab)
+#     return pd.concat([df, text], axis=1)
+
+
+# def _mean_pooling(
+#     model_output: BaseModelOutputWithPoolingAndCrossAttentions,
+#     attention_mask: torch.Tensor,
+# ) -> torch.Tensor:
+#     """Mean Pooling - take attention mask into account for correct averaging.
+
+#     Args:
+#         model_output (BaseModelOutputWithPoolingAndCrossAttentions): model output from pretrained Huggingface transformer
+#         attention_mask (torch.Tensor): attention mask from from pretrained Hugginface tokenizer
+
+#     Returns:
+#         np.ndarray: numpy array with mean pooled embeddings
+#     """
+#     token_embeddings = model_output[
+#         0
+#     ]  # first element of model_output contains all token embeddings
+#     input_mask_expanded = (
+#         attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
+#     )
+#     return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(
+#         input_mask_expanded.sum(1),
+#         min=1e-9,
+#     )
 
 
 def _chunk_text(text: str, seq_length: int) -> list[str]:
     """Chunk text into sequences of length `seq_length`, where `seq_length`
     refers to number of words.
 
     Args:
@@ -159,301 +160,301 @@
             " ".join(word_list)
             for word_list in words_in_chunks
             if len(word_list) == seq_length
         ]  # drop small remainder of shorter size
         return chunks
 
 
-def _huggingface_featurize(
-    df: pd.DataFrame,
-    model_id: str = "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
-    text_col: str = "text",
-) -> pd.DataFrame:
-    """Featurize text using a huggingface model and generate a dataframe with
-    the embeddings. If the text is longer than the maximum sequence length of
-    the model, the text is split into chunks and embeddings are averaged across
-    chunks.
-
-    Args:
-        df (pd.DataFrame): Dataframe with text column
-        model_id (str): Which huggingface model to use. See https://huggingface.co/models for a list of models. Assumes the model is a transformer model and has both a tokenizer and a model.
-        text_col (str, optional): Name of text column. Defaults to "text".
-
-    Returns:
-        pd.DataFrame: Original dataframe with huggingface embeddings appended
-
-    Example:
-        >>> p = PROJECT_ROOT / "tests" / "test_data" / "raw"
-        >>> huggingface_model_id = "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2"
-        >>> df_p = p / "synth_txt_data.csv"
-
-        >>> df = pd.read_csv(df_p)
-        >>> df = df.dropna()
-
-        >>> x = _huggingface_featurize(df, huggingface_model_id)
-    """
-    tokenizer = AutoTokenizer.from_pretrained(model_id)
-    model = AutoModel.from_pretrained(model_id)
-
-    df = df[df[text_col].notna()]
-    text = df[text_col].values
-    df = df.drop(text_col, axis=1)
-
-    max_seq_length = int(
-        tokenizer.model_max_length / 1.5,
-    )  # allowing space for more word piece tokens than words in original sequence
-
-    list_of_embeddings = []
-    for txt in text:
-        chunks = _chunk_text(txt, max_seq_length)
-
-        encoded_input = tokenizer(
-            chunks,
-            padding=True,
-            truncation=True,
-            return_tensors="pt",
-        )
-
-        with torch.no_grad():
-            model_output = model(**encoded_input)
-
-        embedding = _mean_pooling(model_output, encoded_input["attention_mask"])
-
-        if len(chunks) > 1:
-            list_of_embeddings.append(torch.mean(embedding, axis=0).numpy())  # type: ignore
-        else:
-            list_of_embeddings.append(embedding.numpy()[0])
-
-    embeddings_df = pd.DataFrame(list_of_embeddings)
-    embeddings_df.columns = [
-        "embedding-" + str(dimension) for dimension in range(embeddings_df.shape[1])
-    ]
-
-    return pd.concat([df, embeddings_df], axis=1)
-
-
-def _load_and_featurize_notes_per_year(
-    year: str,
-    note_types: Union[str, list[str]],
-    view: str,
-    n_rows: int,
-    featurizer: str,
-    featurizer_kwargs: dict,
-) -> pd.DataFrame:
-    """Loads clinical notes and features them.
-
-    Args:
-        note_types (Union[str, list[str]]): Which note types to load.
-        year (str): Which year to load
-        view (str): Which view to load
-        n_rows (int): How many rows to load
-        featurizer (str): Which featurizer to use (tfidf or huggingface)
-        featurizer_kwargs (dict): kwargs for the featurizer
-
-    Returns:
-        pd.DataFrame: Dataframe of notes and features
-    """
-
-    df = _load_notes_for_year(
-        note_types=note_types,
-        year=year,
-        view=view,
-        n_rows=n_rows,
-    )
-    if featurizer == "tfidf":
-        df = _tfidf_featurize(df, **featurizer_kwargs)
-    elif featurizer == "huggingface":
-        df = _huggingface_featurize(df, **featurizer_kwargs)
-    return df
-
-
-def load_and_featurize_notes(
-    note_types: Union[str, list[str]],
-    featurizer: str,
-    featurizer_kwargs: Optional[dict] = None,
-    n_rows: Optional[int] = None,
-) -> pd.DataFrame:
-    """Loads all clinical notes that match the specified note from all years.
-    Featurizes the notes using the specified featurizer (tf-idf or huggingface
-    model). Kwargs passed to.
-
-    Args:
-        note_types (Union[str, list[str]]): Which note types to load. See
-            `get_all_valid_note_types()` for valid note types.
-        featurizer (str): Which featurizer to use. Either 'tf-idf' or 'huggingface' or
-            `None` to return the raw text.
-        featurizer_kwargs (Optional[dict]): Kwargs passed to the featurizer. Defaults to None.
-            For tf-idf, this is `tfidf_path` to the vectorizer. For huggingface,
-            this is `model_id` to the model.
-        n_rows (Optional[int], optional): How many rows to load. Defaults to None.
-
-    Raises:
-        ValueError: If given invalid featurizer
-        ValueError: If given invlaid note type
-
-    Returns:
-        pd.DataFrame: Featurized clinical notes
-    """
-
-    valid_featurizers = {"tfidf", "huggingface", None}
-    if featurizer not in valid_featurizers:
-        raise ValueError(
-            f"featurizer must be one of {valid_featurizers}, got {featurizer}",
-        )
-
-    if isinstance(note_types, str):
-        note_types = list(note_types)  # pylint: disable=W0642
-    # check for invalid note types
-    if not set(note_types).issubset(get_all_valid_note_types()):
-        raise ValueError(
-            "Invalid note type. Valid note types are: "
-            + str(get_all_valid_note_types()),
-        )
-
-    # convert note_types to sql query
-    note_types = "('" + "', '".join(note_types) + "')"  # pylint: disable=W0642
-
-    view = "FOR_SFI_fritekst_resultat_udfoert_i_psykiatrien_aendret"
-
-    load_and_featurize = partial(
-        _load_and_featurize_notes_per_year,
-        note_types=note_types,
-        view=view,
-        n_rows=n_rows,
-        featurizer=featurizer,
-        featurizer_kwargs=featurizer_kwargs,
-    )
-
-    years = list(range(2011, 2022))
-
-    with Pool(processes=len(years)) as p:
-        dfs = p.map(load_and_featurize, [str(y) for y in years])
-
-    df = pd.concat(dfs)
-
-    df = df.rename(
-        {"datotid_senest_aendret_i_sfien": "timestamp", "fritekst": "text"},
-        axis=1,
-    )
-    return df
-
-
-@data_loaders.register("all_notes")
-def load_all_notes(
-    featurizer: str,
-    n_rows: Optional[int] = None,
-    featurizer_kwargs: Optional[dict] = None,
-) -> pd.DataFrame:
-    """Returns all notes from all years. Featurizes the notes using the
-    specified featurizer ('tfidf', 'huggingface', or `None` for raw text).
-    `featurizer_kwargs` are passed to the featurizer (e.g. "tfidf_path" for
-    tfidf, and "model_id" for huggingface).
-
-    Args:
-        featurizer (str): Which featurizer to use. Either 'tf-idf', 'huggingface', or None
-        n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
-        featurizer_kwargs (Optional[dict], optional): Keyword arguments passed to
-            the featurizer. Defaults to None.
-
-    Returns:
-        pd.DataFrame: (Featurized) notes
-    """
-    return load_and_featurize_notes(
-        note_types=get_all_valid_note_types(),
-        featurizer=featurizer,
-        n_rows=n_rows,
-        featurizer_kwargs=featurizer_kwargs,
-    )
-
-
-@data_loaders.register("aktuelt_psykisk")
-def load_aktuel_psykisk(
-    featurizer: str,
-    n_rows: Optional[int] = None,
-    featurizer_kwargs: Optional[dict] = None,
-) -> pd.DataFrame:
-    """Returns 'Aktuelt psykisk' notes from all years. Featurizes the notes
-    using the specified featurizer ('tfidf', 'huggingface', or `None` for raw
-    text). `featurizer_kwargs` are passed to the featurizer (e.g. "tfidf_path"
-    for tfidf, and "model_id" for huggingface).
-
-    Args:
-        featurizer (str): Which featurizer to use. Either 'tf-idf', 'huggingface', or None
-        n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
-        featurizer_kwargs (Optional[dict], optional): Keyword arguments passed to
-            the featurizer. Defaults to None.
-
-    Returns:
-        pd.DataFrame: (Featurized) notes
-    """
-    return load_and_featurize_notes(
-        note_types="Aktuelt psykisk",
-        featurizer=featurizer,
-        n_rows=n_rows,
-        featurizer_kwargs=featurizer_kwargs,
-    )
-
-
-@data_loaders.register("load_note_types")
-def load_arbitrary_notes(
-    note_names: Union[str, list[str]],
-    featurizer: str,
-    n_rows: Optional[int] = None,
-    featurizer_kwargs: Optional[dict] = None,
-) -> pd.DataFrame:
-    """Returns one or multiple note types from all years. Featurizes the notes
-    using the specified featurizer ('tfidf', 'huggingface', or `None` for raw
-    text). `featurizer_kwargs` are passed to the featurizer (e.g. "tfidf_path"
-    for tfidf, and "model_id" for huggingface).
-
-    Args:
-        note_names (Union[str, list[str]]): Which note types to load. See
-            `get_all_valid_note_types()` for a list of valid note types.
-        featurizer (str): Which featurizer to use. Either 'tf-idf', 'huggingface', or None
-        n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
-        featurizer_kwargs (Optional[dict], optional): Keyword arguments passed to
-            the featurizer. Defaults to None.
-
-    Returns:
-        pd.DataFrame: (Featurized) notes
-    """
-    return load_and_featurize_notes(
-        note_names,
-        featurizer=featurizer,
-        n_rows=n_rows,
-        featurizer_kwargs=featurizer_kwargs,
-    )
-
-
-@data_loaders.register("synth_notes")
-def load_synth_notes(featurizer: str, **featurizer_kwargs) -> pd.DataFrame:
-    """Load (featurized) synthetic notes for testing.
-
-    Args:
-        featurizer (str): Which featurizer to use
-        **featurizer_kwargs: Keyword arguments passed to the featurizer
-
-    Raises:
-        ValueError: If given invalid featurizer
-
-    Returns:
-        pd.DataFrame: (Featurized) synthetic notes
-    """
-    p = PROJECT_ROOT / "tests" / "test_data"
-    df = pd.read_csv(
-        p / "raw" / "synth_txt_data.csv",
-    ).drop("Unnamed: 0", axis=1)
-    df = df.dropna()
-    df["timestamp"] = pd.to_datetime(df["timestamp"])
-
-    if featurizer == "tfidf":
-        return _tfidf_featurize(
-            df,
-            tfidf_path=p / "test_tfidf" / "tfidf_10.pkl",
-        )
-    elif featurizer == "huggingface":
-        return _huggingface_featurize(
-            df,
-            **featurizer_kwargs,
-        )
+# def _huggingface_featurize(
+#     df: pd.DataFrame,
+#     model_id: str = "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
+#     text_col: str = "text",
+# ) -> pd.DataFrame:
+#     """Featurize text using a huggingface model and generate a dataframe with
+#     the embeddings. If the text is longer than the maximum sequence length of
+#     the model, the text is split into chunks and embeddings are averaged across
+#     chunks.
+
+#     Args:
+#         df (pd.DataFrame): Dataframe with text column
+#         model_id (str): Which huggingface model to use. See https://huggingface.co/models for a list of models. Assumes the model is a transformer model and has both a tokenizer and a model.
+#         text_col (str, optional): Name of text column. Defaults to "text".
+
+#     Returns:
+#         pd.DataFrame: Original dataframe with huggingface embeddings appended
+
+#     Example:
+#         >>> p = PROJECT_ROOT / "tests" / "test_data" / "raw"
+#         >>> huggingface_model_id = "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2"
+#         >>> df_p = p / "synth_txt_data.csv"
+
+#         >>> df = pd.read_csv(df_p)
+#         >>> df = df.dropna()
+
+#         >>> x = _huggingface_featurize(df, huggingface_model_id)
+#     """
+#     tokenizer = AutoTokenizer.from_pretrained(model_id)
+#     model = AutoModel.from_pretrained(model_id)
+
+#     df = df[df[text_col].notna()]
+#     text = df[text_col].values
+#     df = df.drop(text_col, axis=1)
+
+#     max_seq_length = int(
+#         tokenizer.model_max_length / 1.5,
+#     )  # allowing space for more word piece tokens than words in original sequence
+
+#     list_of_embeddings = []
+#     for txt in text:
+#         chunks = _chunk_text(txt, max_seq_length)
+
+#         encoded_input = tokenizer(
+#             chunks,
+#             padding=True,
+#             truncation=True,
+#             return_tensors="pt",
+#         )
+
+#         with torch.no_grad():
+#             model_output = model(**encoded_input)
+
+#         embedding = _mean_pooling(model_output, encoded_input["attention_mask"])
+
+#         if len(chunks) > 1:
+#             list_of_embeddings.append(torch.mean(embedding, axis=0).numpy())  # type: ignore
+#         else:
+#             list_of_embeddings.append(embedding.numpy()[0])
+
+#     embeddings_df = pd.DataFrame(list_of_embeddings)
+#     embeddings_df.columns = [
+#         "embedding-" + str(dimension) for dimension in range(embeddings_df.shape[1])
+#     ]
+
+#     return pd.concat([df, embeddings_df], axis=1)
+
+
+# def _load_and_featurize_notes_per_year(
+#     year: str,
+#     note_types: Union[str, list[str]],
+#     view: str,
+#     n_rows: int,
+#     featurizer: str,
+#     featurizer_kwargs: dict,
+# ) -> pd.DataFrame:
+#     """Loads clinical notes and features them.
+
+#     Args:
+#         note_types (Union[str, list[str]]): Which note types to load.
+#         year (str): Which year to load
+#         view (str): Which view to load
+#         n_rows (int): How many rows to load
+#         featurizer (str): Which featurizer to use (tfidf or huggingface)
+#         featurizer_kwargs (dict): kwargs for the featurizer
+
+#     Returns:
+#         pd.DataFrame: Dataframe of notes and features
+#     """
+
+#     df = _load_notes_for_year(
+#         note_types=note_types,
+#         year=year,
+#         view=view,
+#         n_rows=n_rows,
+#     )
+#     if featurizer == "tfidf":
+#         df = _tfidf_featurize(df, **featurizer_kwargs)
+#     elif featurizer == "huggingface":
+#         df = _huggingface_featurize(df, **featurizer_kwargs)
+#     return df
+
+
+# def load_and_featurize_notes(
+#     note_types: Union[str, list[str]],
+#     featurizer: str,
+#     featurizer_kwargs: Optional[dict] = None,
+#     n_rows: Optional[int] = None,
+# ) -> pd.DataFrame:
+#     """Loads all clinical notes that match the specified note from all years.
+#     Featurizes the notes using the specified featurizer (tf-idf or huggingface
+#     model). Kwargs passed to.
+
+#     Args:
+#         note_types (Union[str, list[str]]): Which note types to load. See
+#             `get_all_valid_note_types()` for valid note types.
+#         featurizer (str): Which featurizer to use. Either 'tf-idf' or 'huggingface' or
+#             `None` to return the raw text.
+#         featurizer_kwargs (Optional[dict]): Kwargs passed to the featurizer. Defaults to None.
+#             For tf-idf, this is `tfidf_path` to the vectorizer. For huggingface,
+#             this is `model_id` to the model.
+#         n_rows (Optional[int], optional): How many rows to load. Defaults to None.
+
+#     Raises:
+#         ValueError: If given invalid featurizer
+#         ValueError: If given invlaid note type
+
+#     Returns:
+#         pd.DataFrame: Featurized clinical notes
+#     """
+
+#     valid_featurizers = {"tfidf", "huggingface", None}
+#     if featurizer not in valid_featurizers:
+#         raise ValueError(
+#             f"featurizer must be one of {valid_featurizers}, got {featurizer}",
+#         )
+
+#     if isinstance(note_types, str):
+#         note_types = list(note_types)  # pylint: disable=W0642
+#     # check for invalid note types
+#     if not set(note_types).issubset(get_all_valid_note_types()):
+#         raise ValueError(
+#             "Invalid note type. Valid note types are: "
+#             + str(get_all_valid_note_types()),
+#         )
+
+#     # convert note_types to sql query
+#     note_types = "('" + "', '".join(note_types) + "')"  # pylint: disable=W0642
+
+#     view = "FOR_SFI_fritekst_resultat_udfoert_i_psykiatrien_aendret"
+
+#     load_and_featurize = partial(
+#         _load_and_featurize_notes_per_year,
+#         note_types=note_types,
+#         view=view,
+#         n_rows=n_rows,
+#         featurizer=featurizer,
+#         featurizer_kwargs=featurizer_kwargs,
+#     )
+
+#     years = list(range(2011, 2022))
+
+#     with Pool(processes=len(years)) as p:
+#         dfs = p.map(load_and_featurize, [str(y) for y in years])
+
+#     df = pd.concat(dfs)
+
+#     df = df.rename(
+#         {"datotid_senest_aendret_i_sfien": "timestamp", "fritekst": "text"},
+#         axis=1,
+#     )
+#     return df
+
+
+# @data_loaders.register("all_notes")
+# def load_all_notes(
+#     featurizer: str,
+#     n_rows: Optional[int] = None,
+#     featurizer_kwargs: Optional[dict] = None,
+# ) -> pd.DataFrame:
+#     """Returns all notes from all years. Featurizes the notes using the
+#     specified featurizer ('tfidf', 'huggingface', or `None` for raw text).
+#     `featurizer_kwargs` are passed to the featurizer (e.g. "tfidf_path" for
+#     tfidf, and "model_id" for huggingface).
+
+#     Args:
+#         featurizer (str): Which featurizer to use. Either 'tf-idf', 'huggingface', or None
+#         n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
+#         featurizer_kwargs (Optional[dict], optional): Keyword arguments passed to
+#             the featurizer. Defaults to None.
+
+#     Returns:
+#         pd.DataFrame: (Featurized) notes
+#     """
+#     return load_and_featurize_notes(
+#         note_types=get_all_valid_note_types(),
+#         featurizer=featurizer,
+#         n_rows=n_rows,
+#         featurizer_kwargs=featurizer_kwargs,
+#     )
+
+
+# @data_loaders.register("aktuelt_psykisk")
+# def load_aktuel_psykisk(
+#     featurizer: str,
+#     n_rows: Optional[int] = None,
+#     featurizer_kwargs: Optional[dict] = None,
+# ) -> pd.DataFrame:
+#     """Returns 'Aktuelt psykisk' notes from all years. Featurizes the notes
+#     using the specified featurizer ('tfidf', 'huggingface', or `None` for raw
+#     text). `featurizer_kwargs` are passed to the featurizer (e.g. "tfidf_path"
+#     for tfidf, and "model_id" for huggingface).
+
+#     Args:
+#         featurizer (str): Which featurizer to use. Either 'tf-idf', 'huggingface', or None
+#         n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
+#         featurizer_kwargs (Optional[dict], optional): Keyword arguments passed to
+#             the featurizer. Defaults to None.
+
+#     Returns:
+#         pd.DataFrame: (Featurized) notes
+#     """
+#     return load_and_featurize_notes(
+#         note_types="Aktuelt psykisk",
+#         featurizer=featurizer,
+#         n_rows=n_rows,
+#         featurizer_kwargs=featurizer_kwargs,
+#     )
+
+
+# @data_loaders.register("load_note_types")
+# def load_arbitrary_notes(
+#     note_names: Union[str, list[str]],
+#     featurizer: str,
+#     n_rows: Optional[int] = None,
+#     featurizer_kwargs: Optional[dict] = None,
+# ) -> pd.DataFrame:
+#     """Returns one or multiple note types from all years. Featurizes the notes
+#     using the specified featurizer ('tfidf', 'huggingface', or `None` for raw
+#     text). `featurizer_kwargs` are passed to the featurizer (e.g. "tfidf_path"
+#     for tfidf, and "model_id" for huggingface).
+
+#     Args:
+#         note_names (Union[str, list[str]]): Which note types to load. See
+#             `get_all_valid_note_types()` for a list of valid note types.
+#         featurizer (str): Which featurizer to use. Either 'tf-idf', 'huggingface', or None
+#         n_rows (Optional[int], optional): Number of rows to load. Defaults to None.
+#         featurizer_kwargs (Optional[dict], optional): Keyword arguments passed to
+#             the featurizer. Defaults to None.
+
+#     Returns:
+#         pd.DataFrame: (Featurized) notes
+#     """
+#     return load_and_featurize_notes(
+#         note_names,
+#         featurizer=featurizer,
+#         n_rows=n_rows,
+#         featurizer_kwargs=featurizer_kwargs,
+#     )
+
+
+# @data_loaders.register("synth_notes")
+# def load_synth_notes(featurizer: str, **featurizer_kwargs) -> pd.DataFrame:
+#     """Load (featurized) synthetic notes for testing.
+
+#     Args:
+#         featurizer (str): Which featurizer to use
+#         **featurizer_kwargs: Keyword arguments passed to the featurizer
+
+#     Raises:
+#         ValueError: If given invalid featurizer
+
+#     Returns:
+#         pd.DataFrame: (Featurized) synthetic notes
+#     """
+#     p = PROJECT_ROOT / "tests" / "test_data"
+#     df = pd.read_csv(
+#         p / "raw" / "synth_txt_data.csv",
+#     ).drop("Unnamed: 0", axis=1)
+#     df = df.dropna()
+#     df["timestamp"] = pd.to_datetime(df["timestamp"])
+
+#     if featurizer == "tfidf":
+#         return _tfidf_featurize(
+#             df,
+#             tfidf_path=p / "test_tfidf" / "tfidf_10.pkl",
+#         )
+#     elif featurizer == "huggingface":
+#         return _huggingface_featurize(
+#             df,
+#             **featurizer_kwargs,
+#         )
 
-    raise ValueError("Only tfidf or huggingface featurizer supported for synth notes")
+#     raise ValueError("Only tfidf or huggingface featurizer supported for synth notes")
```

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/load_visits.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/load_visits.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/sql_load.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/sql_load.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/t2d_loaders.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/t2d_loaders.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/raw/utils.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/raw/utils.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/loaders/synth/raw/load_synth_data.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/loaders/synth/raw/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/feature_spec_objects.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/feature_spec_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,14 +262,27 @@
 
     allowed_nan_value_prop: list[float] = [0.0]
     # If NaN is higher than this in the input dataframe during resolution, raise an error.
 
     def __init__(self, **data):
         super().__init__(**data)
 
+        # Check that all passed loaders are valid
+        invalid_loaders = list(
+            set(self.values_loader) - set(data_loaders.get_all().keys())
+        )
+        if len(invalid_loaders) != 0:
+            nl = "\n"  # New line variable as f-string can't handle backslashes
+            raise ValueError(
+                f"""Some loader strings could not be resolved in the data_loaders catalogue. Did you make a typo? If you want to add your own loaders to the catalogue, see explosion / catalogue on GitHub for info. 
+                {nl*2}Loaders that could not be resolved:"""
+                f"""{nl}{nl.join(str(loader) for loader in invalid_loaders)}{nl}{nl}"""
+                f"""Available loaders:{nl}{nl.join(str(loader) for loader in data_loaders.get_all().keys())}"""
+            )
+
         if self.output_col_name_override:
             input_col_name = (
                 "value"
                 if not self.input_col_name_override
                 else self.input_col_name_override
             )
 
@@ -306,14 +319,15 @@
     feature_group_spec: MinGroupSpec,
     output_class: AnySpec,
 ) -> list[AnySpec]:
     """Create a list of specs from a GroupSpec."""
 
     # Create all combinations of top level elements
     # For each attribute in the FeatureGroupSpec
+
     feature_group_spec_dict = feature_group_spec.__dict__
 
     permuted_dicts = create_feature_combinations_from_dict(d=feature_group_spec_dict)
 
     return [output_class(**d) for d in permuted_dicts]  # type: ignore
```

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/flattened_dataset.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/flattened_ds_validator.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/timeseriesflattener/resolve_multiple_functions.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/timeseriesflattener/resolve_multiple_functions.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/utils.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/utils.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/src/psycop_feature_generation/utils_for_testing.py` & `psycop_feature_generation-0.9.0/src/psycop_feature_generation/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `psycop_feature_generation-0.8.0/setup.py` & `psycop_feature_generation-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,21 @@
  'psycopmlutils>=0.2.4,<0.3.0',
  'pyarrow>=9.0.0,<9.1.0',
  'pydantic>=1.9.0,<1.10.0',
  'pyodbc>=4.0.34,<4.0.36',
  'scikit-learn>=1.1.2,<1.1.3',
  'scipy>=1.8.0,<1.9.4',
  'srsly>=2.4.4,<2.4.6',
- 'torch>=1.12.1,<2.0.0',
  'transformers>=4.22.2,<5.0.0',
  'wandb>=0.12.0,<0.13.5',
  'wasabi>=0.9.1,<0.10.2']
 
 setup_kwargs = {
     'name': 'psycop-feature-generation',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': '',
     'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psycop_feature_generation-0.8.0/PKG-INFO` & `psycop_feature_generation-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycop-feature-generation
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,11 +21,10 @@
 Requires-Dist: psycopmlutils (>=0.2.4,<0.3.0)
 Requires-Dist: pyarrow (>=9.0.0,<9.1.0)
 Requires-Dist: pydantic (>=1.9.0,<1.10.0)
 Requires-Dist: pyodbc (>=4.0.34,<4.0.36)
 Requires-Dist: scikit-learn (>=1.1.2,<1.1.3)
 Requires-Dist: scipy (>=1.8.0,<1.9.4)
 Requires-Dist: srsly (>=2.4.4,<2.4.6)
-Requires-Dist: torch (>=1.12.1,<2.0.0)
 Requires-Dist: transformers (>=4.22.2,<5.0.0)
 Requires-Dist: wandb (>=0.12.0,<0.13.5)
 Requires-Dist: wasabi (>=0.9.1,<0.10.2)
```

