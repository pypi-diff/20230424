# Comparing `tmp/rubrical-0.2.0.tar.gz` & `tmp/rubrical-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubrical-0.2.0.tar", max compression
+gzip compressed data, was "rubrical-0.2.1.tar", max compression
```

## Comparing `rubrical-0.2.0.tar` & `rubrical-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    15976 2023-04-23 12:17:43.241480 rubrical-0.2.0/LICENSE
--rw-r--r--   0        0        0     2782 2023-04-23 12:17:43.241480 rubrical-0.2.0/README.md
--rw-r--r--   0        0        0     1865 2023-04-23 12:18:06.421523 rubrical-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/__init__.py
--rw-r--r--   0        0        0      784 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/__init__.py
--rw-r--r--   0        0        0     2255 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/semversion.py
--rw-r--r--   0        0        0      519 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/string.py
--rw-r--r--   0        0        0      295 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/comparisons/utils.py
--rw-r--r--   0        0        0      568 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/enum.py
--rw-r--r--   0        0        0     2623 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/main.py
--rw-r--r--   0        0        0        0 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/__init__.py
--rw-r--r--   0        0        0     2519 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/base_package_manager.py
--rw-r--r--   0        0        0     1242 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/go.py
--rw-r--r--   0        0        0     1479 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/jsonnet.py
--rw-r--r--   0        0        0     4143 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/nodejs.py
--rw-r--r--   0        0        0     1933 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/python.py
--rw-r--r--   0        0        0      271 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/package_managers/utilities/git.py
--rw-r--r--   0        0        0     2352 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/reporters/gh.py
--rw-r--r--   0        0        0     1476 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/reporters/terminal.py
--rw-r--r--   0        0        0     4265 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/rubrical.py
--rw-r--r--   0        0        0      467 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/schemas/configuration.py
--rw-r--r--   0        0        0      251 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/schemas/package.py
--rw-r--r--   0        0        0      235 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/schemas/results.py
--rw-r--r--   0        0        0      633 2023-04-23 12:17:43.241480 rubrical-0.2.0/rubrical/utilities/console.py
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 rubrical-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    15976 2023-04-24 08:57:50.944846 rubrical-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2782 2023-04-24 08:57:50.944846 rubrical-0.2.1/README.md
+-rw-r--r--   0        0        0     1865 2023-04-24 08:58:13.497104 rubrical-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/__init__.py
+-rw-r--r--   0        0        0      784 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/__init__.py
+-rw-r--r--   0        0        0     2255 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/semversion.py
+-rw-r--r--   0        0        0      519 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/string.py
+-rw-r--r--   0        0        0      295 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/comparisons/utils.py
+-rw-r--r--   0        0        0      568 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/enum.py
+-rw-r--r--   0        0        0     2623 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/main.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/__init__.py
+-rw-r--r--   0        0        0     2519 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/base_package_manager.py
+-rw-r--r--   0        0        0     1242 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/go.py
+-rw-r--r--   0        0        0     1479 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/jsonnet.py
+-rw-r--r--   0        0        0     4102 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/nodejs.py
+-rw-r--r--   0        0        0     1933 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/python.py
+-rw-r--r--   0        0        0      271 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/package_managers/utilities/git.py
+-rw-r--r--   0        0        0     2352 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/reporters/gh.py
+-rw-r--r--   0        0        0     1476 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/reporters/terminal.py
+-rw-r--r--   0        0        0     4265 2023-04-24 08:57:50.944846 rubrical-0.2.1/rubrical/rubrical.py
+-rw-r--r--   0        0        0      467 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/schemas/configuration.py
+-rw-r--r--   0        0        0      251 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/schemas/package.py
+-rw-r--r--   0        0        0      235 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/schemas/results.py
+-rw-r--r--   0        0        0      633 2023-04-24 08:57:50.948844 rubrical-0.2.1/rubrical/utilities/console.py
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 rubrical-0.2.1/PKG-INFO
```

### Comparing `rubrical-0.2.0/LICENSE` & `rubrical-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/README.md` & `rubrical-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/pyproject.toml` & `rubrical-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.isort]
 profile = "black"
 
 [tool.setuptools_scm]
 
 [tool.poetry]
 name = "rubrical"
-version = "0.2.0"
+version = "0.2.1"
 description = "A CLI to encourage (😅) people to update their dependencies!"
 authors = ["Ivan Lee <ivanklee86@gmail.com>"]
 license = "MPL-2.0"
 homepage = "https://github.com/ivanklee86/rubrical"
 repository = "https://github.com/ivanklee86/rubrical"
 readme = "README.md"
 classifiers=[
```

### Comparing `rubrical-0.2.0/rubrical/comparisons/__init__.py` & `rubrical-0.2.1/rubrical/comparisons/__init__.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/comparisons/semversion.py` & `rubrical-0.2.1/rubrical/comparisons/semversion.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/comparisons/string.py` & `rubrical-0.2.1/rubrical/comparisons/string.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/enum.py` & `rubrical-0.2.1/rubrical/enum.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/main.py` & `rubrical-0.2.1/rubrical/main.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/package_managers/base_package_manager.py` & `rubrical-0.2.1/rubrical/package_managers/base_package_manager.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/package_managers/go.py` & `rubrical-0.2.1/rubrical/package_managers/go.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/package_managers/jsonnet.py` & `rubrical-0.2.1/rubrical/package_managers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/package_managers/nodejs.py` & `rubrical-0.2.1/rubrical/package_managers/nodejs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import json
 
-from benedict import benedict
-
 from rubrical.enum import DependencySpecifications, SupportedPackageManagers
 from rubrical.package_managers.base_package_manager import BasePackageManager
 from rubrical.schemas.package import Package
 
 
 class NodeJS(BasePackageManager):
     target_files = ["package.json"]
@@ -20,15 +18,15 @@
             DependencySpecifications.COMPATIBLE.value: ["^"],
         }
 
     def _parse_packagelock(
         self, package_file_filename: str, package_file_contents: str
     ):
         self.packages[package_file_filename] = []
-        package_json = benedict(json.loads(package_file_contents))
+        package_json = json.loads(package_file_contents)
 
         for dependency_key in [
             x for x in package_json.keys() if "dependencies" in x.lower()
         ]:
             dependency_section = package_json[dependency_key]
 
             for package, version in dependency_section.items():
```

### Comparing `rubrical-0.2.0/rubrical/package_managers/python.py` & `rubrical-0.2.1/rubrical/package_managers/python.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/reporters/gh.py` & `rubrical-0.2.1/rubrical/reporters/gh.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/reporters/terminal.py` & `rubrical-0.2.1/rubrical/reporters/terminal.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/rubrical.py` & `rubrical-0.2.1/rubrical/rubrical.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/rubrical/utilities/console.py` & `rubrical-0.2.1/rubrical/utilities/console.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.0/PKG-INFO` & `rubrical-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubrical
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI to encourage (😅) people to update their dependencies!
 Home-page: https://github.com/ivanklee86/rubrical
 License: MPL-2.0
 Author: Ivan Lee
 Author-email: ivanklee86@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

