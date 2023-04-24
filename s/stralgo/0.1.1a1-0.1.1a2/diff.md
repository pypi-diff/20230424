# Comparing `tmp/stralgo-0.1.1a1-cp39-none-any.whl.zip` & `tmp/stralgo-0.1.1a2-cp39-abi3-win32.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4177 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat        0 b- defN 22-Mar-12 07:01 stralgo/__init__.py
--rw-rw-rw-  2.0 fat      972 b- defN 23-Feb-20 08:51 stralgo/base.py
--rw-rw-rw-  2.0 fat     3292 b- defN 23-Feb-05 12:27 stralgo/color.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 08:32 stralgo/hash/__init__.py
--rw-rw-rw-  2.0 fat      460 b- defN 23-Feb-20 08:51 stralgo/hash/sha.py
--rw-rw-rw-  2.0 fat     1072 b- defN 23-Mar-17 10:07 stralgo-0.1.1a1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      638 b- defN 23-Mar-17 10:07 stralgo-0.1.1a1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-17 10:07 stralgo-0.1.1a1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-17 10:07 stralgo-0.1.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      764 b- defN 23-Mar-17 10:07 stralgo-0.1.1a1.dist-info/RECORD
-10 files, 7298 bytes uncompressed, 2871 bytes compressed:  60.7%
+Zip file size: 4174 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Mar-11 23:01 stralgo/__init__.py
+-rw-rw-rw-  2.0 fat      972 b- defN 23-Feb-20 00:51 stralgo/base.py
+-rw-rw-rw-  2.0 fat     3292 b- defN 23-Apr-23 14:31 stralgo/color.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-20 00:32 stralgo/hash/__init__.py
+-rw-rw-rw-  2.0 fat      460 b- defN 23-Feb-20 00:51 stralgo/hash/sha.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Apr-23 14:58 stralgo-0.1.1a2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      678 b- defN 23-Apr-23 14:58 stralgo-0.1.1a2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 14:58 stralgo-0.1.1a2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-23 14:58 stralgo-0.1.1a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      764 b- defN 23-Apr-23 14:58 stralgo-0.1.1a2.dist-info/RECORD
+10 files, 7335 bytes uncompressed, 2868 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: stralgo/hash/__init__.py
 Comment: 
 
 Filename: stralgo/hash/sha.py
 Comment: 
 
-Filename: stralgo-0.1.1a1.dist-info/LICENSE
+Filename: stralgo-0.1.1a2.dist-info/LICENSE
 Comment: 
 
-Filename: stralgo-0.1.1a1.dist-info/METADATA
+Filename: stralgo-0.1.1a2.dist-info/METADATA
 Comment: 
 
-Filename: stralgo-0.1.1a1.dist-info/WHEEL
+Filename: stralgo-0.1.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: stralgo-0.1.1a1.dist-info/top_level.txt
+Filename: stralgo-0.1.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: stralgo-0.1.1a1.dist-info/RECORD
+Filename: stralgo-0.1.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stralgo-0.1.1a1.dist-info/LICENSE` & `stralgo-0.1.1a2.dist-info/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) <year> Dash.Bing
+Copyright (c) 2023 DashBing
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `stralgo-0.1.1a1.dist-info/METADATA` & `stralgo-0.1.1a2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: stralgo
-Version: 0.1.1a1
-Summary: A library for various string algorithms
+Version: 0.1.1a2
+Summary: A Python library for various string algorithms
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Stralgo Package README
+# stralgo
+A Python library for various string algorithms
```

## Comparing `stralgo-0.1.1a1.dist-info/RECORD` & `stralgo-0.1.1a2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 stralgo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stralgo/base.py,sha256=TmaSgGadovNn-XX_RG_VoNFARMOwnMg3YCfx3Q0H8f0,972
 stralgo/color.py,sha256=lJqPUt8J_NC-0ua5zC-IozVRs4OxdeSgH8v2XvAY7OI,3292
 stralgo/hash/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stralgo/hash/sha.py,sha256=NXVPE9coza_PqcdvNRz0KVDnzwKhJFvFu33WqEaP7mw,460
-stralgo-0.1.1a1.dist-info/LICENSE,sha256=YXfRJ-iD_qjoAirCkkoFiZQFihgDmjAp5PL6TlfWT5Q,1072
-stralgo-0.1.1a1.dist-info/METADATA,sha256=qxxFQGmMoLU79bYSgTe4Pdc2EFYEG9TLuVSWKiLvgGw,638
-stralgo-0.1.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-stralgo-0.1.1a1.dist-info/top_level.txt,sha256=UAr8FsuTMSRUG7BxdLJoYtMorRWc63vApWp7dwg5U5o,8
-stralgo-0.1.1a1.dist-info/RECORD,,
+stralgo-0.1.1a2.dist-info/LICENSE,sha256=kG_6qUnDa_JpdVPQCJhpccpIACtnNCA9SFkBxv2_I88,1069
+stralgo-0.1.1a2.dist-info/METADATA,sha256=O0vJcHZLBQ_EwFMQG6ff1RFXLlBVUIUBOKl7brJG-h0,678
+stralgo-0.1.1a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+stralgo-0.1.1a2.dist-info/top_level.txt,sha256=UAr8FsuTMSRUG7BxdLJoYtMorRWc63vApWp7dwg5U5o,8
+stralgo-0.1.1a2.dist-info/RECORD,,
```

