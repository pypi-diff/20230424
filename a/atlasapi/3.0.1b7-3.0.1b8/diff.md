# Comparing `tmp/atlasapi-3.0.1b7.tar.gz` & `tmp/atlasapi-3.0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasapi-3.0.1b7.tar", last modified: Sun Apr 23 20:50:26 2023, max compression
+gzip compressed data, was "atlasapi-3.0.1b8.tar", last modified: Mon Apr 24 00:19:04 2023, max compression
```

## Comparing `atlasapi-3.0.1b7.tar` & `atlasapi-3.0.1b8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.572742 atlasapi-3.0.1b7/
--rw-r--r--   0 mgm        (502) staff       (20)    11751 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/LICENSE
--rw-r--r--   0 mgm        (502) staff       (20)    10496 2023-04-23 20:50:26.572304 atlasapi-3.0.1b7/PKG-INFO
--rw-r--r--   0 mgm        (502) staff       (20)     9760 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/README.rst
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.548271 atlasapi-3.0.1b7/atlasapi/
--rw-r--r--   0 mgm        (502) staff       (20)      672 2023-04-23 20:39:28.000000 atlasapi-3.0.1b7/atlasapi/__init__.py
--rw-r--r--   0 mgm        (502) staff       (20)     2824 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/alerts.py
--rw-r--r--   0 mgm        (502) staff       (20)     3942 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/api_keys.py
--rw-r--r--   0 mgm        (502) staff       (20)   110669 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/atlas.py
--rw-r--r--   0 mgm        (502) staff       (20)      447 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/atlas_types.py
--rw-r--r--   0 mgm        (502) staff       (20)     1614 2022-04-13 03:32:09.000000 atlasapi-3.0.1b7/atlasapi/atlas_users.py
--rw-r--r--   0 mgm        (502) staff       (20)    11536 2022-03-21 00:49:03.000000 atlasapi-3.0.1b7/atlasapi/cloud_backup.py
--rw-r--r--   0 mgm        (502) staff       (20)    36466 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/clusters.py
--rw-r--r--   0 mgm        (502) staff       (20)     8523 2023-04-23 20:36:51.000000 atlasapi-3.0.1b7/atlasapi/errors.py
--rw-r--r--   0 mgm        (502) staff       (20)     6832 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/events.py
--rw-r--r--   0 mgm        (502) staff       (20)    60586 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/events_event_types.py
--rw-r--r--   0 mgm        (502) staff       (20)    15455 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/invoices_pydantic.py
--rw-r--r--   0 mgm        (502) staff       (20)     5317 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/lib.py
--rw-r--r--   0 mgm        (502) staff       (20)       24 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/logs.py
--rw-r--r--   0 mgm        (502) staff       (20)     3093 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/maintenance_window.py
--rw-r--r--   0 mgm        (502) staff       (20)    15755 2022-06-22 22:40:25.000000 atlasapi-3.0.1b7/atlasapi/measurements.py
--rw-r--r--   0 mgm        (502) staff       (20)    10967 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/network.py
--rw-r--r--   0 mgm        (502) staff       (20)      863 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/organizations.py
--rw-r--r--   0 mgm        (502) staff       (20)     6419 2023-01-07 00:49:32.000000 atlasapi-3.0.1b7/atlasapi/projects.py
--rw-r--r--   0 mgm        (502) staff       (20)    14835 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/serverless_pydantic.py
--rw-r--r--   0 mgm        (502) staff       (20)    11207 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/settings.py
--rw-r--r--   0 mgm        (502) staff       (20)    23713 2023-04-23 20:30:49.000000 atlasapi-3.0.1b7/atlasapi/specs.py
--rw-r--r--   0 mgm        (502) staff       (20)     2272 2022-04-13 03:32:09.000000 atlasapi-3.0.1b7/atlasapi/teams.py
--rw-r--r--   0 mgm        (502) staff       (20)     3249 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlasapi/whitelist.py
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.550566 atlasapi-3.0.1b7/atlasapi.egg-info/
--rwxrwxrwx   0 mgm        (502) staff       (20)    10496 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/PKG-INFO
--rwxrwxrwx   0 mgm        (502) staff       (20)      866 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/SOURCES.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)        1 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/dependency_links.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       47 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/entry_points.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       90 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/requires.txt
--rwxrwxrwx   0 mgm        (502) staff       (20)       18 2023-04-23 20:50:26.000000 atlasapi-3.0.1b7/atlasapi.egg-info/top_level.txt
-drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-23 20:50:26.571675 atlasapi-3.0.1b7/atlascli/
--rw-r--r--   0 mgm        (502) staff       (20)      581 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/__init__.py
--rw-r--r--   0 mgm        (502) staff       (20)     1190 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/atlaserrors.py
--rw-r--r--   0 mgm        (502) staff       (20)     2011 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/atlaskey.py
--rw-r--r--   0 mgm        (502) staff       (20)     4624 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/cli.py
--rw-r--r--   0 mgm        (502) staff       (20)     1360 2021-07-31 01:06:14.000000 atlasapi-3.0.1b7/atlascli/listcommand.py
--rw-r--r--   0 mgm        (502) staff       (20)       38 2023-04-23 20:50:26.572859 atlasapi-3.0.1b7/setup.cfg
--rw-r--r--   0 mgm        (502) staff       (20)     1770 2023-04-23 20:39:28.000000 atlasapi-3.0.1b7/setup.py
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-24 00:19:04.975423 atlasapi-3.0.1b8/
+-rw-r--r--   0 mgm        (502) staff       (20)    11751 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/LICENSE
+-rw-r--r--   0 mgm        (502) staff       (20)    10496 2023-04-24 00:19:04.975079 atlasapi-3.0.1b8/PKG-INFO
+-rw-r--r--   0 mgm        (502) staff       (20)     9760 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/README.rst
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-24 00:19:04.969953 atlasapi-3.0.1b8/atlasapi/
+-rw-r--r--   0 mgm        (502) staff       (20)      672 2023-04-24 00:17:08.000000 atlasapi-3.0.1b8/atlasapi/__init__.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2824 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlasapi/alerts.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3942 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlasapi/api_keys.py
+-rw-r--r--   0 mgm        (502) staff       (20)   110493 2023-04-24 00:17:08.000000 atlasapi-3.0.1b8/atlasapi/atlas.py
+-rw-r--r--   0 mgm        (502) staff       (20)      447 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlasapi/atlas_types.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1614 2022-04-13 03:32:09.000000 atlasapi-3.0.1b8/atlasapi/atlas_users.py
+-rw-r--r--   0 mgm        (502) staff       (20)    11536 2022-03-21 00:49:03.000000 atlasapi-3.0.1b8/atlasapi/cloud_backup.py
+-rw-r--r--   0 mgm        (502) staff       (20)    36466 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/clusters.py
+-rw-r--r--   0 mgm        (502) staff       (20)     8523 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/errors.py
+-rw-r--r--   0 mgm        (502) staff       (20)     6832 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/events.py
+-rw-r--r--   0 mgm        (502) staff       (20)    60586 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/events_event_types.py
+-rw-r--r--   0 mgm        (502) staff       (20)    15455 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/invoices_pydantic.py
+-rw-r--r--   0 mgm        (502) staff       (20)     5317 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/lib.py
+-rw-r--r--   0 mgm        (502) staff       (20)       24 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlasapi/logs.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3093 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlasapi/maintenance_window.py
+-rw-r--r--   0 mgm        (502) staff       (20)    16132 2023-04-23 23:26:24.000000 atlasapi-3.0.1b8/atlasapi/measurements.py
+-rw-r--r--   0 mgm        (502) staff       (20)    10967 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/network.py
+-rw-r--r--   0 mgm        (502) staff       (20)      863 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/organizations.py
+-rw-r--r--   0 mgm        (502) staff       (20)     6419 2023-01-07 00:49:32.000000 atlasapi-3.0.1b8/atlasapi/projects.py
+-rw-r--r--   0 mgm        (502) staff       (20)    14835 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/serverless_pydantic.py
+-rw-r--r--   0 mgm        (502) staff       (20)    11207 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/settings.py
+-rw-r--r--   0 mgm        (502) staff       (20)    23713 2023-04-23 21:54:35.000000 atlasapi-3.0.1b8/atlasapi/specs.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2272 2022-04-13 03:32:09.000000 atlasapi-3.0.1b8/atlasapi/teams.py
+-rw-r--r--   0 mgm        (502) staff       (20)     3249 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlasapi/whitelist.py
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-24 00:19:04.972236 atlasapi-3.0.1b8/atlasapi.egg-info/
+-rwxrwxrwx   0 mgm        (502) staff       (20)    10496 2023-04-24 00:19:04.000000 atlasapi-3.0.1b8/atlasapi.egg-info/PKG-INFO
+-rwxrwxrwx   0 mgm        (502) staff       (20)      866 2023-04-24 00:19:04.000000 atlasapi-3.0.1b8/atlasapi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)        1 2023-04-24 00:19:04.000000 atlasapi-3.0.1b8/atlasapi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       47 2023-04-24 00:19:04.000000 atlasapi-3.0.1b8/atlasapi.egg-info/entry_points.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       90 2023-04-24 00:19:04.000000 atlasapi-3.0.1b8/atlasapi.egg-info/requires.txt
+-rwxrwxrwx   0 mgm        (502) staff       (20)       18 2023-04-24 00:19:04.000000 atlasapi-3.0.1b8/atlasapi.egg-info/top_level.txt
+drwxr-xr-x   0 mgm        (502) staff       (20)        0 2023-04-24 00:19:04.974475 atlasapi-3.0.1b8/atlascli/
+-rw-r--r--   0 mgm        (502) staff       (20)      581 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlascli/__init__.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1190 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlascli/atlaserrors.py
+-rw-r--r--   0 mgm        (502) staff       (20)     2011 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlascli/atlaskey.py
+-rw-r--r--   0 mgm        (502) staff       (20)     4624 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlascli/cli.py
+-rw-r--r--   0 mgm        (502) staff       (20)     1360 2021-07-31 01:06:14.000000 atlasapi-3.0.1b8/atlascli/listcommand.py
+-rw-r--r--   0 mgm        (502) staff       (20)       38 2023-04-24 00:19:04.975519 atlasapi-3.0.1b8/setup.cfg
+-rw-r--r--   0 mgm        (502) staff       (20)     1770 2023-04-24 00:17:08.000000 atlasapi-3.0.1b8/setup.py
```

### Comparing `atlasapi-3.0.1b7/LICENSE` & `atlasapi-3.0.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/PKG-INFO` & `atlasapi-3.0.1b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasapi
-Version: 3.0.1b7
+Version: 3.0.1b8
 Summary: Expose MongoDB Atlas Cloud provider APIs
 Home-page: https://github.com/mgmonteleone/python-atlasapi
 Author: Matthew G. Monteleone
 Author-email: mgm@mgm.dev
 License: Apache License 2.0
 Keywords: atlas,mongo,mongodb,cloud,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `atlasapi-3.0.1b7/README.rst` & `atlasapi-3.0.1b8/README.rst`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/__init__.py` & `atlasapi-3.0.1b8/atlasapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "3.0.1b7"
