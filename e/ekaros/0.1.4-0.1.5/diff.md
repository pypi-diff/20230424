# Comparing `tmp/ekaros-0.1.4.tar.gz` & `tmp/ekaros-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekaros-0.1.4.tar", max compression
+gzip compressed data, was "ekaros-0.1.5.tar", max compression
```

## Comparing `ekaros-0.1.4.tar` & `ekaros-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 00:50:28.647872 ekaros-0.1.4/LICENSE
--rw-r--r--   0        0        0     3345 2023-04-21 00:50:28.647872 ekaros-0.1.4/README.md
--rw-r--r--   0        0        0     2964 2023-04-21 00:51:01.404156 ekaros-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/__cli__.py
--rw-r--r--   0        0        0      875 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/__init__.py
--rw-r--r--   0        0        0       44 2023-04-21 00:51:01.344155 ekaros-0.1.4/src/ekaros/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/conf/task/__init__.yaml
--rw-r--r--   0        0        0      196 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 00:50:28.647872 ekaros-0.1.4/src/ekaros/py.typed
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 ekaros-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-24 18:50:13.655914 ekaros-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3345 2023-04-24 18:50:13.655914 ekaros-0.1.5/README.md
+-rw-r--r--   0        0        0     2964 2023-04-24 18:50:41.660159 ekaros-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/__cli__.py
+-rw-r--r--   0        0        0      815 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-24 18:50:41.604159 ekaros-0.1.5/src/ekaros/_version.py
+-rw-r--r--   0        0        0        0 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      196 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/project.toml
+-rw-r--r--   0        0        0        0 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/py.typed
+-rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 ekaros-0.1.5/PKG-INFO
```

### Comparing `ekaros-0.1.4/LICENSE` & `ekaros-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.4/README.md` & `ekaros-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.4/pyproject.toml` & `ekaros-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ekaros"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Python Library for Generative AI Art"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://ekaros.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "ekaros", from = "src" }]
```

### Comparing `ekaros-0.1.4/src/ekaros/__init__.py` & `ekaros-0.1.5/src/ekaros/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import os
 
-import toml
 from hyfi import HyFI, about, global_config
 
 from ._version import __version__
 
 # Read and parse pyproject.toml
 current_dir = os.path.dirname(os.path.abspath(__file__))
-pyproject_path = os.path.join(current_dir, "project.toml")
+about_path = os.path.join(current_dir, "conf", "about", "__init__.yaml")
 
-with open(pyproject_path) as f:
-    pyproject_data = toml.load(f)
+about_data = HyFI.load(about_path)
 
-# Extract package information from pyproject.toml
-project_data = pyproject_data.get("metadata", {})
-about.name = project_data.get("name", "package name")
-about.author = project_data.get("authors", ["Author name"])[0]
-about.description = project_data.get("description", "package description")
-about.homepage = project_data.get("homepage", "https://package.homepage")
+# Extract package information
+about.name = about_data.get("name", "package name")
+about.authors = about_data.get("authors", ["Author name"])
+about.description = about_data.get("description", "package description")
+about.homepage = about_data.get("homepage", "https://package.homepage")
+about.license = about_data.get("license", "MIT")
 about.version = __version__
 global_config.hyfi_package_config_path = "pkg://ekaros.conf"
 
 
 def get_version() -> str:
     """This is the cli function of the package"""
     return __version__
```

### Comparing `ekaros-0.1.4/src/ekaros/conf/dotenv/__init__.yaml` & `ekaros-0.1.5/src/ekaros/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.4/src/ekaros/conf/hydra/help/help.yaml` & `ekaros-0.1.5/src/ekaros/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.4/src/ekaros/conf/mode/__init__.yaml` & `ekaros-0.1.5/src/ekaros/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.4/src/ekaros/conf/path/__default__.yaml` & `ekaros-0.1.5/src/ekaros/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.4/src/ekaros/conf/path/__init__.yaml` & `ekaros-0.1.5/src/ekaros/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.4/PKG-INFO` & `ekaros-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ekaros
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python Library for Generative AI Art
 Home-page: https://ekaros.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

