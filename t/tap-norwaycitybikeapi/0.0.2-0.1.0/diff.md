# Comparing `tmp/tap_norwaycitybikeapi-0.0.2.tar.gz` & `tmp/tap_norwaycitybikeapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_norwaycitybikeapi-0.0.2.tar", max compression
+gzip compressed data, was "tap_norwaycitybikeapi-0.1.0.tar", max compression
```

## Comparing `tap_norwaycitybikeapi-0.0.2.tar` & `tap_norwaycitybikeapi-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3229 2023-04-23 20:14:26.791096 tap_norwaycitybikeapi-0.0.2/README.md
--rw-r--r--   0        0        0     1259 2023-04-24 17:38:00.028329 tap_norwaycitybikeapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-23 20:13:17.667392 tap_norwaycitybikeapi-0.0.2/tap_norwaycitybikeapi/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-24 16:59:09.211105 tap_norwaycitybikeapi-0.0.2/tap_norwaycitybikeapi/client.py
--rw-r--r--   0        0        0     3069 2023-04-24 16:55:13.041576 tap_norwaycitybikeapi-0.0.2/tap_norwaycitybikeapi/streams.py
--rw-r--r--   0        0        0     1499 2023-04-24 16:48:06.246234 tap_norwaycitybikeapi-0.0.2/tap_norwaycitybikeapi/tap.py
--rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 tap_norwaycitybikeapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4188 2023-04-24 19:16:31.775538 tap_norwaycitybikeapi-0.1.0/README.md
+-rw-r--r--   0        0        0     1259 2023-04-24 19:16:46.351562 tap_norwaycitybikeapi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-23 20:13:17.667392 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/__init__.py
+-rw-r--r--   0        0        0     2376 2023-04-24 19:14:16.777878 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/client.py
+-rw-r--r--   0        0        0     3069 2023-04-24 16:55:13.041576 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/streams.py
+-rw-r--r--   0        0        0     1470 2023-04-24 19:15:31.550948 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/tap.py
+-rw-r--r--   0        0        0     5060 1970-01-01 00:00:00.000000 tap_norwaycitybikeapi-0.1.0/PKG-INFO
```

### Comparing `tap_norwaycitybikeapi-0.0.2/pyproject.toml` & `tap_norwaycitybikeapi-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-norwaycitybikeapi"
-version = "0.0.2"
+version = "0.1.0"
 description = "`tap-norwaycitybikeapi` is a Singer tap for NorwayCityBikeAPI, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Kristian André Jakobsen <k.andrejakobsen@gmail.com>"]
 keywords = ["ELT", "NorwayCityBikeAPI"]
 license = "Apache 2.0"
 packages = [{ include = "tap_norwaycitybikeapi" }]
```

### Comparing `tap_norwaycitybikeapi-0.0.2/tap_norwaycitybikeapi/client.py` & `tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,14 @@
                 Set dynamically based on `city_name`, which can either
                 be `bergen`, `trondheim` or `oslo`.
         """
         city_name = self.config["city_name"].lower()
         return f"https://gbfs.urbansharing.com/{city_name}bysykkel.no"
 
     records_jsonpath = "$.data.*[*]"  # Or override `parse_response`.
-    next_page_token_jsonpath = "$.next_page"  # Or override `get_next_page_token`.
 
     @property
     def http_headers(self) -> dict:
         """Return the http headers needed.
 
         Returns:
             A dictionary of HTTP headers.
@@ -71,22 +70,8 @@
 
         Args:
             response: The HTTP ``requests.Response`` object.
 
         Yields:
             Each record from the source.
         """
-        # TODO: Parse response body and return a set of records.
         yield from extract_jsonpath(self.records_jsonpath, input=response.json())
-
-    def post_process(self, row: dict, context: dict | None = None) -> dict | None:
-        """As needed, append or transform raw data to match expected structure.
-
-        Args:
-            row: An individual record from the stream.
-            context: The stream context.
-
-        Returns:
-            The updated record dictionary, or ``None`` to skip the record.
-        """
-        # TODO: Delete this method if not needed.
-        return row
```

### Comparing `tap_norwaycitybikeapi-0.0.2/tap_norwaycitybikeapi/streams.py` & `tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/streams.py`

 * *Files identical despite different names*

### Comparing `tap_norwaycitybikeapi-0.0.2/tap_norwaycitybikeapi/tap.py` & `tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/tap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 """NorwayCityBikeAPI tap class."""
 
 from __future__ import annotations
 
 from singer_sdk import Tap
 from singer_sdk import typing as th  # JSON schema typing helpers
 
-# TODO: Import your custom stream types here:
-from tap_norwaycitybikeapi import streams
+from tap_norwaycitybikeapi.streams import (
+    AvailabilityStream,
+    NorwayCityBikeAPIStream,
+    StationsStream,
+)
 
 
 class TapNorwayCityBikeAPI(Tap):
     """NorwayCityBikeAPI tap class."""
 
     name = "tap-norwaycitybikeapi"
 
     config_jsonschema = th.PropertiesList(
         th.Property(
             "client_identifier",
             th.StringType,
             required=True,
             secret=True,  # Flag config as protected.
             description=(
-                "The value should contain your company/organization name,"
-                "follwed by a dash and the application's name"
+                "The value should contain your company/organization name, "
+                "follwed by a dash and the application's name."
             ),
         ),
         th.Property(
             "city_name",
             th.StringType,
             default="oslo",
             required=True,
-            description="Name of Norwegian city having City Bikes",
-        ),
-        th.Property(
-            "start_date",
-            th.DateTimeType,
-            description="The earliest record date to sync",
+            description=(
+                "Name of Norwegian city having City Bikes. "
+                "Currently only available for Trondheim, Oslo and Bergen."
+            ),
         ),
     ).to_dict()
 
-    def discover_streams(self) -> list[streams.NorwayCityBikeAPIStream]:
+    def discover_streams(self) -> list[NorwayCityBikeAPIStream]:
         """Return a list of discovered streams.
 
         Returns:
             A list of discovered streams.
         """
         return [
-            streams.StationsStream(self),
-            streams.AvailabilityStream(self),
+            StationsStream(self),
+            AvailabilityStream(self),
         ]
 
 
 if __name__ == "__main__":
     TapNorwayCityBikeAPI.cli()
```

