# Comparing `tmp/spanish_nlp-0.2.8.tar.gz` & `tmp/spanish_nlp-0.2.9.tar.gz`

## Comparing `spanish_nlp-0.2.8.tar` & `spanish_nlp-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/__about__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/__init__.py
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/classifiers.py
--rw-r--r--   0        0        0    17009 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/preprocess.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/__init__.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/abstract.py
--rw-r--r--   0        0        0    12507 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/masked.py
--rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/spelling.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/augmentation/data/misspelled_words.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/__init__,py
--rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/emo_unicode.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/inclusive_words.py
--rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/stopwords.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/src/spanish_nlp/utils/tokenizers.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/LICENSE
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 spanish_nlp-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/__about__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/__init__.py
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/classifiers.py
+-rw-r--r--   0        0        0    17009 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/preprocess.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/augmentation/__init__.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/augmentation/abstract.py
+-rw-r--r--   0        0        0    12507 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/augmentation/masked.py
+-rw-r--r--   0        0        0    25419 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/augmentation/spelling.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/augmentation/data/misspelled_words.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/utils/__init__,py
+-rw-r--r--   0        0        0     9692 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/utils/emo_unicode.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/utils/inclusive_words.py
+-rw-r--r--   0        0        0    11954 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/utils/stopwords.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/src/spanish_nlp/utils/tokenizers.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/LICENSE
+-rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     9201 2020-02-02 00:00:00.000000 spanish_nlp-0.2.9/PKG-INFO
```

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/classifiers.py` & `spanish_nlp-0.2.9/src/spanish_nlp/classifiers.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/preprocess.py` & `spanish_nlp-0.2.9/src/spanish_nlp/preprocess.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/abstract.py` & `spanish_nlp-0.2.9/src/spanish_nlp/augmentation/abstract.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/masked.py` & `spanish_nlp-0.2.9/src/spanish_nlp/augmentation/masked.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/spelling.py` & `spanish_nlp-0.2.9/src/spanish_nlp/augmentation/spelling.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,17 +667,19 @@
         """
         Increase textual data by modifying characters randomly according to the common grapheme_spellings for Spanish
         """
         aug_percent = self.aug_percent
         self.aug_percent = aug_percent / 7
         output_texts = []
         for i in range(num_samples):
-            text = self._grapheme_spelling_augment_(text, 1)
+            text = self._word_spelling_augmentation_(text, 1)
+            text = self._grapheme_spelling_augment_(text[0], 1)
             text = self._keyboard_augment_(text[0], 1)
             text = self._ocr_augment_(text[0], 1)
+            text = self._random_augment_(text[0], 1)
             text = self._remove_punctuation_augment_(text[0], 1)
+            text = self._remove_spaces_augment_(text[0], 1)
             text = self._remove_accents_augmentation_(text[0], 1)
-            text = self._random_augment_(text[0], 1)
             text = self._random_case_augmentation_(text[0], 1)
             output_texts.append(text[0])
         self.aug_percent = aug_percent
         return output_texts
```

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/augmentation/data/misspelled_words.json` & `spanish_nlp-0.2.9/src/spanish_nlp/augmentation/data/misspelled_words.json`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/utils/emo_unicode.py` & `spanish_nlp-0.2.9/src/spanish_nlp/utils/emo_unicode.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/utils/inclusive_words.py` & `spanish_nlp-0.2.9/src/spanish_nlp/utils/inclusive_words.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/src/spanish_nlp/utils/stopwords.py` & `spanish_nlp-0.2.9/src/spanish_nlp/utils/stopwords.py`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/.gitignore` & `spanish_nlp-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/LICENSE` & `spanish_nlp-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/README.md` & `spanish_nlp-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 - Spelling augmentation
   - Keyboard spelling method
   - OCR spelling method
   - Random spelling replace method
   - Grapheme spelling
   - Word spelling
   - Remove punctuation
+  - Remove spaces
   - Remove accents
   - Lowercase
   - Uppercase
   - Randomcase
   - All method
 - Masked augmentation
   - Sustitute method
```

### Comparing `spanish_nlp-0.2.8/pyproject.toml` & `spanish_nlp-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spanish_nlp-0.2.8/PKG-INFO` & `spanish_nlp-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanish_nlp
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for NLP in Spanish
 Project-URL: Homepage, https://github.com/jorgeortizfuentes/spanish_nlp
 Author-email: Jorge Ortiz-Fuentes <jorge@ortizfuentes.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: augmentation,clasificacion,classifier,español,language,lenguaje,nlp,pln,preprocesamiento,preprocess,spanish
 Classifier: Development Status :: 3 - Alpha
@@ -151,14 +151,15 @@
 - Spelling augmentation
   - Keyboard spelling method
   - OCR spelling method
   - Random spelling replace method
   - Grapheme spelling
   - Word spelling
   - Remove punctuation
+  - Remove spaces
   - Remove accents
   - Lowercase
   - Uppercase
   - Randomcase
   - All method
 - Masked augmentation
   - Sustitute method
```

