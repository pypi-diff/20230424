# Comparing `tmp/shp2metric-1.1.0.tar.gz` & `tmp/shp2metric-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shp2metric-1.1.0.tar", max compression
+gzip compressed data, was "shp2metric-1.2.0.tar", max compression
```

## Comparing `shp2metric-1.1.0.tar` & `shp2metric-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 shp2metric-1.1.0/LICENSE
--rw-r--r--   0        0        0      496 2023-04-24 19:16:32.198127 shp2metric-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-24 15:17:55.079347 shp2metric-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-24 13:37:22.803000 shp2metric-1.1.0/shp2metric/__init__.py
--rw-r--r--   0        0        0     5319 2023-04-24 19:14:22.746170 shp2metric-1.1.0/shp2metric/main.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 shp2metric-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 shp2metric-1.2.0/LICENSE
+-rw-r--r--   0        0        0      496 2023-04-24 20:00:37.316942 shp2metric-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-24 15:17:55.079347 shp2metric-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 13:37:22.803000 shp2metric-1.2.0/shp2metric/__init__.py
+-rw-r--r--   0        0        0     6417 2023-04-24 20:02:03.341542 shp2metric-1.2.0/shp2metric/main.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 shp2metric-1.2.0/PKG-INFO
```

### Comparing `shp2metric-1.1.0/LICENSE` & `shp2metric-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shp2metric-1.1.0/shp2metric/main.py` & `shp2metric-1.2.0/shp2metric/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,73 +33,101 @@
             del chunk, gdf_chunk
 
         # Return a geodataframe from the features
         return gdf, read_task
 
 @app.command()
 def run(
-    input: str = typer.Argument(".", help="The input directory, shapefile or zip file"),
+    input: str = typer.Argument("./", help="The input directory, shapefile or zip file"),
     output: str = typer.Argument("output/", help="The output directory"),
-    zip: bool = typer.Option(True, help="Whether to zip the output files or not"),
-    match: str = typer.Option('*.shp', help="Match string to use if the input is a directory or a zip archive. Any file matching the criteria will be globbed"),
+    zip: bool = typer.Option(True, help="Whether to look for zips in addition to shapefiles (shapefile archives)."),
+    zip_output: bool = typer.Option(True, help="Whether to zip the output files or not"),
 ):
     # Create Path objects for the input and output directories
     input_path = Path(input)
     output_dir = Path(output)
+    tmp_dir = Path(".tmp")
 
     if not output_dir.exists():
         output_dir.mkdir()
     else:
         print(f'[WARNING] output dir "{output_dir}" already exists')
 
+    if not tmp_dir.exists():
+        tmp_dir.mkdir()
+    else:
+        print(f'[WARNING] tmp dir "{tmp_dir}" already exists')
+
     progress = Progress(MofNCompleteColumn(), *Progress.get_default_columns())
 
     # Check if the input is a directory, a shapefile or a zip file
     if input_path.is_dir():
-        # Find all shapefiles in the input directory recursively
-        shapefiles = list(input_path.rglob(match))
-        # TODO search directory for shapefile archived as zip
+        # Find all shapefiles and zip in the input directory recursively
+        if zip:
+            zips = list(input_path.rglob("*.zip"))
+            for z in zips:
+                with zipfile.ZipFile(z, "r") as zf:
+                    zf.extractall(tmp_dir)
+        # Find all shapefiles in the temporary directory recursively
+        shapefiles = list(tmp_dir.rglob("*.shp"))
     elif input_path.suffix == ".shp":
         # Use the input shapefile as a single-item list
         shapefiles = [input_path]
     elif input_path.suffix == ".zip":
-        # Create a temporary directory
-        tmp_dir = Path(".tmp")
         # Extract all the contents of the zip file to the temporary directory
         with zipfile.ZipFile(input_path, "r") as zf:
             zf.extractall(tmp_dir)
         # Find all shapefiles in the temporary directory recursively
