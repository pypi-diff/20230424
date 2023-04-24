# Comparing `tmp/target_mssql-0.1.0.tar.gz` & `tmp/target_mssql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_mssql-0.1.0.tar", max compression
+gzip compressed data, was "target_mssql-0.1.2.tar", max compression
```

## Comparing `target_mssql-0.1.0.tar` & `target_mssql-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0      850 2023-03-09 14:24:19.976304 target_mssql-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/__init__.py
--rw-r--r--   0        0        0    14714 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/connector.py
--rw-r--r--   0        0        0    10780 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/sinks.py
--rw-r--r--   0        0        0     1390 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/target.py
--rw-r--r--   0        0        0       35 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/__init__.py
--rw-r--r--   0        0        0      667 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/array_data.singer
--rw-r--r--   0        0        0      426 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/camelcase.singer
--rw-r--r--   0        0        0     1861 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/camelcase_complex_schema.singer
--rw-r--r--   0        0        0      516 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/column_comments.singer
--rw-r--r--   0        0        0     1227 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/disappearing_columns.singer
--rw-r--r--   0        0        0      721 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/duplicate_records.singer
--rw-r--r--   0        0        0     4319 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/encoded_strings.singer
--rw-r--r--   0        0        0      445 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/insert_merge_part1.singer
--rw-r--r--   0        0        0      433 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/insert_merge_part2.singer
--rw-r--r--   0        0        0      103 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/invalid_schema.singer
--rw-r--r--   0        0        0      362 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/large_int.singer
--rw-r--r--   0        0        0      440 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/long_string.singer
--rw-r--r--   0        0        0      607 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/missing_value.singer
--rw-r--r--   0        0        0     2128 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/multiple_state_messages.singer
--rw-r--r--   0        0        0      449 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/no_primary_keys.singer
--rw-r--r--   0        0        0      610 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/no_primary_keys_append.singer
--rw-r--r--   0        0        0      392 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/null_key.singer
--rw-r--r--   0        0        0      640 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/optional_attributes.singer
--rw-r--r--   0        0        0      378 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/record_before_schema.singer
--rw-r--r--   0        0        0      287 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/record_missing_key_property.singer
--rw-r--r--   0        0        0      313 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/record_missing_required_property.singer
--rw-r--r--   0        0        0      838 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/schema_no_properties.singer
--rw-r--r--   0        0        0     1814 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/schema_updates.singer
--rw-r--r--   0        0        0     1333 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/simple_continents.singer
--rw-r--r--   0        0        0     5549 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/simple_countries.singer
--rw-r--r--   0        0        0      427 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/simple_stream.singer
--rw-r--r--   0        0        0      559 2023-03-09 14:24:19.976304 target_mssql-0.1.0/target_mssql/tests/data_files/special_chars_in_attributes.singer
--rw-r--r--   0        0        0  1859439 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/data_files/tap_aapl.singer
--rw-r--r--   0        0        0    97655 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/data_files/tap_countries.singer
--rw-r--r--   0        0        0      480 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/data_files/target_schema.singer
--rw-r--r--   0        0        0     1991 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/data_files/user_location_data.singer
--rw-r--r--   0        0        0     2322 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/data_files/user_location_upsert_data.singer
--rw-r--r--   0        0        0       15 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/samples/__init__.py
--rw-r--r--   0        0        0   763998 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/samples/aapl/AAPL.json
--rw-r--r--   0        0        0       26 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/samples/aapl/__init__.py
--rw-r--r--   0        0        0      129 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/samples/aapl/__main__.py
--rw-r--r--   0        0        0      654 2023-03-09 14:24:19.984304 target_mssql-0.1.0/target_mssql/tests/samples/aapl/aapl.py
--rw-r--r--   0        0        0  1492450 2023-03-09 14:24:19.988304 target_mssql-0.1.0/target_mssql/tests/samples/aapl/fundamentals.json
--rw-r--r--   0        0        0       28 2023-03-09 14:24:19.988304 target_mssql-0.1.0/target_mssql/tests/samples/sample_tap_countries/__init__.py
--rw-r--r--   0        0        0     2215 2023-03-09 14:24:19.988304 target_mssql-0.1.0/target_mssql/tests/samples/sample_tap_countries/countries_streams.py
--rw-r--r--   0        0        0      812 2023-03-09 14:24:19.988304 target_mssql-0.1.0/target_mssql/tests/samples/sample_tap_countries/countries_tap.py
--rw-r--r--   0        0        0      146 2023-03-09 14:24:19.988304 target_mssql-0.1.0/target_mssql/tests/samples/sample_tap_countries/schemas/continents.json
--rw-r--r--   0        0        0     7316 2023-03-09 14:24:19.988304 target_mssql-0.1.0/target_mssql/tests/test_core.py
--rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 target_mssql-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 06:53:50.732862 target_mssql-0.1.2/LICENSE
+-rw-r--r--   0        0        0      850 2023-04-24 06:53:50.732862 target_mssql-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/__init__.py
+-rw-r--r--   0        0        0    14800 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/connector.py
+-rw-r--r--   0        0        0    11284 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/sinks.py
+-rw-r--r--   0        0        0     1507 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/target.py
+-rw-r--r--   0        0        0       35 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/array_data.singer
+-rw-r--r--   0        0        0      426 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/camelcase.singer
+-rw-r--r--   0        0        0     1861 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/camelcase_complex_schema.singer
+-rw-r--r--   0        0        0      516 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/column_comments.singer
+-rw-r--r--   0        0        0     1227 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/disappearing_columns.singer
+-rw-r--r--   0        0        0      721 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/duplicate_records.singer
+-rw-r--r--   0        0        0     4319 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/encoded_strings.singer
+-rw-r--r--   0        0        0      445 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/insert_merge_part1.singer
+-rw-r--r--   0        0        0      433 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/insert_merge_part2.singer
+-rw-r--r--   0        0        0      103 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/invalid_schema.singer
+-rw-r--r--   0        0        0      362 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/large_int.singer
+-rw-r--r--   0        0        0      440 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/long_string.singer
+-rw-r--r--   0        0        0      607 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/missing_value.singer
+-rw-r--r--   0        0        0     2128 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/multiple_state_messages.singer
+-rw-r--r--   0        0        0      449 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/no_primary_keys.singer
+-rw-r--r--   0        0        0      610 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/no_primary_keys_append.singer
+-rw-r--r--   0        0        0      392 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/null_key.singer
+-rw-r--r--   0        0        0      640 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/optional_attributes.singer
+-rw-r--r--   0        0        0      378 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/record_before_schema.singer
+-rw-r--r--   0        0        0      287 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/record_missing_key_property.singer
+-rw-r--r--   0        0        0      313 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/record_missing_required_property.singer
+-rw-r--r--   0        0        0      838 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/schema_no_properties.singer
+-rw-r--r--   0        0        0     1814 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/schema_updates.singer
+-rw-r--r--   0        0        0     1333 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/simple_continents.singer
+-rw-r--r--   0        0        0     5549 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/simple_countries.singer
+-rw-r--r--   0        0        0      427 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/simple_stream.singer
+-rw-r--r--   0        0        0      559 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/special_chars_in_attributes.singer
+-rw-r--r--   0        0        0  1859439 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/tap_aapl.singer
+-rw-r--r--   0        0        0    97655 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/tap_countries.singer
+-rw-r--r--   0        0        0      480 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/target_schema.singer
+-rw-r--r--   0        0        0     1991 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/user_location_data.singer
+-rw-r--r--   0        0        0     2322 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/user_location_upsert_data.singer
+-rw-r--r--   0        0        0       15 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/samples/__init__.py
+-rw-r--r--   0        0        0   763998 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/AAPL.json
+-rw-r--r--   0        0        0       26 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/__init__.py
+-rw-r--r--   0        0        0      129 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/__main__.py
+-rw-r--r--   0        0        0      654 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/aapl.py
+-rw-r--r--   0        0        0  1492450 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/aapl/fundamentals.json
+-rw-r--r--   0        0        0       28 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/__init__.py
+-rw-r--r--   0        0        0     2215 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_streams.py
+-rw-r--r--   0        0        0      812 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_tap.py
+-rw-r--r--   0        0        0      146 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/schemas/continents.json
+-rw-r--r--   0        0        0     7860 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/test_core.py
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 target_mssql-0.1.2/PKG-INFO
```

### Comparing `target_mssql-0.1.0/pyproject.toml` & `target_mssql-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-mssql"
-version = "0.1.0"
+version = "0.1.2"
 description = "`target-mssql` is a Singer target for mssql, built with the Meltano SDK for Singer Targets."
 authors = ["Henning Holgersen"]
 keywords = [
     "ELT",
     "mssql",
 ]
 license = "Apache 2.0"
