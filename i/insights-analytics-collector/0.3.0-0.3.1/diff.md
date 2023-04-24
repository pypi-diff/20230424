# Comparing `tmp/insights-analytics-collector-0.3.0.tar.gz` & `tmp/insights-analytics-collector-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insights-analytics-collector-0.3.0.tar", last modified: Thu Mar 30 14:16:23 2023, max compression
+gzip compressed data, was "insights-analytics-collector-0.3.1.tar", last modified: Mon Apr 24 15:31:19 2023, max compression
```

## Comparing `insights-analytics-collector-0.3.0.tar` & `insights-analytics-collector-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 daoneill  (1000) daoneill  (1000)        0 2023-03-30 14:16:23.767000 insights-analytics-collector-0.3.0/
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     9304 2023-03-22 16:15:53.000000 insights-analytics-collector-0.3.0/LICENSE.md
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     5929 2023-03-30 14:16:23.766000 insights-analytics-collector-0.3.0/PKG-INFO
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     5245 2023-03-22 16:15:53.000000 insights-analytics-collector-0.3.0/README.md
-drwxr-xr-x   0 daoneill  (1000) daoneill  (1000)        0 2023-03-30 14:16:23.765000 insights-analytics-collector-0.3.0/insights_analytics_collector/
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)      381 2023-03-30 12:29:40.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/__init__.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     4742 2023-03-30 14:16:10.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/collection.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     3557 2023-03-30 12:30:32.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/collection_csv.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     1835 2023-03-30 14:16:10.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/collection_data_status.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     1193 2023-03-30 12:29:39.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/collection_json.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)      608 2023-03-30 12:29:39.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/collection_manifest.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)    19315 2023-03-30 14:16:10.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/collector.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     2032 2023-03-30 12:29:40.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/csv_file_splitter.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     1219 2023-03-30 12:29:40.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/decorators.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)    11028 2023-03-30 14:16:10.000000 insights-analytics-collector-0.3.0/insights_analytics_collector/package.py
-drwxr-xr-x   0 daoneill  (1000) daoneill  (1000)        0 2023-03-30 14:16:23.765000 insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     5929 2023-03-30 14:16:23.000000 insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/PKG-INFO
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     1056 2023-03-30 14:16:23.000000 insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/SOURCES.txt
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)        1 2023-03-30 14:16:23.000000 insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/dependency_links.txt
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)        1 2023-03-30 13:01:55.000000 insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/not-zip-safe
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)       16 2023-03-30 14:16:23.000000 insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/requires.txt
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)       35 2023-03-30 14:16:23.000000 insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/top_level.txt
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)       85 2023-03-22 16:15:53.000000 insights-analytics-collector-0.3.0/pyproject.toml
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)       38 2023-03-30 14:16:23.767000 insights-analytics-collector-0.3.0/setup.cfg
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     1128 2023-03-30 13:14:49.000000 insights-analytics-collector-0.3.0/setup.py
-drwxr-xr-x   0 daoneill  (1000) daoneill  (1000)        0 2023-03-30 14:16:23.766000 insights-analytics-collector-0.3.0/tests/
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)        0 2023-03-22 16:15:53.000000 insights-analytics-collector-0.3.0/tests/__init__.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)        0 2023-03-22 16:15:53.000000 insights-analytics-collector-0.3.0/tests/conftest.py
-drwxr-xr-x   0 daoneill  (1000) daoneill  (1000)        0 2023-03-30 14:16:23.766000 insights-analytics-collector-0.3.0/tests/functional/
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)        0 2023-03-22 16:15:53.000000 insights-analytics-collector-0.3.0/tests/functional/__init__.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     2105 2023-03-30 12:29:42.000000 insights-analytics-collector-0.3.0/tests/functional/collector_module.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)      470 2023-03-30 12:29:41.000000 insights-analytics-collector-0.3.0/tests/functional/collector_module2.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     2671 2023-03-30 12:59:35.000000 insights-analytics-collector-0.3.0/tests/functional/collector_module3.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)      700 2023-03-30 12:29:41.000000 insights-analytics-collector-0.3.0/tests/functional/helpers.py
--rw-r--r--   0 daoneill  (1000) daoneill  (1000)     9680 2023-03-30 14:16:11.000000 insights-analytics-collector-0.3.0/tests/functional/test_gathering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.965939 insights-analytics-collector-0.3.1/insights_analytics_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collection_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/csv_file_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/insights_analytics_collector/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.965939 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 15:31:19.000000 insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:19.969939 insights-analytics-collector-0.3.1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/collector_module4_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/test_gathering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-24 15:31:04.000000 insights-analytics-collector-0.3.1/tests/functional/test_slicing.py
```

### Comparing `insights-analytics-collector-0.3.0/LICENSE.md` & `insights-analytics-collector-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.0/PKG-INFO` & `insights-analytics-collector-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-analytics-collector
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collector Package for Insights for AAP
 Home-page: https://github.com/RedHatInsights/insights-analytics-collector/
 Author: Martin Slemr
 Author-email: mslemr@redhat.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `insights-analytics-collector-0.3.0/README.md` & `insights-analytics-collector-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/collection.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import abstractmethod
+
 from django.utils.timezone import now, timedelta
 
 
 class Collection:
     """Wrapper for gathering function from Collector.collector_module
     Functions decorated with @register are wrapped by kind of this object.
     """
@@ -21,22 +22,25 @@
         self.description = fnc_collecting.__insights_analytics_description__ or ""
         self.key = fnc_collecting.__insights_analytics_key__
         self.shipping_group = fnc_collecting.__insights_analytics_shipping_group__
         self.version = fnc_collecting.__insights_analytics_version__
 
         self.data_type = fnc_collecting.__insights_analytics_type__
         self.filename = f"{self.key}.{self.data_type}"
+        # either since/until or full sync(if enabled)
         self.since = None  # set by Collector._create_collections()
         self.until = None  # set by Collector._create_collections()
+        self.full_sync_enabled = self._is_full_sync_enabled(
+            fnc_collecting.__insights_analytics_full_sync_interval_days__
+        )
 
         self.gathering_started_at = None
         self.gathering_finished_at = None
         self.gathering_successful = None
-        self.last_gathered_entry = self.collector.last_gathered_entry_for(
-            self.key)
+        self.last_gathered_entry = self.collector.last_gathered_entry_for(self.key)
 
     @abstractmethod
     def add_to_tar(self, tar):
         pass
 
     def cleanup(self):
         """There is an action only for CollectionCSV"""
@@ -59,16 +63,15 @@
                 full_path=self.collector.gather_dir,
                 collection_type=self.collector.collection_type,
             )
             self._save_gathering(result)
 
             self.gathering_successful = True
         except Exception as e:
-            self.logger.exception(
-                f"Could not generate metric {self.filename}: {e}")
+            self.logger.exception(f"Could not generate metric {self.filename}: {e}")
             self.gathering_successful = False
         finally:
             self._set_gathering_finished()
 
     @abstractmethod
     def is_empty(self):
         pass
@@ -76,16 +79,23 @@
     def slices(self):
         since = self.collector.gather_since
         until = self.collector.gather_until
         last_gather = self.collector.last_gather
         # These slicer functions may return a generator. The `since` parameter is
         # allowed to be None, and will fall back to LAST_ENTRIES[key] or to
         # LAST_GATHER (truncated appropriately to match the 4-week limit).
+        #
+        # Or it can force full table sync if interval is given
         if self.fnc_slicing:
-            slices = self.fnc_slicing(self.key, since, until, last_gather)
+            if self.full_sync_enabled:
+                slices = self.fnc_slicing(self.key, last_gather, full_sync_enabled=True)
+            else:
+                slices = self.fnc_slicing(
+                    self.key, last_gather, since=since, until=until
+                )
         else:
             slices = [(self._gather_since(), self._gather_until())]
 
         return slices
 
     def ship_immediately(self):
         """
@@ -101,25 +111,45 @@
         pass
 
     def update_last_gathered_entries(self, updates_dict):
         if self.key in updates_dict["locked"]:
             return
 
         if self.gathering_successful:
-            previous = updates_dict["keys"].get(self.key, None)
-            if previous is None:
-                updates_dict["keys"][self.key] = self.until
-            else:
-                updates_dict["keys"][self.key] = max(previous, self.until)
+            self._update_last_gathered_key(updates_dict, self.key, self.until)
+
+            if self.full_sync_enabled:
+                self._update_last_gathered_key(
+                    updates_dict, f"{self.key}_full", self.gathering_finished_at
+                )
         else:
+            # collections are ordered by time slices.
+            # in case of error all collections with newer timestamp are ignored
             updates_dict["locked"].add(self.key)
 
     #
     # Private methods ---------------------------
     #
+    @staticmethod
+    def _update_last_gathered_key(updates_dict, key, timestamp):
+        previous = updates_dict["keys"].get(key, None)
+        if previous is None:
+            updates_dict["keys"][key] = timestamp
+        else:
+            updates_dict["keys"][key] = max(previous, timestamp)
+
+    def _is_full_sync_enabled(self, interval_days):
+        if not interval_days:
+            return False
+
+        last_full_sync = self.collector.last_gathered_entry_for(f"{self.key}_full")
+        return not last_full_sync or last_full_sync < now() - timedelta(
+            days=interval_days
+        )
+
     def _gather_since(self):
         """Start of gathering based on settings excluding slices"""
         last_entry = max(
             self.last_gathered_entry or self.collector.last_gather,
             self.collector.gather_until - timedelta(weeks=4),
         )
         return self.collector.gather_since or last_entry
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/collection_csv.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import os
 import copy
-from .collection import Collection
+import os
+
 from django.utils.timezone import now
 
+from .collection import Collection
+
 
 class CollectionCSV(Collection):
     """Collection for CSV-outputting collecting functions (decorated by @register)
     Collecting functions can return 0+ paths to tmpfiles
     - result of gather() is stored in self.data_filepath
     - In case of multiple files, object clones itself to sub-collections,
       one for each file
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/collection_data_status.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_data_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import os
+
 from .collection_csv import CollectionCSV
 from .decorators import register
 
 
 class CollectionDataStatus(CollectionCSV):
     def __init__(self, collector, package):
         super().__init__(collector, self.data_collection_status)
@@ -23,16 +24,15 @@
                 "collection_start_timestamp",
                 "since",
                 "until",
                 "file_name",
                 "status",
                 "elapsed",
             ]
-            writer = csv.DictWriter(
-                csvfile, delimiter=",", fieldnames=fieldnames)
+            writer = csv.DictWriter(csvfile, delimiter=",", fieldnames=fieldnames)
             writer.writeheader()
 
             for collection in self.package.collections:
                 status = "ok" if collection.gathering_successful else "failed"
                 elapsed = 0
                 if collection.gathering_started_at and collection.gathering_finished_at:
                     elapsed = (
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/collection_json.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_json.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/collection_manifest.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/collection_manifest.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/collector.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from abc import abstractmethod
 import contextlib
-from django.utils.timezone import now, timedelta
 import hashlib
 import inspect
 import logging
 import os
 import pathlib
 import shutil
 import tempfile
+from abc import abstractmethod
 
+from django.utils.timezone import now, timedelta
 
-from .package import Package
 from .collection import Collection
 from .collection_csv import CollectionCSV
+from .collection_data_status import CollectionDataStatus
 from .collection_json import CollectionJSON
 from .collection_manifest import CollectionManifest
-from .collection_data_status import CollectionDataStatus
+from .package import Package
 
 
 class Collector:
     """Abstract class. The Collector is an entry-point for gathering data
        from awx to cloud.
     Abstract and following methods has to be implemented:
     - _package_class() - reference to your implementation of Package
@@ -283,20 +283,18 @@
         self._create_collections(collectors_subset)
 
     def _gather_config(self):
         """Config is special collection, it's added to each Package
         TODO: add "always" flag to @register decorator
         """
         if not self.config_present():
-            self.logger.log(
-                self.log_level, "'config' collector data is missing")
+            self.logger.log(self.log_level, "'config' collector data is missing")
             return False
         else:
-            self.collections["config"].gather(
-                self._package_class().max_data_size())
+            self.collections["config"].gather(self._package_class().max_data_size())
             return True
 
     def _gather_json_collections(self):
         """JSON collections are simpler, they're just gathered and added to the Package"""
         for collection in self.collections[Collection.COLLECTION_TYPE_JSON]:
             collection.gather(self._package_class().max_data_size())
 
@@ -336,31 +334,27 @@
         """Postgres db lock"""
         connection = self.db_connection()
 
         if connection is None:
             yield True
         else:
             # Build 64-bit integer out of the resource id
-            resource_key = int(hashlib.sha512(
-                key.encode()).hexdigest(), 16) % 2**63
+            resource_key = int(hashlib.sha512(key.encode()).hexdigest(), 16) % 2**63
 
             cursor = connection.cursor()
 
             try:
                 if wait:
-                    cursor.execute(
-                        "SELECT pg_advisory_lock(%s);", (resource_key,))
+                    cursor.execute("SELECT pg_advisory_lock(%s);", (resource_key,))
                 else:
-                    cursor.execute(
-                        "SELECT pg_try_advisory_lock(%s);", (resource_key,))
+                    cursor.execute("SELECT pg_try_advisory_lock(%s);", (resource_key,))
                 acquired = cursor.fetchall()[0][0]
                 yield acquired
             finally:
-                cursor.execute("SELECT pg_advisory_unlock(%s);",
-                               (resource_key,))
+                cursor.execute("SELECT pg_advisory_unlock(%s);", (resource_key,))
                 cursor.close()
 
     def _process_packages(self):
         for group, packages in self.packages.items():
             for package in packages:
                 self._process_package(package)
 
@@ -436,14 +430,19 @@
     def _update_last_gathered_entries(self):
         last_gathered_updates = {"keys": {}, "locked": set()}
 
         for _, packages in self.packages.items():
             for package in packages:
                 package.update_last_gathered_entries(last_gathered_updates)
 
+        # Locked key means that gathering wasn't successful at least once.
+        # Full sync timestamp can't be updated (if present)
+        for unsuccessful_key in last_gathered_updates["locked"]:
+            last_gathered_updates.pop(f"{unsuccessful_key}_full", None)
+
         self.last_gathered_entries.update(last_gathered_updates["keys"])
 
         self._save_last_gathered_entries(self.last_gathered_entries)
 
     @abstractmethod
     def _save_last_gathered_entries(self, last_gathered_entries):
         """Saves dictionary with timestamps to persistent storage
@@ -484,29 +483,27 @@
                 if collection.is_config:
                     # It's supposed there is only one registered config
                     self.collections[Collection.COLLECTION_TYPE_CONFIG] = collection
                 else:
                     for since, until in collection.slices():
                         collection.since = since
                         collection.until = until
-                        self.collections[collection.data_type].append(
-                            collection)
+                        self.collections[collection.data_type].append(collection)
                         collection = self._create_collection(fnc)
 
     def _create_collection(self, fnc_collecting):
         data_type = fnc_collecting.__insights_analytics_type__
         collection = None
         if data_type == "json":
             collection = self._collection_json_class()(self, fnc_collecting)
         elif data_type == "csv":
             collection = self._collection_csv_class()(self, fnc_collecting)
 
         if collection is None:
-            raise RuntimeError(
-                f"Collection of type {data_type} not implemented")
+            raise RuntimeError(f"Collection of type {data_type} not implemented")
 
         return collection
 
     def _create_package(self):
         package_class = self._package_class()
         return package_class(self)
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/csv_file_splitter.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/csv_file_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import io
 import os
+
 from .package import Package
 
 
 class CsvFileSplitter(io.StringIO):
     """Helper for writing big data into multiple files splitted by size.
     Expects data written in CSV format (first line is header)
     Could be called from function decorated by @register (see Collector).
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/decorators.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     key,
     version,
     description=None,
     format="json",
     config=False,
     fnc_slicing=None,
     shipping_group="default",
+    full_sync_interval_days=None,
 ):
     """
     A decorator used to register a function as a metric collector.
 
     Decorated functions should do the following based on format:
     - json: return JSON-serializable objects.
     - csv: write CSV data to a filename named 'key'
@@ -25,14 +26,15 @@
         f.__insights_analytics_key__ = key
         f.__insights_analytics_version__ = version
         f.__insights_analytics_description__ = description
         f.__insights_analytics_type__ = format  # CSV/JSON
         f.__insights_analytics_config__ = config  # config
         f.__insights_analytics_fnc_slicing__ = fnc_slicing
         f.__insights_analytics_shipping_group__ = shipping_group
+        f.__insights_analytics_full_sync_interval_days__ = full_sync_interval_days
 
         return f
 
     return decorate
 
 
 def slicing(default=False):
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector/package.py` & `insights-analytics-collector-0.3.1/insights_analytics_collector/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from abc import abstractmethod
 import base64
 import json
 import os
 import pathlib
-import requests
 import tarfile
+from abc import abstractmethod
+
+import requests
 
 
 class Package:
     """
     Abstract class
     Package serves for managing one tarball and shipping it to the cloud.
     Abstract methods has to be implemented, as well as:
@@ -79,16 +80,15 @@
         pass
 
     def has_free_space(self, requested_size):
         return self.total_data_size + requested_size <= self.max_data_size()
 
     def is_shipping_configured(self):
         if not self.tar_path:
-            self.logger.error(
-                "Insights for Ansible Automation Platform TAR not found")
+            self.logger.error("Insights for Ansible Automation Platform TAR not found")
             return False
 
         if not os.path.exists(self.tar_path):
             self.logger.error(
                 f"Insights for Ansible Automation Platform TAR {self.tar_path} not found"
             )
             return False
@@ -149,16 +149,15 @@
                 self._data_collection_status_to_tar(f)
 
                 self._manifest_to_tar(f)
 
                 self.tar_path = f.name
             return True
         except Exception as e:
-            self.logger.exception(
-                f"Failed to write analytics archive file: {e}")
+            self.logger.exception(f"Failed to write analytics archive file: {e}")
             return False
 
     def ship(self):
         """
         Ship gathered metrics to the Insights API
         """
         if not self.is_shipping_configured():
@@ -316,16 +315,15 @@
 
     def _manifest_to_tar(self, tar):
         try:
             self.manifest.gather(None)
             self.manifest.add_to_tar(tar)
             self.add_collection(self.manifest)
         except Exception as e:
-            self.logger.exception(
-                f"Could not generate {self.manifest.filename}: {e}")
+            self.logger.exception(f"Could not generate {self.manifest.filename}: {e}")
 
     def _payload_content_type(self):
         return self.PAYLOAD_CONTENT_TYPE
 
     def _tarname_base(self):
         timestamp = self.collector.gather_until
         return f'analytics-{timestamp.strftime("%Y-%m-%d-%H%M%S%z")}'
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/PKG-INFO` & `insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-analytics-collector
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collector Package for Insights for AAP
 Home-page: https://github.com/RedHatInsights/insights-analytics-collector/
 Author: Martin Slemr
 Author-email: mslemr@redhat.com
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `insights-analytics-collector-0.3.0/insights_analytics_collector.egg-info/SOURCES.txt` & `insights-analytics-collector-0.3.1/insights_analytics_collector.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -20,9 +20,11 @@
 insights_analytics_collector.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/functional/__init__.py
 tests/functional/collector_module.py
 tests/functional/collector_module2.py
 tests/functional/collector_module3.py
