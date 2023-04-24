# Comparing `tmp/jurebes-0.0.1a1-py3-none-any.whl.zip` & `tmp/jurebes-0.0.1a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4168 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8873 b- defN 23-Apr-24 06:45 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 06:45 jurebes/version.py
--rw-r--r--  2.0 unx      733 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      542 b- defN 23-Apr-24 06:45 jurebes-0.0.1a1.dist-info/RECORD
-7 files, 10426 bytes uncompressed, 3200 bytes compressed:  69.3%
+Zip file size: 4733 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    12314 b- defN 23-Apr-24 10:05 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 10:05 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-24 10:05 jurebes-0.0.1a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 10:05 jurebes-0.0.1a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-24 10:05 jurebes-0.0.1a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 10:05 jurebes-0.0.1a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-24 10:05 jurebes-0.0.1a2.dist-info/RECORD
+7 files, 13888 bytes uncompressed, 3765 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.0.1a1.dist-info/METADATA
+Filename: jurebes-0.0.1a2.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.0.1a1.dist-info/WHEEL
+Filename: jurebes-0.0.1a2.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.0.1a1.dist-info/top_level.txt
+Filename: jurebes-0.0.1a2.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.0.1a1.dist-info/zip-safe
+Filename: jurebes-0.0.1a2.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.0.1a1.dist-info/RECORD
+Filename: jurebes-0.0.1a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -33,35 +33,65 @@
             self.tagger = OVOSNgramTagger(default_tag="O")
         elif isinstance(tagger, list):
             self.tagger = SklearnOVOSVotingClassifierTagger(tagger, tagger_pipeline)
         elif isinstance(tagger, OVOSNgramTagger):
             self.tagger = tagger
         else:
             self.tagger = SklearnOVOSClassifierTagger(tagger, tagger_pipeline)
-        self.intent_lines, self.entity_lines = {}, {}
+        self.intent_samples, self.entity_samples = {}, {}
+        self.available_contexts = {}
+        self.required_contexts = {}
+        self.excluded_keywords = {}
+
+    def add_intent(self, intent_name, samples):
+        samples = [l.lower() for l in samples]
+        self.padacioso.add_intent(intent_name, samples)
+        self.intent_samples[intent_name] = samples
+
+    def exclude_keywords(self, intent_name, samples):
+        if intent_name not in self.excluded_keywords:
+            self.excluded_keywords[intent_name] = samples
+        else:
+            self.excluded_keywords[intent_name] += samples
+
+    def set_context(self, intent_name, context_name, context_val=None):
+        if intent_name not in self.available_contexts:
+            self.available_contexts[intent_name] = {}
+        self.available_contexts[intent_name][context_name] = context_val
+
+    def unset_context(self, intent_name, context_name):
+        if intent_name in self.available_contexts:
+            if context_name in self.available_contexts[intent_name]:
+                self.available_contexts[intent_name].pop(context_name)
+
+    def require_context(self, intent_name, context_name):
+        if intent_name not in self.required_contexts:
+            self.required_contexts[intent_name] = [context_name]
+        else:
+            self.required_contexts[intent_name].append(context_name)
 
-    def add_intent(self, name, lines):
-        lines = [l.lower() for l in lines]
-        self.padacioso.add_intent(name, lines)
-        self.intent_lines[name] = lines
-
-    def remove_intent(self, name):
-        self.padacioso.remove_intent(name)
-        if name in self.intent_lines:
-            del self.intent_lines[name]
-
-    def add_entity(self, name, lines):
-        lines = [l.lower() for l in lines]
-        self.padacioso.add_entity(name, lines)
-        self.entity_lines[name] = lines
-
-    def remove_entity(self, name):
-        self.padacioso.remove_entity(name)
-        if name in self.entity_lines:
-            del self.entity_lines[name]
+    def unrequire_context(self, intent_name, context_name):
+        if intent_name in self.required_contexts:
+            self.required_contexts[intent_name] = [c for c in self.required_contexts[intent_name]
+                                                   if context_name != c]
+
+    def remove_intent(self, intent_name):
+        self.padacioso.remove_intent(intent_name)
+        if intent_name in self.intent_samples:
+            del self.intent_samples[intent_name]
+
+    def add_entity(self, entity_name, samples):
+        samples = [l.lower() for l in samples]
+        self.padacioso.add_entity(entity_name, samples)
+        self.entity_samples[entity_name] = samples
+
+    def remove_entity(self, entity_name):
+        self.padacioso.remove_entity(entity_name)
+        if entity_name in self.entity_samples:
+            del self.entity_samples[entity_name]
 
     def get_entities(self, query):
         entities = {}
         in_entity = False
         if isinstance(self.tagger, OVOSNgramTagger):
             tags = self.tagger.tag(query)
         else:
@@ -81,25 +111,48 @@
             elif in_entity:
                 entities[ent_name] += " " + word
 
         return entities
 
     def calc_intents(self, query):
         query = query.lower()
+
+        excluded_intents = []
+        for intent_name, samples in self.excluded_keywords.items():
+            if any(s in query for s in samples):
+                excluded_intents.append(intent_name)
+        for intent_name, contexts in self.required_contexts.items():
+            if intent_name not in self.available_contexts:
+                excluded_intents.append(intent_name)
+            elif any(context not in self.available_contexts[intent_name]
+                     for context in contexts):
+                excluded_intents.append(intent_name)
+
+        # print("excluded intents:", excluded_intents)
+
         for exact_intent in self.padacioso.calc_intents(query):
             if exact_intent["name"]:
                 yield IntentMatch(confidence=exact_intent["conf"],
                                   intent_name=exact_intent["name"],
                                   entities=exact_intent["entities"])
 
