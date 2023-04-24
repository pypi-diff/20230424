# Comparing `tmp/cdrouter-0.9.1.tar.gz` & `tmp/cdrouter-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdrouter-0.9.1.tar", last modified: Wed Apr 19 17:46:31 2023, max compression
+gzip compressed data, was "dist/cdrouter-0.9.2.tar", last modified: Mon Apr 24 18:48:17 2023, max compression
```

## Comparing `cdrouter-0.9.1.tar` & `cdrouter-0.9.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:46:31.000000 cdrouter-0.9.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter/
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-19 17:46:30.000000 cdrouter-0.9.1/cdrouter/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13094 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/alerts.py
--rw-r--r--   0 root         (0) root         (0)     4695 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/annotations.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/attachments.py
--rw-r--r--   0 root         (0) root         (0)     4691 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/captures.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.1/cdrouter/cdr_datetime.py
--rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.1/cdrouter/cdr_error.py
--rw-r--r--   0 root         (0) root         (0)    18267 2023-04-19 17:46:00.000000 cdrouter-0.9.1/cdrouter/cdrouter.py
--rw-r--r--   0 root         (0) root         (0)    19895 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/configs.py
--rw-r--r--   0 root         (0) root         (0)    16563 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/devices.py
--rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.1/cdrouter/exports.py
--rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.1/cdrouter/filters.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/highlights.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/history.py
--rw-r--r--   0 root         (0) root         (0)     9360 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/imports.py
--rw-r--r--   0 root         (0) root         (0)    11003 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/jobs.py
--rw-r--r--   0 root         (0) root         (0)    10408 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/metrics.py
--rw-r--r--   0 root         (0) root         (0)    15834 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/packages.py
--rw-r--r--   0 root         (0) root         (0)    37996 2023-04-19 17:46:00.000000 cdrouter-0.9.1/cdrouter/results.py
--rw-r--r--   0 root         (0) root         (0)    20907 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/system.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/tags.py
--rw-r--r--   0 root         (0) root         (0)    20060 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/testresults.py
--rw-r--r--   0 root         (0) root         (0)    23930 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/testsuites.py
--rw-r--r--   0 root         (0) root         (0)     8849 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7138 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.1/README.rst
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-02 12:33:34.000000 cdrouter-0.9.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 17:46:31.000000 cdrouter-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2022 2022-11-02 12:33:34.000000 cdrouter-0.9.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     7138 2023-04-19 17:46:31.000000 cdrouter-0.9.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:48:17.000000 cdrouter-0.9.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13566 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/alerts.py
+-rw-r--r--   0 root         (0) root         (0)     4747 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/annotations.py
+-rw-r--r--   0 root         (0) root         (0)     7330 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/attachments.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/captures.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.2/cdrouter/cdr_datetime.py
+-rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.2/cdrouter/cdr_error.py
+-rw-r--r--   0 root         (0) root         (0)    18456 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/cdrouter.py
+-rw-r--r--   0 root         (0) root         (0)    20256 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/configs.py
+-rw-r--r--   0 root         (0) root         (0)    16701 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/devices.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.2/cdrouter/exports.py
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.2/cdrouter/filters.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/highlights.py
+-rw-r--r--   0 root         (0) root         (0)     3481 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/history.py
+-rw-r--r--   0 root         (0) root         (0)     9626 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/imports.py
+-rw-r--r--   0 root         (0) root         (0)    11132 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    16100 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/packages.py
+-rw-r--r--   0 root         (0) root         (0)    39213 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/results.py
+-rw-r--r--   0 root         (0) root         (0)    21568 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/system.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/tags.py
+-rw-r--r--   0 root         (0) root         (0)    20275 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/testresults.py
+-rw-r--r--   0 root         (0) root         (0)    24462 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/testsuites.py
+-rw-r--r--   0 root         (0) root         (0)     8901 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)       61 2022-11-02 12:33:34.000000 cdrouter-0.9.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-24 18:48:17.000000 cdrouter-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2022 2022-11-02 12:33:34.000000 cdrouter-0.9.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-04-24 18:48:17.000000 cdrouter-0.9.2/PKG-INFO
```

### Comparing `cdrouter-0.9.1/cdrouter/alerts.py` & `cdrouter-0.9.2/cdrouter/alerts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# Copyright (c) 2020-2022 by QA Cafe.
+# Copyright (c) 2020-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Alerts."""
 
 from collections import namedtuple
 from functools import partial
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 
 class Alert(object):
     """Model for CDRouter Alerts.
 
     :param id: (optional) Result ID as an int.
     :param idx: (optional) Alert index as an int.
@@ -97,14 +97,17 @@
     rule_set = fields.Str()
     severity = fields.Int(as_string=True)
     sid = fields.Int(as_string=True)
     signature = fields.Str()
     src_ip = fields.Str()
     src_port = fields.Int(as_string=True, load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Alert(**data)
 
 class SeverityCount(object):
     """Model for CDRouter Severity Counts.
 
@@ -118,14 +121,17 @@
         self.count = kwargs.get('count', None)
 
 class SeverityCountSchema(Schema):
     name = fields.Str()
     severity = fields.Int(as_string=True)
     count = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return SeverityCount(**data)
 
 class CategoryCount(object):
     """Model for CDRouter Category Counts.
 
@@ -139,14 +145,17 @@
         self.count = kwargs.get('count', None)
 
 class CategoryCountSchema(Schema):
     category = fields.Str()
     severity = fields.Int(as_string=True)
     count = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return CategoryCount(**data)
 
 class RuleSetCount(object):
     """Model for CDRouter RuleSet Counts.
 
@@ -157,14 +166,17 @@
         self.name = kwargs.get('name', None)
         self.count = kwargs.get('count', None)
 
 class RuleSetCountSchema(Schema):
     name = fields.Str()
     count = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return RuleSetCount(**data)
 
 class SignatureCount(object):
     """Model for CDRouter Signature Counts.
 
@@ -178,14 +190,17 @@
         self.count = kwargs.get('count', None)
 
 class SignatureCountSchema(Schema):
     signature = fields.Str()
     severity = fields.Int(as_string=True)
     count = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return SignatureCount(**data)
 
 class TestCount(object):
     """Model for CDRouter Test Counts.
 
@@ -196,14 +211,17 @@
         self.name = kwargs.get('name', None)
         self.count = kwargs.get('count', None)
 
 class TestCountSchema(Schema):
     name = fields.Str()
     count = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TestCount(**data)
 
 class AddrCount(object):
     """Model for CDRouter Addr Counts.
 
@@ -214,14 +232,17 @@
         self.addr = kwargs.get('addr', None)
         self.count = kwargs.get('count', None)
 
 class AddrCountSchema(Schema):
     addr = fields.Str()
     count = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return AddrCount(**data)
 
 class AllStats(object):
     """Model for CDRouter All Alerts Stats.
 
