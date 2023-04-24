# Comparing `tmp/DDesignerAPI-0.0.0.1-py3-none-any.whl.zip` & `tmp/DDesignerAPI-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4937 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       24 b- defN 23-Apr-24 06:54 ddesigner_api/__init__.py
--rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 06:55 DDesignerAPI-0.0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      399 b- defN 23-Apr-24 06:55 DDesignerAPI-0.0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 06:55 DDesignerAPI-0.0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 06:55 DDesignerAPI-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      500 b- defN 23-Apr-24 06:55 DDesignerAPI-0.0.0.1.dist-info/RECORD
-6 files, 10165 bytes uncompressed, 4021 bytes compressed:  60.4%
+Zip file size: 5329 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx      726 b- defN 23-Apr-24 07:15 ddesigner_api/__init__.py
+-rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 07:17 DDesignerAPI-0.0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      399 b- defN 23-Apr-24 07:17 DDesignerAPI-0.0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 07:17 DDesignerAPI-0.0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 07:17 DDesignerAPI-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      501 b- defN 23-Apr-24 07:17 DDesignerAPI-0.0.0.2.dist-info/RECORD
+6 files, 10868 bytes uncompressed, 4413 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ddesigner_api/__init__.py
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.1.dist-info/LICENSE
+Filename: DDesignerAPI-0.0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.1.dist-info/METADATA
+Filename: DDesignerAPI-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.1.dist-info/WHEEL
+Filename: DDesignerAPI-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.1.dist-info/top_level.txt
+Filename: DDesignerAPI-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.1.dist-info/RECORD
+Filename: DDesignerAPI-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddesigner_api/__init__.py

```diff
@@ -1 +1,17 @@
-__version__ = '0.0.0.1'
+# Copyright 2023 The Deeper-I Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+
+
+from ddesigner_api import tensorflow
```

## Comparing `DDesignerAPI-0.0.0.1.dist-info/LICENSE` & `DDesignerAPI-0.0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

