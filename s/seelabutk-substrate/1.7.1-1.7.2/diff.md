# Comparing `tmp/seelabutk-substrate-1.7.1.tar.gz` & `tmp/seelabutk-substrate-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seelabutk-substrate-1.7.1.tar", last modified: Wed Mar 29 17:37:09 2023, max compression
+gzip compressed data, was "seelabutk-substrate-1.7.2.tar", last modified: Mon Apr 24 15:27:00 2023, max compression
```

## Comparing `seelabutk-substrate-1.7.1.tar` & `seelabutk-substrate-1.7.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.038020 seelabutk-substrate-1.7.1/
--rw-r--r--   0 john      (1000) john      (1000)    16674 2022-03-29 18:24:57.000000 seelabutk-substrate-1.7.1/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     3444 2023-03-29 17:37:09.038020 seelabutk-substrate-1.7.1/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     2997 2022-07-27 03:11:50.000000 seelabutk-substrate-1.7.1/README.md
--rw-r--r--   0 john      (1000) john      (1000)      762 2023-03-29 17:36:53.000000 seelabutk-substrate-1.7.1/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)      444 2023-03-29 17:37:09.038020 seelabutk-substrate-1.7.1/setup.cfg
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3444 2023-03-29 17:37:09.000000 seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1422 2023-03-29 17:37:09.000000 seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-03-29 17:37:09.000000 seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       55 2023-03-29 17:37:09.000000 seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) john      (1000)      100 2023-03-29 17:37:09.000000 seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       10 2023-03-29 17:37:09.000000 seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/top_level.txt
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/substrate/
--rw-r--r--   0 john      (1000) john      (1000)       33 2022-03-15 19:56:07.000000 seelabutk-substrate-1.7.1/src/substrate/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)       37 2022-03-15 20:01:04.000000 seelabutk-substrate-1.7.1/src/substrate/__main__.py
--rwxr-xr-x   0 john      (1000) john      (1000)     4260 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.1/src/substrate/substrate.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/substrate/targets/
--rw-r--r--   0 john      (1000) john      (1000)       70 2022-04-26 20:17:06.000000 seelabutk-substrate-1.7.1/src/substrate/targets/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     8833 2022-10-27 18:11:48.000000 seelabutk-substrate-1.7.1/src/substrate/targets/aws_stack.py
--rw-r--r--   0 john      (1000) john      (1000)     4013 2022-10-06 16:06:33.000000 seelabutk-substrate-1.7.1/src/substrate/targets/docker_swarm.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/substrate/tools/
--rw-r--r--   0 john      (1000) john      (1000)      230 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.1/src/substrate/tools/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     1861 2022-10-26 12:39:49.000000 seelabutk-substrate-1.7.1/src/substrate/tools/braid.py
--rw-r--r--   0 john      (1000) john      (1000)     1375 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.1/src/substrate/tools/generic_tool.py
--rw-r--r--   0 john      (1000) john      (1000)     1138 2022-10-03 16:39:17.000000 seelabutk-substrate-1.7.1/src/substrate/tools/hello_world.py
--rw-r--r--   0 john      (1000) john      (1000)     1236 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.1/src/substrate/tools/nc_slicer.py
--rw-r--r--   0 john      (1000) john      (1000)     1141 2022-10-03 16:41:49.000000 seelabutk-substrate-1.7.1/src/substrate/tools/ospray_studio.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/
--rw-r--r--   0 john      (1000) john      (1000)       84 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/constants.js
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.028020 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/css/
--rw-r--r--   0 john      (1000) john      (1000)     3636 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/css/style.css
--rw-r--r--   0 john      (1000) john      (1000)     2604 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/index.html
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.038020 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/
--rw-r--r--   0 john      (1000) john      (1000)    11262 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/arcball.js
--rw-r--r--   0 john      (1000) john      (1000)    48508 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/gremlins.min.js
--rw-r--r--   0 john      (1000) john      (1000)    22951 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/gui.js
--rw-r--r--   0 john      (1000) john      (1000)      447 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/main.js
--rw-r--r--   0 john      (1000) john      (1000)     5837 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/math.js
--rw-r--r--   0 john      (1000) john      (1000)    11962 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/smooth.js
--rw-r--r--   0 john      (1000) john      (1000)    13584 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/sylvester.js
--rw-r--r--   0 john      (1000) john      (1000)    27906 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/tapestry.js
--rw-r--r--   0 john      (1000) john      (1000)     5322 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/testing.js
--rw-r--r--   0 john      (1000) john      (1000)     4682 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/tools.js
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-03-29 17:37:09.038020 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/config/
--rw-r--r--   0 john      (1000) john      (1000)      244 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/config/data.json
--rw-r--r--   0 john      (1000) john      (1000)     2160 2022-10-04 13:27:23.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tapestry.py
--rw-r--r--   0 john      (1000) john      (1000)     1380 2022-10-04 13:28:08.000000 seelabutk-substrate-1.7.1/src/substrate/tools/tool.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/
+-rw-r--r--   0 john      (1000) john      (1000)    16674 2022-03-29 18:24:57.000000 seelabutk-substrate-1.7.2/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     3439 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     2997 2022-07-27 03:11:50.000000 seelabutk-substrate-1.7.2/README.md
+-rw-r--r--   0 john      (1000) john      (1000)      757 2023-04-24 15:26:50.000000 seelabutk-substrate-1.7.2/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)      444 2023-04-24 15:27:00.682733 seelabutk-substrate-1.7.2/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.652733 seelabutk-substrate-1.7.2/src/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3439 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1422 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       55 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) john      (1000)      100 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       10 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/substrate/
+-rw-r--r--   0 john      (1000) john      (1000)       33 2022-03-15 19:56:07.000000 seelabutk-substrate-1.7.2/src/substrate/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)       37 2022-03-15 20:01:04.000000 seelabutk-substrate-1.7.2/src/substrate/__main__.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     4949 2023-04-24 15:23:57.000000 seelabutk-substrate-1.7.2/src/substrate/substrate.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/substrate/targets/
+-rw-r--r--   0 john      (1000) john      (1000)       70 2022-04-26 20:17:06.000000 seelabutk-substrate-1.7.2/src/substrate/targets/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     8833 2022-10-27 18:11:48.000000 seelabutk-substrate-1.7.2/src/substrate/targets/aws_stack.py
+-rw-r--r--   0 john      (1000) john      (1000)     4013 2022-10-06 16:06:33.000000 seelabutk-substrate-1.7.2/src/substrate/targets/docker_swarm.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/
+-rw-r--r--   0 john      (1000) john      (1000)      230 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.2/src/substrate/tools/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     1861 2022-10-26 12:39:49.000000 seelabutk-substrate-1.7.2/src/substrate/tools/braid.py
+-rw-r--r--   0 john      (1000) john      (1000)     1610 2023-04-24 15:25:26.000000 seelabutk-substrate-1.7.2/src/substrate/tools/generic_tool.py
+-rw-r--r--   0 john      (1000) john      (1000)     1138 2022-10-03 16:39:17.000000 seelabutk-substrate-1.7.2/src/substrate/tools/hello_world.py
+-rw-r--r--   0 john      (1000) john      (1000)     1236 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.2/src/substrate/tools/nc_slicer.py
+-rw-r--r--   0 john      (1000) john      (1000)     1141 2022-10-03 16:41:49.000000 seelabutk-substrate-1.7.2/src/substrate/tools/ospray_studio.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/
+-rw-r--r--   0 john      (1000) john      (1000)       84 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/constants.js
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/css/
+-rw-r--r--   0 john      (1000) john      (1000)     3636 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/css/style.css
+-rw-r--r--   0 john      (1000) john      (1000)     2604 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/index.html
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/
+-rw-r--r--   0 john      (1000) john      (1000)    11262 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/arcball.js
+-rw-r--r--   0 john      (1000) john      (1000)    48508 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gremlins.min.js
+-rw-r--r--   0 john      (1000) john      (1000)    22951 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gui.js
+-rw-r--r--   0 john      (1000) john      (1000)      447 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/main.js
+-rw-r--r--   0 john      (1000) john      (1000)     5837 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/math.js
+-rw-r--r--   0 john      (1000) john      (1000)    11962 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/smooth.js
+-rw-r--r--   0 john      (1000) john      (1000)    13584 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/sylvester.js
+-rw-r--r--   0 john      (1000) john      (1000)    27906 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tapestry.js
+-rw-r--r--   0 john      (1000) john      (1000)     5322 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/testing.js
+-rw-r--r--   0 john      (1000) john      (1000)     4682 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tools.js
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/config/
+-rw-r--r--   0 john      (1000) john      (1000)      244 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/config/data.json
+-rw-r--r--   0 john      (1000) john      (1000)     2160 2022-10-04 13:27:23.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry.py
+-rw-r--r--   0 john      (1000) john      (1000)     1401 2023-04-24 15:16:24.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tool.py
```

### Comparing `seelabutk-substrate-1.7.1/LICENSE` & `seelabutk-substrate-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/PKG-INFO` & `seelabutk-substrate-1.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seelabutk-substrate
-Version: 1.7.1
+Version: 1.7.2
 Summary: Automatically deploys visualization services via Docker Swarm
