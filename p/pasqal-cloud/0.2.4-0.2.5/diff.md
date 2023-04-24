# Comparing `tmp/pasqal-cloud-0.2.4.tar.gz` & `tmp/pasqal-cloud-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.2.4.tar", last modified: Mon Apr 24 09:26:10 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.2.5.tar", last modified: Mon Apr 24 13:05:37 2023, max compression
```

## Comparing `pasqal-cloud-0.2.4.tar` & `pasqal-cloud-0.2.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.342655 pasqal-cloud-0.2.4/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.342655 pasqal-cloud-0.2.4/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.342655 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_doubles/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 13:05:37.000000 pasqal-cloud-0.2.5/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.508082 pasqal-cloud-0.2.5/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:37.512082 pasqal-cloud-0.2.5/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 13:05:25.000000 pasqal-cloud-0.2.5/tests/test_doubles/authentication.py
```

### Comparing `pasqal-cloud-0.2.4/LICENSE` & `pasqal-cloud-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/PKG-INFO` & `pasqal-cloud-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.4
+Version: 0.2.5
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.2.4/README.md` & `pasqal-cloud-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/__init__.py` & `pasqal-cloud-0.2.5/pasqal_cloud/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,37 +110,75 @@
 
             if fetch_results:
                 batch_rsp, jobs_rsp = self._client._get_batch(
                     batch_id, fetch_results=True
                 )
         batch = Batch(**batch_rsp, _client=self._client)
         for job_rsp in jobs_rsp:
-            batch.jobs[job_rsp["id"]] = Job(**job_rsp)
+            batch.jobs[job_rsp["id"]] = Job(**job_rsp, _client=self._client)
 
         self.batches[batch.id] = batch
         return batch
 
     def get_batch(self, id: str, fetch_results: bool = False) -> Batch:
         """Retrieve a batch's data and all its jobs.
 
         Args:
-            id: Id of the batch.
+            id: ID of the batch.
             fetch_results: whether to download job results
 
         Returns:
             Batch: the batch stored in the PCS database.
         """
 
         batch_rsp, jobs_rsp = self._client._get_batch(id, fetch_results=fetch_results)
         batch = Batch(**batch_rsp, _client=self._client)
         for job_rsp in jobs_rsp:
-            batch.jobs[job_rsp["id"]] = Job(**job_rsp)
+            batch.jobs[job_rsp["id"]] = Job(**job_rsp, _client=self._client)
         self.batches[batch.id] = batch
         return batch
 
+    def cancel_batch(self, id: str) -> Batch:
+        """Cancel the given batch on the PCS
+
+        Args:
+            id: ID of the batch.
+        """
+        batch_rsp = self._client._cancel_batch(id)
+        batch = Batch(**batch_rsp, _client=self._client)
+        return batch
+
+    def get_job(self, id: str, wait: bool = False) -> Job:
+        """Retrieve a job's data.
+
+        Args:
+            id: ID of the job.
+            wait: Whether to wait for the job to be done
+
+        Returns:
+            Job: the job stored in the PCS database.
+        """
+        job_rsp = self._client._get_job(id)
+        if wait:
+            while job_rsp["status"] in ["PENDING", "RUNNING"]:
+                time.sleep(RESULT_POLLING_INTERVAL)
+                job_rsp = self._client._get_job(id)
+        job = Job(**job_rsp, _client=self._client)
+        return job
+
+    def cancel_job(self, id: str) -> Job:
+        """Cancel the given job on the PCS
+
+        Args:
+            id: ID of the job.
+        """
+        job_rsp = self._client._cancel_job(id)
+        job = Job(**job_rsp, _client=self._client)
+        return job
+
     def get_device_specs_dict(self) -> Dict[str, str]:
         """Retrieve the list of available device specifications.
 
         Returns:
             DeviceSpecs: the list of available device specifications.
         """
