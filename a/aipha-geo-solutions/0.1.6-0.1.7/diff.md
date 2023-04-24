# Comparing `tmp/aipha_geo_solutions-0.1.6.tar.gz` & `tmp/aipha_geo_solutions-0.1.7.tar.gz`

## Comparing `aipha_geo_solutions-0.1.6.tar` & `aipha_geo_solutions-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/example.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/__init__.py
--rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/operators.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/webservice_api.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/LICENSE
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/example.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/__init__.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/operators.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/webservice_api.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/LICENSE
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.7/PKG-INFO
```

### Comparing `aipha_geo_solutions-0.1.6/example.py` & `aipha_geo_solutions-0.1.7/example.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/operators.py` & `aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,61 +26,65 @@
 
 
 def point_cloud_classification_inference(client,
    file_in='file.laz',
    file_out='classified_file.laz',
    model_path='model_path',
    cols_data='x,y,z,intensity',
-   cols_labels='classification'):
+   cols_labels='classification',
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "point cloud classification inference",
     all_parameters,
     client.get_server_address())
 
 
 def convert_laz_point_formats(client,
    file_in='file.laz',
    file_out='converted_file.laz',
-   format=7):
+   format=7,
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "convert laz point formats",
     all_parameters,
     client.get_server_address())
 
 
 def point_cloud_crop_circle(client,
-   file_in='file.laz',
-   file_out='classified_file.laz',
+   in_file='file.laz',
+   out_file='classified_file.laz',
    latitude=0,
    longitude=0,
-   radius=1):
+   radius=1,
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "point cloud crop circle",
     all_parameters,
     client.get_server_address())
 
 
 def union_point_clouds(client,
-   files_in='file.laz',
-   file_out='converted_file.laz'):
+   in_files='file.laz',
+   out_file='converted_file.laz',
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "union point clouds",
@@ -91,15 +95,16 @@
 def point_cloud_filter_label_noise(client,
    file_in_data='file.laz',
    file_in_labels='converted_file.laz',
    file_out='converted_file.laz',
    k_nearest_neighbours=5,
    sigma=10,
    dim=3,
-   invalid_label=0):
+   invalid_label=0,
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "point cloud filter label noise",
@@ -111,15 +116,16 @@
    in_points_file='file.laz',
    in_labels_file='file.laz',
    out_directory='objects',
    out_prefix='object',
    label_col='classification',
    object_class=6,
    max_distance=1,
-   min_points=1):
+   min_points=1,
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "segment objects",
@@ -127,30 +133,32 @@
     client.get_server_address())
 
 
 def select_center_object(client,
    in_directory='objects',
    out_file='selected.laz',
    latitude=1,
-   longitude=1):
+   longitude=1,
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "select center object",
     all_parameters,
     client.get_server_address())
 
 
 def assign_point_labels(client,
    file_source_in='file.laz',
    file_labels_in='file.laz',
-   file_source_out='converted_file.laz'):
+   file_source_out='converted_file.laz',
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "assign point labels",
@@ -159,15 +167,16 @@
 
 
 def select_points_by_value(client,
    file_source_in='file.laz',
    min_value=1,
    max_value=1,
    attribute='classification',
-   file_source_out='selected.laz'):
+   file_source_out='selected.laz',
+   instance_type='P2'):
 
   all_parameters = locals().copy()
   del all_parameters['client']
   return command_request(
     client.get_username(),
     client.get_token(),
     "select points by value",
```

### Comparing `aipha_geo_solutions-0.1.6/src/aipha_geo_solutions/webservice_api.py` & `aipha_geo_solutions-0.1.7/src/aipha_geo_solutions/webservice_api.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.6/LICENSE` & `aipha_geo_solutions-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.6/pyproject.toml` & `aipha_geo_solutions-0.1.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aipha_geo_solutions"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Timo Hackel", email="timo.hackel@aipha.ch" },
 ]
 description = "A python API to the AIPHA webservices"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `aipha_geo_solutions-0.1.6/PKG-INFO` & `aipha_geo_solutions-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipha_geo_solutions
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python API to the AIPHA webservices
 Project-URL: Homepage, https://github.com/AIPHA-Geo-Solutions/
 Project-URL: Bug Tracker, https://github.com/AIPHA-Geo-Solutions/AIPHAPythonAPI/issues
 Author-email: Timo Hackel <timo.hackel@aipha.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

