# Comparing `tmp/dctrackclient-0.2.3.tar.gz` & `tmp/dctrackclient-0.2.4.tar.gz`

## Comparing `dctrackclient-0.2.3.tar` & `dctrackclient-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/.github/workflows/doc.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/LICENSE
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 dctrackclient-0.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/.github/workflows/doc.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/LICENSE
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 dctrackclient-0.2.4/PKG-INFO
```

### Comparing `dctrackclient-0.2.3/.github/workflows/python-publish.yml` & `dctrackclient-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.3/src/dcTrackClient/__init__.py` & `dctrackclient-0.2.4/src/dcTrackClient/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """Delete an item using the item ID."""
         return self.__request('DELETE', 'api/v2/dcimoperations/items/' + str(id))
 
     def getItem(self, id: int):
         """Get item details using the item ID."""
         return self.__request('GET', 'api/v2/dcimoperations/items/' + str(id))
 
-    def quicksearch(self, data: dict, pageNumber: int, pageSize: int):
+    def searchItems(self, data: dict, pageNumber: int, pageSize: int):
         """Search for items using criteria JSON object. Search criteria can be any of the fields applicable to items, including custom fields. Specify the fields to be included in the response. This API supports pagination."""
         return self.__request('POST', 'api/v2/quicksearch/items?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize), data)
 
     def getCabinetItems(self, cabId: int):
         """Returns a list of Items contained in a Cabinet using the ItemID of the Cabinet. The returned list includes all of the Cabinet's Items including Passive Items."""
         return self.__request('POST', 'api/v2/items/cabinetItems/' + str(cabId))
 
@@ -140,12 +140,42 @@
 
     def getPowerPort(self, itemId: int, portId: int):
         """Use the REST API to retrieve details from one power port on an item."""
         return self.__request('GET', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId))
 
     def updatePowerPort(self, itemId: int, portId: int, data: dict, proceedOnWarning: bool = True):
         """Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item."""
-        return self.__request('PUT', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '?proceedOnWarning=' + str(proceedOnWarning), data)
+        return self.__request('PUT', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '?proceedOnWarning=' + str(proceedOnWarning).lower(), data)
 
     def compatibleConnector(self, itemId: int, portId: int, connectorId: int):
         """Use the REST API to determine if a Connector is compatible with a specific Power Port."""
         return self.__request('GET', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '/connectors/' + str(connectorId) + '/isCompatible')
