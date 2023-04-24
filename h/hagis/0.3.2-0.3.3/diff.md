# Comparing `tmp/hagis-0.3.2.tar.gz` & `tmp/hagis-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.3.2.tar", last modified: Sat Apr 22 03:03:30 2023, max compression
+gzip compressed data, was "hagis-0.3.3.tar", last modified: Mon Apr 24 02:08:17 2023, max compression
```

## Comparing `hagis-0.3.2.tar` & `hagis-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 03:03:30.870926 hagis-0.3.2/
--rw-rw-rw-   0        0        0      923 2023-04-22 03:03:30.862928 hagis-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 03:03:30.822360 hagis-0.3.2/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.2/hagis/__init__.py
--rw-rw-rw-   0        0        0    13057 2023-04-22 03:01:48.000000 hagis-0.3.2/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-22 03:03:30.854939 hagis-0.3.2/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 03:03:30.000000 hagis-0.3.2/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-22 02:59:04.000000 hagis-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 03:03:30.870926 hagis-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 02:08:17.334926 hagis-0.3.3/
+-rw-rw-rw-   0        0        0      923 2023-04-24 02:08:17.329131 hagis-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 02:08:17.294603 hagis-0.3.3/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.3/hagis/__init__.py
+-rw-rw-rw-   0        0        0    13240 2023-04-24 02:07:28.000000 hagis-0.3.3/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:08:17.323702 hagis-0.3.3/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-24 02:07:44.000000 hagis-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 02:08:17.337207 hagis-0.3.3/setup.cfg
```

### Comparing `hagis-0.3.2/PKG-INFO` & `hagis-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.2
+Version: 0.3.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.2/hagis/hagis.py` & `hagis-0.3.3/hagis/hagis.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,23 +30,24 @@
         self._model = model
         self._oid_field = oid_field
         self._shape_property_name = shape_property_name
         self._shape_property_type = None
         self._unknown_shape_types = [Any, object, SimpleNamespace]
         self._fields: Dict[str, str] = {}
         self._generate_token: Callable[[], str] = lambda: ""
+        self._requires_init_parameters = hasattr(model, "__dataclass_fields__") or hasattr(model, "_asdict")
         self._is_dynamic = model == SimpleNamespace
 
         if self._is_dynamic:
             return
 
         # List of custom mapping properties that have been handled.
         mapped: List[str] = []
 
-        for model_type in reversed(model.__mro__):
+        for model_type in reversed(model.mro()):
             if hasattr(model_type, "__annotations__"):
                 for property_name, property_type in model_type.__annotations__.items():
                     key = property_name.lower()
 
                     if property_name in mapping:
                         self._fields[key] = mapping[property_name]
                         mapped.append(property_name)
@@ -102,26 +103,29 @@
         """ Sets the static token.
 
         Args:
             token (str): Token.
         """
         self._generate_token = lambda: token
 
-    def query(self, where_clause: str = "1=1", record_count: Optional[int] = None, wkid: Optional[int] = None,
+    def query(self, where_clause: Optional[str] = None, record_count: Optional[int] = None, wkid: Optional[int] = None,
               **kwargs: Any) -> Iterable[T]:
         """ Executes a query.
 
         Args:
-            where_clause (str, optional): Where clause.  Defaults to "1=1".
+            where_clause (str, optional): Where clause.  Defaults to None.
             record_count (Optional[int], optional): Maximum record count.  Defaults to None.
             wkid (Optional[int], optional): Spatial reference.  Defaults to None.
 
         Returns:
             Iterable[T]: Items.
         """
+        if not where_clause:
+            where_clause = "1=1"
+
         if record_count == 0:
             return
 
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
@@ -140,33 +144,35 @@
             kwargs["outSR"] = wkid
 
         for row in islice(self._query(where_clause, fields, keep_querying, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
                 dictionary = {property: getattr(row, field) for (property, field) in self._fields.items()}
-                if hasattr(self._model, "__dataclass_fields__"):
-                    # Support for dataclasses.
+                if self._requires_init_parameters:
+                    # Support for data classes and named tuples.
                     item = self._model(*dictionary.values())
                 else:
-                    # Normal classes require the parameterless constructor.
                     item = self._model()
                     for property_name, property_value in dictionary.items():
                         setattr(item, property_name, property_value)
                 yield item
 
-    def count(self, where_clause: str = "1=1") -> int:
+    def count(self, where_clause: Optional[str] = None) -> int:
         """ Checks the number of items that match the where clause.
 
         Args:
-            where_clause (str, optional): Where clause.  Defaults to "1=1".
+            where_clause (str, optional): Where clause.  Defaults to None.
 
         Returns:
             int: Count.
         """
+        if not where_clause:
+            where_clause = "1=1"
+
         obj = self._call("query", where=where_clause, returnCountOnly=True)
         return obj.count
 
     def find(self, oid: int, **kwargs: Any) -> Optional[T]:
         """ Finds the item by Object ID.
 
         Args:
```

### Comparing `hagis-0.3.2/hagis.egg-info/PKG-INFO` & `hagis-0.3.3/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.2
+Version: 0.3.3
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.2/pyproject.toml` & `hagis-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