+__version__ = "3.0.1b8"
```

### Comparing `atlasapi-3.0.1b7/atlasapi/alerts.py` & `atlasapi-3.0.1b8/atlasapi/alerts.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/api_keys.py` & `atlasapi-3.0.1b8/atlasapi/api_keys.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/atlas.py` & `atlasapi-3.0.1b8/atlasapi/atlas.py`

 * *Files 1% similar despite different names*

```diff
@@ -887,24 +887,20 @@
                 "granularity": granularity, "m": measurement,
                 "period": period, "start": start, "end": end})
 
             logger.debug(f'The URI used will be {uri}')
             # Build the request
             return_val = self.atlas.network.get(Settings.BASE_URL + uri)
             for each_host in return_val:
+                measurement_obj = None
                 try:
                     measurements = each_host.get('measurements')
                 except Exception as e:
-                    logger.error(f"Error getting measurements from results")
-
+                    logger.error(f"Error getting measurements from results, no measurements were found in results")
                     logger.error(e)
-                    logger.error(f"The results look like {results}")
-                    logger.error(f"The results have length {len(list(results))}")
-                    for each in results:
-                        logger.error(f"Results are: {each}")
                     raise e
                 measurements_count = len(measurements)
                 self.logger.info('There are {} measurements.'.format(measurements_count))
 
                 for each in measurements:
                     measurement_obj = AtlasMeasurement(name=each.get('name'),
                                                        period=period,
```

### Comparing `atlasapi-3.0.1b7/atlasapi/atlas_users.py` & `atlasapi-3.0.1b8/atlasapi/atlas_users.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/cloud_backup.py` & `atlasapi-3.0.1b8/atlasapi/cloud_backup.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/clusters.py` & `atlasapi-3.0.1b8/atlasapi/clusters.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/errors.py` & `atlasapi-3.0.1b8/atlasapi/errors.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/events.py` & `atlasapi-3.0.1b8/atlasapi/events.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/events_event_types.py` & `atlasapi-3.0.1b8/atlasapi/events_event_types.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/invoices_pydantic.py` & `atlasapi-3.0.1b8/atlasapi/invoices_pydantic.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/lib.py` & `atlasapi-3.0.1b8/atlasapi/lib.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/maintenance_window.py` & `atlasapi-3.0.1b8/atlasapi/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/measurements.py` & `atlasapi-3.0.1b8/atlasapi/measurements.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from statistics import mean, StatisticsError
 from typing import Optional, Tuple, List, Iterable, NewType
 import logging
 import humanfriendly as hf
 from dateutil.parser import parse
 
 from atlasapi.atlas_types import OptionalFloat
+from typing import Union, Optional
 from atlasapi.lib import _GetAll, AtlasPeriods, AtlasGranularities
 
 logger: logging.Logger = logging.getLogger('Atlas.measurements')
 
 
 class StatisticalValues:
     def __init__(self, data_list: list):
@@ -215,50 +216,58 @@
             percent_used_max = 'MAX_DISK_PARTITION_SPACE_PERCENT_USED'
 
     class Namespaces(_GetAll):
         """Metrics regarding namespaces (databases) on each host.
 
         As found in dbstats (https://www.mongodb.com/docs/manual/reference/command/dbStats/)
             """
-        object_size = 'DATABASE_AVERAGE_OBJECT_SIZE' # dbStats.avgObjSize Average size of each document in bytes. This is the dataSize divided by the number of documents. The scale argument does not affect the avgObjSize value.
+        object_size = 'DATABASE_AVERAGE_OBJECT_SIZE'  # dbStats.avgObjSize Average size of each document in bytes. This is the dataSize divided by the number of documents. The scale argument does not affect the avgObjSize value.
         collection_count = 'DATABASE_COLLECTION_COUNT'
-        data_size = 'DATABASE_DATA_SIZE' # Total size of the uncompressed data held in the database. The dataSize decreases when you remove documents.
-        storage_size = 'DATABASE_STORAGE_SIZE' # Sum of the space allocated to all collections in the database for document storage, including free space. storageSize does not include space allocated to indexes. See indexSize for the total index size.
-        index_size = 'DATABASE_INDEX_SIZE' # Sum of the space allocated to all indexes in the database, including free index space.
+        data_size = 'DATABASE_DATA_SIZE'  # Total size of the uncompressed data held in the database. The dataSize decreases when you remove documents.
+        storage_size = 'DATABASE_STORAGE_SIZE'  # Sum of the space allocated to all collections in the database for document storage, including free space. storageSize does not include space allocated to indexes. See indexSize for the total index size.
+        index_size = 'DATABASE_INDEX_SIZE'  # Sum of the space allocated to all indexes in the database, including free index space.
         index_count = 'DATABASE_INDEX_COUNT'
-        extent_count = 'DATABASE_EXTENT_COUNT' # ?
-        object_count = 'DATABASE_OBJECT_COUNT' # Number of objects (specifically, documents) in the database across all collections.
+        extent_count = 'DATABASE_EXTENT_COUNT'  # ?
+        object_count = 'DATABASE_OBJECT_COUNT'  # Number of objects (specifically, documents) in the database across all collections.
         view_count = 'DATABASE_VIEW_COUNT'
 
 
 # noinspection PyBroadException
 class AtlasMeasurementValue(object):
     def __init__(self, value_dict: dict):
         """
         Class for holding a measurement value
+
+        Does error handling with different data types.
+
+
         :type value_dict: dict
         :param value_dict: An Atlas standard Measurement value dictionary.
         """
-        timestamp: int = value_dict.get('timestamp', None)
+        timestamp: str = value_dict.get('timestamp', None)
         value: float = value_dict.get('value', None)
+        # First cast/validate the timestamp
+        self.timestamp: Optional[datetime] = None
+        self.value: Optional[float] = None
         try:
-            self.timestamp: datetime = parse(timestamp)
+            self.timestamp: Optional[datetime] = parse(timestamp)
         except (ValueError, TypeError):
-            logger.warning('Could not parse "{}" as a datetime.')
-            self.timestamp = None
-        try:
-            if value is None:
-                self.value = None
-            self.value: float = float(value)
-        except ValueError as e:
-            self.value = None
-            logger.warning('Could not parse the metric value "{}". Error was {}'.format(value, e))
-        except TypeError:
-            logger.info('Value is none.')
+            logger.warning(f'Could not parse "{timestamp}" as a datetime.')
+        # Cast/validate the value itself
+        if value is None:
             self.value = None
+        else:
+            try:  # try to cast to a float
+                self.value: float = float(value)
+            except ValueError as e:
+                self.value = None
+                logger.warning(f'Could not parse the metric value "{value}". Error was {e}')
+            except TypeError:
+                logger.warning(f'Could not parse the metric value "{value}" (Type Error). Error was {e}')
+                self.value = None
 
     # noinspection PyBroadException
     @property
     def value_int(self) -> Optional[int]:
         try:
             return int(self.value)
         except Exception as e:
```

### Comparing `atlasapi-3.0.1b7/atlasapi/network.py` & `atlasapi-3.0.1b8/atlasapi/network.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/organizations.py` & `atlasapi-3.0.1b8/atlasapi/organizations.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/projects.py` & `atlasapi-3.0.1b8/atlasapi/projects.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/serverless_pydantic.py` & `atlasapi-3.0.1b8/atlasapi/serverless_pydantic.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/settings.py` & `atlasapi-3.0.1b8/atlasapi/settings.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/specs.py` & `atlasapi-3.0.1b8/atlasapi/specs.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/teams.py` & `atlasapi-3.0.1b8/atlasapi/teams.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi/whitelist.py` & `atlasapi-3.0.1b8/atlasapi/whitelist.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlasapi.egg-info/PKG-INFO` & `atlasapi-3.0.1b8/atlasapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasapi
-Version: 3.0.1b7
+Version: 3.0.1b8
 Summary: Expose MongoDB Atlas Cloud provider APIs
 Home-page: https://github.com/mgmonteleone/python-atlasapi
 Author: Matthew G. Monteleone
 Author-email: mgm@mgm.dev
 License: Apache License 2.0
 Keywords: atlas,mongo,mongodb,cloud,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `atlasapi-3.0.1b7/atlasapi.egg-info/SOURCES.txt` & `atlasapi-3.0.1b8/atlasapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlascli/__init__.py` & `atlasapi-3.0.1b8/atlascli/__init__.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlascli/atlaserrors.py` & `atlasapi-3.0.1b8/atlascli/atlaserrors.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlascli/atlaskey.py` & `atlasapi-3.0.1b8/atlascli/atlaskey.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlascli/cli.py` & `atlasapi-3.0.1b8/atlascli/cli.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/atlascli/listcommand.py` & `atlasapi-3.0.1b8/atlascli/listcommand.py`

 * *Files identical despite different names*

### Comparing `atlasapi-3.0.1b7/setup.py` & `atlasapi-3.0.1b8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import find_packages, setup
 
 setup(
     name='atlasapi',
-    version='3.0.1b7',
+    version='3.0.1b8',
     python_requires='>=3.7',
     packages=find_packages(exclude=("tests",)),
     install_requires=['requests', 'python-dateutil', 'isodate', 'future', 'pytz','coolname',
                       'humanfriendly', 'pydantic', 'pyhumps', 'nose'],
     setup_requires=['wheel'],
     # Metadata
     author="Matthew G. Monteleone",
```

