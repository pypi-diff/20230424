# Comparing `tmp/robotframework_difflibext-0.0.3-py3-none-any.whl.zip` & `tmp/robotframework_difflibext-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3683 bytes, number of entries: 8
+Zip file size: 3682 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       72 b- defN 23-Feb-24 06:44 DiffLibExt/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-24 09:18 DiffLibExt/__version__.py
--rw-r--r--  2.0 unx     2756 b- defN 23-Apr-24 09:18 DiffLibExt/difflibext.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-24 09:19 robotframework_difflibext-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      490 b- defN 23-Apr-24 09:19 robotframework_difflibext-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 09:19 robotframework_difflibext-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-24 09:19 robotframework_difflibext-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      713 b- defN 23-Apr-24 09:19 robotframework_difflibext-0.0.3.dist-info/RECORD
-8 files, 5221 bytes uncompressed, 2413 bytes compressed:  53.8%
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-24 09:20 DiffLibExt/__version__.py
+-rw-r--r--  2.0 unx     2750 b- defN 23-Apr-24 09:20 DiffLibExt/difflibext.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      490 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      713 b- defN 23-Apr-24 09:21 robotframework_difflibext-0.0.4.dist-info/RECORD
+8 files, 5215 bytes uncompressed, 2412 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: DiffLibExt/__version__.py
 Comment: 
 
 Filename: DiffLibExt/difflibext.py
 Comment: 
 
-Filename: robotframework_difflibext-0.0.3.dist-info/LICENSE
+Filename: robotframework_difflibext-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: robotframework_difflibext-0.0.3.dist-info/METADATA
+Filename: robotframework_difflibext-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: robotframework_difflibext-0.0.3.dist-info/WHEEL
+Filename: robotframework_difflibext-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: robotframework_difflibext-0.0.3.dist-info/top_level.txt
+Filename: robotframework_difflibext-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: robotframework_difflibext-0.0.3.dist-info/RECORD
+Filename: robotframework_difflibext-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DiffLibExt/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## DiffLibExt/difflibext.py

```diff
@@ -59,12 +59,12 @@
 
     @keyword
     def text_should_be_equal(self, expected_text: str, actual_text: str):
         if expected_text != actual_text:
             self._report_diff(expected_text, actual_text)
 
     @keyword
-    def object_should_be_equal(self, expected_dict, actual_dict):
-        if expected_dict != actual_dict:
-            expected_json_text = json.dumps(expected_dict, indent=2)
-            actual_json_text = json.dumps(actual_dict, indent=2)
+    def object_should_be_equal(self, expected_obj, actual_obj):
+        if expected_obj != actual_obj:
+            expected_json_text = json.dumps(expected_obj, indent=2)
+            actual_json_text = json.dumps(actual_obj, indent=2)
             self._report_diff(expected_json_text, actual_json_text)
```

## Comparing `robotframework_difflibext-0.0.3.dist-info/LICENSE` & `robotframework_difflibext-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

