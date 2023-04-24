# Comparing `tmp/shp2metric-1.2.1.tar.gz` & `tmp/shp2metric-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shp2metric-1.2.1.tar", max compression
+gzip compressed data, was "shp2metric-1.3.2.tar", max compression
```

## Comparing `shp2metric-1.2.1.tar` & `shp2metric-1.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 shp2metric-1.2.1/LICENSE
--rw-r--r--   0        0        0      496 2023-04-24 20:09:28.831668 shp2metric-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-24 15:17:55.079347 shp2metric-1.2.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 13:37:22.803000 shp2metric-1.2.1/shp2metric/__init__.py
--rw-r--r--   0        0        0     6559 2023-04-24 20:09:54.904332 shp2metric-1.2.1/shp2metric/main.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 shp2metric-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 shp2metric-1.3.2/LICENSE
+-rw-r--r--   0        0        0      496 2023-04-24 20:45:49.815812 shp2metric-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-24 15:17:55.079347 shp2metric-1.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 13:37:22.803000 shp2metric-1.3.2/shp2metric/__init__.py
+-rw-r--r--   0        0        0     6820 2023-04-24 20:54:10.113345 shp2metric-1.3.2/shp2metric/main.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 shp2metric-1.3.2/PKG-INFO
```

### Comparing `shp2metric-1.2.1/LICENSE` & `shp2metric-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shp2metric-1.2.1/shp2metric/main.py` & `shp2metric-1.3.2/shp2metric/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,26 +53,26 @@
         print(f'[WARNING] output dir "{output_dir}" already exists')
 
     if not tmp_dir.exists():
         tmp_dir.mkdir()
     else:
         print(f'[WARNING] tmp dir "{tmp_dir}" already exists')
 
-    progress = Progress(MofNCompleteColumn(), *Progress.get_default_columns())
+    progress = Progress()
 
     # Check if the input is a directory, a shapefile or a zip file
     if input_path.is_dir():
         # Find all shapefiles and zip in the input directory recursively
         if zip:
             zips = list(input_path.rglob("*.zip"))
             for z in zips:
                 with zipfile.ZipFile(z, "r") as zf:
                     zf.extractall(tmp_dir)
         # Find all shapefiles in the temporary directory recursively
-        shapefiles = list(tmp_dir.rglob("*.shp"))
+        shapefiles = list(input_path.rglob("*.shp"))
     elif input_path.suffix == ".shp":
         # Use the input shapefile as a single-item list
         shapefiles = [input_path]
     elif input_path.suffix == ".zip":
         # Extract all the contents of the zip file to the temporary directory
         with zipfile.ZipFile(input_path, "r") as zf:
             zf.extractall(tmp_dir)
@@ -85,20 +85,22 @@
     if not shapefiles:
         print(f'[WARNING] directory "{input_path}" does not contain file that match the criteria')
         exit()
 
     progress.start()
 
     # Add tasks for reading and processing shapefiles
-    process_task = progress.add_task("Processing shapefile", total=len(shapefiles))
+    process_task = progress.add_task("Processing shapefiles", total=len(shapefiles)*3)
 
     # Loop through the shapefiles with a progress bar
     for file in shapefiles:
+        print(f'[INFO] processing "{file}"')
         # Read the input shapefile
         gdf, task = progress_read_shp(file, progress)
+        progress.update(process_task, advance=1)
 
         try:
             gdf["TargtRxVar"] = ((gdf["AppliedRate"] - gdf["TargetRate"]) / gdf["TargetRate"]) * 100
         except KeyError:
             print(f'[WARNING] key error when attempting to calculate Target Rate Variation')
         try:
             gdf["Speed"] = (gdf["DISTANCE"] * 0.0003048) * 3600
@@ -117,17 +119,20 @@
         except KeyError:
             print(f'[WARNING] key error when attempting to convert Applied Rate')
         try:            
             gdf["Yield"] = gdf["VRYIELDVOL"] * 1.1208
         except KeyError:
             print(f'[WARNING] key error when attempting to convert Yield')
 
+        progress.update(process_task, advance=1)
+
         # Save the output shapefile with the same name in the output directory
         output_file = output_dir / file.name
         print(f'[INFO] writing output shapefile')
+        write_task = progress.add_task("Writing shapefile", total=1)
         gdf.to_file(output_file)
 
         # If zip option is True, zip the output file and delete the original one
         if zip_output:
             # Create a zip file name with the same stem as the output file
             zip_file = output_dir / (file.stem + ".zip")
             # Create a zip file object in write mode
@@ -136,16 +141,18 @@
                 # Write the output file and its associated files to the zip file
                 for ext in [".shp", ".dbf", ".prj", ".shx", ".cpg"]:
                     zf.write(output_file.with_suffix(ext), arcname=output_file.with_suffix(ext).name)
                 print(f'[INFO] removing temporary files')
                 # Delete the original output file and its associated files
                 for ext in [".shp", ".dbf", ".prj", ".shx", ".cpg"]:
                     output_file.with_suffix(ext).unlink()
-        progress.remove_task(task)
+        progress.update(write_task, advance=1)
         progress.update(process_task, advance=1)
+        progress.remove_task(task)
+        progress.remove_task(write_task)
         del gdf
 
     # Stop displaying progress
     progress.stop()
 
     # Print a success message
     typer.echo(f"Processed {input_path} and saved to {output_dir}")
```

### Comparing `shp2metric-1.2.1/PKG-INFO` & `shp2metric-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shp2metric
-Version: 1.2.1
+Version: 1.3.2
 Summary: Converts Operations Center shapefiles to metric
 License: GPL-3.0-or-later
 Author: João Fauvel
 Author-email: jmmfauvel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

