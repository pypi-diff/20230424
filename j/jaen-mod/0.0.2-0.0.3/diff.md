# Comparing `tmp/jaen_mod-0.0.2-py3-none-any.whl.zip` & `tmp/jaen_mod-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3655 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       44 b- defN 23-Apr-24 07:21 jaen-mod/__init__.py
+Zip file size: 3636 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       44 b- defN 23-Apr-24 07:28 jaen-mod/__init__.py
 -rw-rw-rw-  2.0 fat     6841 b- defN 23-Apr-24 07:08 jaen-mod/jaen.py
--rw-rw-rw-  2.0 fat      594 b- defN 23-Apr-24 07:22 jaen_mod-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 07:22 jaen_mod-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-24 07:22 jaen_mod-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      448 b- defN 23-Apr-24 07:22 jaen_mod-0.0.2.dist-info/RECORD
-6 files, 8028 bytes uncompressed, 2841 bytes compressed:  64.6%
+-rw-rw-rw-  2.0 fat      526 b- defN 23-Apr-24 07:28 jaen_mod-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 07:28 jaen_mod-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-24 07:28 jaen_mod-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      448 b- defN 23-Apr-24 07:28 jaen_mod-0.0.3.dist-info/RECORD
+6 files, 7960 bytes uncompressed, 2822 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jaen-mod/__init__.py
 Comment: 
 
 Filename: jaen-mod/jaen.py
 Comment: 
 
-Filename: jaen_mod-0.0.2.dist-info/METADATA
+Filename: jaen_mod-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: jaen_mod-0.0.2.dist-info/WHEEL
+Filename: jaen_mod-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: jaen_mod-0.0.2.dist-info/top_level.txt
+Filename: jaen_mod-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: jaen_mod-0.0.2.dist-info/RECORD
+Filename: jaen_mod-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jaen-mod/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .jaen import *
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
```

