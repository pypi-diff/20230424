# Comparing `tmp/macrometa-source-collection-0.0.22.tar.gz` & `tmp/macrometa-source-collection-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.22.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.23.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.22.tar` & `macrometa-source-collection-0.0.23.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8418 2023-04-24 06:37:09.347299 macrometa-source-collection-0.0.22/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     5962 2023-04-24 06:37:09.347299 macrometa-source-collection-0.0.22/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-04-24 06:37:09.599305 macrometa-source-collection-0.0.22/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.22/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0     8418 2023-04-24 11:33:16.759162 macrometa-source-collection-0.0.23/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     6211 2023-04-24 11:33:16.759162 macrometa-source-collection-0.0.23/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-04-24 11:33:17.003165 macrometa-source-collection-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.23/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.23/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.22/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.23/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.22/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.23/macrometa_source_collection/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import singer
 from c8 import C8Client
 from datetime import datetime
 from prometheus_client import start_http_server, Counter, Histogram
 from singer import utils
 from singer.catalog import CatalogEntry
 
+LOGGER = singer.get_logger('macrometa_source_collection')
 
 class GDNCollectionClient:
     """Client for handling GDN collection streams."""
 
     def __init__(self, config) -> None:
         """Init new GDN Collection Client."""
         _host = config.get("region")
@@ -63,18 +64,20 @@
         start_http_server(8000)
 
     def sync(self, stream):
         """Return documents in target GDN collection as records."""
         if self._c8_client.has_collection(self._collection):
             self.send_schema_message(stream)
             self.load_existing_data(stream)
+            LOGGER.info(f"Full table sync completed")
             meta_keys = ['_key', '_sdc_deleted_at']
             while True:
                 try: 
                     msg = self._consumer.receive()
+                    LOGGER.warn(f"Message recevied from stream: {msg}")
                     data = msg.data()
                     if data == None or not data:
                         continue
                     props = msg.properties()
                     j = json.loads(data.decode("utf8"))
                     j['_sdc_deleted_at'] = None
                     if props["op"] == "INSERT" or props["op"] == "UPDATE":
@@ -88,15 +91,16 @@
                         singer.write_message(singer_record)
                     self.exported_bytes.inc(len(data))
                     self.exported_documents.inc()
                     time = datetime.fromtimestamp(msg.publish_timestamp()/1000)
                     event_time = datetime.strptime(time, "%Y-%m-%dT%H:%M:%S.%fZ")
                     self.export_lag.observe((utils.now() - event_time).total_seconds())
                     self._consumer.acknowledge(msg.message_id())
-                except Exception:
+                except Exception as e:
+                    LOGGER.warn(f"Exception received: {e}")
                     self.export_errors.inc()
         
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
     def load_existing_data(self, stream):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
```

### Comparing `macrometa-source-collection-0.0.22/pyproject.toml` & `macrometa-source-collection-0.0.23/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.22'
+version='0.0.23'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.22/setup.py` & `macrometa-source-collection-0.0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.22',
+    'version': '0.0.23',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.22/PKG-INFO` & `macrometa-source-collection-0.0.23/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.22
+Version: 0.0.23
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

