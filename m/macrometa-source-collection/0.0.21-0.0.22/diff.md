# Comparing `tmp/macrometa-source-collection-0.0.21.tar.gz` & `tmp/macrometa-source-collection-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.21.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.22.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.21.tar` & `macrometa-source-collection-0.0.22.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8418 2023-04-17 09:51:14.391056 macrometa-source-collection-0.0.21/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     5895 2023-04-17 09:51:14.391056 macrometa-source-collection-0.0.21/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-04-17 09:51:14.639061 macrometa-source-collection-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.21/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0     8418 2023-04-24 06:37:09.347299 macrometa-source-collection-0.0.22/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     5962 2023-04-24 06:37:09.347299 macrometa-source-collection-0.0.22/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-04-24 06:37:09.599305 macrometa-source-collection-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.22/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.22/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.21/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.22/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.21/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.22/macrometa_source_collection/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,17 @@
                 except Exception:
                     self.export_errors.inc()
         
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
     def load_existing_data(self, stream):
-        cursor = self._c8_client.execute_query(f"FOR d IN @@collection RETURN d",
-                                               bind_vars={"@collection": self._collection})
+        cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
+                                               bind_vars={"@collection": self._collection},
+                                               stream=True)
         while (not cursor.empty()) or cursor.has_more():
             rec = cursor.next()
             rec.pop('_id', None)
             rec.pop('_rev', None)
             singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
             singer.write_message(singer_record)
```

### Comparing `macrometa-source-collection-0.0.21/pyproject.toml` & `macrometa-source-collection-0.0.22/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.21'
+version='0.0.22'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.21/setup.py` & `macrometa-source-collection-0.0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.21',
+    'version': '0.0.22',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.21/PKG-INFO` & `macrometa-source-collection-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.21
+Version: 0.0.22
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

