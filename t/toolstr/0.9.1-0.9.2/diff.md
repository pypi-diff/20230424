# Comparing `tmp/toolstr-0.9.1.tar.gz` & `tmp/toolstr-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolstr-0.9.1.tar", last modified: Sun Jan  1 01:32:18 2023, max compression
+gzip compressed data, was "toolstr-0.9.2.tar", last modified: Mon Apr 24 06:18:02 2023, max compression
```

## Comparing `toolstr-0.9.1.tar` & `toolstr-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.1/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.1/LICENSE
--rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.1/README.md
--rw-r--r--   0        0        0      611 2022-12-12 20:01:41.098721 toolstr-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      245 2023-01-01 01:26:46.316402 toolstr-0.9.1/toolstr/__init__.py
--rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.1/toolstr/charts/README.md
--rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.1/toolstr/charts/__init__.py
--rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.1/toolstr/charts/braille_utils.py
--rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.1/toolstr/charts/char_dicts.py
--rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.1/toolstr/charts/grid_utils.py
--rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.1/toolstr/charts/line_utils.py
--rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.1/toolstr/charts/plot_utils.py
--rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.1/toolstr/charts/raster_utils.py
--rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.1/toolstr/charts/render_utils.py
--rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.1/toolstr/charts/sextant_utils.py
--rw-r--r--   0        0        0      154 2022-12-09 18:24:40.524994 toolstr-0.9.1/toolstr/formats/__init__.py
--rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.1/toolstr/formats/bullet_formats.py
--rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.1/toolstr/formats/column_formats.py
--rw-r--r--   0        0        0     7270 2022-12-25 16:31:04.625640 toolstr-0.9.1/toolstr/formats/datatype_formats.py
--rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.1/toolstr/formats/positional_formats.py
--rw-r--r--   0        0        0     2191 2022-12-09 18:24:40.526344 toolstr-0.9.1/toolstr/formats/rich_formats.py
--rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.1/toolstr/outlines/__init__.py
--rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.1/toolstr/outlines/outline_chars.py
--rw-r--r--   0        0        0     7033 2022-12-09 18:24:40.527200 toolstr-0.9.1/toolstr/outlines/outline_printing.py
--rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.1/toolstr/py.typed
--rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.1/toolstr/spec.py
--rw-r--r--   0        0        0       28 2022-12-12 20:09:48.083313 toolstr-0.9.1/toolstr/summaries/__init__.py
--rw-r--r--   0        0        0     6083 2022-12-23 16:42:27.847087 toolstr-0.9.1/toolstr/summaries/set_summary.py
--rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.1/toolstr/tables/__init__.py
--rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.1/toolstr/tables/multiline_tables.py
--rw-r--r--   0        0        0     2176 2022-12-09 18:24:40.528383 toolstr-0.9.1/toolstr/tables/table_adapters.py
--rw-r--r--   0        0        0    33325 2023-01-01 01:23:23.058551 toolstr-0.9.1/toolstr/tables/table_utils.py
--rw-r--r--   0        0        0     8721 1970-01-01 00:00:00.000000 toolstr-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.2/LICENSE
+-rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.2/README.md
+-rw-r--r--   0        0        0      611 2022-12-12 20:01:41.098721 toolstr-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      245 2023-04-24 06:17:40.740773 toolstr-0.9.2/toolstr/__init__.py
+-rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.2/toolstr/charts/README.md
+-rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.2/toolstr/charts/__init__.py
+-rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.2/toolstr/charts/braille_utils.py
+-rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.2/toolstr/charts/char_dicts.py
+-rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.2/toolstr/charts/grid_utils.py
+-rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.2/toolstr/charts/line_utils.py
+-rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.2/toolstr/charts/plot_utils.py
+-rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.2/toolstr/charts/raster_utils.py
+-rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.2/toolstr/charts/render_utils.py
+-rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.2/toolstr/charts/sextant_utils.py
+-rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.2/toolstr/formats/__init__.py
+-rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.2/toolstr/formats/bullet_formats.py
+-rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.2/toolstr/formats/column_formats.py
+-rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.2/toolstr/formats/datatype_formats.py
+-rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.2/toolstr/formats/positional_formats.py
+-rw-r--r--   0        0        0     2191 2022-12-09 18:24:40.526344 toolstr-0.9.2/toolstr/formats/rich_formats.py
+-rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.2/toolstr/formats/template_formats.py
+-rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.2/toolstr/outlines/__init__.py
+-rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.2/toolstr/outlines/outline_chars.py
+-rw-r--r--   0        0        0     7033 2022-12-09 18:24:40.527200 toolstr-0.9.2/toolstr/outlines/outline_printing.py
+-rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.2/toolstr/py.typed
+-rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.2/toolstr/spec.py
+-rw-r--r--   0        0        0       28 2022-12-12 20:09:48.083313 toolstr-0.9.2/toolstr/summaries/__init__.py
+-rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.2/toolstr/summaries/set_summary.py
+-rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.2/toolstr/tables/__init__.py
+-rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.2/toolstr/tables/multiline_tables.py
+-rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.2/toolstr/tables/table_adapters.py
+-rw-r--r--   0        0        0    33607 2023-03-22 21:23:07.773603 toolstr-0.9.2/toolstr/tables/table_utils.py
+-rw-r--r--   0        0        0     8721 1970-01-01 00:00:00.000000 toolstr-0.9.2/PKG-INFO
```

### Comparing `toolstr-0.9.1/LICENSE` & `toolstr-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/README.md` & `toolstr-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/pyproject.toml` & `toolstr-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/braille_utils.py` & `toolstr-0.9.2/toolstr/charts/braille_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/char_dicts.py` & `toolstr-0.9.2/toolstr/charts/char_dicts.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/grid_utils.py` & `toolstr-0.9.2/toolstr/charts/grid_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/line_utils.py` & `toolstr-0.9.2/toolstr/charts/line_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/plot_utils.py` & `toolstr-0.9.2/toolstr/charts/plot_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/raster_utils.py` & `toolstr-0.9.2/toolstr/charts/raster_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/render_utils.py` & `toolstr-0.9.2/toolstr/charts/render_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/charts/sextant_utils.py` & `toolstr-0.9.2/toolstr/charts/sextant_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/formats/bullet_formats.py` & `toolstr-0.9.2/toolstr/formats/bullet_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/formats/column_formats.py` & `toolstr-0.9.2/toolstr/formats/column_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/formats/datatype_formats.py` & `toolstr-0.9.2/toolstr/formats/datatype_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     import tooltime
 
 from .. import spec
 
 
 def format(
     value: typing.Any,
-    format_type: typing.Literal['number', 'timestamp'] | None = None,
+    format_type: typing.Literal['number', 'timestamp', 'nbytes'] | None = None,
     **kwargs: typing.Any,
 ) -> str:
 
     if format_type is None:
 
         if isinstance(value, bool):
             return str(value)