```

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/_version.py` & `pasqal-cloud-0.2.5/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
```

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/authentication.py` & `pasqal-cloud-0.2.5/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/batch.py` & `pasqal-cloud-0.2.5/pasqal_cloud/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 
 @dataclass
 class Batch:
     """Class for batch data.
 
     A batch groups up several jobs with the same sequence. When a batch is assigned to
     a QPU, all its jobs are ran sequentially and no other batch can be assigned to the
-    device until all its jobs are done and it is declared complete.
+    device until all its jobs are done and declared complete.
 
     Attributes:
         - complete: Whether the batch has been declared as complete.
         - created_at: Timestamp of the creation of the batch.
-        - updated_at: Timestamps of the last update of the batch.
+        - updated_at: Timestamp of the last update of the batch.
         - device_type: Type of device to run the batch on.
-        - group_id: Id of the owner group of the batch.
+        - group_id: ID of the owner group of the batch.
         - id: Unique identifier for the batch.
         - user_id: Unique identifier of the user that created the batch.
         - priority: Level of priority of the batch.
-        - status: Status of the batch.
+        - status: Status of the batch. Possible values are: PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
         - webhook: Webhook where the job results are automatically sent to.
+        - _client: A Client instance to connect to PCS.
         - sequence_builder: Pulser sequence of the batch.
         - start_datetime: Timestamp of the time the batch was sent to the QPU.
-        - end_datetime: Timestamp of when the  batch process was finished.
+        - end_datetime: Timestamp of when the batch process was finished.
         - device_status: Status of the device where the batch is running.
         - jobs: Dictionary of all the jobs added to the batch.
-        - jobs_count: number of jobs added to the batch.
-        - jobs_count_per_status: number of jobs per status.
+        - jobs_count: Number of jobs added to the batch.
+        - jobs_count_per_status: Number of jobs per status.
         - configuration: Further configuration for certain emulators.
-
     """
 
     complete: bool
     created_at: str
     updated_at: str
     device_type: str
     group_id: str
@@ -77,56 +77,61 @@
         runs: int = 100,
         variables: Optional[Dict[str, Any]] = None,
         wait: bool = False,
     ) -> Job:
         """Add and send a new job for this batch.
 
         Args:
-            runs: number of times the job is ran on the QPU.
+            runs: number of times the job is run on the QPU.
             variables (optional): values for variables if sequence is parametrized.
             wait: Whether to wait for the job to be done.
 
         Returns:
             - Job: the created job.
         """
         job_data: Dict[str, Any] = {"runs": runs, "batch_id": self.id}
         if variables:
             job_data["variables"] = variables
         job_rsp = self._client._send_job(job_data)
-        job = Job(**job_rsp)
+        job = Job(**job_rsp, _client=self._client)
         self.jobs[job.id] = job
         if wait:
             while job.status in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 job_rsp = self._client._get_job(job.id)
                 job = Job(**job_rsp)
         return job
 
     def declare_complete(
         self, wait: bool = False, fetch_results: bool = False
     ) -> Dict[str, Any]:
         """Declare to PCS that the batch is complete.
 
         Args:
-            wait: Whether to wait for the batch to be done
-            fetch_results: Whether to download the results. Implies
-                waiting for the batch.
+            wait: Whether to wait for the batch to be done.
+            fetch_results: Whether to download the results. Implies waiting for the batch.
 
         A batch that is complete awaits no extra jobs. All jobs previously added
         will be executed before the batch is terminated. When all its jobs are done,
         the complete batch is unassigned to its running device.
         """
-        self.complete = True
         batch_rsp = self._client._complete_batch(self.id)
+        self.complete = True
         if wait or fetch_results:
             while batch_rsp["status"] in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 batch_rsp, jobs_rsp = self._client._get_batch(
                     self.id,
                 )
             if fetch_results:
                 batch_rsp, jobs_rsp = self._client._get_batch(
                     self.id, fetch_results=True
                 )
             for job_rsp in jobs_rsp:
                 self.jobs[job_rsp["id"]] = Job(**job_rsp)
         return batch_rsp
