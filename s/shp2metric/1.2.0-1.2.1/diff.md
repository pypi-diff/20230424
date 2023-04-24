# Comparing `tmp/shp2metric-1.2.0.tar.gz` & `tmp/shp2metric-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shp2metric-1.2.0.tar", max compression
+gzip compressed data, was "shp2metric-1.2.1.tar", max compression
```

## Comparing `shp2metric-1.2.0.tar` & `shp2metric-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 shp2metric-1.2.0/LICENSE
--rw-r--r--   0        0        0      496 2023-04-24 20:00:37.316942 shp2metric-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-24 15:17:55.079347 shp2metric-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-24 13:37:22.803000 shp2metric-1.2.0/shp2metric/__init__.py
--rw-r--r--   0        0        0     6417 2023-04-24 20:02:03.341542 shp2metric-1.2.0/shp2metric/main.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 shp2metric-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 shp2metric-1.2.1/LICENSE
+-rw-r--r--   0        0        0      496 2023-04-24 20:09:28.831668 shp2metric-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-24 15:17:55.079347 shp2metric-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 13:37:22.803000 shp2metric-1.2.1/shp2metric/__init__.py
+-rw-r--r--   0        0        0     6559 2023-04-24 20:09:54.904332 shp2metric-1.2.1/shp2metric/main.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 shp2metric-1.2.1/PKG-INFO
```

### Comparing `shp2metric-1.2.0/LICENSE` & `shp2metric-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shp2metric-1.2.0/shp2metric/main.py` & `shp2metric-1.2.1/shp2metric/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,18 @@
             zf.extractall(tmp_dir)
         # Find all shapefiles in the temporary directory recursively
         shapefiles = list(tmp_dir.rglob("*.shp"))
     else:
         # Raise an error if the input is not valid
         raise typer.BadParameter("Input must be a directory, a shapefile or a zip file")
     
+    if not shapefiles:
+        print(f'[WARNING] directory "{input_path}" does not contain file that match the criteria')
+        exit()
+
     progress.start()
 
     # Add tasks for reading and processing shapefiles
     process_task = progress.add_task("Processing shapefile", total=len(shapefiles))
 
     # Loop through the shapefiles with a progress bar
     for file in shapefiles:
```

### Comparing `shp2metric-1.2.0/PKG-INFO` & `shp2metric-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shp2metric
-Version: 1.2.0
+Version: 1.2.1
 Summary: Converts Operations Center shapefiles to metric
 License: GPL-3.0-or-later
 Author: João Fauvel
 Author-email: jmmfauvel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

