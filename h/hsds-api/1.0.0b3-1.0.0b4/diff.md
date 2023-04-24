# Comparing `tmp/hsds_api-1.0.0b3-py3-none-any.whl.zip` & `tmp/hsds_api-1.0.0b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12424 bytes, number of entries: 6
--rw-r--r--  2.0 unx       25 b- defN 23-Mar-22 21:15 hsds_api/__init__.py
--rw-r--r--  2.0 unx   132828 b- defN 23-Mar-22 21:15 hsds_api/_hsds_api.py
--rw-r--r--  2.0 unx      736 b- defN 23-Mar-22 21:15 hsds_api-1.0.0b3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-22 21:15 hsds_api-1.0.0b3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-22 21:15 hsds_api-1.0.0b3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      463 b- defN 23-Mar-22 21:15 hsds_api-1.0.0b3.dist-info/RECORD
-6 files, 134153 bytes uncompressed, 11584 bytes compressed:  91.4%
+Zip file size: 12469 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-24 08:49 hsds_api/__init__.py
+-rw-r--r--  2.0 unx   134379 b- defN 23-Apr-24 08:49 hsds_api/_hsds_api.py
+-rw-r--r--  2.0 unx      736 b- defN 23-Apr-24 08:49 hsds_api-1.0.0b4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 08:49 hsds_api-1.0.0b4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-24 08:49 hsds_api-1.0.0b4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      463 b- defN 23-Apr-24 08:49 hsds_api-1.0.0b4.dist-info/RECORD
+6 files, 135704 bytes uncompressed, 11629 bytes compressed:  91.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: hsds_api/__init__.py
 Comment: 
 
 Filename: hsds_api/_hsds_api.py
 Comment: 
 
-Filename: hsds_api-1.0.0b3.dist-info/METADATA
+Filename: hsds_api-1.0.0b4.dist-info/METADATA
 Comment: 
 
-Filename: hsds_api-1.0.0b3.dist-info/WHEEL
+Filename: hsds_api-1.0.0b4.dist-info/WHEEL
 Comment: 
 
-Filename: hsds_api-1.0.0b3.dist-info/top_level.txt
+Filename: hsds_api-1.0.0b4.dist-info/top_level.txt
 Comment: 
 
-Filename: hsds_api-1.0.0b3.dist-info/RECORD
+Filename: hsds_api-1.0.0b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hsds_api/_hsds_api.py