```

### Comparing `toolstr-0.9.1/toolstr/formats/positional_formats.py` & `toolstr-0.9.2/toolstr/formats/positional_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/formats/rich_formats.py` & `toolstr-0.9.2/toolstr/formats/rich_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/outlines/outline_chars.py` & `toolstr-0.9.2/toolstr/outlines/outline_chars.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/outlines/outline_printing.py` & `toolstr-0.9.2/toolstr/outlines/outline_printing.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/spec.py` & `toolstr-0.9.2/toolstr/spec.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/summaries/set_summary.py` & `toolstr-0.9.2/toolstr/summaries/set_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     lhs: typing.Sequence[typing.Any] | None = None,
     rhs: typing.Sequence[typing.Any] | None = None,
     *,
     lhs_name: str = 'lhs',
     rhs_name: str = 'rhs',
     verbose: int = 1,
     include_visuals: bool = True,
+    title: str | None = None,
     **kwargs: typing.Sequence[typing.Any],
 ) -> None:
     if lhs is not None and rhs is not None:
         pass
     elif kwargs is not None and len(kwargs) == 2:
         items = list(kwargs.items())
         lhs_name, lhs = items[0]
@@ -71,15 +72,18 @@
         for visual, row in zip(visuals, rows):
             row.append(visual)
 
         labels = ['', 'size', '% of ∪', 'visual']
     else:
         labels = ['', 'size', '% of ∪']
 