+
+    def cancel(self) -> Dict[str, Any]:
+        """Cancel the current batch on the PCS."""
+        batch_rsp = self._client._cancel_batch(self.id)
+        self.status = batch_rsp.get("status", "CANCELED")
+        return batch_rsp
```

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/client.py` & `pasqal-cloud-0.2.5/pasqal_cloud/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,26 +122,14 @@
             "POST",
             f"{self.endpoints.core}/api/v1/batches",
             batch_data,
         )["data"]
         jobs_data = batch_data.pop("jobs", [])
         return batch_data, jobs_data
 
-    def _complete_batch(self, batch_id: str) -> Dict[str, Any]:
-        response: Dict[str, Any] = self._request(
-            "PUT", f"{self.endpoints.core}/api/v1/batches/{batch_id}/complete"
-        )["data"]
-        return response
-
-    def _send_job(self, job_data: Dict[str, Any]) -> Dict[str, Any]:
-        response: Dict[str, Any] = self._request(
-            "POST", f"{self.endpoints.core}/api/v1/jobs", job_data
-        )["data"]
-        return response
-
     def _get_batch(
         self, id: str, fetch_results: bool = False
     ) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
         batch_data: Dict[str, Any] = self._request(
             "GET", f"{self.endpoints.core}/api/v1/batches/{id}"
         )["data"]
         jobs_data = batch_data.pop("jobs", [])
@@ -149,18 +137,42 @@
             results = self._request(
                 "GET", f"{self.endpoints.core}/api/v1/batches/{id}/results"
             )["data"]
             for job_data in jobs_data:
                 job_data["result"] = results.get(str(job_data["id"]), None)
         return batch_data, jobs_data
 
+    def _complete_batch(self, batch_id: str) -> Dict[str, Any]:
+        response: Dict[str, Any] = self._request(
+            "PUT", f"{self.endpoints.core}/api/v1/batches/{batch_id}/complete"
+        )["data"]
+        return response
+
+    def _cancel_batch(self, batch_id: str) -> Dict[str, Any]:
+        batch: Dict[str, Any] = self._request(
+            "PUT", f"{self.endpoints.core}/api/v1/batches/{batch_id}/cancel"
+        )["data"]
+        return batch
+
+    def _send_job(self, job_data: Dict[str, Any]) -> Dict[str, Any]:
+        response: Dict[str, Any] = self._request(
+            "POST", f"{self.endpoints.core}/api/v1/jobs", job_data
+        )["data"]
+        return response
+
     def _get_job(self, job_id: str) -> Dict[str, Any]:
         job: Dict[str, Any] = self._request(
             "GET", f"{self.endpoints.core}/api/v1/jobs/{job_id}"
         )["data"]
         return job
 
+    def _cancel_job(self, job_id: str) -> Dict[str, Any]:
+        job: Dict[str, Any] = self._request(
+            "PUT", f"{self.endpoints.core}/api/v1/jobs/{job_id}/cancel"
+        )["data"]
+        return job
+
     def get_device_specs_dict(self) -> Dict[str, str]:
         device_specs: Dict[str, str] = self._request(
             "GET", f"{self.endpoints.core}/api/v1/devices/specs"
         )["data"]
         return device_specs
```

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.2.5/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.2.5/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/errors.py` & `pasqal-cloud-0.2.5/pasqal_cloud/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,20 +22,21 @@
     code: int
     message: str
     description: str
     details: JSendPayload
 
     def __init__(self, data: JSendPayload, *args: object) -> None:
         super().__init__(*args)
-        self.code = data["code"]
+        self.code = data.get("code", 0)
+
         # If no error description, display default response message instead
-        if data.get("data"):
-            self.description = data["data"].get("description", data["message"])
+        if data.get("data", ""):
+            self.description = data["data"].get("description", data.get("message"))
         else:
-            self.description = data["message"]
+            self.description = data.get("message", "")
         self.details = data
 
     def __str__(self) -> str:
         return (
             f"Error {self.code}: {self.description}\n"
             f"Details: {json.dumps(self.details, indent=2)}"
         )
