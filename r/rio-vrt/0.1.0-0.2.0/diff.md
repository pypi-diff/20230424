# Comparing `tmp/rio-vrt-0.1.0.tar.gz` & `tmp/rio-vrt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-vrt-0.1.0.tar", last modified: Tue Apr 11 06:09:06 2023, max compression
+gzip compressed data, was "rio-vrt-0.2.0.tar", last modified: Mon Apr 24 08:05:59 2023, max compression
```

## Comparing `rio-vrt-0.1.0.tar` & `rio-vrt-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.456069 rio-vrt-0.1.0/rio_vrt/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/rio_vrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/rio_vrt/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/rio_vrt/vrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/rio_vrt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 06:09:06.000000 rio-vrt-0.1.0/rio_vrt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 06:08:50.000000 rio-vrt-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:09:06.460069 rio-vrt-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 06:08:51.000000 rio-vrt-0.1.0/tests/test_rio_vrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:05:59.222433 rio-vrt-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 08:05:59.222433 rio-vrt-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-24 08:05:38.000000 rio-vrt-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-24 08:05:38.000000 rio-vrt-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:05:59.218433 rio-vrt-0.2.0/rio_vrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 08:05:38.000000 rio-vrt-0.2.0/rio_vrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-24 08:05:38.000000 rio-vrt-0.2.0/rio_vrt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-24 08:05:38.000000 rio-vrt-0.2.0/rio_vrt/vrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:05:59.222433 rio-vrt-0.2.0/rio_vrt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 08:05:59.000000 rio-vrt-0.2.0/rio_vrt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-24 08:05:59.000000 rio-vrt-0.2.0/rio_vrt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:05:59.000000 rio-vrt-0.2.0/rio_vrt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-24 08:05:59.000000 rio-vrt-0.2.0/rio_vrt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 08:05:59.000000 rio-vrt-0.2.0/rio_vrt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:05:59.222433 rio-vrt-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-24 08:05:38.000000 rio-vrt-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:05:59.222433 rio-vrt-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-24 08:05:39.000000 rio-vrt-0.2.0/tests/test_rio_vrt.py
```

### Comparing `rio-vrt-0.1.0/PKG-INFO` & `rio-vrt-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-vrt
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple librairy to build a vrt from multiple raster source relying only on rasterio
 Author-email: pierrick rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/12rambau/rio-vrt
 Keywords: skeleton,Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -55,18 +55,14 @@
     :target: https://codecov.io/gh/12rambau/rio-vrt
     :alt: Test Coverage
 
 .. image:: https://img.shields.io/readthedocs/rio-vrt?logo=readthedocs&logoColor=white
     :target: https://rio-vrt.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
-    :alt: All contributors
-    :target: AUTHORS.rst
-
 Overview
 --------
 
 A simple librairy to build a vrt from multiple raster source relying only on rasterio.
 
 .. code-block:: python
```

### Comparing `rio-vrt-0.1.0/README.rst` & `rio-vrt-0.2.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -34,18 +34,14 @@
     :target: https://codecov.io/gh/12rambau/rio-vrt
     :alt: Test Coverage
 
 .. image:: https://img.shields.io/readthedocs/rio-vrt?logo=readthedocs&logoColor=white
     :target: https://rio-vrt.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
-    :alt: All contributors
-    :target: AUTHORS.rst
-
 Overview
 --------
 
 A simple librairy to build a vrt from multiple raster source relying only on rasterio.
 
 .. code-block:: python