-    outlines.print_text_box('Overlap between sets')
+    if title is None:
+        title = 'Overlap between sets'
+    outlines.print_text_box(title)
+
     if relation != '':
         print()
         print(relation)
     print()
     tables.print_table(
         rows,
         labels=labels,
```

### Comparing `toolstr-0.9.1/toolstr/tables/multiline_tables.py` & `toolstr-0.9.2/toolstr/tables/multiline_tables.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.1/toolstr/tables/table_adapters.py` & `toolstr-0.9.2/toolstr/tables/table_adapters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,75 @@
 from __future__ import annotations
 
 import typing
 
 if typing.TYPE_CHECKING:
-    import pandas as pd
+    from typing_extensions import TypeGuard
+    import pandas as pd  # type: ignore
+    import polars as pl
 
 from . import table_utils
 
 
 def print_dataframe_as_table(
-    df: pd.DataFrame,
+    df: pl.DataFrame | pd.DataFrame,
     columns: typing.Sequence[typing.Any] | None = None,
     include_index: bool = True,
     **table_kwargs: typing.Any,
 ) -> str | None:
 
-    # promote index columns to plain columns
-    if include_index:
-        if df.index.name is not None:
-            name = df.index.name
+    if _is_polars_dataframe(df):
+        rows = df.rows()
+        columns = list(df.columns)
+
+    elif _is_pandas_dataframe(df):
+
+        # promote index columns to plain columns
+        if include_index:
+            if df.index.name is not None:
+                name = df.index.name
+            else:
+                name = 'index'
+            if columns is not None and name not in columns:
+                columns = [name] + list(columns)
+            df = df.reset_index()
+
+        # compile columns
+        if columns is not None:
+            # filter columns
+            df = df[[column for column in columns]]
         else:
-            name = 'index'
-        if columns is not None and name not in columns:
-            columns = [name] + list(columns)
-        df = df.reset_index()
-
-    # compile columns
-    if columns is not None:
-        # filter columns
-        df = df[[column for column in columns]]
-    else:
-        # use all columns
-        columns = list(df.columns.values)
+            # use all columns
+            columns = list(df.columns.values)
+
+        # convert to list of lists
+        rows = df.values.tolist()
 
-    # convert to list of lists
-    rows = df.values.tolist()
+    else:
+        raise Exception('unknown dataframe type: ' + str(type(df)))
 
     return table_utils.print_table(rows=rows, labels=columns, **table_kwargs)
 
 
+def _is_polars_dataframe(df: typing.Any) -> TypeGuard[pl.DataFrame]:
+    for parent in type(df).__mro__:
+        if parent.__module__.startswith('polars'):
+            return True
+    else:
+        return False
+
+
+def _is_pandas_dataframe(df: typing.Any) -> TypeGuard[pd.DataFrame]:
+    for parent in type(df).__mro__:
+        if parent.__module__.startswith('pandas'):
+            return True
+    else:
+        return False
+
+
 def print_dict_of_lists_as_table(
     dict_of_lists: typing.Mapping[typing.Any, typing.Sequence[typing.Any]],
     keys: typing.Sequence[typing.Any] | None = None,
     **table_kwargs: typing.Any,
 ) -> str | None:
 
     # determine keys
@@ -76,7 +103,8 @@
     for item in list_of_dicts:
         row = []
         for key in keys:
             row.append(item.get(key))
         rows.append(row)
 
     return table_utils.print_table(rows=rows, labels=keys, **table_kwargs)
+
```

### Comparing `toolstr-0.9.1/toolstr/tables/table_utils.py` & `toolstr-0.9.2/toolstr/tables/table_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     limit_rows_at: Literal['start', 'middle', 'end'] = 'middle',
     sort_key: typing.Callable[..., typing.Any] | None = None,
     sort_column: str
     | int
     | typing.Sequence[str]
     | typing.Sequence[int]
     | None = None,
+    descending: bool = False,
     missing_columns: typing.Literal['fill', 'clip', 'error'] = 'error',
     empty_str: str = '',
     format: FormatKwargs | None = None,
     column_formats: ColumnData[FormatKwargs] | None = None,
     return_str: bool = False,
     #
     # io
@@ -122,15 +123,15 @@
     # filter row separators
     rows, separator_indices = _filter_separator_indices(rows, separate_all_rows)
 
     # check missing columns
     rows, labels = _fix_missing_data(rows, labels, missing_columns, empty_str)
 
     # sort rows
-    rows = _sort_rows(rows, labels, sort_column, sort_key)
+    rows = _sort_rows(rows, labels, sort_column, sort_key, descending)
 
     # add row index
     rows, labels = _add_index(rows, labels, add_row_index, row_start_index)
     if limit_rows is not None and len(rows) > limit_rows:
         rows = clip_rows(rows, n=limit_rows, clip_position=limit_rows_at)
 
     # convert cells and labels to str
@@ -502,41 +503,49 @@
     labels: typing.Sequence[str] | None,
     sort_column: str
     | int
     | typing.Sequence[str]
     | typing.Sequence[int]
     | None = None,
     sort_key: typing.Callable[..., typing.Any] | None = None,
+    descending: bool = False,
 ) -> list[typing.Sequence[typing.Any]]:
 
     if sort_column is not None and sort_key is not None:
         raise Exception('should not specify both sort_key and sort_column')
     for raw_row in rows:
         if raw_row is None:
             raise Exception('cannot sort gap rows equal to None')
 
     # sort by values of particular columns
     if sort_column is not None:
         if labels is None:
             raise Exception('must specify labels when specifying sort_column')
         if isinstance(sort_column, (str, int)):
             index = _get_label_index(sort_column, labels)