-Author-email: John Duggan <jduggan1@vols.utk.edu>
+Author-email: John Duggan <jduggan1@utk.edu>
 License: CC-BY-4.0
 Project-URL: Homepage, https://github.com/seelabutk/substrate/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `seelabutk-substrate-1.7.1/README.md` & `seelabutk-substrate-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/pyproject.toml` & `seelabutk-substrate-1.7.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "seelabutk-substrate"
-authors = [{name = "John Duggan", email = "jduggan1@vols.utk.edu"}]
+authors = [{name = "John Duggan", email = "jduggan1@utk.edu"}]
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"Operating System :: OS Independent"
 ]
 dependencies = [
 	'aws-cdk-lib ~= 2.24.1',
 	'constructs ~= 10.1.11',
@@ -14,15 +14,15 @@
 	'requests ~= 2.27.1'
 ]
 description = "Automatically deploys visualization services via Docker Swarm"
 entry-points = {console_scripts = {substrate = "substrate.substrate:main"}}
 license = {text = "CC-BY-4.0"}
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.7.1"
+version = "1.7.2"
 
 [project.urls]
 Homepage = "https://github.com/seelabutk/substrate/"
 
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
```

### Comparing `seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/PKG-INFO` & `seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seelabutk-substrate
-Version: 1.7.1
+Version: 1.7.2
 Summary: Automatically deploys visualization services via Docker Swarm