```diff
@@ -1295,15 +1295,15 @@
 """
 
     value: list[object]
     """"""
 
 
 @dataclass(frozen=True)
-class PostValuesResponse:
+class PostValuesAsJsonResponse:
     """
     
 
     Args:
         value: 
     """
 
@@ -2308,15 +2308,15 @@
             __query_values["Limit"] = quote(_to_string(limit), safe="")
 
         __query: str = "?" + "&".join(f"{key}={value}" for (key, value) in __query_values.items())
         __url += __query
 
         return self.___client._invoke(GetValuesAsJsonResponse, "GET", __url, "application/json", None, None)
 
-    def post_values(self, id: str, domain: str, body: object) -> Awaitable[PostValuesResponse]:
+    def post_values_as_json(self, id: str, domain: str, body: object) -> Awaitable[PostValuesAsJsonResponse]:
         """
         Get specific data points from Dataset.
 
         Args:
             id: UUID of the Dataset.
             domain: 
         """
@@ -2327,15 +2327,36 @@
         __query_values: dict[str, str] = {}
 
         __query_values["domain"] = quote(_to_string(domain), safe="")
 
         __query: str = "?" + "&".join(f"{key}={value}" for (key, value) in __query_values.items())
         __url += __query
 
-        return self.___client._invoke(PostValuesResponse, "POST", __url, "application/json", "application/json", json.dumps(JsonEncoder.encode(body, _json_encoder_options)))
+        return self.___client._invoke(PostValuesAsJsonResponse, "POST", __url, "application/json", "application/json", json.dumps(JsonEncoder.encode(body, _json_encoder_options)))
+
+    def post_values_as_stream(self, id: str, domain: str, body: object) -> Awaitable[Response]:
+        """
+        Get specific data points from Dataset.
+
+        Args:
+            id: UUID of the Dataset.
+            domain: 
+        """
+
+        __url = "/datasets/{id}/value"
+        __url = __url.replace("{id}", quote(str(id), safe=""))
+
+        __query_values: dict[str, str] = {}
+
+        __query_values["domain"] = quote(_to_string(domain), safe="")
+
+        __query: str = "?" + "&".join(f"{key}={value}" for (key, value) in __query_values.items())
+        __url += __query
+
+        return self.___client._invoke(Response, "POST", __url, "application/octet-stream", "application/json", json.dumps(JsonEncoder.encode(body, _json_encoder_options)))
 
     def get_attributes(self, collection: str, obj_uuid: str, domain: str, limit: Optional[float] = None, marker: Optional[str] = None) -> Awaitable[GetAttributesResponse]:
         """
         List all Attributes attached to the HDF5 object `obj_uuid`.
 
         Args:
             collection: The collection of the HDF5 object (one of: `groups`, `datasets`, or `datatypes`).
@@ -3640,15 +3661,36 @@
             __query_values["Limit"] = quote(_to_string(limit), safe="")
 
         __query: str = "?" + "&".join(f"{key}={value}" for (key, value) in __query_values.items())
         __url += __query
 
         return self.___client._invoke(GetValuesAsJsonResponse, "GET", __url, "application/json", None, None)
 
-    def post_values(self, id: str, domain: str, body: object) -> PostValuesResponse:
+    def post_values_as_json(self, id: str, domain: str, body: object) -> PostValuesAsJsonResponse:
+        """
+        Get specific data points from Dataset.
+
+        Args:
+            id: UUID of the Dataset.
+            domain: 
+        """
+
+        __url = "/datasets/{id}/value"
+        __url = __url.replace("{id}", quote(str(id), safe=""))
+
+        __query_values: dict[str, str] = {}
+
+        __query_values["domain"] = quote(_to_string(domain), safe="")
+
+        __query: str = "?" + "&".join(f"{key}={value}" for (key, value) in __query_values.items())
+        __url += __query
+
+        return self.___client._invoke(PostValuesAsJsonResponse, "POST", __url, "application/json", "application/json", json.dumps(JsonEncoder.encode(body, _json_encoder_options)))
+
+    def post_values_as_stream(self, id: str, domain: str, body: object) -> Response:
         """
         Get specific data points from Dataset.
 
         Args:
             id: UUID of the Dataset.
             domain: 
         """
@@ -3659,15 +3701,15 @@
         __query_values: dict[str, str] = {}
 
         __query_values["domain"] = quote(_to_string(domain), safe="")
 
         __query: str = "?" + "&".join(f"{key}={value}" for (key, value) in __query_values.items())
         __url += __query
 
-        return self.___client._invoke(PostValuesResponse, "POST", __url, "application/json", "application/json", json.dumps(JsonEncoder.encode(body, _json_encoder_options)))
+        return self.___client._invoke(Response, "POST", __url, "application/octet-stream", "application/json", json.dumps(JsonEncoder.encode(body, _json_encoder_options)))
 
     def get_attributes(self, collection: str, obj_uuid: str, domain: str, limit: Optional[float] = None, marker: Optional[str] = None) -> GetAttributesResponse:
         """
         List all Attributes attached to the HDF5 object `obj_uuid`.
 
         Args:
             collection: The collection of the HDF5 object (one of: `groups`, `datasets`, or `datatypes`).
```

## Comparing `hsds_api-1.0.0b3.dist-info/METADATA` & `hsds_api-1.0.0b4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsds-api
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Client for the Highly Scalable Data Service (HSDS) system.
 Home-page: https://github.com/Apollo3zehn/hsds-api
 Author: https://github.com/Apollo3zehn
 License: MIT
 Project-URL: Project, https://apollo3zehn.github.io/hsds-api/
 Project-URL: Repository, https://github.com/Apollo3zehn/hsds-api
 Keywords: HDF5 Highly Scalable Data Service HSDS
```