-        prob = self.classifier.predict_proba([query])[0]
-        intent = self.classifier.predict([query])[0]
-        yield IntentMatch(confidence=prob,
-                          intent_name=intent,
-                          entities=self.get_entities(query))
+        probs = self.classifier.clf.predict_proba([query])[0]
+        classes = self.classifier.clf.classes_
+        ents = self.get_entities(query)
+
+        for intent, prob in zip(classes, probs):
+            if intent in excluded_intents:
+                continue
+            if intent in self.available_contexts:
+                for context, val in self.available_contexts[intent].items():
+                    ents[context] = val
+
+            yield IntentMatch(confidence=prob,
+                              intent_name=intent,
+                              entities=ents)
 
     def calc_intent(self, query):
         intents = list(self.calc_intents(query))
         if len(intents):
             return max(intents, key=lambda k: k.confidence)
         return None
 
@@ -126,57 +179,57 @@
             self.tagger.train(X, y)
 
     def get_dataset(self):
         X = []
         y = []
 
         def expand(sample, intent):
-            for entity in self.entity_lines:
+            for entity in self.entity_samples:
                 tok = "{" + entity + "}"
                 if tok not in sample:
                     continue
-                for s in self.entity_lines[entity]:
+                for s in self.entity_samples[entity]:
                     X.append(sample.replace(tok, s))
                     y.append(intent)
 
-        for intent, samples in self.intent_lines.items():
-            for s in self.intent_lines[intent]:
+        for intent, samples in self.intent_samples.items():
+            for s in self.intent_samples[intent]:
                 if "{" in s:
                     expand(s, intent)
                 else:
                     X.append(s.lower())
                     y.append(intent)
         return X, y
 
     def get_iob_dataset(self):
         X = []
 
         def expand(sample):
             toks = sample.split(" ")
 
-            for entity in self.entity_lines:
+            for entity in self.entity_samples:
                 tok = "{" + entity + "}"
                 if tok not in toks:
                     continue
-                for s in self.entity_lines[entity]:
+                for s in self.entity_samples[entity]:
                     idx = toks.index(tok)
                     nt = word_tokenize(s)
 
                     pt1 = toks[:idx]
                     pt2 = toks[idx + 1:]
                     toks2 = pt1 + nt + pt2
                     if len(nt) == 1:
                         iob2 = ["O"] * len(pt1) + [f"B-{entity}"] + ["O"] * len(pt2)
                     else:
                         iob2 = ["O"] * len(pt1) + [f"B-{entity}"] + [f"I-{entity}"] * (len(nt) - 1) + ["O"] * len(pt2)
 
                     X.append(list(zip(toks2, iob2)))
 
-        for intent, samples in self.intent_lines.items():
-            for s in self.intent_lines[intent]:
+        for intent, samples in self.intent_samples.items():
+            for s in self.intent_samples[intent]:
                 toks = word_tokenize(s)
                 if "{" in s:
                     expand(s)
                 else:
                     iob = ["O"] * len(toks)
                     X.append(list(zip(toks, iob)))
 
@@ -226,7 +279,27 @@
     # they call me Ana Ferreira IntentMatch(intent_name='name', confidence=0.8599902513687149, entities={'name': 'ferreira'})
     # hello beautiful IntentMatch(intent_name='hello', confidence=0.8475377118056997, entities={})
     # hello bob IntentMatch(intent_name='hello', confidence=0.5025161990154762, entities={'name': 'bob'})
     # hello world IntentMatch(intent_name='hello', confidence=0.8475377118056997, entities={})
     # say joke IntentMatch(intent_name='joke', confidence=0.9785338275012387, entities={})
     # make me laugh IntentMatch(intent_name='name', confidence=0.6135639618555918, entities={})
     # do you know any joke IntentMatch(intent_name='joke', confidence=0.9785338275012387, entities={})
+
+    # force correct prediction
+    engine.exclude_keywords("name", ["laugh"])
+    engine.exclude_keywords("hello", ["laugh"])
+    print(engine.calc_intent("make me laugh"))
+    # IntentMatch(intent_name='joke', confidence=0.13906218566700498, entities={})
+
+    # inject entities
+    engine.set_context("joke", "joke_type", "chuck_norris")
+    print(engine.calc_intent("tell me a chuch norris joke"))
+    # IntentMatch(intent_name='joke', confidence=0.9707841337857908, entities={'joke_type': 'chuck_norris'})
+
+    # require entities
+    engine.require_context("joke", "joke_type")
+    engine.unset_context("joke", "joke_type")
+    print(engine.calc_intent("tell me a chuch norris joke"))
+    # IntentMatch(intent_name='hello', confidence=0.060199275248566525, entities={})
+    engine.unrequire_context("joke", "joke_type")
+    print(engine.calc_intent("tell me a chuch norris joke"))
+    # IntentMatch(intent_name='joke', confidence=0.9462089582801377, entities={})
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 1
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.0.1a1.dist-info/METADATA` & `jurebes-0.0.1a2.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -14,11 +14,12 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: ovos-utils
 Requires-Dist: ovos-classifiers[sklearn] (>=0.0.0a1)
 Requires-Dist: padacioso
 Requires-Dist: quebra-frases
+Requires-Dist: nltk
 
 UNKNOWN
```