-Author-email: John Duggan <jduggan1@vols.utk.edu>
+Author-email: John Duggan <jduggan1@utk.edu>
 License: CC-BY-4.0
 Project-URL: Homepage, https://github.com/seelabutk/substrate/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `seelabutk-substrate-1.7.1/src/seelabutk_substrate.egg-info/SOURCES.txt` & `seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/substrate.py` & `seelabutk-substrate-1.7.2/src/substrate/substrate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,93 @@
 #!/usr/bin/env python3
 from argparse import ArgumentParser
 import os
 import subprocess
 import sys
 from urllib.parse import urlparse
+import json
+import copy
 
 import yaml
 
 from .targets import AWSStack, DockerSwarm
-from .tools import HelloWorld, NetCDFSlicer, OSPRayStudio, Tapestry, Braid, GenericTool
+from .tools import (
+	HelloWorld,
+	NetCDFSlicer,
+	OSPRayStudio,
+	Tapestry,
+	Braid,
+	GenericTool
+)
 
 TOOLS = {
 	'hello-world': HelloWorld,
 	'nc_slicer': NetCDFSlicer,
 	'ospray-studio': OSPRayStudio,
 	'tapestry': Tapestry,
 	'braid': Braid
 }
 
 
+def deep_merge(obj_a, obj_b):
+	new_obj = copy.deepcopy(obj_a)
+	for key, val in obj_b.items():
+		if (
+			key in new_obj and isinstance(new_obj[key], dict) and isinstance(val, dict)
+		):
+			new_obj[key] = deep_merge(new_obj[key], val)
+		else:
+			new_obj[key] = val
+	return new_obj
+
+
+def parse_yaml(path):
+	config_name = 'substrate.config.yaml'
+
+	if path is None:
+		path = os.getcwd()
+
+		files = os.listdir(path)
+		if config_name not in files:
+			raise FileNotFoundError(config_name)
+
+		path = os.path.join(path, config_name)
+
+	with open(path, 'r', encoding='utf8') as stream:
+		_config = yaml.load(stream, Loader=yaml.Loader)
+
+	return (path, _config)
+
+
 class Substrate():
