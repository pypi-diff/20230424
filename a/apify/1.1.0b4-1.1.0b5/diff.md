# Comparing `tmp/apify-1.1.0b4.tar.gz` & `tmp/apify-1.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.1.0b4.tar", last modified: Thu Mar 30 09:27:18 2023, max compression
+gzip compressed data, was "apify-1.1.0b5.tar", last modified: Mon Apr 24 07:10:17 2023, max compression
```

## Comparing `apify-1.1.0b4.tar` & `apify-1.1.0b5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:27:18.603813 apify-1.1.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-03-30 09:26:56.000000 apify-1.1.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-30 09:27:18.603813 apify-1.1.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-30 09:26:56.000000 apify-1.1.0b4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 09:27:18.603813 apify-1.1.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-03-30 09:26:56.000000 apify-1.1.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:27:18.595813 apify-1.1.0b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:27:18.599813 apify-1.1.0b4/src/apify/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:27:18.599813 apify-1.1.0b4/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:27:18.603813 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19628 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19014 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-30 09:27:17.000000 apify-1.1.0b4/src/apify/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:27:18.603813 apify-1.1.0b4/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-30 09:26:56.000000 apify-1.1.0b4/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 09:27:18.599813 apify-1.1.0b4/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-30 09:27:18.000000 apify-1.1.0b4/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-30 09:27:18.000000 apify-1.1.0b4/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 09:27:18.000000 apify-1.1.0b4/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-30 09:27:18.000000 apify-1.1.0b4/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-30 09:27:18.000000 apify-1.1.0b4/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-24 07:10:06.000000 apify-1.1.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-24 07:10:17.486343 apify-1.1.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-24 07:10:06.000000 apify-1.1.0b5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:10:17.486343 apify-1.1.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-24 07:10:06.000000 apify-1.1.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.482343 apify-1.1.0b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.482343 apify-1.1.0b5/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23398 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-24 07:10:06.000000 apify-1.1.0b5/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:10:17.486343 apify-1.1.0b5/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 07:10:17.000000 apify-1.1.0b5/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.1.0b4/LICENSE` & `apify-1.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/PKG-INFO` & `apify-1.1.0b5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b4
+Version: 1.1.0b5
 Summary: Apify SDK for Python
 Home-page: https://github.com/apify/apify-sdk-python
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 License: Apache Software License
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
```

### Comparing `apify-1.1.0b4/README.md` & `apify-1.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/setup.py` & `apify-1.1.0b5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             'filelock ~= 3.9.0',
             'flake8 ~= 6.0.0',
             'flake8-bugbear ~= 23.1.20',
             'flake8-commas ~= 2.1.0',
             'flake8-comprehensions ~= 3.10.1',
             'flake8-datetimez ~= 20.10.0',
             'flake8-docstrings ~= 1.7.0',
+            'flake8-encodings ~= 0.5.0',
             'flake8-isort ~= 6.0.0',
             'flake8-noqa ~= 1.3.0',
             'flake8-pytest-style ~= 1.7.2',
             'flake8-quotes ~= 3.3.1',
             'flake8-unused-arguments ~= 0.0.13',
             'isort ~= 5.12.0',
             'mypy ~= 1.0.0',
```

### Comparing `apify-1.1.0b4/src/apify/_crypto.py` & `apify-1.1.0b5/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.1.0b5/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.1.0b5/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             if os.access(storages_dir, os.F_OK):
                 for entry in os.scandir(storages_dir):
                     if not entry.is_dir():
                         continue
                     metadata_path = os.path.join(entry.path, '__metadata__.json')
                     if not os.access(metadata_path, os.F_OK):
                         continue
-                    with open(metadata_path) as metadata_file:
+                    with open(metadata_path, encoding='utf-8') as metadata_file:
                         metadata = json.load(metadata_file)
                     if id and id == metadata.get('id'):
                         storage_path = entry.path
                         name = metadata.get(name)
                         break
                     if name and name == metadata.get('name'):
                         storage_path = entry.path
```

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,26 +408,26 @@
         # Access the dataset folder
         for entry in os.scandir(storage_directory):
             if entry.is_file():
                 if entry.name == '__metadata__.json':
                     has_seen_metadata_file = True
 
                     # We have found the dataset's metadata file, build out information based on it
-                    with open(os.path.join(storage_directory, entry.name)) as f:
+                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
                         metadata = json.load(f)
                     id = metadata['id']
                     name = metadata['name']
                     item_count = metadata['itemCount']
                     created_at = datetime.fromisoformat(metadata['createdAt'])
                     accessed_at = datetime.fromisoformat(metadata['accessedAt'])
                     modified_at = datetime.fromisoformat(metadata['modifiedAt'])
 
                     continue
 
-                with open(os.path.join(storage_directory, entry.name)) as f:
+                with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
                     entry_content = json.load(f)
                 entry_name = entry.name.split('.')[0]
 
                 entries[entry_name] = entry_content
 
                 if not has_seen_metadata_file:
                     item_count += 1
```

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,27 +379,27 @@
         internal_records: Dict[str, Dict] = {}
 
         # Access the key value store folder
         for entry in os.scandir(storage_directory):
             if entry.is_file():
                 if entry.name == '__metadata__.json':
                     # We have found the store metadata file, build out information based on it
