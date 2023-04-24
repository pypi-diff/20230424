# Comparing `tmp/caf.space-1.2.1.tar.gz` & `tmp/caf.space-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caf.space-1.2.1.tar", last modified: Mon Apr  3 13:17:57 2023, max compression
+gzip compressed data, was "caf.space-1.2.2.tar", last modified: Mon Apr 24 12:13:05 2023, max compression
```

## Comparing `caf.space-1.2.1.tar` & `caf.space-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:17:57.777060 caf.space-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 13:17:41.000000 caf.space-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-03 13:17:57.777060 caf.space-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-03 13:17:41.000000 caf.space-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-03 13:17:41.000000 caf.space-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-03 13:17:57.777060 caf.space-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-03 13:17:41.000000 caf.space-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:17:57.773060 caf.space-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:17:57.773060 caf.space-1.2.1/src/caf/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:17:57.777060 caf.space-1.2.1/src/caf/space/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-03 13:17:57.777060 caf.space-1.2.1/src/caf/space/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/space/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/space/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    24599 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/space/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/space/weighted_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/space/zone_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-03 13:17:41.000000 caf.space-1.2.1/src/caf/space/zone_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:17:57.777060 caf.space-1.2.1/src/caf.space.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-03 13:17:57.000000 caf.space-1.2.1/src/caf.space.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-03 13:17:57.000000 caf.space-1.2.1/src/caf.space.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 13:17:57.000000 caf.space-1.2.1/src/caf.space.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-03 13:17:57.000000 caf.space-1.2.1/src/caf.space.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-03 13:17:57.000000 caf.space-1.2.1/src/caf.space.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-03 13:17:57.000000 caf.space-1.2.1/src/caf.space.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:17:57.777060 caf.space-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-03 13:17:41.000000 caf.space-1.2.1/tests/test_weighted_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-03 13:17:41.000000 caf.space-1.2.1/tests/test_zone_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 12:12:49.000000 caf.space-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-24 12:13:05.554793 caf.space-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-24 12:12:49.000000 caf.space-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-24 12:12:49.000000 caf.space-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 12:13:05.554793 caf.space-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-24 12:12:49.000000 caf.space-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.550794 caf.space-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.550794 caf.space-1.2.2/src/caf/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/src/caf/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-24 12:13:05.554793 caf.space-1.2.2/src/caf/space/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/weighted_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/zone_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-04-24 12:12:49.000000 caf.space-1.2.2/src/caf/space/zone_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/src/caf.space.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 12:13:05.000000 caf.space-1.2.2/src/caf.space.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:13:05.554793 caf.space-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-24 12:12:49.000000 caf.space-1.2.2/tests/test_weighted_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-04-24 12:12:49.000000 caf.space-1.2.2/tests/test_zone_translation.py
```

### Comparing `caf.space-1.2.1/LICENSE` & `caf.space-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.1/PKG-INFO` & `caf.space-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.space
-Version: 1.2.1
+Version: 1.2.2
 Summary: Easily generate translations between transport zoning systems
 Home-page: https://github.com/Transport-for-the-North/caf.space
 Author: Transport for the North
 Maintainer: Transport for the North
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.space/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.space
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.space Version: 1.2.1 Summary: Easily generate
+Metadata-Version: 2.1 Name: caf.space Version: 1.2.2 Summary: Easily generate
 translations between transport zoning systems Home-page: https://github.com/
 Transport-for-the-North/caf.space Author: Transport for the North Maintainer:
 Transport for the North License: GPL-3.0 Project-URL: Bug Tracker, https://
 github.com/Transport-for-the-North/caf.space/issues Project-URL: Source, https:
 //github.com/Transport-for-the-North/caf.space Project-URL: Documentation,
 https://cafspcae.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9 Requires-
```

### Comparing `caf.space-1.2.1/README.md` & `caf.space-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.1/pyproject.toml` & `caf.space-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.1/setup.cfg` & `caf.space-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.1/src/caf/space/inputs.py` & `caf.space-1.2.2/src/caf/space/inputs.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.1/src/caf/space/metadata.py` & `caf.space-1.2.2/src/caf/space/metadata.py`

 * *Files identical despite different names*

### Comparing `caf.space-1.2.1/src/caf/space/ui.py` & `caf.space-1.2.2/src/caf/space/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 "User interface for caf.space."
 # Built-Ins
 from functools import partial
 import tkinter as tk
 from tkinter import ttk, filedialog
 from pathlib import Path
 from typing import Optional
+import os
 import sys
+import logging
 
 # Third Party
 from tkinterweb import HtmlFrame, Notebook
 from caf.space import inputs, zone_translation
 
 # Local Imports
 # pylint: disable=import-error,wrong-import-position
@@ -18,17 +20,42 @@
 
 # pylint: enable=import-error,wrong-import-position
 
 # # # CONSTANTS # # #
 SHAPE_FILEFILTER = (("Shapefiles", "*.shp"), ("All files", "*.*"))
 CSV_FILEFILTER = (("CSV", "*.csv"), ("All files", "*.*"))
 
-
 # # # CLASSES # # #
 # pylint: disable=too-many-ancestors, too-many-instance-attributes, unused-argument
