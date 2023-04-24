# Comparing `tmp/pystorz-0.0.4.tar.gz` & `tmp/pystorz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.0.4.tar", last modified: Mon Apr 24 16:20:28 2023, max compression
+gzip compressed data, was "dist/pystorz-0.0.5.tar", last modified: Mon Apr 24 17:23:27 2023, max compression
```

## Comparing `pystorz-0.0.4.tar` & `pystorz-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.179039 pystorz-0.0.4/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.0.4/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     1471 2023-04-24 16:20:28.178848 pystorz-0.0.4/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1113 2023-04-24 05:33:45.000000 pystorz-0.0.4/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.173241 pystorz-0.0.4/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.0.4/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.174317 pystorz-0.0.4/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.0.4/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.0.4/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.175558 pystorz-0.0.4/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.0.4/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 14:38:47.000000 pystorz-0.0.4/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4159 2023-04-24 14:46:41.000000 pystorz-0.0.4/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.177253 pystorz-0.0.4/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.0.4/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.0.4/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)      616 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.0.4/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.177546 pystorz-0.0.4/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.0.4/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9384 2023-04-24 16:11:55.000000 pystorz-0.0.4/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.178545 pystorz-0.0.4/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.0.4/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2270 2023-04-24 16:09:40.000000 pystorz-0.0.4/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.0.4/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.0.4/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2073 2023-04-24 15:41:15.000000 pystorz-0.0.4/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 16:20:28.174054 pystorz-0.0.4/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     1471 2023-04-24 16:20:28.000000 pystorz-0.0.4/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-24 16:20:28.000000 pystorz-0.0.4/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-24 16:20:28.000000 pystorz-0.0.4/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-24 16:20:28.000000 pystorz-0.0.4/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-24 16:20:28.000000 pystorz-0.0.4/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-24 16:20:28.179089 pystorz-0.0.4/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-24 14:37:45.000000 pystorz-0.0.4/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.185231 pystorz-0.0.5/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.0.5/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 17:23:27.185050 pystorz-0.0.5/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.0.5/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.179028 pystorz-0.0.5/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.0.5/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.180277 pystorz-0.0.5/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.0.5/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.0.5/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.181551 pystorz-0.0.5/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.0.5/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.0.5/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4159 2023-04-24 14:46:41.000000 pystorz-0.0.5/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.183219 pystorz-0.0.5/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.0.5/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.0.5/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      616 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.0.5/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.183505 pystorz-0.0.5/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.0.5/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9384 2023-04-24 16:11:55.000000 pystorz-0.0.5/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.184540 pystorz-0.0.5/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.0.5/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2270 2023-04-24 16:09:40.000000 pystorz-0.0.5/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.0.5/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.0.5/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2073 2023-04-24 15:41:15.000000 pystorz-0.0.5/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 17:23:27.179859 pystorz-0.0.5/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-24 17:23:27.000000 pystorz-0.0.5/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-24 17:23:27.185280 pystorz-0.0.5/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-24 17:23:01.000000 pystorz-0.0.5/setup.py
```

### Comparing `pystorz-0.0.4/LICENSE` & `pystorz-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/PKG-INFO` & `pystorz-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <img src="logo.png" width="300" alt="storz" />
 </p>
 
-**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/main/src/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/main/src/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
 
-**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/storz/tree/main/src/store) interface.
+**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
 
 ## Quick Start Guide
 
 ### Installation
 ```
 pip install pystorz
 ```
```

### Comparing `pystorz-0.0.4/pystorz/mgen/builder.py` & `pystorz-0.0.5/pystorz/mgen/builder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         "from pystorz.store import store",
         "from pystorz.store import meta",
     ]
 
     b = StringIO()
 
     b.write(render("mgen/templates/imports.py", {"imports": imports}))
-    b.write(compileResources(resources))
     b.write(compileStructs(structs))
+    b.write(compileResources(resources))
 
     res = b.getvalue().replace("&#34;", "\"")
 
     # refactor and format python code
     res = reformat_python_code(res)
 
     targetDir = "generated"
```

### Comparing `pystorz-0.0.4/pystorz/mgen/loader.py` & `pystorz-0.0.5/pystorz/mgen/loader.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/mgen/templates/structure.py` & `pystorz-0.0.5/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.0.5/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/mgen/test.py` & `pystorz-0.0.5/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/mgen/utils.py` & `pystorz-0.0.5/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/sql/store.py` & `pystorz-0.0.5/pystorz/sql/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/store/meta.py` & `pystorz-0.0.5/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/store/options.py` & `pystorz-0.0.5/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/store/store.py` & `pystorz-0.0.5/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz/store/utils.py` & `pystorz-0.0.5/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/pystorz.egg-info/PKG-INFO` & `pystorz-0.0.5/pystorz.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <img src="logo.png" width="300" alt="storz" />
 </p>
 
-**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/main/src/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/main/src/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
 
-**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/storz/tree/main/src/store) interface.
+**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
 
 ## Quick Start Guide
 
 ### Installation
 ```
 pip install pystorz
 ```
```

### Comparing `pystorz-0.0.4/pystorz.egg-info/SOURCES.txt` & `pystorz-0.0.5/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.4/setup.py` & `pystorz-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.0.4',
+    version='0.0.5',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

