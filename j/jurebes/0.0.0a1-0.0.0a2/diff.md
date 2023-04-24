# Comparing `tmp/jurebes-0.0.0a1-py3-none-any.whl.zip` & `tmp/jurebes-0.0.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4121 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8833 b- defN 23-Apr-24 05:16 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 05:16 jurebes/version.py
--rw-r--r--  2.0 unx      712 b- defN 23-Apr-24 05:16 jurebes-0.0.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 05:16 jurebes-0.0.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 05:16 jurebes-0.0.0a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 05:16 jurebes-0.0.0a1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      542 b- defN 23-Apr-24 05:16 jurebes-0.0.0a1.dist-info/RECORD
-7 files, 10365 bytes uncompressed, 3153 bytes compressed:  69.6%
+Zip file size: 4148 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8833 b- defN 23-Apr-24 05:24 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 05:24 jurebes/version.py
+-rw-r--r--  2.0 unx      733 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      542 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/RECORD
+7 files, 10386 bytes uncompressed, 3180 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.0.0a1.dist-info/METADATA
+Filename: jurebes-0.0.0a2.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.0.0a1.dist-info/WHEEL
+Filename: jurebes-0.0.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.0.0a1.dist-info/top_level.txt
+Filename: jurebes-0.0.0a2.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.0.0a1.dist-info/zip-safe
+Filename: jurebes-0.0.0a2.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.0.0a1.dist-info/RECORD
+Filename: jurebes-0.0.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.0.0a1.dist-info/METADATA` & `jurebes-0.0.0a2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: ovos-utils
-Requires-Dist: ovos-classifiers
+Requires-Dist: ovos-classifiers[sklearn] (>=0.0.0a1)
 Requires-Dist: padacioso
 Requires-Dist: quebra-frases
 
 UNKNOWN
```

