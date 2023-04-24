# Comparing `tmp/preemo_worker_sdk-0.4.1.tar.gz` & `tmp/preemo_worker_sdk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preemo_worker_sdk-0.4.1.tar", max compression
+gzip compressed data, was "preemo_worker_sdk-0.4.2.tar", max compression
```

## Comparing `preemo_worker_sdk-0.4.1.tar` & `preemo_worker_sdk-0.4.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.4.1/LICENSE
--rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.4.1/README.md
--rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.4.1/preemo/__init__.py
--rw-r--r--   0        0        0      306 2023-04-20 22:13:04.242370 preemo_worker_sdk-0.4.1/preemo/gen/__init__.py
--rw-r--r--   0        0        0      306 2023-04-20 22:13:04.242697 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/__init__.py
--rw-r--r--   0        0        0     4333 2023-04-21 16:59:41.866999 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py
--rw-r--r--   0        0        0     7285 2023-04-21 16:59:41.867117 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi
--rw-r--r--   0        0        0     3035 2023-04-21 16:59:41.867661 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_create_artifact_pb2.py
--rw-r--r--   0        0        0     6629 2023-04-21 16:59:41.867943 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
--rw-r--r--   0        0        0     2642 2023-04-20 22:13:04.136336 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_execute_function_pb2.py
--rw-r--r--   0        0        0     4134 2023-04-20 22:13:04.257705 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_execute_function_pb2.pyi
--rw-r--r--   0        0        0     2837 2023-04-20 22:13:04.136444 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
--rw-r--r--   0        0        0     5106 2023-04-21 16:59:41.868456 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
--rw-r--r--   0        0        0     4502 2023-04-21 16:59:41.868856 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py
--rw-r--r--   0        0        0     7767 2023-04-21 16:59:41.869023 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-04-20 22:13:04.136642 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_pb2.py
--rw-r--r--   0        0        0     5686 2023-04-21 16:59:41.869205 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
--rw-r--r--   0        0        0     4409 2023-04-21 16:59:41.869446 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py
--rw-r--r--   0        0        0     7699 2023-04-21 16:59:41.869645 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi
--rw-r--r--   0        0        0     1382 2023-04-20 22:13:04.136842 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/check_function_pb2.py
--rw-r--r--   0        0        0     1811 2023-04-20 22:13:04.280322 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/check_function_pb2.pyi
--rw-r--r--   0        0        0     1665 2023-04-20 22:13:04.136937 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/execute_function_pb2.py
--rw-r--r--   0        0        0     3019 2023-04-20 22:13:04.284329 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/execute_function_pb2.pyi
--rw-r--r--   0        0        0     1128 2023-04-20 22:13:04.137055 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/header_pb2.py
--rw-r--r--   0        0        0     1515 2023-04-20 22:13:04.288198 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/header_pb2.pyi
--rw-r--r--   0        0        0     1403 2023-04-20 22:13:04.137163 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/register_function_pb2.py
--rw-r--r--   0        0        0     1721 2023-04-20 22:13:04.292227 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/register_function_pb2.pyi
--rw-r--r--   0        0        0     1222 2023-04-20 22:13:04.137267 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/sdk_server_ready_pb2.py
--rw-r--r--   0        0        0     1539 2023-04-20 22:13:04.296209 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
--rw-r--r--   0        0        0     1085 2023-04-20 22:13:04.137366 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/terminate_pb2.py
--rw-r--r--   0        0        0      786 2023-04-20 22:13:04.300561 preemo_worker_sdk-0.4.1/preemo/gen/endpoints/terminate_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-20 22:13:04.243206 preemo_worker_sdk-0.4.1/preemo/gen/models/__init__.py
--rw-r--r--   0        0        0     1104 2023-04-21 16:59:41.869910 preemo_worker_sdk-0.4.1/preemo/gen/models/artifact_type_pb2.py
--rw-r--r--   0        0        0     1129 2023-04-21 16:59:41.870254 preemo_worker_sdk-0.4.1/preemo/gen/models/artifact_type_pb2.pyi
--rw-r--r--   0        0        0     1135 2023-04-20 22:13:04.137575 preemo_worker_sdk-0.4.1/preemo/gen/models/registered_function_pb2.py
--rw-r--r--   0        0        0     1624 2023-04-20 22:13:04.311020 preemo_worker_sdk-0.4.1/preemo/gen/models/registered_function_pb2.pyi
--rw-r--r--   0        0        0     1174 2023-04-20 22:13:04.137675 preemo_worker_sdk-0.4.1/preemo/gen/models/value_pb2.py
--rw-r--r--   0        0        0     1396 2023-04-20 22:13:04.318152 preemo_worker_sdk-0.4.1/preemo/gen/models/value_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-20 22:13:04.243405 preemo_worker_sdk-0.4.1/preemo/gen/services/__init__.py
--rw-r--r--   0        0        0     4369 2023-04-20 22:13:04.235240 preemo_worker_sdk-0.4.1/preemo/gen/services/sdk_pb2_grpc.py
--rw-r--r--   0        0        0     1302 2023-04-20 22:13:04.322250 preemo_worker_sdk-0.4.1/preemo/gen/services/sdk_pb2_grpc.pyi
--rw-r--r--   0        0        0    21861 2023-04-21 16:59:41.870861 preemo_worker_sdk-0.4.1/preemo/gen/services/worker_pb2_grpc.py
--rw-r--r--   0        0        0     6536 2023-04-21 16:59:41.871238 preemo_worker_sdk-0.4.1/preemo/gen/services/worker_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.4.1/preemo/py.typed
--rw-r--r--   0        0        0     2559 2023-04-20 22:59:58.827517 preemo_worker_sdk-0.4.1/preemo/worker/__init__.py
--rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.4.1/preemo/worker/__init__.pyi
--rw-r--r--   0        0        0    13221 2023-04-21 16:59:41.871754 preemo_worker_sdk-0.4.1/preemo/worker/_artifact_manager.py
--rw-r--r--   0        0        0     1748 2023-04-20 22:59:58.827942 preemo_worker_sdk-0.4.1/preemo/worker/_env_manager.py
--rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.4.1/preemo/worker/_function_registry.py
--rw-r--r--   0        0        0    11315 2023-04-21 16:59:41.872373 preemo_worker_sdk-0.4.1/preemo/worker/_messaging_client.py
--rw-r--r--   0        0        0     2538 2023-04-10 22:31:00.968657 preemo_worker_sdk-0.4.1/preemo/worker/_sdk_server.py
--rw-r--r--   0        0        0     3581 2023-04-21 16:59:41.872685 preemo_worker_sdk-0.4.1/preemo/worker/_sdk_service.py
--rw-r--r--   0        0        0     1222 2023-03-22 21:19:28.059400 preemo_worker_sdk-0.4.1/preemo/worker/_types.py
--rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.4.1/preemo/worker/_validation.py
--rw-r--r--   0        0        0     7044 2023-04-21 16:59:41.872944 preemo_worker_sdk-0.4.1/preemo/worker/_worker_client.py
--rw-r--r--   0        0        0     1718 2023-04-21 23:38:57.192956 preemo_worker_sdk-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.4.2/README.md
+-rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.4.2/preemo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.242370 preemo_worker_sdk-0.4.2/preemo/gen/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.242697 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/__init__.py
+-rw-r--r--   0        0        0     4333 2023-04-21 16:59:41.866999 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py
+-rw-r--r--   0        0        0     7285 2023-04-21 16:59:41.867117 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi
+-rw-r--r--   0        0        0     3035 2023-04-21 16:59:41.867661 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_create_artifact_pb2.py
+-rw-r--r--   0        0        0     6629 2023-04-21 16:59:41.867943 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
+-rw-r--r--   0        0        0     2642 2023-04-20 22:13:04.136336 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_execute_function_pb2.py
+-rw-r--r--   0        0        0     4134 2023-04-20 22:13:04.257705 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_execute_function_pb2.pyi
+-rw-r--r--   0        0        0     2837 2023-04-20 22:13:04.136444 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
+-rw-r--r--   0        0        0     5106 2023-04-21 16:59:41.868456 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4502 2023-04-21 16:59:41.868856 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py
+-rw-r--r--   0        0        0     7767 2023-04-21 16:59:41.869023 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-04-20 22:13:04.136642 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_pb2.py
+-rw-r--r--   0        0        0     5686 2023-04-21 16:59:41.869205 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4409 2023-04-21 16:59:41.869446 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py
+-rw-r--r--   0        0        0     7699 2023-04-21 16:59:41.869645 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi
+-rw-r--r--   0        0        0     1382 2023-04-20 22:13:04.136842 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/check_function_pb2.py
+-rw-r--r--   0        0        0     1811 2023-04-20 22:13:04.280322 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/check_function_pb2.pyi
+-rw-r--r--   0        0        0     1665 2023-04-20 22:13:04.136937 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/execute_function_pb2.py
+-rw-r--r--   0        0        0     3019 2023-04-20 22:13:04.284329 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/execute_function_pb2.pyi
+-rw-r--r--   0        0        0     1128 2023-04-20 22:13:04.137055 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/header_pb2.py
+-rw-r--r--   0        0        0     1515 2023-04-20 22:13:04.288198 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/header_pb2.pyi
+-rw-r--r--   0        0        0     1403 2023-04-20 22:13:04.137163 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/register_function_pb2.py
+-rw-r--r--   0        0        0     1721 2023-04-20 22:13:04.292227 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/register_function_pb2.pyi
+-rw-r--r--   0        0        0     1222 2023-04-20 22:13:04.137267 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/sdk_server_ready_pb2.py
+-rw-r--r--   0        0        0     1539 2023-04-20 22:13:04.296209 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
+-rw-r--r--   0        0        0     1085 2023-04-20 22:13:04.137366 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/terminate_pb2.py
+-rw-r--r--   0        0        0      786 2023-04-20 22:13:04.300561 preemo_worker_sdk-0.4.2/preemo/gen/endpoints/terminate_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.243206 preemo_worker_sdk-0.4.2/preemo/gen/models/__init__.py
+-rw-r--r--   0        0        0     1104 2023-04-21 16:59:41.869910 preemo_worker_sdk-0.4.2/preemo/gen/models/artifact_type_pb2.py
+-rw-r--r--   0        0        0     1129 2023-04-21 16:59:41.870254 preemo_worker_sdk-0.4.2/preemo/gen/models/artifact_type_pb2.pyi
+-rw-r--r--   0        0        0     1135 2023-04-20 22:13:04.137575 preemo_worker_sdk-0.4.2/preemo/gen/models/registered_function_pb2.py
+-rw-r--r--   0        0        0     1624 2023-04-20 22:13:04.311020 preemo_worker_sdk-0.4.2/preemo/gen/models/registered_function_pb2.pyi
+-rw-r--r--   0        0        0     1174 2023-04-20 22:13:04.137675 preemo_worker_sdk-0.4.2/preemo/gen/models/value_pb2.py
+-rw-r--r--   0        0        0     1396 2023-04-20 22:13:04.318152 preemo_worker_sdk-0.4.2/preemo/gen/models/value_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.243405 preemo_worker_sdk-0.4.2/preemo/gen/services/__init__.py
+-rw-r--r--   0        0        0     4369 2023-04-20 22:13:04.235240 preemo_worker_sdk-0.4.2/preemo/gen/services/sdk_pb2_grpc.py
+-rw-r--r--   0        0        0     1302 2023-04-20 22:13:04.322250 preemo_worker_sdk-0.4.2/preemo/gen/services/sdk_pb2_grpc.pyi
+-rw-r--r--   0        0        0    21861 2023-04-21 16:59:41.870861 preemo_worker_sdk-0.4.2/preemo/gen/services/worker_pb2_grpc.py
+-rw-r--r--   0        0        0     6536 2023-04-21 16:59:41.871238 preemo_worker_sdk-0.4.2/preemo/gen/services/worker_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.4.2/preemo/py.typed
+-rw-r--r--   0        0        0     2559 2023-04-20 22:59:58.827517 preemo_worker_sdk-0.4.2/preemo/worker/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.4.2/preemo/worker/__init__.pyi
+-rw-r--r--   0        0        0    13221 2023-04-21 16:59:41.871754 preemo_worker_sdk-0.4.2/preemo/worker/_artifact_manager.py
+-rw-r--r--   0        0        0     1748 2023-04-20 22:59:58.827942 preemo_worker_sdk-0.4.2/preemo/worker/_env_manager.py
+-rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.4.2/preemo/worker/_function_registry.py
+-rw-r--r--   0        0        0    11315 2023-04-21 16:59:41.872373 preemo_worker_sdk-0.4.2/preemo/worker/_messaging_client.py
+-rw-r--r--   0        0        0     2538 2023-04-10 22:31:00.968657 preemo_worker_sdk-0.4.2/preemo/worker/_sdk_server.py
+-rw-r--r--   0        0        0     3581 2023-04-21 16:59:41.872685 preemo_worker_sdk-0.4.2/preemo/worker/_sdk_service.py
+-rw-r--r--   0        0        0     1222 2023-03-22 21:19:28.059400 preemo_worker_sdk-0.4.2/preemo/worker/_types.py
+-rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.4.2/preemo/worker/_validation.py
+-rw-r--r--   0        0        0     7044 2023-04-21 16:59:41.872944 preemo_worker_sdk-0.4.2/preemo/worker/_worker_client.py
+-rw-r--r--   0        0        0     1852 2023-04-24 17:48:46.314212 preemo_worker_sdk-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.4.2/PKG-INFO
```

### Comparing `preemo_worker_sdk-0.4.1/LICENSE` & `preemo_worker_sdk-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/README.md` & `preemo_worker_sdk-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_create_artifact_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_create_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_create_artifact_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_execute_function_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_execute_function_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/check_function_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/check_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/check_function_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/check_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/execute_function_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/execute_function_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/header_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/header_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/header_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/header_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/register_function_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/register_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/register_function_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/register_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/sdk_server_ready_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/sdk_server_ready_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/sdk_server_ready_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/sdk_server_ready_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/terminate_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/terminate_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/endpoints/terminate_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/endpoints/terminate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/models/artifact_type_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/models/artifact_type_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/models/artifact_type_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/models/artifact_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/models/registered_function_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/models/registered_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/models/registered_function_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/models/registered_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/models/value_pb2.py` & `preemo_worker_sdk-0.4.2/preemo/gen/models/value_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/models/value_pb2.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/models/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/services/sdk_pb2_grpc.py` & `preemo_worker_sdk-0.4.2/preemo/gen/services/sdk_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/services/sdk_pb2_grpc.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/services/sdk_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/services/worker_pb2_grpc.py` & `preemo_worker_sdk-0.4.2/preemo/gen/services/worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/gen/services/worker_pb2_grpc.pyi` & `preemo_worker_sdk-0.4.2/preemo/gen/services/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/__init__.py` & `preemo_worker_sdk-0.4.2/preemo/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/__init__.pyi` & `preemo_worker_sdk-0.4.2/preemo/worker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_artifact_manager.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_artifact_manager.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_env_manager.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_env_manager.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_function_registry.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_function_registry.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_messaging_client.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_messaging_client.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_sdk_server.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_sdk_server.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_sdk_service.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_sdk_service.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_types.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_types.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_validation.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_validation.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/preemo/worker/_worker_client.py` & `preemo_worker_sdk-0.4.2/preemo/worker/_worker_client.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.4.1/pyproject.toml` & `preemo_worker_sdk-0.4.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "preemo_worker_sdk"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 license = "MIT"
 authors = [
   "Forrest Moret <forrest@preemo.io>",
   "Adrian Miguel <adrian@preemo.io>",
 ]
 readme = "README.md"
