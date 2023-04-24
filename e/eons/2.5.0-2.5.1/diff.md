# Comparing `tmp/eons-2.5.0.tar.gz` & `tmp/eons-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.5.0.tar", last modified: Sat Apr 22 19:53:17 2023, max compression
+gzip compressed data, was "eons-2.5.1.tar", last modified: Mon Apr 24 01:09:37 2023, max compression
```

## Comparing `eons-2.5.0.tar` & `eons-2.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:17.001582 eons-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-22 19:53:17.001582 eons-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-04-22 19:53:00.000000 eons-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84209 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:17.001582 eons-2.5.0/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:53:08.000000 eons-2.5.0/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 19:52:53.000000 eons-2.5.0/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:53:16.997582 eons-2.5.0/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-22 19:53:16.000000 eons-2.5.0/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 19:53:08.000000 eons-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-22 19:53:17.001582 eons-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:09:37.789247 eons-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 01:09:37.789247 eons-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-04-24 01:09:22.000000 eons-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:09:37.785247 eons-2.5.1/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:09:37.785247 eons-2.5.1/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 01:09:29.000000 eons-2.5.1/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84297 2023-04-24 01:09:29.000000 eons-2.5.1/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:09:37.789247 eons-2.5.1/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-24 01:09:17.000000 eons-2.5.1/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:09:29.000000 eons-2.5.1/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:09:37.789247 eons-2.5.1/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:09:29.000000 eons-2.5.1/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 01:09:17.000000 eons-2.5.1/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 01:09:17.000000 eons-2.5.1/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 01:09:17.000000 eons-2.5.1/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 01:09:17.000000 eons-2.5.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 01:09:17.000000 eons-2.5.1/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:09:37.789247 eons-2.5.1/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 01:09:37.000000 eons-2.5.1/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 01:09:37.000000 eons-2.5.1/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:09:37.000000 eons-2.5.1/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 01:09:37.000000 eons-2.5.1/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 01:09:37.000000 eons-2.5.1/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 01:09:29.000000 eons-2.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 01:09:37.789247 eons-2.5.1/setup.cfg
```

### Comparing `eons-2.5.0/PKG-INFO` & `eons-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.0
+Version: 2.5.1
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.0/README.md` & `eons-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.5.0/pkg/eons/eons.py` & `eons-2.5.1/pkg/eons/eons.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,14 +976,17 @@
 		return default, False
 
 
 	def fetch_location_environment(this, varName, default, fetchFrom, attempted):
 		envVar = os.getenv(varName)
 		if (envVar is not None):
 			return envVar, True
+		envVar = os.getenv(varName.upper())
+		if (envVar is not None):
+			return envVar, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
 
 def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
 	raise MethodPendingPopulation("METHOD PENDING POPULATION")
```

### Comparing `eons-2.5.0/pkg/eons/method/External.py` & `eons-2.5.1/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.0/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.5.1/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.0/pkg/eons/resolve/resolve_import_module.py` & `eons-2.5.1/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.5.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.0/pkg/eons.egg-info/PKG-INFO` & `eons-2.5.1/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.0
+Version: 2.5.1
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.0/pkg/eons.egg-info/SOURCES.txt` & `eons-2.5.1/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.5.0/setup.cfg` & `eons-2.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.5.0
+version = 2.5.1
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,17 +18,17 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	tqdm
 	pyyaml
 	requests
+	tqdm
 	jsonpickle
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build =
```

