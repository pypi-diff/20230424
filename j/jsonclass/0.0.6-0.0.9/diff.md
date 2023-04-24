# Comparing `tmp/jsonclass-0.0.6.tar.gz` & `tmp/jsonclass-0.0.9.tar.gz`

## Comparing `jsonclass-0.0.6.tar` & `jsonclass-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jsonclass-0.0.6/test_upload.sh
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jsonclass-0.0.6/upload.sh
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jsonclass-0.0.6/src/jsonclass.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 jsonclass-0.0.6/tests/test.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jsonclass-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.6/LICENSE
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jsonclass-0.0.6/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jsonclass-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jsonclass-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jsonclass-0.0.9/test_upload.sh
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jsonclass-0.0.9/upload.sh
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jsonclass-0.0.9/src/jsonclass/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jsonclass-0.0.9/src/jsonclass/dumps.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 jsonclass-0.0.9/src/jsonclass/jsonclass.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jsonclass-0.0.9/src/jsonclass/loads.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jsonclass-0.0.9/tests/test.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jsonclass-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.9/LICENSE
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jsonclass-0.0.9/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jsonclass-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jsonclass-0.0.9/PKG-INFO
```

### Comparing `jsonclass-0.0.6/src/jsonclass.py` & `jsonclass-0.0.9/src/jsonclass/jsonclass.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,43 @@
-from functools import singledispatch
 from typing import Dict, Type, Any
 
 _json_classes: Dict[str, Type['JSONClass']] = {}
 
 
 class JSONClass:
     _data: Dict[str, Any]
 
     def __init_subclass__(cls):
         object.__init_subclass__()
         _json_classes[cls.__qualname__] = cls
 
-    def __new__(cls, data: Dict[str, Any] = None, /, **kwargs):
-        _instance = object.__new__(cls)
-        object.__setattr__(_instance, "_data", dict(data or {}, **kwargs, __json_class__=cls.__qualname__))
-        return _instance
+    @staticmethod
+    def deserializable(data: Dict[str, Any]):
+        return "__json_class__" in data
+
+    @staticmethod
+    def load(data: Dict[str, Any]):
+        cls = _json_classes[data["__json_class__"]]
+        del data["__json_class__"]
+        return cls(data)
+
+    def __init__(self, data: Dict[str, Any] = None, /, **kwargs):
+        object.__setattr__(
+            self,
+            "_data",
+            dict(data or {}, **kwargs)
+        )
 
     def __getattr__(self, item):
         if item not in self._data:
             typ = self.__class__.__annotations__[item]
             if issubclass(typ, (JSONClass, list, set, dict)):
                 self._data[item] = typ()
             else:
                 raise AttributeError
         return self._data[item]
 
     def __setattr__(self, key, value):
         self._data[key] = value
 
-    def to_json(self):
-        return {
-            name: value.to_json() if isinstance(value, JSONClass) else value
-            for name, value in self._data.items()
-        }
-
-
-@singledispatch
-def load(data):
-    return data
-
-
-@load.register
-def _(data: dict):
-    if "__json_class__" in data:
-        class_name = data["__json_class__"]
-        del data["__json_class__"]
-        return _json_classes[class_name]({key: load(value) for key, value in data.items()})
-    else:
-        return data
+    def to_dict(self):
+        return dict(self._data, __json_class__=self.__class__.__qualname__)
```

### Comparing `jsonclass-0.0.6/.gitignore` & `jsonclass-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.6/LICENSE` & `jsonclass-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.6/pyproject.toml` & `jsonclass-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonclass"
-version = "0.0.6"
+version = "0.0.9"
 authors = [
   { name="soundagain2", email="soundagain2@proton.me" },
 ]
 description = "Convert json to object and back in Python."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
@@ -17,8 +17,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/soundagain2/jsonclass"
 "Bug Tracker" = "https://github.com/soundagain2/jsonclass/issues"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/jsonclass.py"]
+packages = ["src/jsonclass"]
```

### Comparing `jsonclass-0.0.6/PKG-INFO` & `jsonclass-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonclass
-Version: 0.0.6
+Version: 0.0.9
 Summary: Convert json to object and back in Python.
 Project-URL: Homepage, https://github.com/soundagain2/jsonclass
 Project-URL: Bug Tracker, https://github.com/soundagain2/jsonclass/issues
 Author-email: soundagain2 <soundagain2@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