+
+    # Locations
+
+    def getLocations(self):
+        """Returns a list or all Locations."""
+        return self.__request('GET', '/api/v1/locations')
+
+    def getLocation(self, id: int):
+        """Get a single Location."""
+        return self.__request('GET', '/api/v1/locations/' + str(id))
+
+    def addLocation(self, data: dict, proceedOnWarning: bool = False):
+        """Add a Location."""
+        return self.__request('POST', '/api/v1/locations?proceedOnWarning=' + str(proceedOnWarning).lower(), data)
+
+    def modifyLocation(self, id: int, data: dict, proceedOnWarning: bool = False):
+        """Modify Location details for a single Location. Payload contains new location details. You do not have have to provide all details, but only those that you want to modify."""
+        return self.__request('PUT', '/api/v1/locations/' + str(id) + '?proceedOnWarning=' + str(proceedOnWarning).lower(), data)
+
+    def deleteLocation(self, id: int):
+        """Delete a Location."""
+        return self.__request('DELETE', '/api/v1/locations/' + str(id))
+
+    def searchLocations(self, data: dict, pageNumber: int, pageSize: int):
+        """Search for one or more Locations by user supplied search criteria."""
+        return self.__request('POST', '/api/v2/quicksearch/locations?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize), data)
+
+    def getLocationFieldList(self):
+        """Returns a list of all Location fields."""
+        return self.__request('GET', '/api/v2/quicksearch/locations/locationListFields')
```

### Comparing `dctrackclient-0.2.3/LICENSE` & `dctrackclient-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.3/README.md` & `dctrackclient-0.2.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 ```
 > Delete an item using the item ID.
 ```py
 def getItem(self, id: int):
 ```
 > Get item details using the item ID.
 ```py
-def quicksearch(self, data: dict, pageNumber: int, pageSize: int):
+def searchItems(self, data: dict, pageNumber: int, pageSize: int):
 ```
 > Search for items using criteria JSON object. Search criteria can be any of the fields applicable to items, including custom fields. Specify the fields to be included in the response. This API supports pagination.
 ```py
 def getCabinetItems(self, cabId: int):
 ```
 > Returns a list of Items contained in a Cabinet using the ItemID of the Cabinet. The returned list includes all of the Cabinet's Items including Passive Items.
 ```py
@@ -194,7 +194,35 @@
 def updatePowerPort(self, itemId: int, portId: int, data: dict, proceedOnWarning: bool = True):
 ```
 > Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
 ```py
 def compatibleConnector(self, itemId: int, portId: int, connectorId: int):
 ```
 > Use the REST API to determine if a Connector is compatible with a specific Power Port.
+```py
+def getLocations(self):
+```
+> Returns a list or all Locations.
+```py
+def getLocation(self, id: int):
+```
+> Get a single Location.
+```py
+def addLocation(self, data: dict, proceedOnWarning: bool = False):
+```
+> Add a Location.
+```py
+def modifyLocation(self, id: int, data: dict, proceedOnWarning: bool = False):
+```
+> Modify Location details for a single Location. Payload contains new location details. You do not have have to provide all details, but only those that you want to modify.
+```py
+def deleteLocation(self, id: int):
+```
+> Delete a Location.
+```py
+def searchLocations(self, data: dict, pageNumber: int, pageSize: int):
+```
+> Search for one or more Locations by user supplied search criteria.
+```py
+def getLocationFieldList(self):
+```
+> Returns a list of all Location fields.
```

### Comparing `dctrackclient-0.2.3/pyproject.toml` & `dctrackclient-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.2.3/PKG-INFO` & `dctrackclient-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.2.3
+Version: 0.2.4
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -101,15 +101,15 @@
 ```
 > Delete an item using the item ID.
 ```py
 def getItem(self, id: int):
 ```
 > Get item details using the item ID.
 ```py
-def quicksearch(self, data: dict, pageNumber: int, pageSize: int):
+def searchItems(self, data: dict, pageNumber: int, pageSize: int):
 ```
 > Search for items using criteria JSON object. Search criteria can be any of the fields applicable to items, including custom fields. Specify the fields to be included in the response. This API supports pagination.
 ```py
 def getCabinetItems(self, cabId: int):
 ```
 > Returns a list of Items contained in a Cabinet using the ItemID of the Cabinet. The returned list includes all of the Cabinet's Items including Passive Items.
 ```py
@@ -208,7 +208,35 @@
 def updatePowerPort(self, itemId: int, portId: int, data: dict, proceedOnWarning: bool = True):
 ```
 > Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
 ```py
 def compatibleConnector(self, itemId: int, portId: int, connectorId: int):
 ```
 > Use the REST API to determine if a Connector is compatible with a specific Power Port.
+```py
+def getLocations(self):
+```
+> Returns a list or all Locations.
+```py
+def getLocation(self, id: int):
+```
+> Get a single Location.
+```py
+def addLocation(self, data: dict, proceedOnWarning: bool = False):
+```
+> Add a Location.
+```py
+def modifyLocation(self, id: int, data: dict, proceedOnWarning: bool = False):
+```
+> Modify Location details for a single Location. Payload contains new location details. You do not have have to provide all details, but only those that you want to modify.
+```py
+def deleteLocation(self, id: int):
+```
+> Delete a Location.
+```py
+def searchLocations(self, data: dict, pageNumber: int, pageSize: int):
+```
+> Search for one or more Locations by user supplied search criteria.
+```py
+def getLocationFieldList(self):
+```
+> Returns a list of all Location fields.
```