-	def __init__(self, tool_name, path=None):
+	def __init__(self, tool_name, config, path=None):
+		pathconfig = {}
+		if path:
+			path, pathconfig = parse_yaml(path)
+
 		self.tool_name = tool_name
-		self.path, self.config = self._parse_yaml(path)
+		self.config = deep_merge(pathconfig, config)
+		self.path = path
 		self._check_config()
 
 		self.target = None
 		if self.config.get('aws', None) is not None:
 			self.target = AWSStack
 		elif self.config.get('docker', None) is not None:
 			self.target = DockerSwarm
 
 		self.data_sources = self._get_data(self.config)
 		if tool_name not in TOOLS:
 			# look in config for tool
 			if tool_name not in self.config:
 				raise Exception(f'No tool named {tool_name}')
-			else:
-				self.tool = GenericTool(tool_name, self.config, self.data_sources)
+
+			self.tool = GenericTool(tool_name, self.config, self.data_sources)
 		else:
-				self.tool = TOOLS[tool_name](self.config, self.data_sources)
+			self.tool = TOOLS[tool_name](self.config, self.data_sources)
 
 		self.target_obj = self.target(self.path, self.config, self.tool)
 
 	def _check_config(self):
 		config = self.config
 
 		if 'aws' not in config and 'docker' not in config:
@@ -62,17 +106,19 @@
 					'AWS_ACCESS_KEY_ID environment variable must be set to deploy to AWS.'
 				)
 
 			if not os.environ.get('AWS_SECRET_ACCESS_KEY', False):
 				raise Exception(
 					'AWS_SECRET_ACCESS_KEY environment variable must be set to deploy to AWS.'
 				)
-			
-			if not 'service_command' in config['aws']:
-				raise Exception('Option "aws.service_command" must be set to deploy to AWS.')
+
+			if 'service_command' not in config['aws']:
+				raise Exception(
+					'Option "aws.service_command" must be set to deploy to AWS.'
+				)
 
 		if 'docker' in config:
 			try:
 				subprocess.check_call(
 					'docker info',
 					shell=True,
 					stdout=subprocess.DEVNULL,
@@ -81,15 +127,15 @@
 			except subprocess.CalledProcessError as exc:
 				raise Exception(
 					"Docker doesn't appear to be running. Please check that it's installed "
 					"and the daemon is running."
 				) from exc
 
 	def _get_data(self, config):
-		source_paths = config['data']['source']
+		source_paths = config.get('data', {}).get('source', [])
 		data_paths = []
 		data_urls = []
 
 		for source_path in source_paths:
 			is_url = urlparse(source_path).scheme.startswith(('ftp', 'http', 's3'))
 
 			if is_url and self.target == DockerSwarm:
@@ -104,31 +150,14 @@
 				data_paths.append(os.path.abspath(source_path))
 
 			if data_paths and os.path.isfile(data_paths[-1]):
 				data_paths[-1] = os.path.dirname(data_paths[-1])
 
 		return (data_paths, data_urls)
 
-	def _parse_yaml(self, path):
-		config_name = 'substrate.config.yaml'
-
-		if path is None:
-			path = os.getcwd()
-
-			files = os.listdir(path)
-			if config_name not in files:
-				raise FileNotFoundError(config_name)
-
-			path = os.path.join(path, config_name)
-
-		with open(path, 'r', encoding='utf8') as stream:
-			_config = yaml.load(stream, Loader=yaml.Loader)
-
-		return (path, _config)
-
 	def start(self):
 		return f'http://{self.target_obj.start()}'
 
 	def stop(self):
 		self.target_obj.stop()
 
 
@@ -141,19 +170,35 @@
 		metavar='TOOL'
 	)
 	parser.add_argument(
 		'action',
 		help='[start, stop]',
 		metavar='ACTION'
 	)
-	parser.add_argument('-c', '--config', dest='path')
+	parser.add_argument(
+		'-c',
+		'--config',
+		dest='input_config',
+		default='{}',
+		type=str,
+		nargs='?',
+		const=1
+	)
+	parser.add_argument('-f', '--config-file', dest='path')
 	args = parser.parse_args()
 
 	if args.action not in ['start', 'stop', 'synth']:
 		sys.exit('Invalid action specified.')
 