+
+
+class RedirectStdOut:  # pylint: disable=too-few-public-methods
+    """Class to redirect stdout to `ScolledText` widget."""
+
+    def __init__(self, text_widget):
+        self.output = text_widget.text
+
+    def write(self, text: str):
+        """Write given `text` to widget.
+
+        Parameters
+        ----------
+        text : str
+            Message to write to widget.
+        """
+        # Check what tag to add
+        tag = None
+        for i in ("warning", "error", "debug"):
+            if f"[{i}]" in text.lower():
+                tag = i
+        self.output.configure(state="normal")
+        self.output.insert("end", text, tag)
+        self.output.configure(state="disabled")
+
+
 class FileWidget(ttk.Frame):
     """Tkinter widget for an entry box to select a file."""
 
     def __init__(
         self,
         parent,
         variable: Optional[tk.StringVar] = None,
@@ -306,20 +333,27 @@
         """
         Get method for class.
 
         Returns
         -------
         Instance of TransZoneSystemInfo class with parameters read from UI.
         """
-        zone = inputs.TransZoneSystemInfo(
-            shapefile=self.shape_var.get(),
-            name=self.name_var.get(),
-            id_col=self.id_col_var.get(),
-            point_shapefile=self.point_shapefile.get(),
-        )
+        if self.point_shapefile.get() == "":
+            zone = inputs.TransZoneSystemInfo(
+                shapefile=self.shape_var.get(),
+                name=self.name_var.get(),
+                id_col=self.id_col_var.get(),
+            )
+        else:
+            zone = inputs.TransZoneSystemInfo(
+                shapefile=self.shape_var.get(),
+                name=self.name_var.get(),
+                id_col=self.id_col_var.get(),
+                point_shapefile=self.point_shapefile.get(),
+            )
         return zone
 
     def validate(self):
         """
         Confirm that this frame is sufficiently provided.
         """
         return self.shape_var.get().endswith(".shp")
@@ -718,38 +752,85 @@
         # Change stdout
         sys.stdout = self.StdoutRedirector(self.text)
         sys.stderr = self.StdoutRedirector(self.text)
 
         # Pack widgets
         yscroll.pack(side="right", fill="y")
         xscroll.pack(side="bottom", fill="x")
+        self.text.tag_configure("warning", foreground="orange")
+        self.text.tag_configure("error", foreground="red")
+        self.text.tag_configure("debug", foreground="gray")
         self.text.pack(side="left", fill="both", expand=True)
 
 
-class SpaceUI:
+class NotebookApp(tk.Tk):
     """
     Main notebook, containing three pages.
 
     One for the UI, one for the documentation, one for the console.
     """
 
     def __init__(self):
-        self.root = tk.Tk()
-        self.notebook = Notebook(self.root)
+        super().__init__()
+        # self.logger = logging.getLogger("SPACE")
+        self.notebook = Notebook(self)
         self.notebook.pack(fill="both", expand=True)
 
         # Add MyUI instance as a tab
         my_ui_tab = ttk.Frame(self.notebook)
         my_ui = UiTab(master=my_ui_tab)
         my_ui.pack(fill="both", expand=True)
         self.notebook.add(my_ui_tab, text="Zone translation parameters")
         readme_tab = HtmlFrame(self.notebook, messages_enabled=False)
         readme_tab.load_website("https://cafspcae.readthedocs.io/en/latest/")
         self.notebook.add(readme_tab, text="Documentation")
         console_tab = ttk.Frame(self.notebook)
-        console_text = ConsoleFrame(console_tab)
-        console_text.pack(fill="both", expand=True)
+        self.console_text = ConsoleFrame(console_tab)
+        self._redirect_logging()
+        self.console_text.pack(fill="both", expand=True)
         self.notebook.add(console_tab, text="Console Output")
-        self.root.mainloop()
+        self.mainloop()
+
+    def _redirect_logging(self):
+        """Add new handler to root logger which outputs to `self.terminal`."""
+        self._logger = logging.getLogger("SPACE")
+        self.console_handler = logging.StreamHandler(stream=RedirectStdOut(self.console_text))
+        fmt = logging.Formatter("[{levelname}] {message}", style="{")
+        self.console_handler.setFormatter(fmt)
+        self.console_handler.setLevel(logging.INFO)
+        self._logger.addHandler(self.console_handler)
+        self._logger.info("Log file saved here: %s", (Path(os.getcwd()) / SpaceUI._LOG_NAME))
+
+
+class SpaceUI:
+    """
+    Main class to launch UI.
+    """
+
+    _LOG_NAME = "SPACE.log"
+
+    def __init__(self):
+        self.log_file = Path(os.getcwd()) / self._LOG_NAME
+        # Remove log file if present
+        if os.path.exists(self.log_file):
+            os.remove(self.log_file)
+
+        # Initiate logger object
+        self.logger = logging.getLogger("SPACE")
+        self.logger.setLevel(logging.DEBUG)
+
+        # Create file handler which logs everything
+        f_h = logging.FileHandler(self.log_file)
+        f_h.setLevel(logging.DEBUG)
+
+        # Create formatter and add to handlers
+        fmt = logging.Formatter(
+            "%(asctime)s [%(name)-20.20s] [%(levelname)-8.8s]  %(message)s"
+        )
+        f_h.setFormatter(fmt)
+        self.logger.addHandler(f_h)
+        # Start it with initial line
+        self.logger.info("Initialised log file.")
+        self._gui = NotebookApp()
 
 
 # pylint: enable=too-many-ancestors, too-many-instance-attributes, unused-argument
```

### Comparing `caf.space-1.2.1/src/caf/space/weighted_funcs.py` & `caf.space-1.2.2/src/caf/space/weighted_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 Contains functionality for creating weighted translations.
 
 These are called in the 'weighted_trans' method in ZoneTranslation.
 """
 ##### IMPORTS #####
+from typing import Optional
 import logging
 import warnings
 from functools import reduce
 import pandas as pd
 
+
 # pylint: disable=import-error
 import geopandas as gpd
 
 # pylint: enable=import-error
 
-from caf.space import inputs, zone_correspondence
+from caf.space import inputs
 
 ##### CONSTANTS #####
 logging.captureWarnings(True)
-LOG = logging.getLogger(__name__)
+LOG = logging.getLogger("SPACE")
 
 
 ##### FUNCTIONS #####
 def _weighted_lower(
     lower_zoning: inputs.LowerZoneSystemInfo,
 ) -> gpd.GeoDataFrame:
     """
@@ -40,17 +42,19 @@
     lower_zone.set_index(lower_zoning.id_col, inplace=True)
     weighting = pd.read_csv(
         lower_zoning.weight_data,
         index_col=lower_zoning.weight_id_col,
     )
     weighted = lower_zone.join(weighting)
     missing = weighted[lower_zoning.data_col].isna().sum()
-    warnings.warn(
-        f"{missing} zones do not match up between the lower zoning and weighting data."
-    )
+    if missing > 0:
+        warnings.warn(
+            f"{missing} zones do not match up between the lower zoning and weighting data.",
+            stacklevel=2,
+        )
     weighted["lower_area"] = weighted.area
     return weighted
 
 
 def _point_handling(
     zone: gpd.GeoDataFrame,
     zone_id: str,
@@ -80,71 +84,74 @@
     the geometry changed. Where there are no zones smaller than threshold the
     function simply returns zone unchanged.
     """
     zone.loc[zone.geometry.geometry.type == "Point", "geometry"] = zone.loc[
         zone.geometry.geometry.type == "Point", "geometry"
     ].buffer(0.1)
     points = zone[zone.area < tolerance]
+    points = points.set_crs("EPSG:27700")
     if len(points) > 0:
         lower.reset_index(inplace=True)
         joined = gpd.sjoin(points, lower, how="left", predicate="within")
         new = pd.merge(lower.reset_index(), joined, how="inner", on=lower_id)
         new = gpd.GeoDataFrame(data=new[zone_id], geometry=new["geometry_x"])
-        overlay = zone.overlay(new, how="symmetric_difference")
+        overlay = zone.overlay(new, how="symmetric_difference", keep_geom_type=False)
         overlay.rename(columns={f"{zone_id}_1": zone_id}, inplace=True)
         out = overlay[~overlay[zone_id].isna()]
         zone = pd.concat([out.loc[:, [zone_id, "geometry"]], new])
     return zone
 
 
 def _create_tiles(
+    zones: dict,
     zone_1: inputs.TransZoneSystemInfo,
     zone_2: inputs.TransZoneSystemInfo,
     lower_zoning: inputs.LowerZoneSystemInfo,
     point_handling: bool,
     point_tolerance: float,
+    zone_1_points: Optional[gpd.GeoDataFrame] = None,
+    zone_2_points: Optional[gpd.GeoDataFrame] = None,
 ) -> pd.DataFrame:
     """
     Create a spanning set of tiles for the weighted translation.
 
     Parameters
     ----------
     zone_1: Info on first zone system
     zone_2: Info on second zone system
     lower_zoning: Info on lower zoning and weight data
 
     Returns
     -------
     A set of weighted tiles used for weighted translation.
     """
-    zones = zone_correspondence.read_zone_shapefiles(zone_1, zone_2)
     zone_1_gdf = zones[zone_1.name]["Zone"][[f"{zone_1.name}_id", "geometry"]]
     zone_2_gdf = zones[zone_2.name]["Zone"][[f"{zone_2.name}_id", "geometry"]]
     weighting = _weighted_lower(lower_zoning)
     if point_handling:
-        if zone_1.point_shapefile:
-            zone_1_points = gpd.read_file(zone_1.point_shapefile)[[zone_1.id_col, "geometry"]]
+        if zone_1_points is not None:
+            zone_1_points = zone_1_points.loc[:, [zone_1.id_col, "geometry"]]
             zone_1_points.rename(columns={zone_1.id_col: f"{zone_1.name}_id"}, inplace=True)
             zone_1_gdf = pd.concat([zone_1_gdf, zone_1_points])
         zone_1_gdf = _point_handling(
             zone_1_gdf, f"{zone_1.name}_id", weighting, lower_zoning.id_col, point_tolerance
         )
-        if zone_2.point_shapefile:
-            zone_2_points = gpd.read_file(zone_2.point_shapefile)[[zone_2.id_col, "geometry"]]
+        if zone_2_points is not None:
+            zone_2_points = zone_2_points.loc[:, [zone_2.id_col, "geometry"]]
             zone_2_points.rename(columns={zone_2.id_col: f"{zone_2.name}_id"}, inplace=True)
             zone_2_gdf = pd.concat([zone_2_gdf, zone_2_points])
         zone_2_gdf = _point_handling(
             zone_2_gdf, f"{zone_2.name}_id", weighting, lower_zoning.id_col, point_tolerance
         )
     tiles = reduce(
         lambda x, y: gpd.overlay(x, y, keep_geom_type=True),
         [zone_1_gdf, zone_2_gdf, weighting],
     )
-    tiles.overlay_area = tiles.area
-    tiles.prop = tiles.overlay_area / tiles.lower_area
+    tiles["overlay_area"] = tiles.area
+    tiles["prop"] = tiles.overlay_area / tiles.lower_area
     tiles[lower_zoning.data_col] *= tiles.prop
     return tiles[
         [
             f"{zone_1.name}_id",
             f"{zone_2.name}_id",
             lower_zoning.data_col,
         ]
@@ -166,19 +173,22 @@
     Grouped and summed df
     """
     totals = frame.groupby(id_col).sum().loc[:, data_col]
     return totals
 
 
 def get_weighted_translation(
+    zones: dict,
     zone_1: inputs.TransZoneSystemInfo,
     zone_2: inputs.TransZoneSystemInfo,
     lower_zoning: inputs.LowerZoneSystemInfo,
     point_handling: bool,
     point_tolerance: float,
+    zone_1_points: Optional[gpd.GeoDataFrame] = None,
+    zone_2_points: Optional[gpd.GeoDataFrame] = None,
 ) -> pd.DataFrame:
     """
     Create overlap totals for zone systems.
 
     Creates totals and joins back up.
 
     Parameters
@@ -192,15 +202,24 @@
     Returns
     -------
     Dataframe with columns for overlap total, zone 1 total, zone 2 total
     weights.
     """
     # create a set of spanning weighted, tiles. These tiles will be
     # grouped in different ways to produce the translation.
-    tiles = _create_tiles(zone_1, zone_2, lower_zoning, point_handling, point_tolerance)
+    tiles = _create_tiles(
+        zones,
+        zone_1,
+        zone_2,
+        lower_zoning,
+        point_handling,
+        point_tolerance,
+        zone_1_points,
+        zone_2_points,
+    )
     # produce total weights by each respective zone system.
     totals_1 = return_totals(tiles, f"{zone_1.name}_id", lower_zoning.data_col).to_frame()
     totals_2 = return_totals(tiles, f"{zone_2.name}_id", lower_zoning.data_col).to_frame()
     # get values of overlaps between zone systems by grouping by both
     # zone systems and summing.
     overlap = (
         tiles.groupby([f"{zone_1.name}_id", f"{zone_2.name}_id"])
@@ -210,19 +229,22 @@
     )
     return overlap.join(totals_1, rsuffix="_1").join(
         totals_2, lsuffix="_overlap", rsuffix="_2"
     )
 
 
 def final_weighted(
+    zones: dict,
     zone_1: inputs.TransZoneSystemInfo,
     zone_2: inputs.TransZoneSystemInfo,
     lower_zoning: inputs.LowerZoneSystemInfo,
     point_handling: bool,
     point_tolerance: float,
+    zone_1_points: Optional[gpd.GeoDataFrame] = None,
+    zone_2_points: Optional[gpd.GeoDataFrame] = None,
 ) -> pd.DataFrame:
     """
     Run functions from module to produce a weighted translation.
 
     Parameters
     ----------
     zone_1: Info on first zone system
@@ -232,15 +254,22 @@
     Returns
     -------
     A weighted zone translation DataFrame. This contains more column than the
     final output and will be passed through more checks for slither and
     rounding before being output, according to the input parameters.
     """
     full_df = get_weighted_translation(
-        zone_1, zone_2, lower_zoning, point_handling, point_tolerance
+        zones,
+        zone_1,
+        zone_2,
+        lower_zoning,
+        point_handling,
+        point_tolerance,
+        zone_1_points,
+        zone_2_points,
     )
     full_df[f"{zone_1.name}_to_{zone_2.name}"] = (
         full_df[f"{lower_zoning.data_col}_overlap"] / full_df[f"{lower_zoning.data_col}_1"]
     )
     full_df[f"{zone_2.name}_to_{zone_1.name}"] = (
         full_df[f"{lower_zoning.data_col}_overlap"] / full_df[f"{lower_zoning.data_col}_2"]
     )
```

### Comparing `caf.space-1.2.1/src/caf/space/zone_correspondence.py` & `caf.space-1.2.2/src/caf/space/zone_correspondence.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import warnings
 
 import geopandas as gpd
 import pandas as pd
 from caf.space import inputs
 
 ##### CONSTANTS #####
-LOG = logging.getLogger(__name__)
+LOG = logging.getLogger("SPACE")
 logging.captureWarnings(True)
 
 ##### FUNCTIONS #####
 
 
 def read_zone_shapefiles(
     zone_1: inputs.TransZoneSystemInfo, zone_2: inputs.TransZoneSystemInfo
@@ -80,15 +80,17 @@
             columns={zone["ID_col"]: f"{name}_id"},
             inplace=True,
         )
         zone["Zone"][f"{name}_area"] = zone["Zone"].area
 
         if not zone["Zone"].crs:
             warnings.warn(f"Zone {name} has no CRS, setting crs to EPSG:27700.")
-            zone["Zone"].crs = "EPSG:27700"
+            zone["Zone"].set_crs = "EPSG:27700"
+        else:
+            zone["Zone"].to_crs("EPSG:27700")
 
     return zones
 
 
 def spatial_zone_correspondence(
     zones: dict,
     zone_1: inputs.TransZoneSystemInfo,
```

### Comparing `caf.space-1.2.1/src/caf/space/zone_translation.py` & `caf.space-1.2.2/src/caf/space/zone_translation.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 Module containing ZoneTranslation class.
 
 Class for producing zone translations from a set of inputs, provided by the
 ZoneTranslationInputs class in 'inputs'.
 """
 import logging
 import warnings
+from pathlib import Path
 import pandas as pd
-from caf.space import weighted_funcs, zone_correspondence, inputs
+import geopandas as gpd
+
+from caf.space import weighted_funcs, zone_correspondence, inputs, utils
 
 ##### CONSTANTS #####
-LOG = logging.getLogger(__name__)
+LOG = logging.getLogger("SPACE")
+# logging.basicConfig(format="%(asctime)s [%(name)-20.20s] [%(levelname)-8.8s]  %(message)s")
 logging.captureWarnings(True)
 
 
 ##### CLASSES #####
 class ZoneTranslation:
     """
     Store paramaters and create zone translations.
@@ -39,27 +43,37 @@
         self.zone_translation
     """
 
     def __init__(self, params: inputs.ZoningTranslationInputs):
         self.params = params
         self.zone_1 = params.zone_1
         self.zone_2 = params.zone_2
+
         self.cache_path = params.cache_path
         if params.lower_zoning:
             self.lower_zoning = params.lower_zoning
         if params.method:
             self.method = params.method
         self.slither_tolerance = params.sliver_tolerance
         self.rounding = params.rounding
         self.filter_slithers = params.filter_slivers
         self.point_handling = params.point_handling
         self.point_tolerance = params.point_tolerance
         self.run_date = params.run_date
         sorted_names = sorted([params.zone_1.name, params.zone_2.name])
         self.names = (sorted_names[0], sorted_names[1])
+        self.logger = logging.getLogger("SPACE")
+        self.handler = logging.FileHandler(
+            self.cache_path / f"{self.names[0]}_{self.names[1]}.log", mode="w"
+        )
+        self.handler.setFormatter(
+            logging.Formatter("%(asctime)s [%(name)-20.20s] [%(levelname)-8.8s]  %(message)s")
+        )
+        self.logger.addHandler(self.handler)
+        self.logger.setLevel(logging.INFO)
 
     def spatial_translation(self) -> pd.DataFrame:
         """
         Create spatial zone translation.
 
         Performs zone correspondence between two zoning systems, zone 1 and
         zone 2. Default correspondence is spatial (by zone area), but includes
@@ -74,43 +88,17 @@
         """
         zones = zone_correspondence.read_zone_shapefiles(self.zone_1, self.zone_2)
         spatial_correspondence = zone_correspondence.spatial_zone_correspondence(
             zones, self.zone_1, self.zone_2
         )
         final_zone_corr = self._slithers_and_rounding(spatial_correspondence)
         # Save correspondence output
-        (
-            missing_zones_1,
-            missing_zones_2,
-        ) = zone_correspondence.missing_zones_check(
-            zones, final_zone_corr, self.zone_1, self.zone_2
-        )
-
-        warnings.warn(f"Missing Zones from 1 : {len(missing_zones_1)}")
-        warnings.warn(f"Missing Zones from 2 : {len(missing_zones_2)}")
         out_path = self.cache_path / f"{self.names[0]}_{self.names[1]}"
-        out_path.mkdir(exist_ok=True, parents=True)
-        log_file = out_path / "missing_zones_log.xlsx"
-        with pd.ExcelWriter(
-            log_file, engine="openpyxl"
-        ) as writer:  # pylint: disable=abstract-class-instantiated
-            missing_zones_1.to_excel(
-                writer,
-                sheet_name=f"{self.names[0]}_missing",
-                index=False,
-            )
-            missing_zones_2.to_excel(
-                writer,
-                sheet_name=f"{self.names[1]}_missing",
-                index=False,
-            )
-        LOG.info(
-            "List of missing zones can be found in log file found here: %s",
-            log_file,
-        )
+        out_path.mkdir(exist_ok=True, parents=False)
+        self.post_processing(zones, final_zone_corr, out_path)
         out_name = f"{self.names[0]}_to_{self.names[1]}_spatial"
         final_zone_corr.to_csv(out_path / f"{out_name}.csv", index=False)
         self.params.save_yaml(out_path / f"{out_name}.yml")
         return final_zone_corr
 
     def weighted_translation(self) -> pd.DataFrame:
         """
@@ -126,66 +114,83 @@
         self: for this to run self.params must contain lower zoning and a method.
 
         Returns
         -------
         weighted_translation: pd.DataFrame
             Dataframe containing weighted zone translation between zone 1 and zone 2.
         """
-        LOG.info("Starting weighted translation")
+        self.logger.info("Starting weighted translation")
         # Init
         if self.params.method is False:
             raise ValueError("A method must be provided to perform a weighted translation.")
         if self.params.lower_zoning is False:
             raise ValueError("Lower zoning data is required for a weighted translations.")
+        zones = zone_correspondence.read_zone_shapefiles(self.zone_1, self.zone_2)
+        points_1 = None
+        points_2 = None
+        if self.zone_1.point_shapefile:
+            if self.zone_2.point_shapefile:
+                points_1 = gpd.read_file(self.zone_1.point_shapefile)
+                points_2 = gpd.read_file(self.zone_2.point_shapefile)
+                if len(points_1) > len(points_2):
+                    matches = utils.find_point_matches(
+                        points_1,
+                        points_2,
+                        1000,
+                        self.zone_1.id_col,
+                        self.zone_2.id_col,
+                        self.zone_1.name,
+                        self.zone_2.name,
+                    )
+                else:
+                    matches = utils.find_point_matches(
+                        points_2,
+                        points_1,
+                        1000,
+                        self.zone_2.id_col,
+                        self.zone_1.id_col,
+                        self.zone_2.name,
+                        self.zone_1.name,
+                    )
+                points_1 = utils.points_update(
+                    points_1, matches, self.zone_1.id_col, f"{self.zone_1.name}_id"
+                )
+                points_2 = utils.points_update(
+                    points_2, matches, self.zone_2.id_col, f"{self.zone_2.name}_id"
+                )
+            else:
+                points_1 = gpd.read_file(self.zone_1.point_shapefile)
+        elif self.zone_2.point_shapefile:
+            points_2 = gpd.read_file(self.zone_2.point_shapefile)
         weighted_translation = weighted_funcs.final_weighted(
+            zones,
             self.zone_1,
             self.zone_2,
             self.lower_zoning,
             self.point_handling,
             self.point_tolerance,
+            points_1,
+            points_2,
         )
         weighted_translation = weighted_translation[
             [
                 f"{self.names[0]}_to_{self.names[1]}",
                 f"{self.names[1]}_to_{self.names[0]}",
             ]
         ]
+        fill_columns = list(weighted_translation.columns)
         weighted_translation.reset_index(inplace=True)
 
         weighted_translation = self._slithers_and_rounding(weighted_translation)
-
-        column_list = list(weighted_translation.columns)
-
-        summary_table_1 = weighted_translation.groupby(column_list[0])[column_list[2]].sum()
-        summary_table_2 = weighted_translation.groupby(column_list[1])[column_list[3]].sum()
-
-        under_1_zones_1 = summary_table_1[summary_table_1 < 0.999999]
-        under_1_zones_2 = summary_table_2[summary_table_2 < 0.999999]
-
-        if len(pd.unique(weighted_translation[column_list[0]])) == sum(summary_table_1):
-            LOG.info("Split factors add up to 1 for %s", column_list[0])
-        else:
-            LOG.warning(
-                "Split factors DO NOT add up to 1 for %s. CHECK "
-                "TRANSLATION IS ACCURATE\n%s",
-                column_list[0],
-                under_1_zones_1,
-            )
-
-        if len(pd.unique(weighted_translation[column_list[1]])) == sum(summary_table_2):
-            LOG.info("Split factors add up to 1 for %s", column_list[1])
-        else:
-            LOG.warning(
-                "Split factors DO NOT add up to 1 for %s. CHECK "
-                "TRANSLATION IS ACCURATE\n%s",
-                column_list[1],
-                under_1_zones_2,
-            )
         out_path = self.cache_path / f"{self.names[0]}_{self.names[1]}"
-        out_path.mkdir(exist_ok=True, parents=True)
+        out_path.mkdir(exist_ok=True, parents=False)
+        if "matches" in locals():
+            matches[fill_columns] = 1
+            weighted_translation = pd.concat([weighted_translation, matches])
+        self.post_processing(zones, weighted_translation, out_path)
         out_name = f"{self.names[0]}_to_{self.names[1]}_{self.method}_{self.lower_zoning.weight_data_year}"
         weighted_translation.to_csv(out_path / f"{out_name}.csv", index=False)
         self.params.save_yaml(out_path / f"{out_name}.yml")
         return weighted_translation
 
     def _slithers_and_rounding(self, translation: pd.DataFrame) -> pd.DataFrame:
         """
@@ -200,32 +205,102 @@
 
         Returns
         -------
         The input dataframe with slithers removed and/or values rounded
         according to input params.
         """
         if self.params.filter_slivers:
-            LOG.info("Filtering out small overlaps.")
+            self.logger.info("Filtering out small overlaps.")
             (
                 _,
                 spatial_correspondence_no_slithers,
             ) = zone_correspondence.find_slithers(
                 translation, self.names, self.params.sliver_tolerance
             )
 
             if self.params.rounding:
-                LOG.info("Checking all adjustment factors add to 1")
+                self.logger.info("Checking all adjustment factors add to 1")
                 final_zone_corr = zone_correspondence.round_zone_correspondence(
                     spatial_correspondence_no_slithers, self.names
                 )
             else:
                 final_zone_corr = spatial_correspondence_no_slithers
         else:
             if self.params.rounding:
-                LOG.info("Checking all adjustment factors add to 1")
+                self.logger.info("Checking all adjustment factors add to 1")
                 final_zone_corr = zone_correspondence.round_zone_correspondence(
                     translation, self.names
                 )
             else:
                 final_zone_corr = translation
 
         return final_zone_corr
+
+    def post_processing(self, zones: dict, zone_translation: gpd.GeoDataFrame, out_path: Path):
+        """
+        Log info after producing a zone translation.
+
+        Parameters
+        ----------
+        zones: dict produced by zone_correspondence.read_zone_shapefile
+        zone_translation: A dataframe containing a weighted or spatial translation.
+        out_path: Path logging files will be written to.
+
+        Returns
+        -------
+        Nothing.
+        """
+        (
+            missing_zones_1,
+            missing_zones_2,
+        ) = zone_correspondence.missing_zones_check(
+            zones, zone_translation, self.zone_1, self.zone_2
+        )
+        if len(missing_zones_1) > 0:
+            warnings.warn(f"Missing Zones from 1 : {len(missing_zones_1)}", stacklevel=2)
+        if len(missing_zones_2) > 0:
+            warnings.warn(f"Missing Zones from 2 : {len(missing_zones_2)}", stacklevel=2)
+        log_file = out_path / "missing_zones_log.xlsx"
+        with pd.ExcelWriter(
+            log_file, engine="openpyxl"
+        ) as writer:  # pylint: disable=abstract-class-instantiated
+            missing_zones_1.to_excel(
+                writer,
+                sheet_name=f"{self.names[0]}_missing",
+                index=False,
+            )
+            missing_zones_2.to_excel(
+                writer,
+                sheet_name=f"{self.names[1]}_missing",
+                index=False,
+            )
+        self.logger.info(
+            "List of missing zones can be found in log file found here: %s",
+            log_file,
+        )
+        column_list = list(zone_translation.columns)
+
+        summary_table_1 = zone_translation.groupby(column_list[0])[column_list[2]].sum()
+        summary_table_2 = zone_translation.groupby(column_list[1])[column_list[3]].sum()
+
+        under_1_zones_1 = summary_table_1[summary_table_1 < 0.999999]
+        under_1_zones_2 = summary_table_2[summary_table_2 < 0.999999]
+
+        if len(pd.unique(zone_translation[column_list[0]])) == sum(summary_table_1):
+            self.logger.info("Split factors add up to 1 for %s", column_list[0])
+        else:
+            self.logger.warning(
+                "Split factors DO NOT add up to 1 for %s. CHECK "
+                "TRANSLATION IS ACCURATE\n%s",
+                column_list[0],
+                under_1_zones_1,
+            )
+
+        if len(pd.unique(zone_translation[column_list[1]])) == sum(summary_table_2):
+            self.logger.info("Split factors add up to 1 for %s", column_list[1])
+        else:
+            self.logger.warning(
+                "Split factors DO NOT add up to 1 for %s. CHECK "
+                "TRANSLATION IS ACCURATE\n%s",
+                column_list[1],
+                under_1_zones_2,
+            )
```

### Comparing `caf.space-1.2.1/src/caf.space.egg-info/PKG-INFO` & `caf.space-1.2.2/src/caf.space.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.space
-Version: 1.2.1
+Version: 1.2.2
 Summary: Easily generate translations between transport zoning systems
 Home-page: https://github.com/Transport-for-the-North/caf.space
 Author: Transport for the North
 Maintainer: Transport for the North
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.space/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.space
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.space Version: 1.2.1 Summary: Easily generate
+Metadata-Version: 2.1 Name: caf.space Version: 1.2.2 Summary: Easily generate
 translations between transport zoning systems Home-page: https://github.com/
 Transport-for-the-North/caf.space Author: Transport for the North Maintainer:
 Transport for the North License: GPL-3.0 Project-URL: Bug Tracker, https://
 github.com/Transport-for-the-North/caf.space/issues Project-URL: Source, https:
 //github.com/Transport-for-the-North/caf.space Project-URL: Documentation,
 https://cafspcae.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9 Requires-
```

### Comparing `caf.space-1.2.1/src/caf.space.egg-info/SOURCES.txt` & `caf.space-1.2.2/src/caf.space.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 src/caf.space.egg-info/requires.txt
 src/caf.space.egg-info/top_level.txt
 src/caf/space/__init__.py
 src/caf/space/_version.py
 src/caf/space/inputs.py
 src/caf/space/metadata.py
 src/caf/space/ui.py
+src/caf/space/utils.py
 src/caf/space/weighted_funcs.py
 src/caf/space/zone_correspondence.py
 src/caf/space/zone_translation.py
 tests/test_weighted_funcs.py
 tests/test_zone_translation.py
```

### Comparing `caf.space-1.2.1/tests/test_weighted_funcs.py` & `caf.space-1.2.2/tests/test_weighted_funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 """
 Module for testing the weighted_funcs module
 """
 from copy import deepcopy
 import pytest
 import pandas as pd
 import geopandas as gpd
-from caf.space import weighted_funcs
+from caf.space import weighted_funcs, zone_correspondence
+
+
+@pytest.fixture(name="zones", scope="session")
+def fixture_zones(weighted_config):
+    zones = zone_correspondence.read_zone_shapefiles(
+        weighted_config.zone_1, weighted_config.zone_2
+    )
+    return zones
 
 
 @pytest.fixture(name="weighted", scope="class")
 def fixture_weighted(weighted_config):
     """
     Fixture returning a lower zone system with a weighting vector attached to
     it.
     """
     weighted = weighted_funcs._weighted_lower(weighted_config.lower_zoning)
     return weighted
 
 
 @pytest.fixture(name="tiles", scope="class")
-def fixture_tiles(weighted_config):
+def fixture_tiles(weighted_config, zones):
     """
     Fixture returning tiles from the _create_tiles function
     """
     tiles = weighted_funcs._create_tiles(
+        zones,
         weighted_config.zone_1,
         weighted_config.zone_2,
         weighted_config.lower_zoning,
         point_handling=False,
         point_tolerance=1,
     )
     return tiles
 
 
 @pytest.fixture(name="overlaps", scope="class")
-def fixture_overlaps(weighted_config):
+def fixture_overlaps(weighted_config, zones):
     """
     Fixture returning overlaps ond totals.
     """
     overlaps = weighted_funcs.get_weighted_translation(
-        weighted_config.zone_1, weighted_config.zone_2, weighted_config.lower_zoning, False, 1
+        zones,
+        weighted_config.zone_1,
+        weighted_config.zone_2,
+        weighted_config.lower_zoning,
+        False,
+        1,
     )
     return overlaps
 
 
 @pytest.fixture(name="point_handling_no_points", scope="class")
 def fixture_no_points(weighted_config):
     zone = gpd.read_file(weighted_config.zone_2.shapefile)
@@ -56,17 +70,17 @@
         tolerance=weighted_config.point_tolerance,
     )
 
     return adjusted, zone
 
 
 @pytest.fixture(name="points_handled", scope="class")
-def fixture_points(point_zones, point_shapefile, weighted_config):
+def fixture_points(point_zones, point_shapefile_2, weighted_config):
     polygons = gpd.read_file(point_zones)
-    points = gpd.read_file(point_shapefile)
+    points = gpd.read_file(point_shapefile_2)
     zone = pd.concat([polygons, points])
     lower = gpd.read_file(weighted_config.lower_zoning.shapefile)
     adjusted = weighted_funcs._point_handling(
         zone=zone,
         zone_id=weighted_config.zone_2.id_col,
         lower=lower,
         lower_id=weighted_config.lower_zoning.id_col,
@@ -141,15 +155,15 @@
     Class for testing _point_handling
     """
 
     def test_no_points(self, point_handling_no_points):
         handled, zone = point_handling_no_points
         pd.testing.assert_frame_equal(handled, zone)
 
-    @pytest.mark.parametrize("column", ["true_point", "pseudo_point"])
+    @pytest.mark.parametrize("column", ["true_point_2", "pseudo_point"])
     def test_point(self, points_handled, column):
         handled = points_handled
         assert (handled.loc[handled["zone_2_id"] == column, "geometry"].area == 4).all()
 
     @pytest.mark.parametrize("column, area", [("Y", 8), ("X", 16)])
     def test_cutout(self, points_handled, column, area):
         handled = points_handled
```

### Comparing `caf.space-1.2.1/tests/test_zone_translation.py` & `caf.space-1.2.2/tests/test_zone_translation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
     Module for testing the zone_translation module
 """
+from math import sqrt
 from pathlib import Path
 import pytest
 import pandas as pd
 import geopandas as gpd
+from copy import deepcopy
 
 # pylint: disable=import-error, wrong-import-position
 from caf.space import zone_translation
 from caf.space import inputs
 
 
 # pylint: enable=import-error,wrong-import-position
@@ -45,17 +47,17 @@
     ----------
     weighted_config:
         weighted config to modify and use for a new translation.
     Returns
     -------
         A new config with lower zoning and zone 2 the same.
     """
-    config = weighted_config.copy()
-    config.zone_2 = weighted_config.lower_zoning
-    config.zone_2.name = weighted_config.zone_2.name
+    config = deepcopy(weighted_config)
+    config.zone_2.shapefile = weighted_config.lower_zoning.shapefile
+    config.zone_2.id_col = weighted_config.lower_zoning.id_col
     config.lower_zoning.name = weighted_config.zone_2.name
     return config
 
 
 @pytest.fixture(name="expected_weighted", scope="class")
 def fixture_expected_weighted() -> pd.DataFrame:
     """
@@ -84,27 +86,37 @@
 
 @pytest.fixture(name="expected_points", scope="class")
 def fixture_expected_points() -> pd.DataFrame:
     # fmt: off
     output = pd.DataFrame(
         {
             "zone_1_id": ["A", "A", "A", "A", "B", "B", "B", "C", "C", "C"],
-            "zone_2_id": ["W", "X", "Y", "Z", "X", "Z", "true_point", "Y", "Z", "pseudo_point"],
+            "zone_2_id": ["W", "X", "Y", "Z", "X", "Z", "true_point_2", "Y", "Z", "pseudo_point"],
             "zone_1_to_zone_2": [
                 0.529, 0.176, 0.235, 0.059, 0.526, 0.263, 0.211, 0.269, 0.5, 0.231
             ],
             "zone_2_to_zone_1": [
                 1, 0.231, 0.364, 0.053, 0.769, 0.263, 1, 0.636, 0.684, 1
             ],
         }
     )
     # fmt: on
     return output
 
 
+@pytest.fixture(name="expected_point_to_point", scope="class")
+def fixture_expetced_point_to_point(expected_weighted) -> pd.DataFrame:
+    df = deepcopy(expected_weighted)
+    df["dist"] = 0
+    df.loc[8] = ["true_point_1", "true_point_2", 1, 1, round(sqrt(2), 3)]
+    df.set_index(["zone_1_id", "zone_2_id"], inplace=True)
+
+    return df
+
+
 @pytest.fixture(name="expected_spatial", scope="class")
 def fixture_expected_spatial() -> pd.DataFrame:
     """
     The expected output from a weighted translation using vanila inputs.
     Compare to output from weighted translation in testing
     Returns:
         pd.DataFrame: 4 columns of zone_1, zone_2, zone_1_to_zone_2,
@@ -144,15 +156,22 @@
 
 class TestZoneTranslation:
     """
     Class containing tests for the ZoneTranslation class
     """
 
     @pytest.mark.parametrize(
-        "translation_str", ["spatial_trans", "weighted_trans", "dupe_trans", "point_trans"]
+        "translation_str",
+        [
+            "spatial_trans",
+            "weighted_trans",
+            "dupe_trans",
+            "point_trans",
+            "point_to_point_trans",
+        ],
     )
     @pytest.mark.parametrize("origin_zone", [1, 2])
     def test_sum_to_1(self, translation_str: str, origin_zone: int, request):
         """
         Test that translation totals from each zone sum to 1.
         Parameters
         ----------
@@ -169,15 +188,22 @@
         summed = trans.groupby(f"zone_{origin_zone}_id").sum()
         rounded = round(summed[f"zone_{origin_zone}_to_zone_{dic[origin_zone]}"], 5).astype(
             "int"
         )
         assert (rounded == 1).all()
 
     @pytest.mark.parametrize(
-        "translation_str", ["spatial_trans", "weighted_trans", "dupe_trans", "point_trans"]
+        "translation_str",
+        [
+            "spatial_trans",
+            "weighted_trans",
+            "dupe_trans",
+            "point_trans",
+            "point_to_point_trans",
+        ],
     )
     @pytest.mark.parametrize("col", ["zone_1_to_zone_2", "zone_2_to_zone_1"])
     def test_positive(self, translation_str: str, col: str, request):
         """
         Tests that all translation values are positive
         Parameters
         ----------
@@ -207,14 +233,15 @@
 
     @pytest.mark.parametrize(
         "expected_str,trans_str",
         [
             ("expected_spatial", "spatial_trans"),
             ("expected_weighted", "weighted_trans"),
             ("expected_points", "point_trans"),
+            ("expected_point_to_point", "point_to_point_trans"),
         ],
     )
     def test_output(self, trans_str: str, expected_str: str, request):
         """
         Test to see if generated test case zone translations match expected values calculated
         independently.
         Parameters
```