@@ -15,20 +15,21 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 packages = [
   { include = "preemo" },
 ]
 
+# TODO(adrian@preemo.io, 05/01/2023): Push these versions as low as possible to make it easier for users to meet the requirements
 [tool.poetry.dependencies]
-grpcio = "1.51.3"
-protobuf = "4.21.12"
-pydantic = "1.10.6"
+grpcio = "^1.51.3"
+protobuf = "^4.21.12"
+pydantic = "^1.10.6"
 python = "^3.8.13"
-requests = "2.28.2"
+requests = "^2.28.2"
 
 [tool.poetry.dev-dependencies]
 autoflake = "2.0.1"
 black = "22.3.0"
 build = "0.10.0"
 flake8 = "6.0.0"
 grpc-stubs = "1.24.12"
```

### Comparing `preemo_worker_sdk-0.4.1/PKG-INFO` & `preemo_worker_sdk-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: preemo-worker-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Home-page: https://www.preemo.io/
 License: MIT
 Author: Forrest Moret
 Author-email: forrest@preemo.io
 Requires-Python: >=3.8.13,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: grpcio (==1.51.3)
-Requires-Dist: protobuf (==4.21.12)
-Requires-Dist: pydantic (==1.10.6)
-Requires-Dist: requests (==2.28.2)
+Requires-Dist: grpcio (>=1.51.3,<2.0.0)
+Requires-Dist: protobuf (>=4.21.12,<5.0.0)
+Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/Preemo-Inc/worker-sdk
 Description-Content-Type: text/markdown
 
 # Preemo Worker SDK
 
 [![PyPi Version](https://img.shields.io/pypi/v/preemo-worker-sdk)](https://pypi.org/project/preemo-worker-sdk/)
 [![License](https://img.shields.io/github/license/Preemo-Inc/worker-sdk)](https://github.com/Preemo-Inc/worker-sdk/blob/master/python/LICENSE)
```

