# Comparing `tmp/stac_geoparquet-0.1.0.tar.gz` & `tmp/stac_geoparquet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_geoparquet-0.1.0.tar", last modified: Wed Jun 22 18:00:38 2022, max compression
+gzip compressed data, was "stac_geoparquet-0.2.0.tar", last modified: Mon Apr 24 17:00:06 2023, max compression
```

## Comparing `stac_geoparquet-0.1.0.tar` & `stac_geoparquet-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1081 2022-06-01 20:43:53.928454 stac_geoparquet-0.1.0/LICENSE
--rw-r--r--   0        0        0     1810 2022-06-17 20:38:48.534415 stac_geoparquet-0.1.0/README.md
--rw-r--r--   0        0        0     1203 2022-06-22 16:55:13.955679 stac_geoparquet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      137 2022-06-22 16:55:19.625678 stac_geoparquet-0.1.0/stac_geoparquet/__init__.py
--rw-r--r--   0        0        0     1527 2022-06-07 13:53:09.055314 stac_geoparquet-0.1.0/stac_geoparquet/cli.py
--rw-r--r--   0        0        0     3561 2022-06-22 14:38:36.402661 stac_geoparquet-0.1.0/stac_geoparquet/pc_runner.py
--rw-r--r--   0        0        0     9778 2022-06-22 16:53:19.879653 stac_geoparquet-0.1.0/stac_geoparquet/pgstac_reader.py
--rw-r--r--   0        0        0     3142 2022-06-22 16:52:35.425259 stac_geoparquet-0.1.0/stac_geoparquet/stac_geoparquet.py
--rw-r--r--   0        0        0     2480 2022-06-22 16:47:37.510332 stac_geoparquet-0.1.0/stac_geoparquet/utils.py
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 stac_geoparquet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1810 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/README.md
+-rw-r--r--   0        0        0     1275 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/_compat.py
+-rw-r--r--   0        0        0     3823 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/cli.py
+-rw-r--r--   0        0        0     4455 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/pc_runner.py
+-rw-r--r--   0        0        0    12037 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/pgstac_reader.py
+-rw-r--r--   0        0        0     3799 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/stac_geoparquet.py
+-rw-r--r--   0        0        0     2480 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/utils.py
+-rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 stac_geoparquet-0.2.0/PKG-INFO
```

### Comparing `stac_geoparquet-0.1.0/LICENSE` & `stac_geoparquet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.1.0/README.md` & `stac_geoparquet-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.1.0/pyproject.toml` & `stac_geoparquet-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
     "pystac",
     "geopandas",
     "pandas",
     "pyarrow",
