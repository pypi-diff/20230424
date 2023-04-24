# Comparing `tmp/fibsem_tools-3.1.2.tar.gz` & `tmp/fibsem_tools-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibsem_tools-3.1.2.tar", max compression
+gzip compressed data, was "fibsem_tools-3.2.0.tar", max compression
```

## Comparing `fibsem_tools-3.1.2.tar` & `fibsem_tools-3.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-3.1.2/LICENSE
--rw-r--r--   0        0        0     1397 2023-04-05 15:57:18.218031 fibsem_tools-3.1.2/pyproject.toml
--rw-r--r--   0        0        0      183 2023-03-23 18:14:36.952245 fibsem_tools-3.1.2/src/fibsem_tools/__init__.py
--rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-3.1.2/src/fibsem_tools/cli/tiff2zarr.css
--rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-3.1.2/src/fibsem_tools/cli/tiff2zarr.py
--rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-3.1.2/src/fibsem_tools/io/__init__.py
--rw-r--r--   0        0        0     8540 2023-03-26 19:15:38.082791 fibsem_tools-3.1.2/src/fibsem_tools/io/core.py
--rw-r--r--   0        0        0    13817 2023-04-02 16:17:25.433740 fibsem_tools-3.1.2/src/fibsem_tools/io/dask.py
--rw-r--r--   0        0        0    29922 2023-03-23 19:37:34.954215 fibsem_tools-3.1.2/src/fibsem_tools/io/fibsem.py
--rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-3.1.2/src/fibsem_tools/io/h5.py
--rw-r--r--   0        0        0     3521 2023-03-23 19:35:10.739716 fibsem_tools-3.1.2/src/fibsem_tools/io/mrc.py
--rw-r--r--   0        0        0     6759 2023-04-05 15:51:53.357061 fibsem_tools-3.1.2/src/fibsem_tools/io/multiscale.py
--rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-3.1.2/src/fibsem_tools/io/neuroglancer.py
--rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-3.1.2/src/fibsem_tools/io/server.py
--rw-r--r--   0        0        0     3551 2023-03-25 02:44:53.556172 fibsem_tools-3.1.2/src/fibsem_tools/io/util.py
--rw-r--r--   0        0        0     1454 2023-04-05 15:50:28.371811 fibsem_tools-3.1.2/src/fibsem_tools/io/xr.py
--rw-r--r--   0        0        0    13187 2023-04-02 12:58:33.871409 fibsem_tools-3.1.2/src/fibsem_tools/io/zarr.py
--rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-3.1.2/src/fibsem_tools/metadata/__init__.py
--rw-r--r--   0        0        0     3195 2023-04-05 15:51:53.357628 fibsem_tools-3.1.2/src/fibsem_tools/metadata/cosem.py
--rw-r--r--   0        0        0     3479 2023-03-22 20:52:50.925475 fibsem_tools-3.1.2/src/fibsem_tools/metadata/groundtruth.py
--rw-r--r--   0        0        0     2123 2023-03-16 20:03:20.243743 fibsem_tools-3.1.2/src/fibsem_tools/metadata/neuroglancer.py
--rw-r--r--   0        0        0     3373 2023-03-16 20:01:35.764425 fibsem_tools-3.1.2/src/fibsem_tools/metadata/transform.py
--rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-3.1.2/src/fibsem_tools/py.typed
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 fibsem_tools-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-3.2.0/LICENSE
+-rw-r--r--   0        0        0     1397 2023-04-24 15:38:16.499953 fibsem_tools-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-03-23 18:14:36.952245 fibsem_tools-3.2.0/src/fibsem_tools/__init__.py
+-rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.css
+-rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-3.2.0/src/fibsem_tools/io/__init__.py
+-rw-r--r--   0        0        0     9151 2023-04-24 15:38:06.907899 fibsem_tools-3.2.0/src/fibsem_tools/io/core.py
+-rw-r--r--   0        0        0    13817 2023-04-02 16:17:25.433740 fibsem_tools-3.2.0/src/fibsem_tools/io/dask.py
+-rw-r--r--   0        0        0    29922 2023-03-23 19:37:34.954215 fibsem_tools-3.2.0/src/fibsem_tools/io/fibsem.py
+-rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-3.2.0/src/fibsem_tools/io/h5.py
+-rw-r--r--   0        0        0     3521 2023-03-23 19:35:10.739716 fibsem_tools-3.2.0/src/fibsem_tools/io/mrc.py
+-rw-r--r--   0        0        0     6759 2023-04-05 15:51:53.357061 fibsem_tools-3.2.0/src/fibsem_tools/io/multiscale.py
+-rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-3.2.0/src/fibsem_tools/io/neuroglancer.py
+-rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-3.2.0/src/fibsem_tools/io/server.py
+-rw-r--r--   0        0        0     3551 2023-03-25 02:44:53.556172 fibsem_tools-3.2.0/src/fibsem_tools/io/util.py
+-rw-r--r--   0        0        0     1454 2023-04-05 15:50:28.371811 fibsem_tools-3.2.0/src/fibsem_tools/io/xr.py
+-rw-r--r--   0        0        0    13187 2023-04-15 17:19:41.433351 fibsem_tools-3.2.0/src/fibsem_tools/io/zarr.py
+-rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-3.2.0/src/fibsem_tools/metadata/__init__.py
+-rw-r--r--   0        0        0     3195 2023-04-05 15:51:53.357628 fibsem_tools-3.2.0/src/fibsem_tools/metadata/cosem.py
+-rw-r--r--   0        0        0     3479 2023-03-22 20:52:50.925475 fibsem_tools-3.2.0/src/fibsem_tools/metadata/groundtruth.py
+-rw-r--r--   0        0        0     2123 2023-03-16 20:03:20.243743 fibsem_tools-3.2.0/src/fibsem_tools/metadata/neuroglancer.py
+-rw-r--r--   0        0        0     3373 2023-03-16 20:01:35.764425 fibsem_tools-3.2.0/src/fibsem_tools/metadata/transform.py
+-rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-3.2.0/src/fibsem_tools/py.typed
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 fibsem_tools-3.2.0/PKG-INFO
```

### Comparing `fibsem_tools-3.1.2/LICENSE` & `fibsem_tools-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/pyproject.toml` & `fibsem_tools-3.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fibsem-tools"
-version = "3.1.2"
+version = "3.2.0"
 description = "Tools for processing FIBSEM datasets"
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 distributed = ">=2021.10.0"
```

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/cli/tiff2zarr.css` & `fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.css`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/cli/tiff2zarr.py` & `fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/core.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     access_n5,
     access_parent,
     access_zarr,
     n5_to_dask,
     infer_coords as z_infer_coords,
     zarr_to_dask,
 )