```

### Comparing `target_mssql-0.1.0/target_mssql/connector.py` & `target_mssql-0.1.2/target_mssql/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     def get_sqlalchemy_url(self, config: dict) -> str:
         """Generates a SQLAlchemy URL for mssql.
 
         Args:
             config: The configuration for the connector.
         """
 
+        if config.get("sqlalchemy_url"):
+            return config["sqlalchemy_url"]
+
         connection_url = sqlalchemy.engine.url.URL.create(
             drivername="mssql+pymssql",
             username=config["username"],
             password=config["password"],
             host=config["host"],
             port=config["port"],
             database=config["database"],
```

### Comparing `target_mssql-0.1.0/target_mssql/sinks.py` & `target_mssql-0.1.2/target_mssql/sinks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 """mssql target sink class, which handles writing streams."""
 
 from __future__ import annotations
 
 import json
 import re
-from typing import Any, Dict, Iterable, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional
 
 import sqlalchemy
 from singer_sdk.helpers._conformers import replace_leading_digit
-from singer_sdk.sinks import SQLSink
+from singer_sdk.sinks import SQLConnector, SQLSink
 from sqlalchemy import Column
 
 from target_mssql.connector import mssqlConnector
 
+if TYPE_CHECKING:
+    from singer_sdk.plugin_base import PluginBase
+
 
 class mssqlSink(SQLSink):
     """mssql target sink class."""
 
     connector_class = mssqlConnector
 
+    def __init__(
+        self,
+        target: PluginBase,
+        stream_name: str,
+        schema: dict,
+        key_properties: list[str] | None,
+        connector: SQLConnector | None = None,
+    ) -> None:
+        super().__init__(target, stream_name, schema, key_properties)
+        if self._config.get("table_prefix"):
+            self.stream_name = self._config.get("table_prefix") + stream_name
+
     # Copied purely to help with type hints
     @property
     def connector(self) -> mssqlConnector:
         """The connector object.
         Returns:
             The connector object.
         """
```

### Comparing `target_mssql-0.1.0/target_mssql/target.py` & `target_mssql-0.1.2/target_mssql/target.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,14 +45,17 @@
             description="SQL Server database",
         ),
         th.Property(
             "default_target_schema",
             th.StringType,
             description="Default target schema to write to",
         ),
