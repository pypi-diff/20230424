# Comparing `tmp/dai_python_commons-4.8.1.tar.gz` & `tmp/dai_python_commons-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dai_python_commons-4.8.1.tar", max compression
+gzip compressed data, was "dai_python_commons-4.9.0.tar", max compression
```

## Comparing `dai_python_commons-4.8.1.tar` & `dai_python_commons-4.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      108 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/__init__.py
--rw-r--r--   0        0        0     1353 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/cloudwatch_utils.py
--rw-r--r--   0        0        0     4383 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/dai_error.py
--rw-r--r--   0        0        0     2390 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/event_bridge.py
--rw-r--r--   0        0        0     5269 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/glue_utils.py
--rw-r--r--   0        0        0     1660 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/logging_utils.py
--rw-r--r--   0        0        0    10203 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/parquet_utils.py
--rw-r--r--   0        0        0    23860 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/s3_event_object_copy.py
--rw-r--r--   0        0        0     7285 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/s3_utils.py
--rw-r--r--   0        0        0     2391 2023-01-27 10:14:19.960411 dai_python_commons-4.8.1/dai_python_commons/time_utils.py
--rw-r--r--   0        0        0      782 2023-01-27 10:14:19.964411 dai_python_commons-4.8.1/pyproject.toml
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 dai_python_commons-4.8.1/setup.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 dai_python_commons-4.8.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/__init__.py
+-rw-r--r--   0        0        0     1372 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/cloudwatch_utils.py
+-rw-r--r--   0        0        0     4383 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/dai_error.py
+-rw-r--r--   0        0        0     2390 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/event_bridge.py
+-rw-r--r--   0        0        0     5269 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/glue_utils.py
+-rw-r--r--   0        0        0     1660 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/logging_utils.py
+-rw-r--r--   0        0        0    10203 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/parquet_utils.py
+-rw-r--r--   0        0        0    23860 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/s3_event_object_copy.py
+-rw-r--r--   0        0        0     7285 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/s3_utils.py
+-rw-r--r--   0        0        0     2391 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/dai_python_commons/time_utils.py
+-rw-r--r--   0        0        0      782 2023-02-21 14:36:00.478572 dai_python_commons-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 dai_python_commons-4.9.0/setup.py
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 dai_python_commons-4.9.0/PKG-INFO
```

### Comparing `dai_python_commons-4.8.1/dai_python_commons/cloudwatch_utils.py` & `dai_python_commons-4.9.0/dai_python_commons/cloudwatch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         Increase counter for our dai-code metric for its kind of action in cloudwatch.
 
         :param cw_client: A boto3.client("cloudwatch") to use to write the logs
         :param metric_name: Which counter to increase
         :param dai_code: The dai_code (e.g. `tr-tms-obs-0008`) which will be used for setting the dimension of the metric
         :param function_name: The lambda name which will be used for setting the namespace of the metric
         """
-        allowed_metric_names = ["invocation", "error"]
+        allowed_metric_names = ["invocation", "error", "validationError"]
         if metric_name not in allowed_metric_names:
             raise DaiInputError(f"{metric_name} not in {allowed_metric_names}")
 
         cw_client.put_metric_data(
             Namespace=f"DAI/Lambda/{function_name}",
             MetricData=[
                 {
```

### Comparing `dai_python_commons-4.8.1/dai_python_commons/dai_error.py` & `dai_python_commons-4.9.0/dai_python_commons/dai_error.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/dai_python_commons/event_bridge.py` & `dai_python_commons-4.9.0/dai_python_commons/event_bridge.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/dai_python_commons/glue_utils.py` & `dai_python_commons-4.9.0/dai_python_commons/glue_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/dai_python_commons/logging_utils.py` & `dai_python_commons-4.9.0/dai_python_commons/logging_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/dai_python_commons/parquet_utils.py` & `dai_python_commons-4.9.0/dai_python_commons/parquet_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/dai_python_commons/s3_event_object_copy.py` & `dai_python_commons-4.9.0/dai_python_commons/s3_event_object_copy.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/dai_python_commons/s3_utils.py` & `dai_python_commons-4.9.0/dai_python_commons/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/dai_python_commons/time_utils.py` & `dai_python_commons-4.9.0/dai_python_commons/time_utils.py`

 * *Files identical despite different names*

### Comparing `dai_python_commons-4.8.1/pyproject.toml` & `dai_python_commons-4.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dai-python-commons"
-version = "4.8.1"
+version = "4.9.0"
 description = "Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration."
 authors = []
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 loguru = "^0.6.0"
 boto3 = "^1.18.31"
```

### Comparing `dai_python_commons-4.8.1/setup.py` & `dai_python_commons-4.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = \
 {'data-consolidation': ['pyarrow==3.0.0', 's3fs==0.4.2'],
  'glue': ['awswrangler==2.18.0', 'cryptography==38.0.1']}
 
 setup_kwargs = {
     'name': 'dai-python-commons',
-    'version': '4.8.1',
+    'version': '4.9.0',
     'description': 'Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration.',
     'long_description': 'None',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dai_python_commons-4.8.1/PKG-INFO` & `dai_python_commons-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dai-python-commons
-Version: 4.8.1
+Version: 4.9.0
 Summary: Collection of small python utilities useful for lambda functions or glue jobs. By the Stockholm Public Transport Administration.
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