-            return sorted(rows, key=lambda row: row[index])  # type: ignore
+            sorted_rows = sorted(rows, key=lambda row: row[index])  # type: ignore
         elif isinstance(sort_column, (list, tuple)):
             indices = [_get_label_index(label, labels) for label in sort_column]
-            return sorted(
+            sorted_rows = sorted(
                 rows, key=lambda row: tuple(row[i] for i in indices)
             )
         else:
             raise Exception('unknown sort_column format')
 
+        if descending:
+            sorted_rows = sorted_rows[::-1]
+        return sorted_rows
+
     if sort_key is not None:
         pairs = [(row, dict(zip(labels, row))) for row in rows]  # type: ignore
         pairs = sorted(pairs, key=sort_key(pairs[1]))
-        return [pair[0] for pair in pairs]
+        sorted_rows = [pair[0] for pair in pairs]
+        if descending:
+            sorted_rows = sorted_rows[::-1]
+        return sorted_rows
 
     return rows
 
 
 def _get_label_index(label: str | int, labels: typing.Sequence[str]) -> int:
     if isinstance(label, str):
         return labels.index(label)
```

### Comparing `toolstr-0.9.1/PKG-INFO` & `toolstr-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolstr
-Version: 0.9.1
+Version: 0.9.2
 Summary: toolstr is a suite of str processing tools, including formatting and drawing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.1.4
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: scikit-image>=0.19.2 ; extra == "full"
 Requires-Dist: rich>=12.1.0 ; extra == "full"
```