+from warnings import warn
 
 
 _formats = (".dat", ".mrc", ".tif")
 _container_extensions = (".zarr", ".n5", ".h5")
 _suffixes = (*_formats, *_container_extensions)
 
 
@@ -199,32 +200,48 @@
     return daskifiers[suffix](uri, chunks, **kwargs)
 
 
 def read_xarray(
     url: str,
     chunks: Union[str, Tuple[int, ...]] = "auto",
     coords: Any = "auto",
+    keep_attrs: bool = False,
     use_dask: bool = True,
     storage_options: Dict[str, Any] = {},
     **kwargs: Any,
 ) -> DataArray:
     """
     Create an xarray.DataArray from data found at a path.
     """
     raw_array = read(url, storage_options=storage_options)
+    attrs = {}
+    if keep_attrs:
+        if hasattr(raw_array, "attrs"):
+            attrs = dict(raw_array.attrs)
+        else:
+            warn(
+                f"""
+            The read_xarray function was invoked with the `keep_attrs` keyword argument 
+            set to `True`, but the array found at the url {url} was read as an instance 
+            of {type(raw_array)} which does not have an `attrs` property. This may 
+            generate an error in the future.
+            """
+            )
     if use_dask:
         array = read_dask(url, chunks=chunks, storage_options=storage_options)
+    else:
+        array = raw_array
 
     if coords == "auto":
         coords = infer_coordinates(raw_array)
 
     elif isinstance(coords, STTransform):
         coords = coords.to_coords(array.shape)
 
-    result = DataArray(array, coords=coords, **kwargs)
+    result = DataArray(array, coords=coords, attrs=attrs, **kwargs)
     return result
 
 
 def infer_coordinates(arr: npt.ArrayLike) -> List[DataArray]:
 
     if isinstance(arr, zarr.core.Array):
         coords = z_infer_coords(
```

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/dask.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/dask.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/fibsem.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/fibsem.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/h5.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/h5.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/mrc.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/mrc.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/multiscale.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/multiscale.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/server.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/server.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/util.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/util.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/xr.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/xr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/io/zarr.py` & `fibsem_tools-3.2.0/src/fibsem_tools/io/zarr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/metadata/cosem.py` & `fibsem_tools-3.2.0/src/fibsem_tools/metadata/cosem.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/metadata/groundtruth.py` & `fibsem_tools-3.2.0/src/fibsem_tools/metadata/groundtruth.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/metadata/neuroglancer.py` & `fibsem_tools-3.2.0/src/fibsem_tools/metadata/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/src/fibsem_tools/metadata/transform.py` & `fibsem_tools-3.2.0/src/fibsem_tools/metadata/transform.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.1.2/PKG-INFO` & `fibsem_tools-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibsem-tools
-Version: 3.1.2
+Version: 3.2.0
 Summary: Tools for processing FIBSEM datasets
 License: MIT
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