-    "shapely"
+    "shapely",
+    "packaging",
 ]
 
 [project.optional-dependencies]
 pgstac = [
+    "fsspec",
     "pypgstac",
     "psycopg[binary,pool]",
     "tqdm",
     "python-dateutil",
 ]
 pc = [
     "adlfs",
@@ -49,19 +51,22 @@
 minversion = "6.0"
 filterwarnings = [
     "ignore:.*distutils Version.*:DeprecationWarning",
 ]
 
 [tool.mypy]
 
+python_version = "3.10"
+
 [[tool.mypy.overrides]]
 module = [
     "shapely.*",
     "geopandas.*",
     "pandas.*",
     "fsspec.*",
     "tqdm.*",
     "pypgstac.*",
-    "pyarrow.*"
+    "pyarrow.*",
+    "rich.*",
 ]
 
 ignore_missing_imports = true
```

### Comparing `stac_geoparquet-0.1.0/stac_geoparquet/pgstac_reader.py` & `stac_geoparquet-0.2.0/stac_geoparquet/pgstac_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import textwrap
+import hashlib
 
 import datetime
 import logging
 from typing import Any
 import collections.abc
 import itertools
 
@@ -12,15 +13,15 @@
 import pystac
 import dateutil.tz
 import dataclasses
 import pyarrow.fs
 import pypgstac.db
 import pypgstac.hydration
 import shapely.wkb
-import tqdm
+import tqdm.auto
 from stac_geoparquet import to_geodataframe
 
 
 logger = logging.getLogger(__name__)
 
 
 def _pairwise(
@@ -116,14 +117,24 @@
 
         if end_datetime and end_datetime.tzinfo == dateutil.tz.tz.tzlocal():
             end_datetime = end_datetime.astimezone(datetime.timezone.utc)
 
         if end_datetime is None:
             end_datetime = pd.Timestamp.utcnow()
 
+        # we need to ensure that the `end_datetime` is past the end of the last partition
+        # to avoid missing out on the last partition of data.
+        offset = pd.tseries.frequencies.to_offset(self.partition_frequency)
+
+        if not offset.is_on_offset(start_datetime):
+            start_datetime = start_datetime - offset
+
+        if not offset.is_on_offset(end_datetime):
+            end_datetime = end_datetime + offset
+
         idx = pd.date_range(start_datetime, end_datetime, freq=self.partition_frequency)
 
         if since:
             idx = idx[idx >= since]
 
         pairs = _pairwise(idx)
         return list(pairs)
@@ -142,30 +153,72 @@
         az_fs = fsspec.filesystem(output_protocol, **storage_options)
         if az_fs.exists(output_path) and not rewrite:
             logger.debug("Path %s already exists.", output_path)
             return output_path
 
         db = pypgstac.db.PgstacDB(conninfo)
         with db:
+            db.connection.execute("set statement_timeout = 300000;")
             # logger.debug("Reading base item")
             # TODO: proper escaping
             base_item = db.query_one(
                 f"select * from collection_base_item('{self.collection_id}');"
             )
             records = list(db.query(query))
 
         if skip_empty_partitions and len(records) == 0:
+            logger.debug("No records found for query %s.", query)
             return None
 
         items = self.make_pgstac_items(records, base_item)
         df = to_geodataframe(items)
         filesystem = pyarrow.fs.PyFileSystem(pyarrow.fs.FSSpecHandler(az_fs))
         df.to_parquet(output_path, index=False, filesystem=filesystem)
         return output_path
 
+    def export_partition_for_endpoints(
+        self,
+        endpoints: tuple[datetime.datetime, datetime.datetime],
+        conninfo: str,
+        output_protocol: str,
+        output_path: str,
+        storage_options: dict[str, Any],
+        part_number: int | None = None,
+        total: int | None = None,
+        rewrite=False,
+        skip_empty_partitions=False,
+    ) -> str | None:
+        """
+        Export results for a pair of endpoints.
+        """
+        a, b = endpoints
+        base_query = textwrap.dedent(
+            f"""\
+        select *
+        from pgstac.items
+        where collection = '{self.collection_id}'
+        """
+        )
+
+        query = (
+            base_query
+            + f"and datetime >= '{a.isoformat()}' and datetime < '{b.isoformat()}'"
+        )
+
+        partition_path = _build_output_path(output_path, part_number, total, a, b)
+        return self.export_partition(
+            conninfo,
+            query,
+            output_protocol=output_protocol,
+            output_path=partition_path,
+            storage_options=storage_options,
+            rewrite=rewrite,
+            skip_empty_partitions=skip_empty_partitions,
+        )
+
     def export_collection(
         self,
         conninfo: str,
         output_protocol: str,
         output_path: str,
         storage_options: dict[str, Any],
         rewrite=False,
@@ -193,40 +246,32 @@
                     storage_options=storage_options,
                     rewrite=rewrite,
                 )
             ]
 
         else:
             endpoints = self.generate_endpoints()
-            extra_wheres = [
-                f"and datetime >= '{a.isoformat()}' and datetime < '{b.isoformat()}'"
-                for a, b in endpoints
-            ]
-            queries = [base_query + where for where in extra_wheres]
-            N = len(endpoints)
-            output_paths = [
-                f"{output_path}/part-{i:0{len(str(N + 1))}}_{a.isoformat()}_{b.isoformat()}.parquet"
-                for i, (a, b) in enumerate(endpoints)
-            ]
-
+            total = len(endpoints)
             logger.info(
-                "Exporting %d partitions for collection %s", N, self.collection_id
+                "Exporting %d partitions for collection %s", total, self.collection_id
             )
 
             results = []
-            for (query, part_path) in tqdm.tqdm(zip(queries, output_paths), total=N):
+            for i, endpoint in tqdm.auto.tqdm(enumerate(endpoints), total=total):
                 results.append(
-                    self.export_partition(
-                        conninfo,
-                        query,
-                        output_protocol,
-                        part_path,
+                    self.export_partition_for_endpoints(
+                        endpoints=endpoint,
+                        conninfo=conninfo,
+                        output_protocol=output_protocol,
+                        output_path=output_path,
                         storage_options=storage_options,
                         rewrite=rewrite,
                         skip_empty_partitions=skip_empty_partitions,
+                        part_number=i,
+                        total=total,
                     )
                 )
 
         return results
 
     def make_pgstac_items(
         self,
@@ -284,7 +329,32 @@
             if self.should_inject_dynamic_properties:
                 self.inject_links(item)
                 self.inject_assets(item)
 
             items.append(item)
 
         return items
+
+
+def _build_output_path(
+    base_output_path: str,
+    part_number: int | None,
+    total: int | None,
+    start_datetime: datetime.datetime,
+    end_datetime: datetime.datetime,
+) -> str:
+    a, b = start_datetime, end_datetime
+    base_output_path = base_output_path.rstrip("/")
+
+    if part_number is not None and total is not None:
+        output_path = (
+            f"{base_output_path}/part-{part_number:0{len(str(total * 10))}}_"
+            f"{a.isoformat()}_{b.isoformat()}.parquet"
+        )
+    else:
+        token = hashlib.md5(
+            "".join([a.isoformat(), b.isoformat()]).encode()
+        ).hexdigest()
+        output_path = (
+            f"{base_output_path}/part-{token}_{a.isoformat()}_{b.isoformat()}.parquet"
+        )
+    return output_path
```

### Comparing `stac_geoparquet-0.1.0/stac_geoparquet/stac_geoparquet.py` & `stac_geoparquet-0.2.0/stac_geoparquet/stac_geoparquet.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,30 @@
 from __future__ import annotations
 
 from typing import Sequence, Any
 
 import pystac
 import geopandas
 import pandas as pd
+import numpy as np
 import shapely.geometry
 
 from stac_geoparquet.utils import fix_empty_multipolygon
 
 
+def _fix_array(v):
+    if isinstance(v, np.ndarray):
+        v = v.tolist()
+
+    elif isinstance(v, dict):
+        v = {k: _fix_array(v2) for k, v2 in v.items()}
+
+    return v
+
+
 def to_geodataframe(items: Sequence[dict[str, Any]]) -> geopandas.GeoDataFrame:
     """
     Convert a sequence of STAC items to a :class:`geopandas.GeoDataFrame`.
 
     The objects under `properties` are moved up to the top-level of the
     DataFrame, similar to :meth:`geopandas.GeoDataFrame.from_features`.
 
@@ -90,32 +101,46 @@
         "links",
         "assets",
         "collection",
         "stac_extensions",
     }
     item = {}
     for k, v in record.items():
+        v = _fix_array(v)
 
         if k in top_level_keys:
             item[k] = v
         else:
             properties[k] = v
 
     item["geometry"] = shapely.geometry.mapping(item["geometry"])
     item["properties"] = properties
 
     return item
 
 
 def to_item_collection(df: geopandas.GeoDataFrame) -> pystac.ItemCollection:
+    """
+    Convert a GeoDataFrame of STAC items to an :class:`pystac.ItemCollection`.
+
+    Parameters
+    ----------
+    df : geopandas.GeoDataFrame
+        A GeoDataFrame with a schema similar to that exported by stac-geoparquet.
+
+    Returns
+    -------
+    item_collection : pystac.ItemCollection
+        The converted ItemCollection. There will be one record / feature per
+        row in the in the GeoDataFrame.
+    """
     df2 = df.copy()
     datelike = df2.select_dtypes(
         include=["datetime64[ns, UTC]", "datetime64[ns]"]
     ).columns
     for k in datelike:
         df2[k] = (
             df2[k].dt.strftime("%Y-%m-%dT%H:%M:%S.%fZ").fillna("").replace({"": None})
         )
 
-    return pystac.ItemCollection(
-        [to_dict(record) for record in df2.to_dict(orient="records")]
-    )
+    records = [to_dict(record) for record in df2.to_dict(orient="records")]
+    return pystac.ItemCollection(records)
```

### Comparing `stac_geoparquet-0.1.0/stac_geoparquet/utils.py` & `stac_geoparquet-0.2.0/stac_geoparquet/utils.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.1.0/PKG-INFO` & `stac_geoparquet-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: stac_geoparquet
-Version: 0.1.0
+Version: 0.2.0
 Summary: stac-geoparquet
 Author-email: Tom Augspurger <taugspurger@microsoft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pystac
 Requires-Dist: geopandas
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: shapely
+Requires-Dist: packaging
 Requires-Dist: adlfs ; extra == "pc"
 Requires-Dist: pypgstac ; extra == "pc"
 Requires-Dist: psycopg[binary,pool] ; extra == "pc"
 Requires-Dist: tqdm ; extra == "pc"
 Requires-Dist: azure-data-tables ; extra == "pc"
+Requires-Dist: fsspec ; extra == "pgstac"
 Requires-Dist: pypgstac ; extra == "pgstac"
 Requires-Dist: psycopg[binary,pool] ; extra == "pgstac"
 Requires-Dist: tqdm ; extra == "pgstac"
 Requires-Dist: python-dateutil ; extra == "pgstac"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: requests ; extra == "test"
 Requires-Dist: pre-commit ; extra == "test"
```

