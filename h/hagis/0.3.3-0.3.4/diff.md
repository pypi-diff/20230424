# Comparing `tmp/hagis-0.3.3.tar.gz` & `tmp/hagis-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.3.3.tar", last modified: Mon Apr 24 02:08:17 2023, max compression
+gzip compressed data, was "hagis-0.3.4.tar", last modified: Mon Apr 24 11:59:46 2023, max compression
```

## Comparing `hagis-0.3.3.tar` & `hagis-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 02:08:17.334926 hagis-0.3.3/
--rw-rw-rw-   0        0        0      923 2023-04-24 02:08:17.329131 hagis-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 02:08:17.294603 hagis-0.3.3/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.3/hagis/__init__.py
--rw-rw-rw-   0        0        0    13240 2023-04-24 02:07:28.000000 hagis-0.3.3/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:08:17.323702 hagis-0.3.3/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 02:08:17.000000 hagis-0.3.3/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-24 02:07:44.000000 hagis-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 02:08:17.337207 hagis-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 11:59:46.708927 hagis-0.3.4/
+-rw-rw-rw-   0        0        0      923 2023-04-24 11:59:46.707913 hagis-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 11:59:46.693738 hagis-0.3.4/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.4/hagis/__init__.py
+-rw-rw-rw-   0        0        0    13373 2023-04-24 11:56:52.000000 hagis-0.3.4/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:59:46.705802 hagis-0.3.4/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-24 11:57:16.000000 hagis-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 11:59:46.708927 hagis-0.3.4/setup.cfg
```

### Comparing `hagis-0.3.3/PKG-INFO` & `hagis-0.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.3
+Version: 0.3.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.3/hagis/hagis.py` & `hagis-0.3.4/hagis/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ A high availability GIS client. """
 from datetime import datetime
 from hashlib import md5
-from itertools import islice
+from inspect import signature
+from itertools import chain, islice
 from json import dumps, loads
 from time import time
 from types import SimpleNamespace
 from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 from requests import post
 
 T = TypeVar("T")
@@ -30,16 +31,20 @@
         self._model = model
         self._oid_field = oid_field
         self._shape_property_name = shape_property_name
         self._shape_property_type = None
         self._unknown_shape_types = [Any, object, SimpleNamespace]
         self._fields: Dict[str, str] = {}
         self._generate_token: Callable[[], str] = lambda: ""
-        self._requires_init_parameters = hasattr(model, "__dataclass_fields__") or hasattr(model, "_asdict")
-        self._is_dynamic = model == SimpleNamespace
+
+        self._has_parameterless_constructor = len(set(chain(
+            signature(model.__init__).parameters.keys(),
+            signature(model.__new__).parameters.keys()))) == 3
+
+        self._is_dynamic = issubclass(model, SimpleNamespace)
 
         if self._is_dynamic:
             return
 
         # List of custom mapping properties that have been handled.
         mapped: List[str] = []
 
@@ -144,21 +149,22 @@
             kwargs["outSR"] = wkid
 
         for row in islice(self._query(where_clause, fields, keep_querying, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
                 dictionary = {property: getattr(row, field) for (property, field) in self._fields.items()}
-                if self._requires_init_parameters:
-                    # Support for data classes and named tuples.
-                    item = self._model(*dictionary.values())
-                else:
+                if self._has_parameterless_constructor:
                     item = self._model()
                     for property_name, property_value in dictionary.items():
                         setattr(item, property_name, property_value)
+                else:
+                    # Support for data classes and named tuples.
+                    item = self._model(*dictionary.values())
+
                 yield item
 
     def count(self, where_clause: Optional[str] = None) -> int:
         """ Checks the number of items that match the where clause.
 
         Args:
             where_clause (str, optional): Where clause.  Defaults to None.
```

### Comparing `hagis-0.3.3/hagis.egg-info/PKG-INFO` & `hagis-0.3.4/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.3
+Version: 0.3.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.3/pyproject.toml` & `hagis-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

