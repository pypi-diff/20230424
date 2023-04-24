# Comparing `tmp/eons-2.5.4.tar.gz` & `tmp/eons-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.5.4.tar", last modified: Mon Apr 24 05:59:02 2023, max compression
+gzip compressed data, was "eons-2.5.5.tar", last modified: Mon Apr 24 06:27:52 2023, max compression
```

## Comparing `eons-2.5.4.tar` & `eons-2.5.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:59:02.388243 eons-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 05:59:02.392243 eons-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-04-24 05:58:44.000000 eons-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:59:02.384243 eons-2.5.4/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:59:02.388243 eons-2.5.4/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 05:58:52.000000 eons-2.5.4/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84395 2023-04-24 05:58:52.000000 eons-2.5.4/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:59:02.388243 eons-2.5.4/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-24 05:58:37.000000 eons-2.5.4/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:58:52.000000 eons-2.5.4/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:59:02.388243 eons-2.5.4/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:58:52.000000 eons-2.5.4/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 05:58:37.000000 eons-2.5.4/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 05:58:37.000000 eons-2.5.4/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 05:58:37.000000 eons-2.5.4/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 05:58:37.000000 eons-2.5.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 05:58:37.000000 eons-2.5.4/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:59:02.388243 eons-2.5.4/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 05:59:02.000000 eons-2.5.4/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 05:59:02.000000 eons-2.5.4/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:59:02.000000 eons-2.5.4/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 05:59:02.000000 eons-2.5.4/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 05:59:02.000000 eons-2.5.4/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 05:58:52.000000 eons-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 05:59:02.392243 eons-2.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:27:52.928168 eons-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 06:27:52.928168 eons-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-04-24 06:27:36.000000 eons-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:27:52.924168 eons-2.5.5/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:27:52.924168 eons-2.5.5/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 06:27:44.000000 eons-2.5.5/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84396 2023-04-24 06:27:44.000000 eons-2.5.5/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:27:52.928168 eons-2.5.5/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-24 06:27:29.000000 eons-2.5.5/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:27:44.000000 eons-2.5.5/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:27:52.928168 eons-2.5.5/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:27:44.000000 eons-2.5.5/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 06:27:29.000000 eons-2.5.5/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 06:27:29.000000 eons-2.5.5/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 06:27:29.000000 eons-2.5.5/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 06:27:29.000000 eons-2.5.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 06:27:29.000000 eons-2.5.5/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:27:52.928168 eons-2.5.5/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-24 06:27:52.000000 eons-2.5.5/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 06:27:52.000000 eons-2.5.5/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:27:52.000000 eons-2.5.5/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 06:27:52.000000 eons-2.5.5/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 06:27:52.000000 eons-2.5.5/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 06:27:44.000000 eons-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 06:27:52.928168 eons-2.5.5/setup.cfg
```

### Comparing `eons-2.5.4/PKG-INFO` & `eons-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.4
+Version: 2.5.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.4/README.md` & `eons-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.5.4/pkg/eons/eons.py` & `eons-2.5.5/pkg/eons/eons.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,15 +712,15 @@
 			# setattr(this, method.name, method.__call__.__get__(this, this.__class__))
 
 			# appears to work for all python versions >= 3.8
 			setattr(this, method.name, method.__call__.__get__(method, method.__class__))
 
 
 
-# Set this.precursor
+	# Set this.precursor
 	# Also set this.executor because it's easy.
 	def PopulatePrecursor(this):
 		if (this.executor is None):
 			if ('executor' in this.kwargs):
 				this.executor = this.kwargs.pop('executor')
 			else:
 				logging.warning(f"{this.name} was not given an 'executor'. Some features will not be available.")
```

### Comparing `eons-2.5.4/pkg/eons/method/External.py` & `eons-2.5.5/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.4/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.5.5/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.4/pkg/eons/resolve/resolve_import_module.py` & `eons-2.5.5/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.5.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.5.4/pkg/eons.egg-info/PKG-INFO` & `eons-2.5.5/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.5.4
+Version: 2.5.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.5.4/pkg/eons.egg-info/SOURCES.txt` & `eons-2.5.5/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.5.4/setup.cfg` & `eons-2.5.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.5.4
+version = 2.5.5
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,18 +18,18 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	jsonpickle
 	pyyaml
-	tqdm
+	jsonpickle
 	requests
+	tqdm
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

