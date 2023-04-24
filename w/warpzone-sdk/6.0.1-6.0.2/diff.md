# Comparing `tmp/warpzone_sdk-6.0.1.tar.gz` & `tmp/warpzone_sdk-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-6.0.1.tar", max compression
+gzip compressed data, was "warpzone_sdk-6.0.2.tar", max compression
```

## Comparing `warpzone_sdk-6.0.1.tar` & `warpzone_sdk-6.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1121 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/pyproject.toml
--rw-r--r--   0        0        0     1185 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2877 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      187 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1501 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/functionize.py
--rw-r--r--   0        0        0     2606 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/monitor.py
--rw-r--r--   0        0        0     1486 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/process.py
--rw-r--r--   0        0        0       32 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0     1337 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1379 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/signature.py
--rw-r--r--   0        0        0       80 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5433 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       47 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/tablestorage/__init__.py
--rw-r--r--   0        0        0     2882 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/tablestorage/client.py
--rw-r--r--   0        0        0     2509 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/tablestorage/client_async.py
--rw-r--r--   0        0        0      521 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/tablestorage/helpers.py
--rw-r--r--   0        0        0     2446 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/tablestorage/operations.py
--rw-r--r--   0        0        0      176 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3499 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/testing/data.py
--rw-r--r--   0        0        0       19 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-04-20 06:58:37.328157 warpzone_sdk-6.0.1/warpzone/transform/data.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-04-24 06:27:18.750425 warpzone_sdk-6.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2877 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1501 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     2606 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     1486 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/process.py
+-rw-r--r--   0        0        0       32 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0     1337 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1379 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/signature.py
+-rw-r--r--   0        0        0       80 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5433 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       47 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/__init__.py
+-rw-r--r--   0        0        0     2882 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/client.py
+-rw-r--r--   0        0        0     2509 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/client_async.py
+-rw-r--r--   0        0        0      521 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/helpers.py
+-rw-r--r--   0        0        0     2470 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/tablestorage/operations.py
+-rw-r--r--   0        0        0      176 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3499 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/testing/data.py
+-rw-r--r--   0        0        0       19 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-04-24 06:27:18.754425 warpzone_sdk-6.0.2/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.2/PKG-INFO
```

### Comparing `warpzone_sdk-6.0.1/pyproject.toml` & `warpzone_sdk-6.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "6.0.1"
+version = "6.0.2"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Anders Launer Baek-Petersen <alp@energinet.dk>", "Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-6.0.1/warpzone/__init__.py` & `warpzone_sdk-6.0.2/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/blobstorage/client.py` & `warpzone_sdk-6.0.2/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/function/functionize.py` & `warpzone_sdk-6.0.2/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/function/integrations.py` & `warpzone_sdk-6.0.2/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/function/monitor.py` & `warpzone_sdk-6.0.2/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/function/process.py` & `warpzone_sdk-6.0.2/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/function/processors/outputs.py` & `warpzone_sdk-6.0.2/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/function/processors/triggers.py` & `warpzone_sdk-6.0.2/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/function/signature.py` & `warpzone_sdk-6.0.2/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/healthchecks/__init__.py` & `warpzone_sdk-6.0.2/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/healthchecks/model.py` & `warpzone_sdk-6.0.2/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/monitor/logs.py` & `warpzone_sdk-6.0.2/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/monitor/traces.py` & `warpzone_sdk-6.0.2/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/servicebus/data/client.py` & `warpzone_sdk-6.0.2/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/servicebus/events/client.py` & `warpzone_sdk-6.0.2/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/tablestorage/client.py` & `warpzone_sdk-6.0.2/warpzone/tablestorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/tablestorage/client_async.py` & `warpzone_sdk-6.0.2/warpzone/tablestorage/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/tablestorage/helpers.py` & `warpzone_sdk-6.0.2/warpzone/tablestorage/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/tablestorage/operations.py` & `warpzone_sdk-6.0.2/warpzone/tablestorage/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     ):
         datetime_columns = df.select_dtypes(["datetime", "datetimetz"]).columns
 
         for column in datetime_columns:
             df[column] = df[column].dt.strftime("%Y-%m-%dT%H:%M:%SZ")
             df[f"{column}@odata.type"] = "Edm.DateTime"
 
-        df["PartitionKey"] = df[partition_keys].agg("_".join, axis=1)
-        df["RowKey"] = df[row_keys].agg("_".join, axis=1)
+        df["PartitionKey"] = df[partition_keys].astype(str).agg("_".join, axis=1)
+        df["RowKey"] = df[row_keys].astype(str).agg("_".join, axis=1)
 
         operations = cls()
         for _, partition_group in df.groupby(partition_keys):
             entities = partition_group.to_dict("records")
             operations.add(entities, operation_type)
 
         return operations
```

### Comparing `warpzone_sdk-6.0.1/warpzone/testing/assertions.py` & `warpzone_sdk-6.0.2/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/testing/data.py` & `warpzone_sdk-6.0.2/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/warpzone/transform/data.py` & `warpzone_sdk-6.0.2/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-6.0.1/PKG-INFO` & `warpzone_sdk-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 6.0.1
+Version: 6.0.2
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Anders Launer Baek-Petersen
 Author-email: alp@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

