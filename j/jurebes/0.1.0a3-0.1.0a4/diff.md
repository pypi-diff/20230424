# Comparing `tmp/jurebes-0.1.0a3-py3-none-any.whl.zip` & `tmp/jurebes-0.1.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4857 bytes, number of entries: 7
--rw-r--r--  2.0 unx    13678 b- defN 23-Apr-24 11:13 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 11:13 jurebes/version.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 11:13 jurebes-0.1.0a3.dist-info/RECORD
-7 files, 15252 bytes uncompressed, 3889 bytes compressed:  74.5%
+Zip file size: 4934 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    14267 b- defN 23-Apr-24 11:19 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 11:19 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 11:19 jurebes-0.1.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 11:19 jurebes-0.1.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 11:19 jurebes-0.1.0a4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 11:19 jurebes-0.1.0a4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 11:19 jurebes-0.1.0a4.dist-info/RECORD
+7 files, 15841 bytes uncompressed, 3966 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.1.0a3.dist-info/METADATA
+Filename: jurebes-0.1.0a4.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.1.0a3.dist-info/WHEEL
+Filename: jurebes-0.1.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.1.0a3.dist-info/top_level.txt
+Filename: jurebes-0.1.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.1.0a3.dist-info/zip-safe
+Filename: jurebes-0.1.0a4.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.1.0a3.dist-info/RECORD
+Filename: jurebes-0.1.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -39,14 +39,15 @@
             self.tagger = SklearnOVOSClassifierTagger(tagger, tagger_pipeline)
         self.intent_samples, self.entity_samples = {}, {}
         self.available_contexts = {}
         self.required_contexts = {}
         self.excluded_keywords = {}
         self.excluded_contexts = {}
         self.detached_intents = []
+        self.detached_entities = []
 
     def enable_fuzzy(self):
         self.padacioso.fuzz = True
 
     def disable_fuzzy(self):
         self.padacioso.fuzz = False
 
@@ -59,14 +60,22 @@
         if intent_name not in self.detached_intents:
             self.detached_intents.append(intent_name)
 
     def reatach_intent(self, intent_name):
         if intent_name in self.detached_intents:
             self.detached_intents.remove(intent_name)
 
+    def detach_entity(self, entity_name):
+        if entity_name not in self.detached_entities:
+            self.detached_entities.append(entity_name)
+
+    def reatach_entity(self, entity_name):
+        if entity_name in self.detached_entities:
+            self.detached_entities.remove(entity_name)
+
     def exclude_keywords(self, intent_name, samples):
         if intent_name not in self.excluded_keywords:
             self.excluded_keywords[intent_name] = samples
         else:
             self.excluded_keywords[intent_name] += samples
 
     def set_context(self, intent_name, context_name, context_val=None):
@@ -98,24 +107,26 @@
 
     def unrequire_context(self, intent_name, context_name):
         if intent_name in self.required_contexts:
             self.required_contexts[intent_name] = [c for c in self.required_contexts[intent_name]
                                                    if context_name != c]
 
     def remove_intent(self, intent_name):
+        self.detach_intent(intent_name)
         self.padacioso.remove_intent(intent_name)
         if intent_name in self.intent_samples:
             del self.intent_samples[intent_name]
 
     def add_entity(self, entity_name, samples):
         samples = [l.lower() for l in samples]
         self.padacioso.add_entity(entity_name, samples)
         self.entity_samples[entity_name] = samples
 
     def remove_entity(self, entity_name):
+        self.detach_entity(entity_name)
         self.padacioso.remove_entity(entity_name)
         if entity_name in self.entity_samples:
             del self.entity_samples[entity_name]
 
     def get_entities(self, query):
         entities = {}
         in_entity = False
@@ -164,20 +175,22 @@
         ents = self.get_entities(query)
 
         for exact_intent in self.padacioso.calc_intents(query):
             if exact_intent["name"]:
                 if exact_intent["name"] in excluded_intents:
                     continue
                 ents.update(exact_intent["entities"])
+                ents = {k: v for k, v in ents.items() if k not in self.detached_entities}
                 yield IntentMatch(confidence=exact_intent["conf"],
                                   intent_name=exact_intent["name"],
                                   entities=ents)
 
         probs = self.classifier.clf.predict_proba([query])[0]
         classes = self.classifier.clf.classes_
+        ents = {k: v for k, v in ents.items() if k not in self.detached_entities}
 
         for intent, prob in zip(classes, probs):
             if intent in excluded_intents:
                 continue
             if intent in self.available_contexts:
                 for context, val in self.available_contexts[intent].items():
                     if val is not None:
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
 VERSION_BUILD = 0
-VERSION_ALPHA = 3
+VERSION_ALPHA = 4
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.1.0a3.dist-info/METADATA` & `jurebes-0.1.0a4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `jurebes-0.1.0a3.dist-info/RECORD` & `jurebes-0.1.0a4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-jurebes/__init__.py,sha256=kpQTVAcYIkrqqA0GSdNCXxtB-tOisKBzYZBWco70SF4,13678
-jurebes/version.py,sha256=TPUc4tX9vfV0rY4QrxWq5dYC9bCZ0x0PHiyBtSqxX2g,177
-jurebes-0.1.0a3.dist-info/METADATA,sha256=ddoumV569E9COFblaBdh8z250LLWyZeWeRka0_wSIwE,753
-jurebes-0.1.0a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-jurebes-0.1.0a3.dist-info/top_level.txt,sha256=skXuo7YYkUuI3qzkaJUFtHRIf9MgjyABZuwIDsxC5xw,8
-jurebes-0.1.0a3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-jurebes-0.1.0a3.dist-info/RECORD,,
+jurebes/__init__.py,sha256=LnYvP88BXlMslTsX7MrB_japtJ-MZvCTGjyg7KTl7Z8,14267
+jurebes/version.py,sha256=evG3_hDv9Mt1wugomGynwVj6EZ_F5nw07QoOFlv6tPw,177
+jurebes-0.1.0a4.dist-info/METADATA,sha256=beIPYme1AISnWYqdjZUHVzgJx9ZSPSOtagz-tIV0gNo,753
+jurebes-0.1.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+jurebes-0.1.0a4.dist-info/top_level.txt,sha256=skXuo7YYkUuI3qzkaJUFtHRIf9MgjyABZuwIDsxC5xw,8
+jurebes-0.1.0a4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+jurebes-0.1.0a4.dist-info/RECORD,,
```