@@ -239,21 +260,24 @@
         self.rule_sets = kwargs.get('rule_sets', None)
         self.signatures = kwargs.get('signatures', None)
         self.tests = kwargs.get('tests', None)
         self.frequent_sources = kwargs.get('frequent_sources', None)
         self.frequent_destinations = kwargs.get('frequent_destinations', None)
 
 class AllStatsSchema(Schema):
-    severities = fields.Dict(keys=fields.Int(), values=fields.Nested(SeverityCountSchema()))
-    categories = fields.Nested(lambda: CategoryCountSchema(many=True))
-    rule_sets = fields.Nested(lambda: RuleSetCountSchema(many=True))
-    signatures = fields.Nested(lambda: SignatureCountSchema(many=True))
-    tests = fields.Nested(lambda: TestCountSchema(many=True))
-    frequent_sources = fields.Nested(lambda: AddrCountSchema(many=True))
-    frequent_destinations = fields.Nested(lambda: AddrCountSchema(many=True))
+    severities = fields.Dict(keys=fields.Int(), values=fields.Nested(SeverityCountSchema()), unknown=EXCLUDE)
+    categories = fields.Nested(lambda: CategoryCountSchema(many=True), unknown=EXCLUDE)
+    rule_sets = fields.Nested(lambda: RuleSetCountSchema(many=True), unknown=EXCLUDE)
+    signatures = fields.Nested(lambda: SignatureCountSchema(many=True), unknown=EXCLUDE)
+    tests = fields.Nested(lambda: TestCountSchema(many=True), unknown=EXCLUDE)
+    frequent_sources = fields.Nested(lambda: AddrCountSchema(many=True), unknown=EXCLUDE)
+    frequent_destinations = fields.Nested(lambda: AddrCountSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return AllStats(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/annotations.py` & `cdrouter-0.9.2/cdrouter/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Annotations."""
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 
 class Annotation(object):
     """Model for CDRouter Annotations.
 
     :param id: (optional) Result ID as an int.
     :param seq: (optional) TestResult sequence ID as an int.
     :param line: (optional) Line number in TestResult's logfile as an int.
@@ -24,14 +24,17 @@
 
 class AnnotationSchema(Schema):
     id = fields.Int(as_string=True)
     seq = fields.Int(as_string=True)
     line = fields.Int(as_string=True)
     comment = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Annotation(**data)
 
 class AnnotationsService(object):
     """Service for accessing CDRouter Annotations."""
```

### Comparing `cdrouter-0.9.1/cdrouter/attachments.py` & `cdrouter-0.9.2/cdrouter/attachments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 from collections import namedtuple
 from functools import partial
 import io
 
 from requests_toolbelt.downloadutils import stream
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 
 class Attachment(object):
     """Model for CDRouter Attachments.
 
     :param id: (optional) Attachment ID as an int.
     :param name: (optional) Name as string.
@@ -39,14 +39,17 @@
     description = fields.Str()
     created = DateTime()
     updated = DateTime()
     size = fields.Int()
     path = fields.Str()
     device_id = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Attachment(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/captures.py` & `cdrouter-0.9.2/cdrouter/captures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Captures."""
 
 import io
 
 from requests_toolbelt.downloadutils import stream
-from marshmallow import Schema, post_load
+from marshmallow import Schema, post_load, EXCLUDE
 from marshmallow import fields as mfields
 
 class Capture(object):
     """Model for CDRouter Captures.
 
     :param id: (optional) Result ID as an int.
     :param seq: (optional) TestResult sequence ID as an int.
@@ -30,14 +30,17 @@
 class CaptureSchema(Schema):
     id = mfields.Int(as_string=True)
     seq = mfields.Int(as_string=True)
     type = mfields.Str(load_default=None)
     interface = mfields.Str()
     filename = mfields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Capture(**data)
 
 class CloudShark(object):
     """Model for CDRouter CloudShark uploads.
 
@@ -45,14 +48,17 @@
     """
     def __init__(self, **kwargs):
         self.url = kwargs.get('url', None)
 
 class CloudSharkSchema(Schema):
     url = mfields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return CloudShark(**data)
 
 class CapturesService(object):
     """Service for accessing CDRouter Captures."""
```

### Comparing `cdrouter-0.9.1/cdrouter/cdr_datetime.py` & `cdrouter-0.9.2/cdrouter/cdr_datetime.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.1/cdrouter/cdrouter.py` & `cdrouter-0.9.2/cdrouter/cdrouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
     last = fields.Int()
     current = fields.Int()
     total = fields.Int()
     limit = fields.Int()
     next = fields.Int(load_default=None)
     prev = fields.Int(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Links(**data)
 
 class Response(object):
     def __init__(self, **kwargs):
         self.timestamp = kwargs.get('timestamp', None)
@@ -80,21 +83,27 @@
         self.links = kwargs.get('links', None)
 
 class ResponseSchema(Schema):
     timestamp = DateTime()
     error = fields.Str(load_default=None)
     data = fields.Dict(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Response(**data)
 
 class ListResponseSchema(ResponseSchema):
     data = fields.List(fields.Dict(), load_default=None)
-    links = fields.Nested(LinksSchema(), load_default=None)
+    links = fields.Nested(LinksSchema(), load_default=None, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Response(**data)
 
 class Share(object):
     """Model for CDRouter Shares.
@@ -112,14 +121,17 @@
 
 class ShareSchema(Schema):
     user_id = fields.Int(as_string=True)
     read = fields.Bool()
     write = fields.Bool()
     execute = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Share(**data)
 
 class Auth(requests.auth.AuthBase): # pylint: disable=too-few-public-methods
     """Class for authorizing CDRouter Web API requests."""
```

### Comparing `cdrouter-0.9.1/cdrouter/configs.py` & `cdrouter-0.9.2/cdrouter/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Configs."""
 
 from collections import namedtuple
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_error import CDRouterError
 from .cdr_datetime import DateTime
 from .filters import Field as field
 
 class ConfigError(object):
     """Model for CDRouter Check Config Error.
 
@@ -22,28 +22,34 @@
         self.lines = kwargs.get('lines', None)
         self.error = kwargs.get('error', None)
 
 class ConfigErrorSchema(Schema):
     lines = fields.List(fields.Str())
     error = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return ConfigError(**data)
 
 class CheckConfig(object):
     """Model for CDRouter Check Config.
 
     :param errors: (optional) :class:`configs.ConfigError <configs.ConfigError>` list
     """
     def __init__(self, **kwargs):
         self.errors = kwargs.get('errors', None)
 
 class CheckConfigSchema(Schema):
-    errors = fields.Nested(lambda: ConfigErrorSchema(many=True))
+    errors = fields.Nested(lambda: ConfigErrorSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return CheckConfig(**data)
 
 class UpgradeConfig(object):
     """Model for CDRouter Config Upgrades.
@@ -55,14 +61,17 @@
         self.success = kwargs.get('success', None)
         self.output = kwargs.get('output', None)
 
 class UpgradeConfigSchema(Schema):
     success = fields.Bool()
     output = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return UpgradeConfig(**data)
 
 class Networks(object):
     """Model for CDRouter Config Networks.
 
@@ -80,15 +89,18 @@
         self.children = kwargs.get('children', None)
 
 class NetworksSchema(Schema):
     name = fields.Str()
     type = fields.Str()
     side = fields.Str()
     title = fields.Str(load_default=None)
-    children = fields.Nested(lambda: NetworksSchema(many=True))
+    children = fields.Nested(lambda: NetworksSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Networks(**data)
 
 class Interfaces(object):
     """Model for CDRouter Config Interfaces.
@@ -106,14 +118,17 @@
 
 class InterfacesSchema(Schema):
     name = fields.Str(load_default=None)
     value = fields.Str()
     is_wireless = fields.Bool()
     is_ics = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Interfaces(**data)
 
 class Testvar(object):
     """Model for CDRouter Config Testvars.
 
@@ -136,14 +151,17 @@
     group = fields.Str()
     name = fields.Str()
     value = fields.Str()
     default = fields.Str()
     isdefault = fields.Bool()
     line = fields.Int()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Testvar(**data)
 
 class Config(object):
     """Model for CDRouter Configs.
 
@@ -179,15 +197,18 @@
     created = DateTime()
     updated = DateTime()
     contents = fields.Str()
     user_id = fields.Int(as_string=True)
     result_id = fields.Int(as_string=True, load_default=None)
     tags = fields.List(fields.Str())
     note = fields.Str()
-    interfaces = fields.Nested(InterfacesSchema, many=True)
+    interfaces = fields.Nested(InterfacesSchema, many=True, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Config(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/devices.py` & `cdrouter-0.9.2/cdrouter/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Devices."""
 
 from collections import namedtuple
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_error import CDRouterError
 from .cdr_datetime import DateTime
 from .filters import Field as field
 
 class PowerCmd(object):
     """Model for CDRouter Device Power command result.
 
@@ -20,14 +20,17 @@
 
     def __init__(self, **kwargs):
         self.output = kwargs.get('output', None)
 
 class PowerCmdSchema(Schema):
     output = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return PowerCmd(**data)
 
 class Connection(object):
     """Model for CDRouter Device Connections.
 
@@ -40,14 +43,17 @@
         self.proxy_https = kwargs.get('proxy_https', None)
 
 
 class ConnectionSchema(Schema):
     proxy_port = fields.Int()
     proxy_https = fields.Int()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Connection(**data)
 
 class Device(object):
     """Model for CDRouter Devices.
 
@@ -160,14 +166,17 @@
     mgmt_url = fields.Str(load_default=None)
     add_mgmt_addr = fields.Bool(load_default=None)
     mgmt_interface = fields.Str(load_default=None)
     mgmt_addr = fields.Str(load_default=None)
     power_on_cmd = fields.Str(load_default=None)
     power_off_cmd = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Device(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/exports.py` & `cdrouter-0.9.2/cdrouter/exports.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.1/cdrouter/filters.py` & `cdrouter-0.9.2/cdrouter/filters.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.1/cdrouter/highlights.py` & `cdrouter-0.9.2/cdrouter/highlights.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Highlights."""
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 
 class Highlight(object):
     """Model for CDRouter Highlights.
 
     :param id: (optional) Result ID as an int.
     :param seq: (optional) TestResult sequence ID as an int.
     :param line: (optional) Line number in TestResult's logfile as an int.
@@ -23,14 +23,17 @@
 
 class HighlightSchema(Schema):
     id = fields.Int(as_string=True)
     seq = fields.Int(as_string=True)
     line = fields.Int(as_string=True)
     color = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Highlight(**data)
 
 class HighlightsService(object):
     """Service for accessing CDRouter Highlights."""
```

### Comparing `cdrouter-0.9.1/cdrouter/history.py` & `cdrouter-0.9.2/cdrouter/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter History."""
 
 from collections import namedtuple
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 
 class History(object):
     """Model for CDRouter History entries.
 
     :param user_id: (optional) User ID as an int.
     :param created: (optional) Entry creation time as `DateTime`.
@@ -35,14 +35,17 @@
     created = DateTime()
     resource = fields.Str()
     id = fields.Int(as_string=True)
     name = fields.Str()
     action = fields.Str()
     description = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return History(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/imports.py` & `cdrouter-0.9.2/cdrouter/imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Imports."""
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 
 class Import(object):
     """Model for CDRouter Staged Imports.
 
     :param id: (optional) Staged import ID as an int.
     :param user_id: (optional) User ID as an int.
@@ -39,14 +39,17 @@
     updated = DateTime()
     archive = fields.Str()
     path = fields.Str()
     url = fields.Str()
     insecure = fields.Bool()
     size = fields.Int()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Import(**data)
 
 class Response(object):
     """Model for CDRouter Import Responses.
 
@@ -63,14 +66,17 @@
 
 class ResponseSchema(Schema):
     imported = fields.Bool()
     id = fields.Int(as_string=True, load_default=None)
     name = fields.Str(load_default=None)
     message = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Response(**data)
 
 class Resource(object):
     """Model for CDRouter Import Resources.
 
@@ -85,15 +91,18 @@
         self.existing_id = kwargs.get('existing_id', None)
         self.response = kwargs.get('response', None)
 
 class ResourceSchema(Schema):
     name = fields.Str(load_default=None)
     should_import = fields.Bool(attribute='should_import', data_key='import')
     existing_id = fields.Int(as_string=True, load_default=None)
-    response = fields.Nested(ResponseSchema(), load_default=None)
+    response = fields.Nested(ResponseSchema(), load_default=None, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Resource(**data)
 
 class Request(object):
     """Model for CDRouter Import Requests.
@@ -114,21 +123,24 @@
         self.results = kwargs.get('results', None)
 
         self.tags = kwargs.get('tags', None)
 
 class RequestSchema(Schema):
     replace_existing = fields.Bool()
 
-    configs = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()))
-    devices = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()))
-    packages = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()))
-    results = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()))
+    configs = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()), unknown=EXCLUDE)
+    devices = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()), unknown=EXCLUDE)
+    packages = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()), unknown=EXCLUDE)
+    results = fields.Dict(keys=fields.Str(), values=fields.Nested(ResourceSchema()), unknown=EXCLUDE)
 
     tags = fields.List(fields.Str(), load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Request(**data)
 
 class ImportsService(object):
     """Service for accessing CDRouter Imports."""
```

### Comparing `cdrouter-0.9.1/cdrouter/jobs.py` & `cdrouter-0.9.2/cdrouter/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Jobs."""
 
 from collections import namedtuple
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 from .configs import InterfacesSchema
 
 class Options(object):
     """Model for CDRouter Job Options.
 
     :param tags: (optional) Tags as string list.
@@ -30,14 +30,17 @@
 class OptionsSchema(Schema):
     tags = fields.List(fields.Str(), load_default=None)
     skip_tests = fields.List(fields.Str(), load_default=None)
     begin_at = fields.Str()
     end_at = fields.Str()
     extra_cli_args = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Options(**data)
 
 class Job(object):
     """Model for CDRouter Jobs.
 
@@ -84,32 +87,35 @@
         self.uses_wireless = kwargs.get('uses_wireless', None)
         self.uses_ics = kwargs.get('uses_ics', None)
 
 class JobSchema(Schema):
     id = fields.Int(as_string=True)
     active = fields.Bool()
     status = fields.Str()
-    options = fields.Nested(OptionsSchema)
+    options = fields.Nested(OptionsSchema, unknown=EXCLUDE)
     package_id = fields.Int(as_string=True)
     package_name = fields.Str()
     config_id = fields.Int(as_string=True)
     config_name = fields.Str()
     device_id = fields.Int(as_string=True)
     device_name = fields.Str()
     result_id = fields.Int(as_string=True, load_default=None)
     user_id = fields.Int(as_string=True)
     created = DateTime()
     updated = DateTime()
     automatic = fields.Bool()
     run_at = DateTime()
-    interfaces = fields.Nested(InterfacesSchema, many=True)
+    interfaces = fields.Nested(InterfacesSchema, many=True, unknown=EXCLUDE)
     interface_names = fields.List(fields.Str())
     uses_wireless = fields.Bool()
     uses_ics = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Job(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/metrics.py` & `cdrouter-0.9.2/cdrouter/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Metrics."""
 
 from collections import namedtuple
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 
 class Metric(object):
     """Model for CDRouter Metrics.
 
     :param id: (optional) Result ID as an int.
     :param seq: (optional) TestResult sequence ID as an int.
@@ -35,14 +35,17 @@
     seq = fields.Int(as_string=True)
     created = DateTime()
     updated = DateTime()
     test_name = fields.Str()
     metric = fields.Str()
     filename = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Metric(**data)
 
 class Bandwidth(object):
     """Model for CDRouter Bandwidth Metrics.
 
@@ -92,14 +95,17 @@
     protocol = fields.Str()
     direction = fields.Str()
     loss_percentage = fields.Float(load_default=None)
     loss_percentage_units = fields.Str(load_default=None)
     client_device = fields.Str(load_default=None)
     server_device = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Bandwidth(**data)
 
 class Latency(object):
     """Model for CDRouter Latency Metrics.
 
@@ -137,14 +143,17 @@
     result = fields.Str()
     interface = fields.Str()
     download_latency = fields.Int(load_default=None)
     download_latency_units = fields.Str(load_default=None)
     upload_latency = fields.Int(load_default=None)
     upload_latency_units = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Latency(**data)
 
 class ClientBandwidth(object):
     """Model for CDRouter Client Bandwidth Metrics.
 
@@ -158,14 +167,17 @@
         self.rates = kwargs.get('rates', None)
 
 class ClientBandwidthSchema(Schema):
     timestamp = DateTime()
     num_rates = fields.Int()
     rates = fields.List(fields.Float())
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return ClientBandwidth(**data)
 
 class ClientLatency(object):
     """Model for CDRouter Client Latency Metrics.
 
@@ -179,14 +191,17 @@
         self.rates = kwargs.get('rates', None)
 
 class ClientLatencySchema(Schema):
     timestamp = DateTime()
     num_rates = fields.Int()
     rates = fields.List(fields.Int())
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return ClientLatency(**data)
 
 class GraphMetric(object):
     """Model for CDRouter Graph Metrics.
 
@@ -236,14 +251,17 @@
     protocol = fields.Str()
     direction = fields.Str()
     value_2 = fields.Float(as_string=True)
     units_2 = fields.Str()
     device_1 = fields.Str()
     device_2 = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return GraphMetric(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/packages.py` & `cdrouter-0.9.2/cdrouter/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Packages."""
 
 from collections import namedtuple
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_error import CDRouterError
 from .results import OptionsSchema as ResultOptionsSchema
 from .testsuites import TestSchema
 from .cdr_datetime import DateTime
 from .filters import Field as field
 from .configs import InterfacesSchema
 
@@ -29,15 +29,18 @@
         self.skipped_count = kwargs.get('skipped_count', None)
         self.skipped_tests = kwargs.get('skipped_tests', None)
 
 class AnalysisSchema(Schema):
     total_count = fields.Int()
     run_count = fields.Int()
     skipped_count = fields.Int()
-    skipped_tests = fields.Nested(lambda: TestSchema(many=True))
+    skipped_tests = fields.Nested(lambda: TestSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Analysis(**data)
 
 class Options(object):
     """Model for CDRouter Package Options.
@@ -78,14 +81,17 @@
     pause = fields.Bool()
     shuffle = fields.Bool()
     seed = fields.Int(as_string=True)
     retry = fields.Int(as_string=True)
     rdelay = fields.Int(as_string=True)
     sync = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Options(**data)
 
 class Schedule(object):
     """Model for CDRouter Package Schedule.
 
@@ -97,15 +103,18 @@
         self.enabled = kwargs.get('enabled', None)
         self.spec = kwargs.get('spec', None)
         self.options = kwargs.get('options', None)
 
 class ScheduleSchema(Schema):
     enabled = fields.Bool()
     spec = fields.Str()
-    options = fields.Nested(ResultOptionsSchema)
+    options = fields.Nested(ResultOptionsSchema, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Schedule(**data)
 
 class Package(object):
     """Model for CDRouter Packages.
@@ -161,20 +170,23 @@
     testlist = fields.List(fields.Str(), load_default=None)
     extra_cli_args = fields.Str()
     user_id = fields.Int(as_string=True)
     agent_id = fields.Int(as_string=True)
     config_id = fields.Int(as_string=True)
     result_id = fields.Int(as_string=True, load_default=None)
     device_id = fields.Int(as_string=True)
-    options = fields.Nested(OptionsSchema)
+    options = fields.Nested(OptionsSchema, unknown=EXCLUDE)
     tags = fields.List(fields.Str())
     use_as_testlist = fields.Bool()
     note = fields.Str(load_default=None)
-    schedule = fields.Nested(ScheduleSchema)
-    interfaces = fields.Nested(InterfacesSchema, many=True)
+    schedule = fields.Nested(ScheduleSchema, unknown=EXCLUDE)
+    interfaces = fields.Nested(InterfacesSchema, many=True, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Package(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/results.py` & `cdrouter-0.9.2/cdrouter/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,17 @@
         self.name = kwargs.get('name', None)
         self.count = kwargs.get('count', None)
 
 class TestCountSchema(Schema):
     name = fields.Str()
     count = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TestCount(**data)
 
 class TestDuration(object):
     """Model for CDRouter Test Durations.
 
@@ -44,14 +47,17 @@
         self.name = kwargs.get('name', None)
         self.duration = kwargs.get('duration', None)
 
 class TestDurationSchema(Schema):
     name = fields.Str()
     duration = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TestDuration(**data)
 
 class ResultBreakdown(object):
     """Model for CDRouter Result Breakdowns.
 
@@ -68,14 +74,17 @@
 
 class ResultBreakdownSchema(Schema):
     passed = fields.Int(as_string=True)
     failed = fields.Int(as_string=True)
     skipped = fields.Int(as_string=True)
     alerted = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return ResultBreakdown(**data)
 
 class TimeBreakdown(object):
     """Model for CDRouter Time Breakdowns.
 
@@ -86,14 +95,17 @@
         self.passed = kwargs.get('passed', None)
         self.failed = kwargs.get('failed', None)
 
 class TimeBreakdownSchema(Schema):
     passed = fields.Int(as_string=True)
     failed = fields.Int(as_string=True)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TimeBreakdown(**data)
 
 class SetStats(object):
     """Model for CDRouter Result Set Stats.
 
@@ -105,18 +117,21 @@
     def __init__(self, **kwargs):
         self.frequent_failures = kwargs.get('frequent_failures', None)
         self.longest_tests = kwargs.get('longest_tests', None)
         self.result_breakdown = kwargs.get('result_breakdown', None)
         self.time_breakdown = kwargs.get('time_breakdown', None)
 
 class SetStatsSchema(Schema):
-    frequent_failures = fields.Nested(lambda: TestCountSchema(many=True))
-    longest_tests = fields.Nested(lambda: TestDurationSchema(many=True))
-    result_breakdown = fields.Nested(ResultBreakdownSchema)
-    time_breakdown = fields.Nested(TimeBreakdownSchema)
+    frequent_failures = fields.Nested(lambda: TestCountSchema(many=True), unknown=EXCLUDE)
+    longest_tests = fields.Nested(lambda: TestDurationSchema(many=True), unknown=EXCLUDE)
+    result_breakdown = fields.Nested(ResultBreakdownSchema, unknown=EXCLUDE)
+    time_breakdown = fields.Nested(TimeBreakdownSchema, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return SetStats(**data)
 
 class TestResultSummary(object):
     """Model for CDRouter TestResult summaries.
@@ -146,14 +161,17 @@
     result = fields.Str()
     alerts = fields.Int()
     duration = fields.Int()
     flagged = fields.Bool()
     name = fields.Str()
     description = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TestResultSummary(**data)
 
 class TestResultDiff(object):
     """Model for CDRouter TestResult diffs.
 
@@ -162,30 +180,36 @@
     """
     def __init__(self, **kwargs):
         self.name = kwargs.get('name', None)
         self.summaries = kwargs.get('summaries', None)
 
 class TestResultDiffSchema(Schema):
     name = fields.Str()
-    summaries = fields.Nested(lambda: TestResultSummarySchema(many=True))
+    summaries = fields.Nested(lambda: TestResultSummarySchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TestResultDiff(**data)
 
 class DiffStats(object):
     """Model for CDRouter Result Diff Stats.
 
     :param tests: (optional) :class:`results.TestResultDiff <results.TestResultDiff>` list
     """
     def __init__(self, **kwargs):
         self.tests = kwargs.get('tests', None)
 
 class DiffStatsSchema(Schema):
-    tests = fields.Nested(lambda: TestResultDiffSchema(many=True))
+    tests = fields.Nested(lambda: TestResultDiffSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return DiffStats(**data)
 
 class TestResultBreakdown(object):
     """Model for CDRouter TestResult Breakdowns.
@@ -194,16 +218,19 @@
     :param passed_every_time: (optional) :class:`results.TestCount <results.TestCount>` list
     """
     def __init__(self, **kwargs):
         self.failed_at_least_once = kwargs.get('failed_at_least_once', None)
         self.passed_every_time = kwargs.get('passed_every_time', None)
 
 class TestResultBreakdownSchema(Schema):
-    failed_at_least_once = fields.Nested(lambda: TestCountSchema(many=True))
-    passed_every_time = fields.Nested(lambda: TestCountSchema(many=True))
+    failed_at_least_once = fields.Nested(lambda: TestCountSchema(many=True), unknown=EXCLUDE)
+    passed_every_time = fields.Nested(lambda: TestCountSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TestResultBreakdown(**data)
 
 class Progress(object):
     """Model for CDRouter Result Progress.
@@ -221,14 +248,17 @@
 
 class ProgressSchema(Schema):
     finished = fields.Int()
     total = fields.Int()
     progress = fields.Int()
     unit = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Progress(**data)
 
 class SingleStats(object):
     """Model for CDRouter Single Results Stats.
 
@@ -236,16 +266,19 @@
     :param progress: (optional) :class:`results.Progress <results.Progress>` object
     """
     def __init__(self, **kwargs):
         self.result_breakdown = kwargs.get('result_breakdown', None)
         self.progress = kwargs.get('progress', None)
 
 class SingleStatsSchema(Schema):
-    result_breakdown = fields.Nested(TestResultBreakdownSchema)
-    progress = fields.Nested(ProgressSchema)
+    result_breakdown = fields.Nested(TestResultBreakdownSchema, unknown=EXCLUDE)
+    progress = fields.Nested(ProgressSchema, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return SingleStats(**data)
 
 class SummaryStats(object):
     """Model for CDRouter Summary Results Stats.
@@ -254,16 +287,19 @@
     :param test_summaries: (optional) :class:`testresults.TestResult <testresults.TestResult>` list
     """
     def __init__(self, **kwargs):
         self.result_breakdown = kwargs.get('result_breakdown', None)
         self.test_summaries = kwargs.get('test_summaries', None)
 
 class SummaryStatsSchema(Schema):
-    result_breakdown = fields.Nested(ResultBreakdownSchema)
-    test_summaries = fields.Nested(lambda: TestResultSchema(many=True), load_default=None)
+    result_breakdown = fields.Nested(ResultBreakdownSchema, unknown=EXCLUDE)
+    test_summaries = fields.Nested(lambda: TestResultSchema(many=True), load_default=None, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return SummaryStats(**data)
 
 class PackageCount(object):
     """Model for CDRouter Package Counts.
@@ -275,14 +311,17 @@
         self.package_name = kwargs.get('package_name', None)
         self.count = kwargs.get('count', None)
 
 class PackageCountSchema(Schema):
     package_name = fields.Str()
     count = fields.Int(as_string=True, load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return PackageCount(**data)
 
 class DeviceCount(object):
     """Model for CDRouter Device Counts.
 
@@ -293,14 +332,17 @@
         self.device_name = kwargs.get('device_name', None)
         self.count = kwargs.get('count', None)
 
 class DeviceCountSchema(Schema):
     device_name = fields.Str()
     count = fields.Int(as_string=True, load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return DeviceCount(**data)
 
 class AllStats(object):
     """Model for CDRouter All Results Stats.
 
@@ -312,18 +354,21 @@
     def __init__(self, **kwargs):
         self.frequent_packages = kwargs.get('frequent_packages', None)
         self.package_names = kwargs.get('package_names', None)
         self.frequent_devices = kwargs.get('frequent_devices', None)
         self.device_names = kwargs.get('device_names', None)
 
 class AllStatsSchema(Schema):
-    frequent_packages = fields.Nested(lambda: PackageCountSchema(many=True))
-    package_names = fields.Nested(lambda: PackageCountSchema(many=True))
-    frequent_devices = fields.Nested(lambda: DeviceCountSchema(many=True))
-    device_names = fields.Nested(lambda: DeviceCountSchema(many=True))
+    frequent_packages = fields.Nested(lambda: PackageCountSchema(many=True), unknown=EXCLUDE)
+    package_names = fields.Nested(lambda: PackageCountSchema(many=True), unknown=EXCLUDE)
+    frequent_devices = fields.Nested(lambda: DeviceCountSchema(many=True), unknown=EXCLUDE)
+    device_names = fields.Nested(lambda: DeviceCountSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return AllStats(**data)
 
 # type aliases for Metric and MetricSchema types which were moved to
 # metrics.GraphMetric and metrics.GraphMetricSchema in cdrouter.py
@@ -345,14 +390,17 @@
         self.modified = kwargs.get('modified', None)
 
 class LogDirFileSchema(Schema):
     name = fields.Str()
     size = fields.Int()
     modified = DateTime()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return LogDirFile(**data)
 
 class Options(object):
     """Model for CDRouter Result Options.
 
@@ -372,14 +420,17 @@
 class OptionsSchema(Schema):
     tags = fields.List(fields.Str(), load_default=None)
     skip_tests = fields.List(fields.Str(), load_default=None)
     begin_at = fields.Str()
     end_at = fields.Str()
     extra_cli_args = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Options(**data)
 
 class Feature(object):
     """Model for CDRouter Result Feature.
 
@@ -393,14 +444,17 @@
         self.reason = kwargs.get('reason', None)
 
 class FeatureSchema(Schema):
     feature = fields.Str()
     enabled = fields.Bool()
     reason = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Feature(**data)
 
 class UpdateField(fields.Field):
     def _deserialize(self, value, attr, data, **kwargs):
         if 'result' in value and 'status' in value:
@@ -427,18 +481,21 @@
         self.progress = kwargs.get('progress', None)
         self.running = kwargs.get('running', None)
         self.updates = kwargs.get('updates', None)
 
 class UpdateSchema(Schema):
     id = fields.Int(as_string=True)
     timestamp = DateTime()
-    progress = fields.Nested(ProgressSchema(), load_default=None)
-    running = fields.Nested(TestResultSchema(), load_default=None)
+    progress = fields.Nested(ProgressSchema(), load_default=None, unknown=EXCLUDE)
+    running = fields.Nested(TestResultSchema(), load_default=None, unknown=EXCLUDE)
     updates = fields.List(UpdateField, load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Update(**data)
 
 class Result(object):
     """Model for CDRouter Results.
 
@@ -535,17 +592,20 @@
     config_id = fields.Int(as_string=True)
     user_id = fields.Int(as_string=True)
     note = fields.Str()
     pause_message = fields.Str(load_default=None)
     build_info = fields.Str(load_default=None)
     tags = fields.List(fields.Str())
     testcases = fields.List(fields.Str(), load_default=None)
-    options = fields.Nested(OptionsSchema)
-    features = fields.Dict(keys=fields.Str(), values=fields.Nested(FeatureSchema()))
-    interfaces = fields.Nested(InterfacesSchema, many=True)
+    options = fields.Nested(OptionsSchema, unknown=EXCLUDE)
+    features = fields.Dict(keys=fields.Str(), values=fields.Nested(FeatureSchema()), unknown=EXCLUDE)
+    interfaces = fields.Nested(InterfacesSchema, many=True, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Result(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/system.py` & `cdrouter-0.9.2/cdrouter/system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter System."""
 
 import io
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from requests_toolbelt.downloadutils import stream
 
 class Version(object):
     """Model for CDRouter Release Versions.
 
     :param raw: (optional) Raw version as string.
     :param major: (optional) Major version as int.
@@ -26,14 +26,17 @@
 
 class VersionSchema(Schema):
     raw = fields.Str()
     major = fields.Int()
     minor = fields.Int()
     build = fields.Int()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Version(**data)
 
 class ReleaseLatest(object):
     """Model for CDRouter Latest Releases.
 
@@ -43,18 +46,21 @@
     """
     def __init__(self, **kwargs):
         self.latest = kwargs.get('latest', None)
         self.current = kwargs.get('current', None)
         self.newer = kwargs.get('newer', None)
 
 class ReleaseLatestSchema(Schema):
-    latest = fields.Nested(VersionSchema)
-    current = fields.Nested(VersionSchema)
+    latest = fields.Nested(VersionSchema, unknown=EXCLUDE)
+    current = fields.Nested(VersionSchema, unknown=EXCLUDE)
     newer = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return ReleaseLatest(**data)
 
 class Testsuite(object):
     """Model for CDRouter Testsuite names.
 
@@ -65,14 +71,17 @@
         self.shortname = kwargs.get('shortname', None)
         self.name = kwargs.get('name', None)
 
 class TestsuiteSchema(Schema):
     shortname = fields.Str()
     name = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Testsuite(**data)
 
 class Release(object):
     """Model for CDRouter Releases.
 
@@ -88,18 +97,21 @@
         self.version = kwargs.get('version', None)
         self.testsuite = kwargs.get('testsuite', None)
         self.nonce = kwargs.get('nonce', None)
 
 class ReleaseSchema(Schema):
     build_date = fields.Str()
     filename = fields.Str()
-    version = fields.Nested(VersionSchema)
-    testsuite = fields.Nested(TestsuiteSchema)
+    version = fields.Nested(VersionSchema, unknown=EXCLUDE)
+    testsuite = fields.Nested(TestsuiteSchema, unknown=EXCLUDE)
     nonce = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Release(**data)
 
 class Upgrade(object):
     """Model for CDRouter Upgrades.
 
@@ -116,14 +128,17 @@
 
 class UpgradeSchema(Schema):
     success = fields.Bool()
     installer_path = fields.Str(load_default=None)
     output = fields.Str(load_default=None)
     error = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Upgrade(**data)
 
 class InterfaceFlags(object):
     """Model for CDRouter Interface Flags.
 
@@ -143,14 +158,17 @@
 class InterfaceFlagsSchema(Schema):
     up = fields.Bool()
     broadcast = fields.Bool()
     loopback = fields.Bool()
     point_to_point = fields.Bool()
     multicast = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return InterfaceFlags(**data)
 
 class InterfaceAddr(object):
     """Model for CDRouter Interface Addresses.
 
@@ -161,14 +179,17 @@
         self.network = kwargs.get('network', None)
         self.address = kwargs.get('address', None)
 
 class InterfaceAddrSchema(Schema):
     network = fields.Str()
     address = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return InterfaceAddr(**data)
 
 class Interface(object):
     """Model for CDRouter Interfaces.
 
@@ -190,17 +211,20 @@
         self.multicast_addresses = kwargs.get('multicast_addresses', None)
 
 class InterfaceSchema(Schema):
     index = fields.Int(as_string=True)
     mtu = fields.Int(as_string=True)
     name = fields.Str()
     hardware_addr = fields.Str()
-    flags = fields.Nested(InterfaceFlagsSchema)
-    addresses = fields.Nested(lambda: InterfaceAddrSchema(many=True), load_default=None)
-    multicast_addresses = fields.Nested(lambda: InterfaceAddrSchema(many=True), load_default=None)
+    flags = fields.Nested(InterfaceFlagsSchema, unknown=EXCLUDE)
+    addresses = fields.Nested(lambda: InterfaceAddrSchema(many=True), load_default=None, unknown=EXCLUDE)
+    multicast_addresses = fields.Nested(lambda: InterfaceAddrSchema(many=True), load_default=None, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Interface(**data)
 
 class InUseInterfaceFlags(object):
     """Model for CDRouter In Use Interface Flags.
@@ -215,14 +239,17 @@
         self.is_ics = kwargs.get('is_ics', None)
 
 class InUseInterfaceFlagsSchema(Schema):
     in_use = fields.Bool()
     is_wireless = fields.Bool()
     is_ics = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return InUseInterfaceFlags(**data)
 
 class InUseInterface(object):
     """Model for CDRouter In Use Interfaces.
 
@@ -231,15 +258,18 @@
     """
     def __init__(self, **kwargs):
         self.name = kwargs.get('name', None)
         self.flags = kwargs.get('flags', None)
 
 class InUseInterfaceSchema(Schema):
     name = fields.Str()
-    flags = fields.Nested(InUseInterfaceFlagsSchema)
+    flags = fields.Nested(InUseInterfaceFlagsSchema, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return InUseInterface(**data)
 
 class Preferences(object):
     """Model for CDRouter Preferences.
@@ -299,14 +329,17 @@
     force_https = fields.Str()
     use_cloudshark = fields.Str()
     log_timestamp_format = fields.Str()
     editor_keymap = fields.Str()
     lounge_url = fields.Str()
     lounge_insecure = fields.Bool()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Preferences(**data)
 
 class Space(object):
     """Model for CDRouter Disk Space Usage.
 
@@ -329,14 +362,17 @@
     avail = fields.Int()
     path = fields.Str()
     pcent = fields.Int()
     size = fields.Int()
     unit = fields.Str()
     used = fields.Int()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Space(**data)
 
 class SystemService(object):
     """Service for accessing CDRouter System."""
```

### Comparing `cdrouter-0.9.1/cdrouter/tags.py` & `cdrouter-0.9.2/cdrouter/tags.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Tags."""
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 
 class ResourceTags(object):
     """Model for CDRouter Resource Tags.
 
     :param id: (optional) Resource ID as an int.
     :param name: (optional) Resource name as string.
     :param tags: (optional) Resource tags as a string list.
@@ -20,14 +20,17 @@
         self.tags = kwargs.get('tags', None)
 
 class ResourceTagsSchema(Schema):
     id = fields.Str()
     name = fields.Str()
     tags = fields.List(fields.Str())
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return ResourceTags(**data)
 
 class Tag(object):
     """Model for CDRouter Tags.
 
@@ -56,18 +59,21 @@
 class TagSchema(Schema):
     resource = fields.Str()
     id = fields.Int(as_string=True)
     name = fields.Str()
     count = fields.Int()
     tags = fields.List(fields.Str())
 
-    configs = fields.Nested(lambda: ResourceTagsSchema(many=True))
-    devices = fields.Nested(lambda: ResourceTagsSchema(many=True))
-    packages = fields.Nested(lambda: ResourceTagsSchema(many=True))
-    results = fields.Nested(lambda: ResourceTagsSchema(many=True))
+    configs = fields.Nested(lambda: ResourceTagsSchema(many=True), unknown=EXCLUDE)
+    devices = fields.Nested(lambda: ResourceTagsSchema(many=True), unknown=EXCLUDE)
+    packages = fields.Nested(lambda: ResourceTagsSchema(many=True), unknown=EXCLUDE)
+    results = fields.Nested(lambda: ResourceTagsSchema(many=True), unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Tag(**data)
 
 class TagsService(object):
     """Service for accessing CDRouter Tags."""
```

### Comparing `cdrouter-0.9.1/cdrouter/testresults.py` & `cdrouter-0.9.2/cdrouter/testresults.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 
 """Module for accessing CDRouter TestResults."""
 
 from collections import namedtuple
 from functools import partial
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 from .metrics import BandwidthSchema, ClientBandwidthSchema, ClientLatencySchema, LatencySchema, MetricSchema, Page as MetricPage
 
 class Summary(object):
     """Model for CDRouter Log Section Summaries.
 
     :param errors: (optional) Error log count as int.
@@ -31,14 +31,17 @@
 class SummarySchema(Schema):
     errors = fields.Int()
     fails = fields.Int()
     passes = fields.Int()
     warnings = fields.Int()
     alerts = fields.Int()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Summary(**data)
 
 class Line(object):
     """Model for CDRouter Log Lines.
 
@@ -138,15 +141,18 @@
     alert_dst_port = fields.Int(as_string=True, load_default=None)
     alert_signature = fields.Str(load_default=None)
     alert_severity = fields.Int(as_string=True, load_default=None)
     alert_severity_display = fields.Str(load_default=None)
     alert_sid = fields.Int(as_string=True, load_default=None)
     alert_rev = fields.Int(as_string=True, load_default=None)
 
-    summary = fields.Nested(SummarySchema)
+    summary = fields.Nested(SummarySchema, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Line(**data)
 
 class Log(object):
     """Model for CDRouter Log.
@@ -163,18 +169,21 @@
         self.lines = kwargs.get('lines', None)
         self.total = kwargs.get('total', None)
         self.more = kwargs.get('more', None)
 
 class LogSchema(Schema):
     offset = fields.Int()
     limit = fields.Int()
-    lines = fields.Nested(lambda: LineSchema(many=True))
+    lines = fields.Nested(lambda: LineSchema(many=True), unknown=EXCLUDE)
     total = fields.Int()
     more = fields.Bool(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Log(**data)
 
 class TestResult(object):
     """Model for CDRouter TestResults.
 
@@ -230,14 +239,17 @@
     description = fields.Str()
     skip_name = fields.Str()
     skip_reason = fields.Str()
     log = fields.Str()
     keylog = fields.Str(load_default=None)
     note = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return TestResult(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter/testsuites.py` & `cdrouter-0.9.2/cdrouter/testsuites.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Testsuites."""
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 from .configs import InterfacesSchema
 
 class LicenseInfo(object):
     """Model for CDRouter License Info.
 
     :param is_expired (optional): Bool `True` if license is expired.
@@ -25,14 +25,17 @@
 
 class LicenseInfoSchema(Schema):
     is_expired = fields.Bool()
     expires_date = fields.Str()
     expires_at = DateTime()
     expires_in = fields.Int()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return LicenseInfo(**data)
 
 class Info(object):
     """Model for CDRouter Testsuite Info.
 
@@ -90,17 +93,20 @@
     os_type = fields.Str(load_default=None)
     serial_number = fields.Str()
     system_id = fields.Str()
     testsuite = fields.Str()
     release = fields.Str()
     addons = fields.List(fields.Str())
     all_addons = fields.List(fields.Str())
-    interfaces = fields.Nested(InterfacesSchema, many=True)
+    interfaces = fields.Nested(InterfacesSchema, many=True, unknown=EXCLUDE)
     execute_instances = fields.Int()
-    license_info = fields.Nested(LicenseInfoSchema, load_default=None)
+    license_info = fields.Nested(LicenseInfoSchema, load_default=None, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Info(**data)
 
 class Group(object):
     """Model for CDRouter Groups.
@@ -121,14 +127,17 @@
 class GroupSchema(Schema):
     id = fields.Int(load_default=None)
     name = fields.Str()
     index = fields.Int()
     test_count = fields.Int()
     modules = fields.List(fields.Str())
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Group(**data)
 
 class Module(object):
     """Model for CDRouter Modules.
 
@@ -160,14 +169,17 @@
     group = fields.Str()
     description = fields.Str()
     test_count = fields.Int()
     tests = fields.List(fields.Str())
     labels = fields.List(fields.Str())
     aliases = fields.List(fields.Str())
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Module(**data)
 
 class Test(object):
     """Model for CDRouter Tests.
 
@@ -210,14 +222,17 @@
     labels = fields.List(fields.Str(), load_default=None)
     aliases = fields.List(fields.Str(), load_default=None)
     testvars = fields.List(fields.Str(), load_default=None)
 
     skip_name = fields.Str(load_default=None)
     skip_reason = fields.Str(load_default=None)
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Test(**data)
 
 class Label(object):
     """Model for CDRouter Skip Labels.
 
@@ -243,14 +258,17 @@
     name = fields.Str()
     index = fields.Int()
     reason = fields.Str()
     description = fields.Str()
     modules = fields.List(fields.Str())
     tests = fields.List(fields.Str())
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Label(**data)
 
 class Error(object):
     """Model for CDRouter Start Errors.
 
@@ -267,14 +285,17 @@
 
 class ErrorSchema(Schema):
     id = fields.Int(load_default=None)
     name = fields.Str()
     index = fields.Int()
     description = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Error(**data)
 
 class Testvar(object):
     """Model for CDRouter Start Errors.
 
@@ -348,14 +369,17 @@
     alsoaccept = fields.List(fields.Str())
     wildcard = fields.Bool()
     instances = fields.Int()
     parent = fields.Str()
     children = fields.List(fields.Str())
     tests = fields.List(fields.Str())
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Testvar(**data)
 
 class Search(object):
     """Model for CDRouter Testsuite Searches.
 
@@ -371,20 +395,23 @@
         self.modules = kwargs.get('modules', None)
         self.tests = kwargs.get('tests', None)
         self.reasons = kwargs.get('reasons', None)
         self.errors = kwargs.get('errors', None)
         self.testvars = kwargs.get('testvars', None)
 
 class SearchSchema(Schema):
-    addons = fields.Nested(lambda: GroupSchema(many=True), load_default=None)
-    modules = fields.Nested(lambda: ModuleSchema(many=True), load_default=None)
-    tests = fields.Nested(lambda: TestSchema(many=True), load_default=None)
-    reasons = fields.Nested(lambda: LabelSchema(many=True), load_default=None)
-    errors = fields.Nested(lambda: ErrorSchema(many=True), load_default=None)
-    testvars = fields.Nested(lambda: TestvarSchema(many=True), load_default=None)
+    addons = fields.Nested(lambda: GroupSchema(many=True), load_default=None, unknown=EXCLUDE)
+    modules = fields.Nested(lambda: ModuleSchema(many=True), load_default=None, unknown=EXCLUDE)
+    tests = fields.Nested(lambda: TestSchema(many=True), load_default=None, unknown=EXCLUDE)
+    reasons = fields.Nested(lambda: LabelSchema(many=True), load_default=None, unknown=EXCLUDE)
+    errors = fields.Nested(lambda: ErrorSchema(many=True), load_default=None, unknown=EXCLUDE)
+    testvars = fields.Nested(lambda: TestvarSchema(many=True), load_default=None, unknown=EXCLUDE)
+
+    class Meta:
+        unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Search(**data)
 
 class TestsuitesService(object):
     """Service for accessing CDRouter Testsuites."""
```

### Comparing `cdrouter-0.9.1/cdrouter/users.py` & `cdrouter-0.9.2/cdrouter/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 """Module for accessing CDRouter Users."""
 
 from collections import namedtuple
 
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_error import CDRouterError
 from .cdr_datetime import DateTime
 from .filters import Field as field
 
 class User(object):
     """Model for CDRouter Users.
 
@@ -47,14 +47,17 @@
     created = DateTime()
     updated = DateTime()
     token = fields.Str()
 
     password = fields.Str()
     password_confirm = fields.Str()
 
+    class Meta:
+        unknown = EXCLUDE
+
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return User(**data)
 
 class Page(namedtuple('Page', ['data', 'links'])):
     """Named tuple for a page of list response data.
```

### Comparing `cdrouter-0.9.1/cdrouter.egg-info/PKG-INFO` & `cdrouter-0.9.2/cdrouter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```

### Comparing `cdrouter-0.9.1/cdrouter.egg-info/SOURCES.txt` & `cdrouter-0.9.2/cdrouter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.1/LICENSE.txt` & `cdrouter-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.1/README.rst` & `cdrouter-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.1/setup.py` & `cdrouter-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.1/PKG-INFO` & `cdrouter-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```

