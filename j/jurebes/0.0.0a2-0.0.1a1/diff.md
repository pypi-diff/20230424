# Comparing `tmp/jurebes-0.0.0a2-py3-none-any.whl.zip` & `tmp/jurebes-0.0.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4148 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8833 b- defN 23-Apr-24 05:24 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 05:24 jurebes/version.py
--rw-r--r--  2.0 unx      733 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      542 b- defN 23-Apr-24 05:24 jurebes-0.0.0a2.dist-info/RECORD
-7 files, 10386 bytes uncompressed, 3180 bytes compressed:  69.4%
+Zip file size: 4168 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8873 b- defN 23-Apr-24 06:45 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 06:45 jurebes/version.py
+-rw-r--r--  2.0 unx      733 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      542 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/RECORD
+7 files, 10426 bytes uncompressed, 3200 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.0.0a2.dist-info/METADATA
+Filename: jurebes-0.0.1a1.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.0.0a2.dist-info/WHEEL
+Filename: jurebes-0.0.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.0.0a2.dist-info/top_level.txt
+Filename: jurebes-0.0.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.0.0a2.dist-info/zip-safe
+Filename: jurebes-0.0.1a1.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.0.0a2.dist-info/RECORD
+Filename: jurebes-0.0.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -14,19 +14,19 @@
 class IntentMatch:
     intent_name: str
     confidence: float
     entities: dict
 
 
 class JurebesIntentContainer:
-    def __init__(self, clf=None, tagger=None, pipeline="tfidf_lemma", tagger_pipeline="naive"):
+    def __init__(self, clf=None, tagger=None, pipeline="tfidf_lemma", tagger_pipeline="naive", fuzzy=False):
         clf = clf or [SVC(probability=True),
                       LogisticRegression(),
                       DecisionTreeClassifier()]
-        self.padacioso = PadaciosoIntentContainer()
+        self.padacioso = PadaciosoIntentContainer(fuzz=fuzzy)
 
         if isinstance(clf, list):
             self.classifier = SklearnOVOSVotingClassifier(clf, pipeline)
         else:
             self.classifier = SklearnOVOSClassifier(pipeline, clf)
 
         if tagger is None:
@@ -83,15 +83,15 @@
 
         return entities
 
     def calc_intents(self, query):
         query = query.lower()
         for exact_intent in self.padacioso.calc_intents(query):
             if exact_intent["name"]:
-                yield IntentMatch(confidence=1.0,
+                yield IntentMatch(confidence=exact_intent["conf"],
                                   intent_name=exact_intent["name"],
                                   entities=exact_intent["entities"])
 
         prob = self.classifier.predict_proba([query])[0]
         intent = self.classifier.predict([query])[0]
         yield IntentMatch(confidence=prob,
                           intent_name=intent,
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
-VERSION_BUILD = 0
-VERSION_ALPHA = 2
+VERSION_BUILD = 1
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.0.0a2.dist-info/METADATA` & `jurebes-0.0.1a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.0.0a2
+Version: 0.0.1a1
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

