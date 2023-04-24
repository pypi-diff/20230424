# Comparing `tmp/trailwatch-0.3.3.tar.gz` & `tmp/trailwatch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailwatch-0.3.3.tar", max compression
+gzip compressed data, was "trailwatch-1.0.0.tar", max compression
```

## Comparing `trailwatch-0.3.3.tar` & `trailwatch-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-04-21 22:06:02.373101 trailwatch-0.3.3/LICENSE
--rw-r--r--   0        0        0     7527 2023-04-21 22:06:02.373101 trailwatch-0.3.3/README.md
--rw-r--r--   0        0        0     2026 2023-04-21 22:06:02.373101 trailwatch-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3305 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/__init__.py
--rw-r--r--   0        0        0     6071 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/config.py
--rw-r--r--   0        0        0        0 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/__init__.py
--rw-r--r--   0        0        0       85 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/aws/__init__.py
--rw-r--r--   0        0        0     8308 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/aws/api.py
--rw-r--r--   0        0        0     3912 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/aws/connector.py
--rw-r--r--   0        0        0      809 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/aws/handler.py
--rw-r--r--   0        0        0     1081 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/base.py
--rw-r--r--   0        0        0      306 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/salesforce/__init__.py
--rw-r--r--   0        0        0     6461 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/connectors/salesforce/connector.py
--rw-r--r--   0        0        0     7103 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/context.py
--rw-r--r--   0        0        0      414 2023-04-21 22:06:02.373101 trailwatch-0.3.3/src/trailwatch/exceptions.py
--rw-r--r--   0        0        0     8253 1970-01-01 00:00:00.000000 trailwatch-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 17:30:25.166837 trailwatch-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7527 2023-04-24 17:30:25.170837 trailwatch-1.0.0/README.md
+-rw-r--r--   0        0        0     2026 2023-04-24 17:30:25.170837 trailwatch-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3305 2023-04-24 17:30:25.170837 trailwatch-1.0.0/src/trailwatch/__init__.py
+-rw-r--r--   0        0        0     6071 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/config.py
+-rw-r--r--   0        0        0        0 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/aws/__init__.py
+-rw-r--r--   0        0        0     8308 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/aws/api.py
+-rw-r--r--   0        0        0     3912 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/aws/connector.py
+-rw-r--r--   0        0        0      809 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/aws/handler.py
+-rw-r--r--   0        0        0     1081 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/base.py
+-rw-r--r--   0        0        0      306 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/salesforce/__init__.py
+-rw-r--r--   0        0        0     6461 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/connectors/salesforce/connector.py
+-rw-r--r--   0        0        0     8866 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/context.py
+-rw-r--r--   0        0        0      414 2023-04-24 17:30:25.174837 trailwatch-1.0.0/src/trailwatch/exceptions.py
+-rw-r--r--   0        0        0     8253 1970-01-01 00:00:00.000000 trailwatch-1.0.0/PKG-INFO
```

### Comparing `trailwatch-0.3.3/LICENSE` & `trailwatch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/README.md` & `trailwatch-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/pyproject.toml` & `trailwatch-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trailwatch"
-version = "0.3.3"
+version = "1.0.0"
 description = "Python SDK for TrailWatch by Kicksaw"
 license = "Apache-2.0"
 authors = ["George Bocharov <george@kicksaw.com>"]
 readme = "README.md"
 homepage = "https://www.kicksaw.com/"
 repository = "https://github.com/Kicksaw-Consulting/trailwatch-python-sdk"
 packages = [
```

### Comparing `trailwatch-0.3.3/src/trailwatch/__init__.py` & `trailwatch-1.0.0/src/trailwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/src/trailwatch/config.py` & `trailwatch-1.0.0/src/trailwatch/config.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/src/trailwatch/connectors/aws/api.py` & `trailwatch-1.0.0/src/trailwatch/connectors/aws/api.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/src/trailwatch/connectors/aws/connector.py` & `trailwatch-1.0.0/src/trailwatch/connectors/aws/connector.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/src/trailwatch/connectors/aws/handler.py` & `trailwatch-1.0.0/src/trailwatch/connectors/aws/handler.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/src/trailwatch/connectors/base.py` & `trailwatch-1.0.0/src/trailwatch/connectors/base.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/src/trailwatch/connectors/salesforce/connector.py` & `trailwatch-1.0.0/src/trailwatch/connectors/salesforce/connector.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.3/PKG-INFO` & `trailwatch-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailwatch
-Version: 0.3.3
+Version: 1.0.0
 Summary: Python SDK for TrailWatch by Kicksaw
 Home-page: https://www.kicksaw.com/
 License: Apache-2.0
 Author: George Bocharov
 Author-email: george@kicksaw.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

