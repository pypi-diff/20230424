# Comparing `tmp/superpathlib-1.0.0.tar.gz` & `tmp/superpathlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpathlib-1.0.0.tar", last modified: Thu Feb 23 21:46:14 2023, max compression
+gzip compressed data, was "superpathlib-1.0.1.tar", last modified: Mon Apr 24 04:31:06 2023, max compression
```

## Comparing `superpathlib-1.0.0.tar` & `superpathlib-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 21:46:14.117014 superpathlib-1.0.0/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-02-23 21:41:09.000000 superpathlib-1.0.0/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2808 2023-02-23 21:46:14.117014 superpathlib-1.0.0/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2511 2023-02-23 21:41:09.000000 superpathlib-1.0.0/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 21:46:14.113014 superpathlib-1.0.0/plib/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-02-23 21:41:09.000000 superpathlib-1.0.0/plib/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)    15005 2023-02-23 21:41:09.000000 superpathlib-1.0.0/plib/plib.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-02-23 21:41:09.000000 superpathlib-1.0.0/plib/tags.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      808 2023-02-23 21:41:09.000000 superpathlib-1.0.0/plib/utils.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      549 2023-02-23 21:46:14.117014 superpathlib-1.0.0/setup.cfg
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-02-23 21:41:15.000000 superpathlib-1.0.0/setup.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 21:46:14.117014 superpathlib-1.0.0/superpathlib.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2808 2023-02-23 21:46:13.000000 superpathlib-1.0.0/superpathlib.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      280 2023-02-23 21:46:14.000000 superpathlib-1.0.0/superpathlib.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-02-23 21:46:13.000000 superpathlib-1.0.0/superpathlib.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        7 2023-02-23 21:46:13.000000 superpathlib-1.0.0/superpathlib.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-02-23 21:46:13.000000 superpathlib-1.0.0/superpathlib.egg-info/top_level.txt
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-04-24 04:20:41.000000 superpathlib-1.0.1/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2808 2023-04-24 04:31:06.834797 superpathlib-1.0.1/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2511 2023-04-24 04:20:41.000000 superpathlib-1.0.1/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/plib/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-04-24 04:20:41.000000 superpathlib-1.0.1/plib/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)    15026 2023-04-24 04:25:02.000000 superpathlib-1.0.1/plib/plib.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-04-24 04:20:41.000000 superpathlib-1.0.1/plib/tags.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      808 2023-04-24 04:20:41.000000 superpathlib-1.0.1/plib/utils.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      549 2023-04-24 04:31:06.834797 superpathlib-1.0.1/setup.cfg
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-04-24 04:20:41.000000 superpathlib-1.0.1/setup.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/superpathlib.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2808 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      353 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        7 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-04-24 04:31:06.000000 superpathlib-1.0.1/superpathlib.egg-info/top_level.txt
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 04:31:06.834797 superpathlib-1.0.1/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     4150 2023-04-24 04:20:41.000000 superpathlib-1.0.1/tests/test_content.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1532 2023-04-24 04:20:41.000000 superpathlib-1.0.1/tests/test_functionality.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1271 2023-04-24 04:20:41.000000 superpathlib-1.0.1/tests/test_metadata.py
```

### Comparing `superpathlib-1.0.0/LICENSE` & `superpathlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.0/PKG-INFO` & `superpathlib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: extended pathlib
 Home-page: https://github.com/quintenroets/superpathlib
 Author: Quinten Roets
 Author-email: quinten.roets@gmail.com
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `superpathlib-1.0.0/README.md` & `superpathlib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.0/plib/plib.py` & `superpathlib-1.0.1/plib/plib.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
             shutil.copytree(temp_dest, dest, dirs_exist_ok=True)
             temp_dest.rmtree()
 
     def is_empty(self):
         return (
             not self.exists()
             or (self.is_dir() and next(self.iterdir(), None) is None)
-            or self.size == 0
+            or (self.is_file() and self.size == 0)
         )
 
     def load_yaml(self, trusted=False):
         """
         :param trusted: if the path is trusted, an unsafe loader
                         can be used to instantiate any object
         :return: Content in path that contains yaml format
```

### Comparing `superpathlib-1.0.0/plib/tags.py` & `superpathlib-1.0.1/plib/tags.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.0/plib/utils.py` & `superpathlib-1.0.1/plib/utils.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.0/setup.cfg` & `superpathlib-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = superpathlib
-version = 1.0.0
+version = 1.0.1
 author = Quinten Roets
 author_email = quinten.roets@gmail.com
 description = extended pathlib
 description-file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/quintenroets/superpathlib
```

### Comparing `superpathlib-1.0.0/superpathlib.egg-info/PKG-INFO` & `superpathlib-1.0.1/superpathlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: extended pathlib
 Home-page: https://github.com/quintenroets/superpathlib
 Author: Quinten Roets
 Author-email: quinten.roets@gmail.com
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