+        th.Property(
+            "table_prefix", th.StringType, description="Prefix to add to table name"
+        ),
     ).to_dict()
 
     default_sink_class = mssqlSink
 
 
 if __name__ == "__main__":
     Targetmssql.cli()
```

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/array_data.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/array_data.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/camelcase_complex_schema.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/camelcase_complex_schema.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/column_comments.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/column_comments.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/disappearing_columns.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/disappearing_columns.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/duplicate_records.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/duplicate_records.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/encoded_strings.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/encoded_strings.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/missing_value.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/missing_value.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/multiple_state_messages.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/multiple_state_messages.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/no_primary_keys_append.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/no_primary_keys_append.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/optional_attributes.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/optional_attributes.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/schema_no_properties.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/schema_no_properties.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/schema_updates.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/schema_updates.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/simple_continents.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/simple_continents.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/simple_countries.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/simple_countries.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/special_chars_in_attributes.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/special_chars_in_attributes.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/tap_aapl.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/tap_aapl.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/tap_countries.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/tap_countries.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/user_location_data.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/user_location_data.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/data_files/user_location_upsert_data.singer` & `target_mssql-0.1.2/target_mssql/tests/data_files/user_location_upsert_data.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/samples/aapl/AAPL.json` & `target_mssql-0.1.2/target_mssql/tests/samples/aapl/AAPL.json`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/samples/aapl/aapl.py` & `target_mssql-0.1.2/target_mssql/tests/samples/aapl/aapl.py`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/samples/aapl/fundamentals.json` & `target_mssql-0.1.2/target_mssql/tests/samples/aapl/fundamentals.json`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/samples/sample_tap_countries/countries_streams.py` & `target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_streams.py`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/samples/sample_tap_countries/countries_tap.py` & `target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_tap.py`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.0/target_mssql/tests/test_core.py` & `target_mssql-0.1.2/target_mssql/tests/test_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Attempt at making some standard Target Tests. """
 # flake8: noqa
 import io
 from contextlib import redirect_stdout
 from pathlib import Path
+from urllib.parse import quote
 
 import pytest
 from singer_sdk.testing import sync_end_to_end
 
 from target_mssql.target import Targetmssql
 from target_mssql.tests.samples.aapl.aapl import Fundamentals
 from target_mssql.tests.samples.sample_tap_countries.countries_tap import (
@@ -20,22 +21,41 @@
         # "sqlalchemy_url": "mssql+pymssql://sa:p@55w0rd@localhost:1433/master",
         "schema": "dbo",
         "username": "sa",
         "password": "P@55w0rd",
         "host": "localhost",
         "port": "1433",
         "database": "master",
+        "table_prefix": "prfx_",
+    }
+
+
+@pytest.fixture()
+def mssql_dualconfig():
+    return {
+        "sqlalchemy_url": f"mssql+pymssql://sa:P%4055w0rd@localhost:1433/master",
+        "schema": "dbo",
+        "username": "sa",
+        "password": "wrong_password",
+        "host": "localhost",
+        "port": "1433",
+        "database": "master",
     }
 
 
 @pytest.fixture
 def mssql_target(mssql_config) -> Targetmssql:
     return Targetmssql(config=mssql_config)
 
 
+@pytest.fixture
+def mssql_dualtarget(mssql_dualconfig) -> Targetmssql:
+    return Targetmssql(config=mssql_dualconfig)
+
+
 def singer_file_to_target(file_name, target) -> None:
     """Singer file to Target, emulates a tap run
     Equivalent to running cat file_path | target-name --config config.json.
     Note that this function loads all lines into memory, so it is
     not good very large files.
     Args:
         file_name: name to file in .tests/data_files to be sent into target