-                    with open(os.path.join(storage_directory, entry.name), encoding='utf8') as f:
+                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
                         metadata = json.load(f)
                     id = metadata['id']
                     name = metadata['name']
                     created_at = datetime.fromisoformat(metadata['createdAt'])
                     accessed_at = datetime.fromisoformat(metadata['accessedAt'])
                     modified_at = datetime.fromisoformat(metadata['modifiedAt'])
 
                     continue
 
                 if '.__metadata__.' in entry.name:
                     # This is an entry's metadata file, we can use it to create/extend the record
-                    with open(os.path.join(storage_directory, entry.name), encoding='utf8') as f:
+                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
                         metadata = json.load(f)
 
                     new_record = {
                         **internal_records.get(metadata['key'], {}),
                         **metadata,
                     }
 
@@ -425,15 +425,15 @@
                             If you want to have correct interpretation of the file, you should add a file extension to the entry.""",
                             Warning,
                             stacklevel=2,
                         )
                 elif 'application/json' in content_type:
                     try:
                         # Try parsing the JSON ahead of time (not ideal but solves invalid files being loaded into stores)
-                        json.loads(file_content)
+                        json.loads(file_content.decode('utf-8'))
                     except json.JSONDecodeError:
                         # We need to override and then restore the warnings filter so that the warning gets printed out,
                         # Otherwise it would be silently swallowed
                         with warnings.catch_warnings():
                             warnings.simplefilter('always')
                             warnings.warn(
                                 (f'Key-value entry "{entry.name}" for store {name or id} has invalid JSON content'
```

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,27 +419,27 @@
         entries: List[Dict] = []
 
         # Access the request queue folder
         for entry in os.scandir(storage_directory):
             if entry.is_file():
                 if entry.name == '__metadata__.json':
                     # We have found the queue's metadata file, build out information based on it
-                    with open(os.path.join(storage_directory, entry.name)) as f:
+                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
                         metadata = json.load(f)
                     id = metadata['id']
                     name = metadata['name']
                     created_at = datetime.fromisoformat(metadata['createdAt'])
                     accessed_at = datetime.fromisoformat(metadata['accessedAt'])
                     modified_at = datetime.fromisoformat(metadata['modifiedAt'])
                     handled_request_count = metadata['handledRequestCount']
                     pending_request_count = metadata['pendingRequestCount']
 
                     continue
 
-                with open(os.path.join(storage_directory, entry.name)) as f:
+                with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
                     request = json.load(f)
                     if request.get('orderNo'):
                         request['orderNo'] = Decimal(request.get('orderNo'))
                 entries.append(request)
 
         new_client = cls(
             base_storage_directory=memory_storage_client._request_queues_directory,
```

### Comparing `apify-1.1.0b4/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.1.0b5/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/_utils.py` & `apify-1.1.0b5/src/apify/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
     # but then the check would be super complex, judging from how the 'requests' library does it.
     # This way should be good enough for the vast majority of use cases, if it causes issues, we can improve it later.
     return isinstance(value, (bytes, bytearray, io.IOBase))
 
 
 def _maybe_parse_body(body: bytes, content_type: str) -> Any:
     if _is_content_type_json(content_type):
-        return json.loads(body)  # Returns any
+        return json.loads(body.decode('utf-8'))  # Returns any
     elif _is_content_type_xml(content_type) or _is_content_type_text(content_type):
         return body.decode('utf-8')
     return body
 
 
 def _unique_key_to_request_id(unique_key: str) -> str:
     """Generate request ID based on unique key in a deterministic way."""
```

### Comparing `apify-1.1.0b4/src/apify/actor.py` & `apify-1.1.0b5/src/apify/actor.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/config.py` & `apify-1.1.0b5/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/consts.py` & `apify-1.1.0b5/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/event_manager.py` & `apify-1.1.0b5/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/log.py` & `apify-1.1.0b5/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/proxy_configuration.py` & `apify-1.1.0b5/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/storages/base_storage.py` & `apify-1.1.0b5/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/storages/dataset.py` & `apify-1.1.0b5/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/storages/key_value_store.py` & `apify-1.1.0b5/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/storages/request_queue.py` & `apify-1.1.0b5/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify/storages/storage_client_manager.py` & `apify-1.1.0b5/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify.egg-info/PKG-INFO` & `apify-1.1.0b5/src/apify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.0b4
+Version: 1.1.0b5
 Summary: Apify SDK for Python
 Home-page: https://github.com/apify/apify-sdk-python
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 License: Apache Software License
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
```

### Comparing `apify-1.1.0b4/src/apify.egg-info/SOURCES.txt` & `apify-1.1.0b5/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.1.0b4/src/apify.egg-info/requires.txt` & `apify-1.1.0b5/src/apify.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 filelock~=3.9.0
 flake8~=6.0.0
 flake8-bugbear~=23.1.20
 flake8-commas~=2.1.0
 flake8-comprehensions~=3.10.1
 flake8-datetimez~=20.10.0
 flake8-docstrings~=1.7.0
+flake8-encodings~=0.5.0
 flake8-isort~=6.0.0
 flake8-noqa~=1.3.0
 flake8-pytest-style~=1.7.2
 flake8-quotes~=3.3.1
 flake8-unused-arguments~=0.0.13
 isort~=5.12.0
 mypy~=1.0.0
```