+tests/functional/collector_module4_slicing.py
 tests/functional/helpers.py
-tests/functional/test_gathering.py
+tests/functional/test_gathering.py
+tests/functional/test_slicing.py
```

### Comparing `insights-analytics-collector-0.3.0/setup.py` & `insights-analytics-collector-0.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
-from setuptools import setup, find_packages
 
-__version__ = "0.3.0"
+from setuptools import find_packages, setup
+
+__version__ = "0.3.1"
 
 # We use the README as the long_description
 readme_path = os.path.join(os.path.dirname(__file__), "README.md")
 
 
 setup(
     name="insights-analytics-collector",
@@ -26,9 +27,9 @@
         "Programming Language :: Python :: 3.9",
     ],
     license="Apache",
     zip_safe=False,
     packages=find_packages(),
     include_package_data=False,
     install_requires=["django", "requests"],
-    tests_require=["pytest", "pytest-mock"],
+    tests_require=["pytest", "pytest-mock", "pytz"],
 )
```

### Comparing `insights-analytics-collector-0.3.0/tests/functional/collector_module.py` & `insights-analytics-collector-0.3.1/tests/functional/collector_module.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.0/tests/functional/collector_module3.py` & `insights-analytics-collector-0.3.1/tests/functional/collector_module3.py`

 * *Files identical despite different names*

### Comparing `insights-analytics-collector-0.3.0/tests/functional/test_gathering.py` & `insights-analytics-collector-0.3.1/tests/functional/test_gathering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from tests.classes.analytics_collector import AnalyticsCollector
-import tests.functional.collector_module
-import tests.functional.collector_module2
-import tests.functional.collector_module3
 import json
 import logging
