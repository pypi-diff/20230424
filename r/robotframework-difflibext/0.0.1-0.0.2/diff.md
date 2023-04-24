# Comparing `tmp/robotframework_difflibext-0.0.1-py3-none-any.whl.zip` & `tmp/robotframework_difflibext-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3684 bytes, number of entries: 8
+Zip file size: 3681 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       72 b- defN 23-Feb-24 06:44 DiffLibExt/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Feb-24 06:36 DiffLibExt/__version__.py
--rw-r--r--  2.0 unx     2766 b- defN 23-Feb-28 03:36 DiffLibExt/difflibext.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Feb-28 06:08 robotframework_difflibext-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      490 b- defN 23-Feb-28 06:08 robotframework_difflibext-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-28 06:08 robotframework_difflibext-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-28 06:08 robotframework_difflibext-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      713 b- defN 23-Feb-28 06:08 robotframework_difflibext-0.0.1.dist-info/RECORD
-8 files, 5231 bytes uncompressed, 2414 bytes compressed:  53.9%
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-24 09:15 DiffLibExt/__version__.py
+-rw-r--r--  2.0 unx     2754 b- defN 23-Apr-24 09:11 DiffLibExt/difflibext.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-24 09:15 robotframework_difflibext-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      490 b- defN 23-Apr-24 09:15 robotframework_difflibext-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 09:15 robotframework_difflibext-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-24 09:15 robotframework_difflibext-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      713 b- defN 23-Apr-24 09:15 robotframework_difflibext-0.0.2.dist-info/RECORD
+8 files, 5219 bytes uncompressed, 2411 bytes compressed:  53.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: DiffLibExt/__version__.py
 Comment: 
 
 Filename: DiffLibExt/difflibext.py
 Comment: 
 
-Filename: robotframework_difflibext-0.0.1.dist-info/LICENSE
+Filename: robotframework_difflibext-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: robotframework_difflibext-0.0.1.dist-info/METADATA
+Filename: robotframework_difflibext-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: robotframework_difflibext-0.0.1.dist-info/WHEEL
+Filename: robotframework_difflibext-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: robotframework_difflibext-0.0.1.dist-info/top_level.txt
+Filename: robotframework_difflibext-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: robotframework_difflibext-0.0.1.dist-info/RECORD
+Filename: robotframework_difflibext-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DiffLibExt/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## DiffLibExt/difflibext.py

```diff
@@ -59,12 +59,12 @@
 
     @keyword
     def text_should_be_equal(self, expected_text: str, actual_text: str):
         if expected_text != actual_text:
             self._report_diff(expected_text, actual_text)
 
     @keyword
-    def dict_should_be_equal(self, expected_dict: dict, actual_dict: dict):
+    def dict_should_be_equal(self, expected_dict, actual_dict):
         if expected_dict != actual_dict:
             expected_json_text = json.dumps(expected_dict, indent=2)
             actual_json_text = json.dumps(actual_dict, indent=2)
             self._report_diff(expected_json_text, actual_json_text)
```

## Comparing `robotframework_difflibext-0.0.1.dist-info/LICENSE` & `robotframework_difflibext-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