-	substrate = Substrate(args.tool, args.path)
+	tool = args.tool
+	path = args.path
+	config = json.loads(args.input_config)
+
+	if (not bool(config)) and (path is None):
+		sys.exit('no config file specified')
+
+	substrate = Substrate(tool, config, path)
 	if args.action == 'start':
 		print(f'You may view your new visualization stack here: {substrate.start()}.')  # noqa: E501
 
 	if args.action == 'stop':
 		substrate.stop()
```

### Comparing `seelabutk-substrate-1.7.1/src/substrate/targets/aws_stack.py` & `seelabutk-substrate-1.7.2/src/substrate/targets/aws_stack.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/targets/docker_swarm.py` & `seelabutk-substrate-1.7.2/src/substrate/targets/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/braid.py` & `seelabutk-substrate-1.7.2/src/substrate/tools/braid.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/generic_tool.py` & `seelabutk-substrate-1.7.2/src/substrate/tools/generic_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from docker import from_env
 from docker.types.services import EndpointSpec, ServiceMode
 
 from . import Tool
 
 
-class GenericTool(Tool):
+class GenericTool(Tool):  # pylint: disable=too-many-instance-attributes
 	def __init__(self, name, config, data_sources):
 		super().__init__(config, data_sources)
 		# Provide a name for this tool
 		self.name = name
 
 		self.config = config
 		self.tool_config = config[name]
@@ -22,24 +22,33 @@
 		if self.internal_port is None:
 			raise Exception('Option "internal_port" must be defined.')
 
 	# Start a local Docker swarm service
 	def start(self):
 		# ensure image is defined
 		if self.image is None:
-			raise Exception('Option "docker.image" must be defined when running substrate generic tool locally.')
+			raise Exception(
+				'Option "docker.image" must be defined when running substrate generic '
+				'tool locally.'
+			)
 
 		mounts = super().start()
 		docker = from_env()
 		self.port = self.config['docker'].get('port', self.port)
+		environment_variables = self.config['docker'].get('env', [])
+		arguments = self.config.get('args', [])
 		docker.services.create(
 			self.image,
-			endpoint_spec=EndpointSpec(ports={self.port: (self.internal_port, 'tcp')}),
+			endpoint_spec=EndpointSpec(
+				ports={self.port: (self.internal_port, 'tcp', 'host')}
+			),
 			mode=ServiceMode(
 				mode='replicated',
 				replicas=self.config['docker'].get('replicas', 1)
 			),
+			args=arguments,
+			env=environment_variables,
 			mounts=mounts,
 			name=self.name,
 			networks=[f'substrate-{self.name}-net'],
 			init=True
 		)
```

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/hello_world.py` & `seelabutk-substrate-1.7.2/src/substrate/tools/hello_world.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/nc_slicer.py` & `seelabutk-substrate-1.7.2/src/substrate/tools/nc_slicer.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/ospray_studio.py` & `seelabutk-substrate-1.7.2/src/substrate/tools/ospray_studio.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/css/style.css` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/css/style.css`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/index.html` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/index.html`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/arcball.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/arcball.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/gremlins.min.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gremlins.min.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/gui.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gui.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/math.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/math.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/smooth.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/smooth.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/sylvester.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/sylvester.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/tapestry.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tapestry.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/testing.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/testing.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry/app/js/tools.js` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tools.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tapestry.py` & `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.1/src/substrate/tools/tool.py` & `seelabutk-substrate-1.7.2/src/substrate/tools/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 		mounts = []
 		data_paths = self.data_sources[0]
 		if len(data_paths) > 1:
 			for index, data_path in enumerate(data_paths):
 				mounts.append(
 					Mount(f'/data/{index}', data_path, type='bind', read_only=True)
 				)
-		else:
+		elif len(data_paths) == 1:
 			mounts.append(Mount('/data', data_paths[0], type='bind', read_only=True))
 
 		return mounts
 
 	# Upload files needed to run your service to S3.
 	# Upload them to mirror the directory structure you want on EFS.
 	def upload_to_s3(self):
```