-import pytest
 import tarfile
 
-from django.conf import settings
-
-settings.configure(USE_TZ=True)
+import pytest
+import tests.functional.collector_module
+import tests.functional.collector_module2
+import tests.functional.collector_module3
+from tests.classes.analytics_collector import AnalyticsCollector
+from tests.functional.helpers import assert_common_files, decode_csv_line
 
 
 @pytest.fixture
 def collector(mocker):
     collector = AnalyticsCollector(
         collector_module=tests.functional.collector_module,
         collection_type=AnalyticsCollector.DRY_RUN,
@@ -22,16 +20,15 @@
 
     return collector
 
 
 def test_missing_config(mocker, collector):
     mock_logger = mocker.patch.object(collector, "logger")
 
-    tgz_files = collector.gather(
-        subset=["json_collection_1", "json_collection_2"])
+    tgz_files = collector.gather(subset=["json_collection_1", "json_collection_2"])
 
     assert tgz_files is None
     mock_logger.log.assert_called_with(
         logging.ERROR, "'config' collector data is missing"
     )
 
 
@@ -43,41 +40,38 @@
     assert len(tgz_files) == 1
 
     files = {}
     with tarfile.open(tgz_files[0], "r:gz") as archive:
         for member in archive.getmembers():
             files[member.name] = archive.extractfile(member)
 
-        _assert_common_files(files)
+        assert_common_files(files)
         assert "./json_collection_1.json" in files.keys()
         assert "./json_collection_2.json" in files.keys()
 
         assert json.loads(files["./config.json"].read()) == {"version": "1.0"}
-        assert json.loads(
-            files["./json_collection_1.json"].read()) == {"json1": "True"}
-        assert json.loads(
-            files["./json_collection_2.json"].read()) == {"json2": "True"}
+        assert json.loads(files["./json_collection_1.json"].read()) == {"json1": "True"}
+        assert json.loads(files["./json_collection_2.json"].read()) == {"json2": "True"}
 
     collector._gather_cleanup()
 
 
 def test_small_csvs(collector):
     tgz_files = collector.gather(
-        subset=["config", "csv_collection_1",
-                "csv_collection_2", "csv_collection_3"]
+        subset=["config", "csv_collection_1", "csv_collection_2", "csv_collection_3"]
     )
 
     assert len(tgz_files) == 1
 
     files = {}
     with tarfile.open(tgz_files[0], "r:gz") as archive:
         for member in archive.getmembers():
             files[member.name] = archive.extractfile(member)
 
-        _assert_common_files(files)
+        assert_common_files(files)
         assert "./csv_collection_1.csv" in files.keys()
         assert "./csv_collection_2.csv" in files.keys()
         assert "./csv_collection_3.csv" in files.keys()
 
         # length defined by @registered function
         assert len(files["./csv_collection_1.csv"].read()) == 100
         assert len(files["./csv_collection_2.csv"].read()) == 200
@@ -101,15 +95,15 @@
 
     for i in range(len(tgz_files)):
         files = {}
         with tarfile.open(tgz_files[i], "r:gz") as archive:
             for member in archive.getmembers():
                 files[member.name] = archive.extractfile(member)
 
-            _assert_common_files(files)
+            assert_common_files(files)
             if i == 0:
                 assert "./json_collection_1.json" in files.keys()
                 assert "./json_collection_2.json" in files.keys()
                 assert "./csv_slicing_1.csv" in files.keys()
             if i == 1:
                 assert "./csv_slicing_2.csv" in files.keys()
             if i == 2:
@@ -123,39 +117,38 @@
 
     for i in range(len(tgz_files)):
         files = {}
         with tarfile.open(tgz_files[i], "r:gz") as archive:
             for member in archive.getmembers():
                 files[member.name] = archive.extractfile(member)
 
-            _assert_common_files(files)
+            assert_common_files(files)
             assert len(files.keys()) == 1 + _common_files_count()
             assert "./big_table.csv" in files.keys()
             assert len(files["./big_table.csv"].read()) == 1000
 
     collector._gather_cleanup()
 
 
 def test_multiple_collections_multiple_tarballs(mocker, collector):
     mocker.patch("tests.classes.package.Package.MAX_DATA_SIZE", 1000)
 
     tgz_files = collector.gather(
-        subset=["config", "big_table_2",
-                "csv_collection_1", "csv_collection_2"]
+        subset=["config", "big_table_2", "csv_collection_1", "csv_collection_2"]
     )
 
     assert len(tgz_files) == 3
 
     for i in range(len(tgz_files)):
         files = {}
         with tarfile.open(tgz_files[i], "r:gz") as archive:
             for member in archive.getmembers():
                 files[member.name] = archive.extractfile(member)
 
-            _assert_common_files(files)
+            assert_common_files(files)
             if i == 0:
                 assert len(files.keys()) == 2 + _common_files_count()
                 assert "./big_table_2.csv" in files.keys()
                 assert "./csv_collection_1.csv" in files.keys()
             elif i == 1:
                 assert len(files.keys()) == 2 + _common_files_count()
                 assert "./big_table_2.csv" in files.keys()
@@ -180,15 +173,15 @@
 
     for i in range(len(tgz_files)):
         files = {}
         with tarfile.open(tgz_files[i], "r:gz") as archive:
             for member in archive.getmembers():
                 files[member.name] = archive.extractfile(member)
 
-            _assert_common_files(files)
+            assert_common_files(files)
             if i == 0:
                 assert "./simple_json1.json" in files.keys()
             else:
                 assert "./simple_json1.json" not in files.keys()
 
             # CSVs with no slicing start at index 0
             if 0 <= i <= 1:
@@ -240,15 +233,15 @@
     assert len(tgz_files) == 1
 
     files = {}
     with tarfile.open(tgz_files[0], "r:gz") as archive:
         for member in archive.getmembers():
             files[member.name] = archive.extractfile(member)
 
-        _assert_common_files(files)
+        assert_common_files(files)
         assert len(files.keys()) == 3 + _common_files_count()
 
         assert json.loads(files["./manifest.json"].read()) == {
             "config.json": "1.0",
             "data_collection_status.csv": "1.0",
             "json1.json": "1.1",
             "json2.json": "1.2",
@@ -270,30 +263,20 @@
         "since",
         "until",
         "file_name",
         "status",
         "elapsed",
     ]
     header = lines.pop(0)
-    assert _decode_csv_line(header) == fieldnames
+    assert decode_csv_line(header) == fieldnames
     for line in lines:
-        row = _decode_csv_line(line)
+        row = decode_csv_line(line)
         assert len(row) == len(fieldnames)
         assert row[4] == "ok"  # status
         assert row[5] == "0"  # elapsed
         files.pop(files.index(row[3]))
 
     assert len(files) == 0
 
 
-def _decode_csv_line(line):
-    return line.decode("utf-8").replace("\r", "").replace("\n", "").split(",")
-
-
-def _assert_common_files(files):
-    assert "./config.json" in files.keys()
-    assert "./manifest.json" in files.keys()
-    assert "./data_collection_status.csv" in files.keys()
-
-
 def _common_files_count():
     return 3
```

