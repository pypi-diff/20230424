# Comparing `tmp/jurebes-0.1.0a2-py3-none-any.whl.zip` & `tmp/jurebes-0.1.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4730 bytes, number of entries: 7
--rw-r--r--  2.0 unx    12950 b- defN 23-Apr-24 10:52 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 10:52 jurebes/version.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 10:52 jurebes-0.1.0a2.dist-info/RECORD
-7 files, 14524 bytes uncompressed, 3762 bytes compressed:  74.1%
+Zip file size: 4857 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    13678 b- defN 23-Apr-24 11:13 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 11:13 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/RECORD
+7 files, 15252 bytes uncompressed, 3889 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.1.0a2.dist-info/METADATA
+Filename: jurebes-0.1.0a3.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.1.0a2.dist-info/WHEEL
+Filename: jurebes-0.1.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.1.0a2.dist-info/top_level.txt
+Filename: jurebes-0.1.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.1.0a2.dist-info/zip-safe
+Filename: jurebes-0.1.0a3.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.1.0a2.dist-info/RECORD
+Filename: jurebes-0.1.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -38,26 +38,35 @@
         else:
             self.tagger = SklearnOVOSClassifierTagger(tagger, tagger_pipeline)
         self.intent_samples, self.entity_samples = {}, {}
         self.available_contexts = {}
         self.required_contexts = {}
         self.excluded_keywords = {}
         self.excluded_contexts = {}
+        self.detached_intents = []
 
     def enable_fuzzy(self):
         self.padacioso.fuzz = True
 
     def disable_fuzzy(self):
         self.padacioso.fuzz = False
 
     def add_intent(self, intent_name, samples):
         samples = [l.lower() for l in samples]
         self.padacioso.add_intent(intent_name, samples)
         self.intent_samples[intent_name] = samples
 
+    def detach_intent(self, intent_name):
+        if intent_name not in self.detached_intents:
+            self.detached_intents.append(intent_name)
+
+    def reatach_intent(self, intent_name):
+        if intent_name in self.detached_intents:
+            self.detached_intents.remove(intent_name)
+
     def exclude_keywords(self, intent_name, samples):
         if intent_name not in self.excluded_keywords:
             self.excluded_keywords[intent_name] = samples
         else:
             self.excluded_keywords[intent_name] += samples
 
     def set_context(self, intent_name, context_name, context_val=None):
@@ -130,15 +139,15 @@
                 entities[ent_name] += " " + word
 
         return entities
 
     def calc_intents(self, query):
         query = query.lower()
 
-        excluded_intents = []
+        excluded_intents = self.detached_intents
         for intent_name, samples in self.excluded_keywords.items():
             if any(s in query for s in samples):
                 excluded_intents.append(intent_name)
         for intent_name, contexts in self.required_contexts.items():
             if intent_name not in self.available_contexts:
                 excluded_intents.append(intent_name)
             elif any(context not in self.available_contexts[intent_name]
@@ -316,7 +325,15 @@
     engine.enable_fuzzy()
     sent = "they call me Ana Ferreira"
     print(engine.calc_intent(sent))
     # IntentMatch(intent_name='name', confidence=0.8716633619210677, entities={'name': 'ana ferreira'})
     engine.disable_fuzzy()
     print(engine.calc_intent(sent))
     # IntentMatch(intent_name='name', confidence=0.8282293617609358, entities={'name': 'ferreira'})
+
+    # temporarily disable a intent
+    engine.detach_intent("name")
+    print(engine.calc_intent(sent))
+    # IntentMatch(intent_name='hello', confidence=0.06113697262028985, entities={'name': 'ferreira'})
+    engine.reatach_intent("name")
+    print(engine.calc_intent(sent))
+    # IntentMatch(intent_name='name', confidence=0.8548664325189478, entities={'name': 'ferreira'})
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
 VERSION_BUILD = 0
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.1.0a2.dist-info/METADATA` & `jurebes-0.1.0a3.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