-        shapefiles = list(tmp_dir.rglob(match))
+        shapefiles = list(tmp_dir.rglob("*.shp"))
     else:
         # Raise an error if the input is not valid
         raise typer.BadParameter("Input must be a directory, a shapefile or a zip file")
     
     progress.start()
 
     # Add tasks for reading and processing shapefiles
     process_task = progress.add_task("Processing shapefile", total=len(shapefiles))
 
     # Loop through the shapefiles with a progress bar
     for file in shapefiles:
         # Read the input shapefile
         gdf, task = progress_read_shp(file, progress)
 
-        gdf["TargtRxVar"] = ((gdf["AppliedRate"] - gdf["TargetRate"]) / gdf["TargetRate"]) * 100
-        gdf["Speed"] = (gdf["DISTANCE"] * 0.0003048) * 3600
-        gdf["FieldProd"] = (((gdf["DISTANCE"] * 0.3048) * (gdf["SWATHWIDTH"] * 0.3048)) / 10000) * 3600
-        gdf["TargetRate"] = gdf["TargetRate"] * 2.47105381
-        gdf["AppliedRate"] = gdf["AppliedRate"] * 2.47105381
+        try:
+            gdf["TargtRxVar"] = ((gdf["AppliedRate"] - gdf["TargetRate"]) / gdf["TargetRate"]) * 100
+        except KeyError:
+            print(f'[WARNING] key error when attempting to calculate Target Rate Variation')
+        try:
+            gdf["Speed"] = (gdf["DISTANCE"] * 0.0003048) * 3600
+        except KeyError:
+            print(f'[WARNING] key error when attempting to calculate Speed')
+        try:
+            gdf["FieldProd"] = (((gdf["DISTANCE"] * 0.3048) * (gdf["SWATHWIDTH"] * 0.3048)) / 10000) * 3600
+        except KeyError:
+            print(f'[WARNING] key error when attempting to calculate Field Productivity')
+        try:
+            gdf["TargetRate"] = gdf["TargetRate"] * 2.47105381
+        except KeyError:
+            print(f'[WARNING] key error when attempting to convert Target Rate')
+        try:
+            gdf["AppliedRate"] = gdf["AppliedRate"] * 2.47105381
+        except KeyError:
+            print(f'[WARNING] key error when attempting to convert Applied Rate')
+        try:            
+            gdf["Yield"] = gdf["VRYIELDVOL"] * 1.1208
+        except KeyError:
+            print(f'[WARNING] key error when attempting to convert Yield')
 
         # Save the output shapefile with the same name in the output directory
         output_file = output_dir / file.name
         print(f'[INFO] writing output shapefile')
         gdf.to_file(output_file)
 
         # If zip option is True, zip the output file and delete the original one
-        if zip:
+        if zip_output:
             # Create a zip file name with the same stem as the output file
             zip_file = output_dir / (file.stem + ".zip")
             # Create a zip file object in write mode
             with zipfile.ZipFile(zip_file, "w") as zf:
                 print(f'[INFO] zipping shapefile')
                 # Write the output file and its associated files to the zip file
                 for ext in [".shp", ".dbf", ".prj", ".shx", ".cpg"]:
@@ -108,15 +136,14 @@
                 # Delete the original output file and its associated files
                 for ext in [".shp", ".dbf", ".prj", ".shx", ".cpg"]:
                     output_file.with_suffix(ext).unlink()
         progress.remove_task(task)
         progress.update(process_task, advance=1)
         del gdf
 
-    if tmp_dir.exists():
-        shutil.rmtree(tmp_dir, ignore_errors=True)
-
     # Stop displaying progress
     progress.stop()
 
     # Print a success message
     typer.echo(f"Processed {input_path} and saved to {output_dir}")
+    if tmp_dir.exists():
+        shutil.rmtree(tmp_dir, ignore_errors=True)
```

### Comparing `shp2metric-1.1.0/PKG-INFO` & `shp2metric-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shp2metric
-Version: 1.1.0
+Version: 1.2.0
 Summary: Converts Operations Center shapefiles to metric
 License: GPL-3.0-or-later
 Author: João Fauvel
 Author-email: jmmfauvel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