```

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/job.py` & `pasqal-cloud-0.2.5/pasqal_cloud/job.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
+from pasqal_cloud.client import Client
+
 
 @dataclass
 class Job:
     """Class for job data.
 
     Attributes:
-        - runs: Number of time the job should be ran.
-        - created_at: Timestamp of the creation of the batch.
-        - updated_at: Timestamps of the last update of the batch.
-        - start_timestamp(optional): The timestamp of when the job began processing.
-        - end_timestamp(optional): The timestamp of when the job finished processing.
+        - runs: Number of times the job should be run.
+        - created_at: Timestamp of the creation of the job.
+        - updated_at: Timestamp of the last update of the job.
+        - start_timestamp: The timestamp of when the job began processing.
+        - end_timestamp: The timestamp of when the job finished processing.
         - batch_id: ID of the batch which the job belongs to.
-        - errors: Error messages that occured while processing job.
-        - id: Unique identifier for the batch
+        - errors: Error messages that occurred while processing job.
+        - id: Unique identifier for the job.
         - group_id: ID of the group which the users scheduling the job belong to.
-        - status: Status of the job
-        - result(optional): Result of the job.
-        - variables (optional): dictionnary of variables of the job.
-            None if the associated batch is non-parametrized
+        - status: Status of the job. Possible values are: PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
+        - _client: A Client instance to connect to PCS.
+        - result: Result of the job.
+        - variables: Dictionary of variables of the job.
+          None if the associated batch is non-parametrized.
     """
 
     runs: int
     batch_id: str
     id: str
     group_id: str
     status: str
+    _client : Client
     created_at: str
     updated_at: str
     errors: List[str]
     start_timestamp: Optional[str] = None
     end_timestamp: Optional[str] = None
     result: Optional[Dict[str, Any]] = None
     variables: Optional[Dict[str, Any]] = None
+
+    def cancel(self) -> Dict[str, Any]:
+        """Cancel the current job on the PCS."""
+        job_rsp = self._client._cancel_job(self.id)
+        self.status = job_rsp.get("status", "CANCELED")
+        return job_rsp
```

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.2.5/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.2.5/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.4
+Version: 0.2.5
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.2.4/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.2.5/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/sdk/setup.py` & `pasqal-cloud-0.2.5/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/setup.py` & `pasqal-cloud-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/tests/test_batch.py` & `pasqal-cloud-0.2.5/tests/test_batch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from unittest.mock import patch
 from uuid import uuid4
 
 import pytest
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
-from pasqal_cloud import SDK
+from pasqal_cloud import SDK, Batch, Job
 from pasqal_cloud.device import BaseConfig, EmuFreeConfig, EmulatorType, EmuTNConfig
 
 
 class TestBatch:
     @pytest.fixture(autouse=True)
-    @patch("sdk.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
+    @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
     def init_sdk(self, start_mock_request):
         self.sdk = SDK(
             username="me@test.com", password="password", group_id=str(uuid4())
         )
         self.pulser_sequence = "pulser_test_sequence"
         self.batch_id = "00000000-0000-0000-0000-000000000001"
         self.job_result = {"1001": 12, "0110": 35, "1111": 1}
@@ -68,14 +68,65 @@
         assert batch.complete
         assert batch.jobs
         for job_id, job in batch.jobs.items():
             assert self.job_id == job_id
             assert job.result == self.job_result
         assert request_mock.last_request.method == "GET"
 
+    def test_get_batch(self, batch):
+        batch_requested = self.sdk.get_batch(batch.id)
+        assert (
+            batch_requested.id == self.batch_id
+        )
+
+    def test_cancel_batch_self(self, request_mock, batch):
+        batch.cancel()
+        assert batch.status == 'CANCELED'
+        assert request_mock.last_request.method == "PUT"
+        assert (
+            request_mock.last_request.url
+            == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}/cancel"
+        )
+
+    def test_cancel_batch_sdk(self, request_mock):
+        client_rsp = self.sdk.cancel_batch(self.batch_id)
+        assert type(client_rsp) == Batch
+        assert client_rsp.status == 'CANCELED'
+        assert request_mock.last_request.method == "PUT"
+        assert (
+                request_mock.last_request.url
+                == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}/cancel"
+        )
+
+    def test_get_job(self, job):
+        job_requested = self.sdk.get_job(job.id)
+        print(self.sdk)
+        assert (
+            job_requested.id == job.id
+        )
+
+    def test_cancel_job_self(self, request_mock, job):
+        job.cancel()
+        assert job.status == 'CANCELED'
+        assert request_mock.last_request.method == "PUT"
+        assert (
+            request_mock.last_request.url
+            == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
+        )
+
+    def test_cancel_job_sdk(self, request_mock):
+        client_rsp = self.sdk.cancel_job(self.job_id)
+        assert type(client_rsp) == Job
+        assert client_rsp.status == 'CANCELED'
+        assert request_mock.last_request.method == "PUT"
+        assert (
+            request_mock.last_request.url
+            == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
+        )
+
     @pytest.mark.skip(reason="Not enabled during Iroise MVP")
     def test_batch_add_job(self, request_mock):
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
         )
         job = batch.add_job(
             runs=self.n_job_runs,
```

### Comparing `pasqal-cloud-0.2.4/tests/test_client.py` & `pasqal-cloud-0.2.5/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,44 +7,43 @@
 from pasqal_cloud.authentication import TokenProvider
 from tests.test_doubles.authentication import (
     FakeAuth0AuthenticationFailure,
     FakeAuth0AuthenticationSuccess,
 )
 
 
-@patch("sdk.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
+@patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
 class TestAuthSuccess:
     group_id = "random_group_id"
     username = "random_username"
     password = "random_password"
     new_core_endpoint = "random_endpoint"
 
-    @patch("sdk.client.getpass")
+    @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_success(self, getpass):
         getpass.return_value = self.password
         SDK(group_id=self.group_id, username=self.username)
         getpass.assert_called_once()
 
     def test_authentication_success(self):
         SDK(group_id=self.group_id, username=self.username, password=self.password)
 
     def test_good_token_provider(self):
         SDK(
             group_id=self.group_id,
             token_provider=FakeAuth0AuthenticationSuccess("username", "password", None),
         )
-    
+
     def test_custom_token_provider(self):
         """Test that the custom provider suggested in the readme is working"""
         class CustomTokenProvider(TokenProvider):
             def get_token(self):
                 return "your-token" # Replace this value with your token
         SDK(token_provider=CustomTokenProvider(), group_id="group_id")
 
-
     def test_correct_endpoints(self):
         sdk = SDK(
             group_id=self.group_id,
             username=self.username,
             password=self.password,
             endpoints=Endpoints(core=self.new_core_endpoint),
         )
@@ -56,23 +55,23 @@
             group_id=self.group_id,
             username=self.username,
             password=self.password,
             auth0=new_auth0,
         )
 
 
-@patch("sdk.client.Auth0TokenProvider", FakeAuth0AuthenticationFailure)
+@patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationFailure)
 class TestAuthFailure:
     group_id = "random_group_id"
     username = "random_username"
     no_username = ""
     password = "random_password"
     no_password = ""
 