```

### Comparing `rio-vrt-0.1.0/pyproject.toml` & `rio-vrt-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rio-vrt"
-version = "0.1.0"
+version = "0.2.0"
 description = "A simple librairy to build a vrt from multiple raster source relying only on rasterio"
 keywords = ["skeleton", "Python"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
@@ -45,15 +45,15 @@
 [tool.setuptools.packages.find]
 include = ["rio_vrt*"]
 exclude = ["docs*", "tests*"]
 
 [tool.commitizen]
 tag_format = "v$major.$minor.$patch$prerelease"
 update_changelog_on_bump = false
-version = "0.1.0"
+version = "0.2.0"
 version_files = [
     "pyproject.toml:version",
     "rio_vrt/__init__.py:__version__",
     "docs/conf.py:release"
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `rio-vrt-0.1.0/rio_vrt/vrt.py` & `rio-vrt-0.2.0/rio_vrt/vrt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,63 @@
 """Rasterio based vrt creation."""
 
 import xml.etree.cElementTree as ET
+from os.path import relpath
 from pathlib import Path
 from typing import List, Union
 from xml.dom import minidom
 
 import rasterio as rio
 from rasterio.enums import ColorInterp
 
 from .enums import types
 
 
+def _add_source_content(
+    Source: ET.Element, src: rio.DatasetReader, type: str, xoff: str, yoff: str
+) -> None:
+    """Add the content of a sourcefile in xml."""
+    width, height = str(src.width), str(src.height)
+    blockx, blocky = str(src.profile["blockxsize"]), str(src.profile["blockysize"])
+
+    attr = {
+        "RasterXSize": width,
+        "RasterYSize": height,
+        "DataType": type,
+        "BlockXSize": blockx,
+        "BlockYSize": blocky,
+    }
+    ET.SubElement(Source, "SourceProperties", attr)
+
+    attr = {"xOff": "0", "yOff": "0", "xSize": width, "ySize": height}
+    ET.SubElement(Source, "SrcRect", attr)
+
+    attr = {"xOff": xoff, "yOff": yoff, "xSize": width, "ySize": height}
+    ET.SubElement(Source, "DstRect", attr)
+
+
 def build_vrt(
-    vrt_path: Union[str, Path], files: List[Union[str, Path]], relative: bool = False
+    vrt_path: Union[str, Path],
+    files: List[Union[str, Path]],
+    relative: bool = False,
+    mosaic: bool = True,
 ) -> Path:
     """Create a vrt file from multiple files.
 
     Arguments:
         vrt_path: the final vrt file
         files: a list of rasterio readable files
         relative: use a path relative to the vrt file. The files path must be relative to the vrt.
+        mosaic: The method to use to gather images in the vrt. ``MOSAIC`` (True) will mosaic each band of each image together. ``STACK`` (False) will create one band for each file using the first band of each file.
 
     Returns:
         the path to the vrt file
     """
     # transform the final file in Path
-    vrt_path = Path(vrt_path)
+    vrt_path = Path(vrt_path).resolve()
 
     # transform all the file path into Path objects
     files = [Path(f).resolve() for f in files]
 
     # cannot do anything if there are no files
     if len(files) == 0:
         raise ValueError("There should be at least 1 file to create a vrt.")
@@ -41,121 +69,129 @@
         x_res, y_res = f.res
         count = f.count
         dtypes = f.dtypes
         colorinterps = f.colorinterp
         indexes = f.indexes
         nodatavals = f.nodatavals
 
+    # for stacks replace count and indexes as we only take the first band
+    if not mosaic:
+        count, indexes = len(files), [1]
+
     # sanity checks
     for file in files:
         with rio.open(file) as f:
             if f.crs != crs:
                 raise ValueError(
                     f'the crs ({f.crs}) from file "{file}" is not corresponding to the global one ({crs})'
                 )
 
-            if f.count != count:
+            if mosaic and f.count != count:
                 raise ValueError(
                     f'the crs ({f.count}) from file "{file}" is not corresponding to the global one ({count})'
                 )
 
-    # read all files to extract information and perform
+    # read all files to extract information on the spatial extend of the vrt
     for file in files:
         with rio.open(file) as f:
             left = min(left, f.bounds.left)
             bottom = min(bottom, f.bounds.bottom)
             right = max(right, f.bounds.right)
             top = max(top, f.bounds.top)
 
-        # rebuild the affine transformation from gathered information
-        # negative y_res as we start from the top-left corner
-        transform = rio.Affine.from_gdal(left, x_res, 0, top, 0, -y_res)
-
+    # rebuild the affine transformation from gathered information along with total bounds
+    # negative y_res as we start from the top-left corner
+    transform = rio.Affine.from_gdal(left, x_res, 0, top, 0, -y_res)
     total_width = round((right - left) / x_res)
     total_height = round((top - bottom) / y_res)
 
     # start the tree
-    VRTDataset = ET.Element(
-        "VRTDataset",
-        {"rasterXSize": str(total_width), "rasterYSize": str(total_height)},
-    )
+    attr = {"rasterXSize": str(total_width), "rasterYSize": str(total_height)}
+    VRTDataset = ET.Element("VRTDataset", attr)
+
     ET.SubElement(VRTDataset, "SRS", {"dataAxisToSRSAxisMapping": "2,1"}).text = crs.wkt
-    ET.SubElement(VRTDataset, "GeoTransform").text = ", ".join(
-        [str(i) for i in transform.to_gdal()]
-    )
+
+    text = ", ".join([str(i) for i in transform.to_gdal()])
+    ET.SubElement(VRTDataset, "GeoTransform").text = text
+
     ET.SubElement(VRTDataset, "OverviewList", {"resampling": "nearest"}).text = "2 4 8"
 
-    # create the bands subelements
-    VRTRasterBands = {}
-    for i in indexes:
-        VRTRasterBands[i] = ET.SubElement(
-            VRTDataset,
-            "VRTRasterBand",
-            {"dataType": types[dtypes[i - 1]], "band": str(i)},
-        )
-        ET.SubElement(VRTRasterBands[i], "Offset").text = "0.0"
-        ET.SubElement(VRTRasterBands[i], "Scale").text = "1.0"
-        if colorinterps[i - 1] != ColorInterp.undefined:
-            ET.SubElement(VRTRasterBands[i], "ColorInterp").text = colorinterps[
-                i - 1
-            ].name.capitalize()
-
-    # add the files
-    for f in files:
-        relativeToVRT = "1" if relative is True else "0"
-        with rio.open(f) as src:
-            for i in indexes:
-                if colorinterps[i - 1] == ColorInterp.alpha:
-                    source_type = "ComplexSource"
-                else:
-                    source_type = "SimpleSource"
-
-                Source = ET.SubElement(VRTRasterBands[i], source_type)
-                ET.SubElement(
-                    Source, "SourceFilename", {"relativeToVRT": relativeToVRT}
-                ).text = (
-                    str(f) if relative is False else str(f.relative_to(vrt_path.parent))
-                )
-                ET.SubElement(Source, "SourceBand").text = str(i)
-                ET.SubElement(
-                    Source,
-                    "SourceProperties",
-                    {
-                        "RasterXSize": str(src.width),
-                        "RasterYSize": str(src.height),
-                        "DataType": types[dtypes[i - 1]],
-                        "BlockXSize": str(src.profile["blockxsize"]),
-                        "BlockYSize": str(src.profile["blockysize"]),
-                    },
-                )
-                ET.SubElement(
-                    Source,
-                    "SrcRect",
-                    {
-                        "xOff": "0",
-                        "yOff": "0",
-                        "xSize": str(src.width),
-                        "ySize": str(src.height),
-                    },
-                )
-                ET.SubElement(
-                    Source,
-                    "DstRect",
-                    {
-                        "xOff": str(abs(round((src.bounds.left - left) / x_res))),
-                        "yOff": str(abs(round((src.bounds.top - top) / y_res))),
-                        "xSize": str(src.width),
-                        "ySize": str(src.height),
-                    },
-                )
-                if nodatavals[i - 1] is not None:
-                    ET.SubElement(Source, "NoDataValue").text = str(nodatavals[i - 1])
+    # add the rasterbands
 
-                if colorinterps[i - 1] == ColorInterp.alpha:
-                    ET.SubElement(Source, "UseMaskBand").text = "true"
+    # mosaicking create 1 band for each band of the images and add al the fils as
+    # simple sources along with color informations
+    if mosaic:
+        VRTRasterBands_dict = {}
+        for i in indexes:
+            attr = {"dataType": types[dtypes[i - 1]], "band": str(i)}
+            VRTRasterBands_dict[i] = ET.SubElement(VRTDataset, "VRTRasterBand", attr)
+
+            ET.SubElement(VRTRasterBands_dict[i], "Offset").text = "0.0"
+
+            ET.SubElement(VRTRasterBands_dict[i], "Scale").text = "1.0"
+
+            if colorinterps[i - 1] != ColorInterp.undefined:
+                color = colorinterps[i - 1].name.capitalize()
+                ET.SubElement(VRTRasterBands_dict[i], "ColorInterp").text = color
+
+        # add the files
+        for f in files:
+            relativeToVRT = "1" if relative is True else "0"
+            with rio.open(f) as src:
+                for i in indexes:
+                    is_alpha = colorinterps[i - 1] == ColorInterp.alpha
+                    source_type = "ComplexSource" if is_alpha else "SimpleSource"
+                    Source = ET.SubElement(VRTRasterBands_dict[i], source_type)
+
+                    attr = {"relativeToVRT": relativeToVRT}
+                    text = str(f) if not relative else relpath(f, vrt_path.parent)
+                    ET.SubElement(Source, "SourceFilename", attr).text = text
+
+                    ET.SubElement(Source, "SourceBand").text = str(i)
+
+                    _add_source_content(
+                        Source=Source,
+                        src=src,
+                        type=types[dtypes[i - 1]],
+                        xoff=str(abs(round((src.bounds.left - left) / x_res))),
+                        yoff=str(abs(round((src.bounds.top - top) / y_res))),
+                    )
+
+                    if nodatavals[i - 1] is not None:
+                        text = str(nodatavals[i - 1])
+                        ET.SubElement(Source, "NoDataValue").text = text
+
+                    if colorinterps[i - 1] == ColorInterp.alpha:
+                        ET.SubElement(Source, "UseMaskBand").text = "true"
+
+    # in stacked vrt, each file is added as a single band and only the first band is
+    # considered. They are all complex sources to make sure GIS softwares don't do funny
+    # display upon reading
+    elif not mosaic:
+        for i, f in enumerate(files):
+            attr = {"dataType": types[dtypes[0]], "band": str(i)}
+            VRTRasterBands = ET.SubElement(VRTDataset, "VRTRasterBand", attr)
+
+            ComplexSource = ET.SubElement(VRTRasterBands, "ComplexSource")
+
+            relativeToVRT = "1" if relative is True else "0"
+            attr = {"relativeToVRT": relativeToVRT}
+            text = str(f) if not relative else relpath(f, vrt_path.parent)
+            ET.SubElement(ComplexSource, "SourceFilename", attr).text = text
+
+            ET.SubElement(ComplexSource, "SourceBand").text = "1"
+
+            with rio.open(f) as src:
+                _add_source_content(
+                    Source=ComplexSource,
+                    src=src,
+                    type=types[dtypes[0]],
+                    xoff=str(abs(round((src.bounds.left - left) / x_res))),
+                    yoff=str(abs(round((src.bounds.top - top) / y_res))),
+                )
 
     # write the file
     vrt_path.resolve().write_text(
         minidom.parseString(ET.tostring(VRTDataset).decode("utf-8"))
         .toprettyxml(indent="  ")
         .replace("&quot;", '"')
     )
```

### Comparing `rio-vrt-0.1.0/rio_vrt.egg-info/PKG-INFO` & `rio-vrt-0.2.0/rio_vrt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-vrt
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple librairy to build a vrt from multiple raster source relying only on rasterio
 Author-email: pierrick rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/12rambau/rio-vrt
 Keywords: skeleton,Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -55,18 +55,14 @@
     :target: https://codecov.io/gh/12rambau/rio-vrt
     :alt: Test Coverage
 
 .. image:: https://img.shields.io/readthedocs/rio-vrt?logo=readthedocs&logoColor=white
     :target: https://rio-vrt.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/badge/all_contributors-0-orange.svg
-    :alt: All contributors
-    :target: AUTHORS.rst
-
 Overview
 --------
 
 A simple librairy to build a vrt from multiple raster source relying only on rasterio.
 
 .. code-block:: python
```

### Comparing `rio-vrt-0.1.0/tests/test_rio_vrt.py` & `rio-vrt-0.2.0/tests/test_rio_vrt.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,40 @@
 from urllib.request import urlopen
 
 import xmlschema
 from bs4 import BeautifulSoup
 
 import rio_vrt
 
+_xsd_file = "https://raw.githubusercontent.com/OSGeo/gdal/master/data/gdalvrt.xsd"
 
-def test_build_vrt_shema(tiles: List[Path], data_dir: Path) -> None:
+
+def test_build_vrt_html_shema(tiles: List[Path], data_dir: Path) -> None:
     """Ensure the build vrt is respecting GDAL shema.
 
     Args:
         tiles: the list of tile path
         data_dir: the data directory
     """
     with NamedTemporaryFile(suffix=".vrt", dir=data_dir) as vrt_path:
         vrt_file = rio_vrt.build_vrt(vrt_path.name, tiles)
-        xsd_file = (
-            "https://raw.githubusercontent.com/OSGeo/gdal/master/data/gdalvrt.xsd"
-        )
-        xml_schema = xmlschema.XMLSchema(urlopen(xsd_file))
+        xml_schema = xmlschema.XMLSchema(urlopen(_xsd_file))
+        assert xml_schema.is_valid(vrt_file)
+
+
+def test_build_vrt_stack_shema(tiles: List[Path], data_dir: Path) -> None:
+    """Ensure the build vrt is respecting GDAL shema.
+
+    Args:
+        tiles: the list of tile path
+        data_dir: the data directory
+    """
+    with NamedTemporaryFile(suffix=".vrt", dir=data_dir) as vrt_path:
+        vrt_file = rio_vrt.build_vrt(vrt_path.name, tiles, mosaic=False)
+        xml_schema = xmlschema.XMLSchema(urlopen(_xsd_file))
         assert xml_schema.is_valid(vrt_file)
 
 
 def test_build_vrt_complete(tiles: List[Path], data_dir: Path, file_regression) -> None:
     """Test a complete vrt where all tiles are touching each other.
 
     Args:
@@ -50,7 +62,23 @@
     """
     # filter only the pair tiles
     tiles = [t for i, t in enumerate(tiles) if i % 2]
     with NamedTemporaryFile(suffix=".vrt", dir=data_dir) as vrt_path:
         file = rio_vrt.build_vrt(vrt_path.name, tiles, relative=True)
         vrt_tree = BeautifulSoup(file.read_text(), "xml").prettify()
         file_regression.check(vrt_tree, basename="hollow_vrt", extension=".vrt")
+
+
+def test_build_vrt_stack(tiles: List[Path], data_dir: Path, file_regression) -> None:
+    """Test a complete vrt where some tiles are missing.
+
+    Args:
+        tiles: the list of tile path
+        data_dir: the data directory
+        file_regression: the pytest regression file fixture
+    """
+    # filter only the pair tiles
+    tiles = [t for i, t in enumerate(tiles) if i % 2]
+    with NamedTemporaryFile(suffix=".vrt", dir=data_dir) as vrt_path:
+        file = rio_vrt.build_vrt(vrt_path.name, tiles, relative=True, mosaic=False)
+        vrt_tree = BeautifulSoup(file.read_text(), "xml").prettify()
+        file_regression.check(vrt_tree, basename="stack_vrt", extension=".vrt")
```

