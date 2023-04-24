# Comparing `tmp/jurebes-0.1.0a1-py3-none-any.whl.zip` & `tmp/jurebes-0.1.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4723 bytes, number of entries: 7
--rw-r--r--  2.0 unx    12906 b- defN 23-Apr-24 10:49 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 10:49 jurebes/version.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 10:49 jurebes-0.1.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 10:49 jurebes-0.1.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 10:49 jurebes-0.1.0a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 10:49 jurebes-0.1.0a1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 10:49 jurebes-0.1.0a1.dist-info/RECORD
-7 files, 14480 bytes uncompressed, 3755 bytes compressed:  74.1%
+Zip file size: 4730 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    12950 b- defN 23-Apr-24 10:52 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 10:52 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/RECORD
+7 files, 14524 bytes uncompressed, 3762 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.1.0a1.dist-info/METADATA
+Filename: jurebes-0.1.0a2.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.1.0a1.dist-info/WHEEL
+Filename: jurebes-0.1.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.1.0a1.dist-info/top_level.txt
+Filename: jurebes-0.1.0a2.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.1.0a1.dist-info/zip-safe
+Filename: jurebes-0.1.0a2.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.1.0a1.dist-info/RECORD
+Filename: jurebes-0.1.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -167,15 +167,16 @@
         classes = self.classifier.clf.classes_
 
         for intent, prob in zip(classes, probs):
             if intent in excluded_intents:
                 continue
             if intent in self.available_contexts:
                 for context, val in self.available_contexts[intent].items():
-                    ents[context] = val
+                    if val is not None:
+                        ents[context] = val
 
             yield IntentMatch(confidence=prob,
                               intent_name=intent,
                               entities=ents)
 
     def calc_intent(self, query):
         intents = list(self.calc_intents(query))
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
 VERSION_BUILD = 0
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.1.0a1.dist-info/METADATA` & `jurebes-0.1.0a2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