-    @patch("sdk.client.getpass")
+    @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_bad_password(self, getpass):
         getpass.return_value = self.password
 
         with pytest.raises(Auth0Error):
             SDK(group_id=self.group_id, username=self.username)
 
         getpass.assert_called_once()
@@ -93,25 +92,25 @@
         with pytest.raises(ValueError):
             SDK(
                 group_id=self.group_id,
                 username=self.no_username,
                 password=self.password,
             )
 
-    @patch("sdk.client.getpass")
+    @patch("pasqal_cloud.client.getpass")
     def test_module_no_password(self, getpass):
         getpass.return_value = ""
         with pytest.raises(ValueError):
             SDK(
                 group_id=self.group_id,
                 username=self.username,
                 password=self.no_password,
             )
 
-    @patch("sdk.client.getpass")
+    @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_no_password(self, getpass):
         getpass.return_value = self.no_password
 
         with pytest.raises(ValueError):
             SDK(group_id=self.group_id, username=self.username)
 
         getpass.assert_called_once()
```

### Comparing `pasqal-cloud-0.2.4/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.2.5/tests/test_cloud_sdk_import.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import inspect
+import warnings
+
+import pytest
 
 """
 Tests written to verify if the backward compatibility is working between the new name of the package `pasqal-cloud` 
 and its main folder renamed to `pasqal_cloud` and the previous package name that was `pasqal-cloud` 
 with the former folder called `sdk`.
 """
 
 
 def test_verify_import_sdk_is_module():
-    import sdk
-    assert inspect.ismodule(sdk)
+    with pytest.warns(DeprecationWarning):
+        import sdk
+        assert inspect.ismodule(sdk)
 
 
 def test_verify_import_classes_from_sdk():
-    from sdk import SDK
-    from sdk import Batch
-    from sdk import Job
-    from sdk import Endpoints
-    from sdk import EmulatorType
-    from sdk.device.configuration import BaseConfig
-    from sdk.device.configuration import EmuFreeConfig
-    from sdk.device.configuration import EmuTNConfig
-    from sdk.utils import JSendPayload
-    from sdk.utils import StrEnum
+    with pytest.warns(DeprecationWarning):
+        from sdk import SDK
+        from sdk import Batch
+        from sdk import Job
+        from sdk import Endpoints
+        from sdk import EmulatorType
+        from sdk.device.configuration import BaseConfig
+        from sdk.device.configuration import EmuFreeConfig
+        from sdk.device.configuration import EmuTNConfig
+        from sdk.utils import JSendPayload
+        from sdk.utils import StrEnum
```

### Comparing `pasqal-cloud-0.2.4/tests/test_config.py` & `pasqal-cloud-0.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/tests/test_device_specs.py` & `pasqal-cloud-0.2.5/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.4/tests/test_doubles/authentication.py` & `pasqal-cloud-0.2.5/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

