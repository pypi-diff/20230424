# Comparing `tmp/tap_jotform-0.0.5b1.tar.gz` & `tmp/tap_jotform-0.0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_jotform-0.0.5b1.tar", max compression
+gzip compressed data, was "tap_jotform-0.0.6b1.tar", max compression
```

## Comparing `tap_jotform-0.0.5b1.tar` & `tap_jotform-0.0.6b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2023-04-11 04:26:25.288194 tap_jotform-0.0.5b1/LICENSE
--rw-r--r--   0        0        0     3508 2023-04-11 04:26:25.288194 tap_jotform-0.0.5b1/README.md
--rw-r--r--   0        0        0     1838 2023-04-11 04:26:46.052260 tap_jotform-0.0.5b1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/__init__.py
--rw-r--r--   0        0        0      116 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/__main__.py
--rw-r--r--   0        0        0     5305 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/client.py
--rw-r--r--   0        0        0     8419 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/streams.py
--rw-r--r--   0        0        0     2738 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/tap.py
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 tap_jotform-0.0.5b1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/LICENSE
+-rw-r--r--   0        0        0     3508 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/README.md
+-rw-r--r--   0        0        0     1838 2023-04-24 20:19:28.196800 tap_jotform-0.0.6b1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/__main__.py
+-rw-r--r--   0        0        0     5305 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/client.py
+-rw-r--r--   0        0        0     8462 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/streams.py
+-rw-r--r--   0        0        0     2738 2023-04-24 20:19:11.720788 tap_jotform-0.0.6b1/tap_jotform/tap.py
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 tap_jotform-0.0.6b1/PKG-INFO
```

### Comparing `tap_jotform-0.0.5b1/LICENSE` & `tap_jotform-0.0.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5b1/README.md` & `tap_jotform-0.0.6b1/README.md`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5b1/pyproject.toml` & `tap_jotform-0.0.6b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 88
 
 [tool.poetry]
 name = "tap-jotform"
-version = "0.0.5b1"
+version = "0.0.6b1"
 description = "Singer tap for Jotform, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-jotform"
 repository = "https://github.com/edgarrmondragon/tap-jotform"
@@ -19,15 +19,15 @@
 keywords = ["ELT", "Jotform"]
 
 [tool.poetry.dependencies]
 colorama = "==0.4.6"
 importlib-metadata = {version = "<5.0.0", python = "<3.8"}
 python = "<3.12,>=3.7.1"
 requests-cache = "==1.0.1"
-singer-sdk = "==0.23.0"
+singer-sdk = "==0.24.0"
 structlog = "==23.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [tool.poetry.scripts]
 # CLI declaration
```

### Comparing `tap_jotform-0.0.5b1/tap_jotform/client.py` & `tap_jotform-0.0.6b1/tap_jotform/client.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5b1/tap_jotform/streams.py` & `tap_jotform-0.0.6b1/tap_jotform/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         """
         return {"form_id": record["id"]}
 
 
 class QuestionsStream(JotformStream):
     """Questions stream."""
 
+    INTEGER_FIELDS = ["order"]
+
     name = "questions"
     path = "/form/{form_id}/questions"
     primary_keys = ["form_id", "qid"]
     replication_key = None
     parent_stream_type = FormsStream
 
     schema = th.PropertiesList(
@@ -149,15 +151,15 @@
         th.Property("flag", th.IntegerType),
         th.Property("notes", th.StringType),
         CREATED_AT,
         UPDATED_AT,
         th.Property(
             "status",
             th.StringType,
-            allowed_values=["ACTIVE", "OVERQUOTA"],
+            allowed_values=["ACTIVE", "OVERQUOTA", "DELETED"],
         ),
         th.Property(
             "new",
             th.IntegerType,
             description="Total number of unread submissions",
         ),
         th.Property(
```

### Comparing `tap_jotform-0.0.5b1/tap_jotform/tap.py` & `tap_jotform-0.0.6b1/tap_jotform/tap.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5b1/PKG-INFO` & `tap_jotform-0.0.6b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-jotform
-Version: 0.0.5b1
+Version: 0.0.6b1
 Summary: Singer tap for Jotform, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-jotform
 License: Apache-2.0
 Keywords: ELT,Jotform
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
 Requires-Dist: requests-cache (==1.0.1)
-Requires-Dist: singer-sdk (==0.23.0)
+Requires-Dist: singer-sdk (==0.24.0)
 Requires-Dist: structlog (==23.1.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-jotform/#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-jotform
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: tap-jotform Version: 0.0.5b1 Summary: Singer tap
+Metadata-Version: 2.1 Name: tap-jotform Version: 0.0.6b1 Summary: Singer tap
 for Jotform, built with the Meltano SDK for Singer Taps. Home-page: https://
 github.com/edgarrmondragon/tap-jotform License: Apache-2.0 Keywords:
 ELT,Jotform Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: colorama
 (==0.4.6) Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
-Requires-Dist: requests-cache (==1.0.1) Requires-Dist: singer-sdk (==0.23.0)
+Requires-Dist: requests-cache (==1.0.1) Requires-Dist: singer-sdk (==0.24.0)
 Requires-Dist: structlog (==23.1.0) Project-URL: Documentation, https://
 github.com/edgarrmondragon/tap-jotform/#readme Project-URL: Repository, https:/
 /github.com/edgarrmondragon/tap-jotform Description-Content-Type: text/markdown
                                  # tap-jotform
                        [pre-commit.ci_status] [License]
      Singer Tap for Jotform. Built with the [Meltano Singer SDK](https://
                                sdk.meltano.com).
```