@@ -199,17 +219,17 @@
 
 
 def test_db_schema(mssql_target):
     file_name = "target_schema.singer"
     singer_file_to_target(file_name, mssql_target)
 
 
-def test_simple_stream(mssql_target):
+def test_dual_target_config(mssql_dualtarget):
     file_name = "simple_stream.singer"
-    singer_file_to_target(file_name, mssql_target)
+    singer_file_to_target(file_name, mssql_dualtarget)
 
 
 def test_null_key(mssql_target):
     file_name = "null_key.singer"
     singer_file_to_target(file_name, mssql_target)
 
 
@@ -226,12 +246,13 @@
 
 def test_disappearing_columns(mssql_target):
     file_name = "disappearing_columns.singer"
     singer_file_to_target(file_name, mssql_target)
 
 
 def test_insert_merge(mssql_target):
+    print(dir(mssql_target))
     file_name = "insert_merge_part1.singer"
     singer_file_to_target(file_name, mssql_target)
 
     file_name = "insert_merge_part2.singer"
     singer_file_to_target(file_name, mssql_target)
```

### Comparing `target_mssql-0.1.0/PKG-INFO` & `target_mssql-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-mssql
-Version: 0.1.0
+Version: 0.1.2
 Summary: `target-mssql` is a Singer target for mssql, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,mssql
 Author: Henning Holgersen
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

