# Comparing `tmp/anyjsonthing-0.3.0.tar.gz` & `tmp/anyjsonthing-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyjsonthing-0.3.0.tar", last modified: Tue Mar 14 14:16:02 2023, max compression
+gzip compressed data, was "anyjsonthing-0.3.1.tar", last modified: Mon Apr 24 09:14:19 2023, max compression
```

## Comparing `anyjsonthing-0.3.0.tar` & `anyjsonthing-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:16:02.046597 anyjsonthing-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-14 14:15:09.000000 anyjsonthing-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-14 14:16:02.046597 anyjsonthing-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-03-14 14:15:09.000000 anyjsonthing-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-14 14:15:09.000000 anyjsonthing-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-14 14:16:02.046597 anyjsonthing-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:16:02.046597 anyjsonthing-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:16:02.046597 anyjsonthing-0.3.0/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:16:02.046597 anyjsonthing-0.3.0/src/main/anyjsonthing/
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-03-14 14:15:09.000000 anyjsonthing-0.3.0/src/main/anyjsonthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-03-14 14:15:09.000000 anyjsonthing-0.3.0/src/main/anyjsonthing/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-03-14 14:15:09.000000 anyjsonthing-0.3.0/src/main/anyjsonthing/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-03-14 14:15:09.000000 anyjsonthing-0.3.0/src/main/anyjsonthing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:16:02.046597 anyjsonthing-0.3.0/src/main/anyjsonthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-14 14:16:02.000000 anyjsonthing-0.3.0/src/main/anyjsonthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-14 14:16:02.000000 anyjsonthing-0.3.0/src/main/anyjsonthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:16:02.000000 anyjsonthing-0.3.0/src/main/anyjsonthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-14 14:16:02.000000 anyjsonthing-0.3.0/src/main/anyjsonthing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-24 09:14:19.013360 anyjsonthing-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.005360 anyjsonthing-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/src/main/anyjsonthing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-24 09:14:18.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 09:14:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:18.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 09:14:18.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/top_level.txt
```

### Comparing `anyjsonthing-0.3.0/LICENSE` & `anyjsonthing-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.0/PKG-INFO` & `anyjsonthing-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjsonthing
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library that implements serialization of simple data objects as JSON data.
 Home-page: https://github.com/phohenecker/anyjsonthing
 Author: Patrick Hohenecker
 Author-email: patrick.hohenecker@gmx.at
 License: Simplified BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anyjsonthing-0.3.0/README.md` & `anyjsonthing-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.0/pyproject.toml` & `anyjsonthing-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.0/setup.cfg` & `anyjsonthing-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.0/src/main/anyjsonthing/__init__.py` & `anyjsonthing-0.3.1/src/main/anyjsonthing/__init__.py`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.0/src/main/anyjsonthing/io.py` & `anyjsonthing-0.3.1/src/main/anyjsonthing/io.py`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.0/src/main/anyjsonthing/serializer.py` & `anyjsonthing-0.3.1/src/main/anyjsonthing/serializer.py`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.0/src/main/anyjsonthing/utils.py` & `anyjsonthing-0.3.1/src/main/anyjsonthing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,18 @@
 
         # Kw-only args are stored (in a full arg-spec) as tuple "kwonlyargs" and the according default values as dict
         # "kwonlydefaults", which maps parameter names to default values.
         for kw_only_arg in arg_spec.kwonlyargs:
 
             # Based on whether the arg has a default value, we decide whether to add it to the required or optional
             # args.
-            if kw_only_arg in arg_spec.kwonlydefaults:  # -> The arg has a default value.
+            if (
+                    arg_spec.kwonlydefaults and  # -> NOTICE: this can be None.
+                    kw_only_arg in arg_spec.kwonlydefaults
+            ):  # -> The arg has a default value.
 
                 optional_args.append(kw_only_arg)
 
             else:  # -> The arg does not have a default value.
 
                 required_args.append(kw_only_arg)
```

### Comparing `anyjsonthing-0.3.0/src/main/anyjsonthing.egg-info/PKG-INFO` & `anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjsonthing
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library that implements serialization of simple data objects as JSON data.
 Home-page: https://github.com/phohenecker/anyjsonthing
 Author: Patrick Hohenecker
 Author-email: patrick.hohenecker@gmx.at
 License: Simplified BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

