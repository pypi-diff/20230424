# Comparing `tmp/andtate-0.0.4.tar.gz` & `tmp/andtate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andtate-0.0.4.tar", last modified: Sun Apr 23 11:50:45 2023, max compression
+gzip compressed data, was "andtate-0.0.5.tar", last modified: Mon Apr 24 15:44:15 2023, max compression
```

## Comparing `andtate-0.0.4.tar` & `andtate-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 11:50:45.606596 andtate-0.0.4/
--rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      553 2023-04-23 11:50:45.605448 andtate-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 11:50:45.572346 andtate-0.0.4/andtate/
--rw-rw-rw-   0        0        0     1400 2023-04-23 10:24:00.000000 andtate-0.0.4/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py
--rw-rw-rw-   0        0        0      876 2023-04-23 10:23:38.000000 andtate-0.0.4/andtate/AMDL Linear Regression (Diabetes Dataset).py
--rw-rw-rw-   0        0        0     1558 2023-04-23 10:23:58.000000 andtate-0.0.4/andtate/AMDL Logistic Regression (Iris Dataset).py
--rw-rw-rw-   0        0        0     3299 2023-04-23 10:23:53.000000 andtate-0.0.4/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py
--rw-rw-rw-   0        0        0     1884 2023-04-23 10:23:40.000000 andtate-0.0.4/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py
--rw-rw-rw-   0        0        0     1260 2023-04-23 10:23:51.000000 andtate-0.0.4/andtate/AMDL SVM classifier (Iris Dataset).py
--rw-rw-rw-   0        0        0     1243 2023-04-23 10:23:46.000000 andtate-0.0.4/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py
--rw-rw-rw-   0        0        0     1029 2023-04-23 10:23:49.000000 andtate-0.0.4/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py
--rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.4/andtate/AMDL.py
--rw-rw-rw-   0        0        0      737 2023-04-23 10:46:47.000000 andtate-0.0.4/andtate/NLP Dependency parsing of a given text.py
--rw-rw-rw-   0        0        0     1317 2023-04-23 10:46:38.000000 andtate-0.0.4/andtate/NLP Implement a tri-gram model.py
--rw-rw-rw-   0        0        0      644 2023-04-23 10:46:48.000000 andtate-0.0.4/andtate/NLP Lemmatization.py
--rw-rw-rw-   0        0        0      667 2023-04-23 10:46:32.000000 andtate-0.0.4/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py
--rw-rw-rw-   0        0        0      491 2023-04-23 10:46:51.000000 andtate-0.0.4/andtate/NLP Named Entity Recognition (NER) using spaCy Library.py
--rw-rw-rw-   0        0        0      921 2023-04-23 10:46:44.000000 andtate-0.0.4/andtate/NLP Stemming.py
--rw-rw-rw-   0        0        0     1169 2023-04-23 10:46:46.000000 andtate-0.0.4/andtate/NLP Syntactic parsing of a given text.py
--rw-rw-rw-   0        0        0     2255 2023-04-23 10:46:27.000000 andtate-0.0.4/andtate/NLP Text summarization using NLTK Library.py
--rw-rw-rw-   0        0        0     1178 2023-04-23 10:46:53.000000 andtate-0.0.4/andtate/NLP Text summarization using gensim Library.py
--rw-rw-rw-   0        0        0     2598 2023-04-23 10:46:41.000000 andtate-0.0.4/andtate/NLP Text summarization using spaCy Library.py
--rw-rw-rw-   0        0        0      813 2023-04-23 10:46:28.000000 andtate-0.0.4/andtate/NLP Tokenization using Gensim.py
--rw-rw-rw-   0        0        0      802 2023-04-23 10:46:49.000000 andtate-0.0.4/andtate/NLP Tokenization using NLTK.py
--rw-rw-rw-   0        0        0      710 2023-04-23 10:46:29.000000 andtate-0.0.4/andtate/NLP Tokenization using Python’s split function.py
--rw-rw-rw-   0        0        0      758 2023-04-23 10:46:40.000000 andtate-0.0.4/andtate/NLP Tokenization using Regular Expressions (RegEx).py
--rw-rw-rw-   0        0        0     1062 2023-04-23 10:46:39.000000 andtate-0.0.4/andtate/NLP Tokenization using the spaCy library.py
--rw-rw-rw-   0        0        0    17204 2023-04-23 10:19:53.000000 andtate-0.0.4/andtate/NLP.py
--rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.4/andtate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 11:50:45.599743 andtate-0.0.4/andtate.egg-info/
--rw-rw-rw-   0        0        0      553 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 11:50:45.000000 andtate-0.0.4/andtate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 11:50:45.607595 andtate-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-04-23 11:50:24.000000 andtate-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:44:15.613950 andtate-0.0.5/
+-rw-rw-rw-   0        0        0     1064 2023-04-22 11:08:16.000000 andtate-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      553 2023-04-24 15:44:15.612952 andtate-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 15:44:15.570979 andtate-0.0.5/andtate/
+-rw-rw-rw-   0        0        0     1400 2023-04-23 10:24:00.000000 andtate-0.0.5/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py
+-rw-rw-rw-   0        0        0      876 2023-04-23 10:23:38.000000 andtate-0.0.5/andtate/AMDL Linear Regression (Diabetes Dataset).py
+-rw-rw-rw-   0        0        0     1558 2023-04-23 10:23:58.000000 andtate-0.0.5/andtate/AMDL Logistic Regression (Iris Dataset).py
+-rw-rw-rw-   0        0        0     3299 2023-04-23 10:23:53.000000 andtate-0.0.5/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py
+-rw-rw-rw-   0        0        0     1884 2023-04-23 10:23:40.000000 andtate-0.0.5/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py
+-rw-rw-rw-   0        0        0     1260 2023-04-23 10:23:51.000000 andtate-0.0.5/andtate/AMDL SVM classifier (Iris Dataset).py
+-rw-rw-rw-   0        0        0     1243 2023-04-23 10:23:46.000000 andtate-0.0.5/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py
+-rw-rw-rw-   0        0        0     1029 2023-04-23 10:23:49.000000 andtate-0.0.5/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py
+-rw-rw-rw-   0        0        0    13739 2023-04-22 09:06:22.000000 andtate-0.0.5/andtate/AMDL.py
+-rw-rw-rw-   0        0        0      737 2023-04-23 10:46:47.000000 andtate-0.0.5/andtate/NLP Dependency parsing of a given text.py
+-rw-rw-rw-   0        0        0     1317 2023-04-23 10:46:38.000000 andtate-0.0.5/andtate/NLP Implement a tri-gram model.py
+-rw-rw-rw-   0        0        0      644 2023-04-23 10:46:48.000000 andtate-0.0.5/andtate/NLP Lemmatization.py
+-rw-rw-rw-   0        0        0      667 2023-04-23 10:46:32.000000 andtate-0.0.5/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py
+-rw-rw-rw-   0        0        0      491 2023-04-23 10:46:51.000000 andtate-0.0.5/andtate/NLP Named Entity Recognition (NER) using spaCy Library.py
+-rw-rw-rw-   0        0        0     4729 2023-04-24 15:26:06.000000 andtate-0.0.5/andtate/NLP POS tagging using HMM.py
+-rw-rw-rw-   0        0        0      921 2023-04-23 10:46:44.000000 andtate-0.0.5/andtate/NLP Stemming.py
+-rw-rw-rw-   0        0        0     1169 2023-04-23 10:46:46.000000 andtate-0.0.5/andtate/NLP Syntactic parsing of a given text.py
+-rw-rw-rw-   0        0        0     2255 2023-04-23 10:46:27.000000 andtate-0.0.5/andtate/NLP Text summarization using NLTK Library.py
+-rw-rw-rw-   0        0        0     1178 2023-04-23 10:46:53.000000 andtate-0.0.5/andtate/NLP Text summarization using gensim Library.py
+-rw-rw-rw-   0        0        0     2598 2023-04-23 10:46:41.000000 andtate-0.0.5/andtate/NLP Text summarization using spaCy Library.py
+-rw-rw-rw-   0        0        0      813 2023-04-23 10:46:28.000000 andtate-0.0.5/andtate/NLP Tokenization using Gensim.py
+-rw-rw-rw-   0        0        0      802 2023-04-23 10:46:49.000000 andtate-0.0.5/andtate/NLP Tokenization using NLTK.py
+-rw-rw-rw-   0        0        0      710 2023-04-23 10:46:29.000000 andtate-0.0.5/andtate/NLP Tokenization using Python’s split function.py
+-rw-rw-rw-   0        0        0      758 2023-04-23 10:46:40.000000 andtate-0.0.5/andtate/NLP Tokenization using Regular Expressions (RegEx).py
+-rw-rw-rw-   0        0        0     1062 2023-04-23 10:46:39.000000 andtate-0.0.5/andtate/NLP Tokenization using the spaCy library.py
+-rw-rw-rw-   0        0        0    21939 2023-04-24 15:42:21.000000 andtate-0.0.5/andtate/NLP.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 10:15:55.000000 andtate-0.0.5/andtate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:44:15.608959 andtate-0.0.5/andtate.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1488 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 15:44:13.000000 andtate-0.0.5/andtate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 15:44:15.613950 andtate-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-24 15:43:38.000000 andtate-0.0.5/setup.py
```

### Comparing `andtate-0.0.4/LICENSE` & `andtate-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/PKG-INFO` & `andtate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.4
+Version: 0.0.5
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.4/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py` & `andtate-0.0.5/andtate/AMDL Batch Gradient Descent with early stopping for Softmax Regression.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL Linear Regression (Diabetes Dataset).py` & `andtate-0.0.5/andtate/AMDL Linear Regression (Diabetes Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL Logistic Regression (Iris Dataset).py` & `andtate-0.0.5/andtate/AMDL Logistic Regression (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py` & `andtate-0.0.5/andtate/AMDL MLP for classification of handwritten digits (MNIST Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py` & `andtate-0.0.5/andtate/AMDL Multinomial Logistic Regression (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL SVM classifier (Iris Dataset).py` & `andtate-0.0.5/andtate/AMDL SVM classifier (Iris Dataset).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py` & `andtate-0.0.5/andtate/AMDL Train an SVM regressor on the California Housing Dataset.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py` & `andtate-0.0.5/andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/AMDL.py` & `andtate-0.0.5/andtate/AMDL.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Dependency parsing of a given text.py` & `andtate-0.0.5/andtate/NLP Dependency parsing of a given text.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Implement a tri-gram model.py` & `andtate-0.0.5/andtate/NLP Implement a tri-gram model.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Lemmatization.py` & `andtate-0.0.5/andtate/NLP Lemmatization.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py` & `andtate-0.0.5/andtate/NLP Named Entity Recognition (NER) using NLTK Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Stemming.py` & `andtate-0.0.5/andtate/NLP Stemming.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Syntactic parsing of a given text.py` & `andtate-0.0.5/andtate/NLP Syntactic parsing of a given text.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Text summarization using NLTK Library.py` & `andtate-0.0.5/andtate/NLP Text summarization using NLTK Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Text summarization using gensim Library.py` & `andtate-0.0.5/andtate/NLP Text summarization using gensim Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Text summarization using spaCy Library.py` & `andtate-0.0.5/andtate/NLP Text summarization using spaCy Library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Tokenization using Gensim.py` & `andtate-0.0.5/andtate/NLP Tokenization using Gensim.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Tokenization using NLTK.py` & `andtate-0.0.5/andtate/NLP Tokenization using NLTK.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Tokenization using Python’s split function.py` & `andtate-0.0.5/andtate/NLP Tokenization using Python’s split function.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Tokenization using Regular Expressions (RegEx).py` & `andtate-0.0.5/andtate/NLP Tokenization using Regular Expressions (RegEx).py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP Tokenization using the spaCy library.py` & `andtate-0.0.5/andtate/NLP Tokenization using the spaCy library.py`

 * *Files identical despite different names*

### Comparing `andtate-0.0.4/andtate/NLP.py` & `andtate-0.0.5/andtate/NLP.py`

 * *Files 19% similar despite different names*

```diff
@@ -188,14 +188,165 @@
       sentence_finished = True
  
 print (' '.join([t for t in text if t]))
 
 ################### Write a program to Implement a POS tagging using HMM ###################
 ################### P4 ###################
 
+
+import nltk
+import numpy as np
+import pandas as pd
+import random
+from sklearn.model_selection import train_test_split
+from IPython.display import display
+import pprint, time
+
+nltk.download('treebank')
+nltk.download('universal_tagset')
+
+nltk_data = list(nltk.corpus.treebank.tagged_sents(tagset='universal'))
+print("\n")
+print(nltk_data[:2])
+print("\n")
+for sent in nltk_data[:2]:
+  for tuple in sent:
+    print(tuple)
+print("\n")
+train_set,test_set =train_test_split(nltk_data,train_size=0.80,test_size=0.20,random_state = 101)
+
+train_tagged_words = [ tup for sent in train_set for tup in sent ]
+test_tagged_words = [ tup for sent in test_set for tup in sent ]
+print(len(train_tagged_words))
+print(len(test_tagged_words))
+print("\n")
+
+train_tagged_words[:5]
+print("\n")
+
+tags = {tag for word,tag in train_tagged_words}
+print(len(tags))
+print(tags)
+
+vocab = {word for word,tag in train_tagged_words}
+
+def word_given_tag(word, tag, train_bag = train_tagged_words):
+    tag_list = [pair for pair in train_bag if pair[1]==tag]
+    count_tag = len(tag_list)
+    w_given_tag_list = [pair[0] for pair in tag_list if pair[0]==word]
+    count_w_given_tag = len(w_given_tag_list)
+    return (count_w_given_tag, count_tag)
+
+def t2_given_t1(t2, t1, train_bag = train_tagged_words):
+    tags = [pair[1] for pair in train_bag]
+    count_t1 = len([t for t in tags if t==t1])
+    count_t2_t1 = 0
+    for index in range(len(tags)-1):
+        if tags[index]==t1 and tags[index+1] == t2:
+            count_t2_t1 += 1
+    return (count_t2_t1, count_t1)
+
+print("\n")
+tags_matrix = np.zeros((len(tags), len(tags)), dtype='float32')
+for i, t1 in enumerate(list(tags)):
+    for j, t2 in enumerate(list(tags)): 
+        tags_matrix[i, j] = t2_given_t1(t2, t1)[0]/t2_given_t1(t2, t1)[1]
+ 
+print(tags_matrix)
+print("\n")
+
+tags_df = pd.DataFrame(tags_matrix, columns = list(tags), index=list(tags))
+display(tags_df)
+
+def Viterbi(words, train_bag = train_tagged_words):
+    state = []
+    T = list(set([pair[1] for pair in train_bag]))
+     
+    for key, word in enumerate(words):
+        p = [] 
+        for tag in T:
+            if key == 0:
+                transition_p = tags_df.loc['.', tag]
+            else:
+                transition_p = tags_df.loc[state[-1], tag]
+            emission_p = word_given_tag(words[key], tag)[0]/word_given_tag(words[key], tag)[1]
+            state_probability = emission_p * transition_p    
+            p.append(state_probability)
+             
+        pmax = max(p)
+        state_max = T[p.index(pmax)] 
+        state.append(state_max)
+    return list(zip(words, state))
+
+random.seed(1234)
+rndom = [random.randint(1,len(test_set)) for x in range(10)]
+test_run = [test_set[i] for i in rndom]
+test_run_base = [tup for sent in test_run for tup in sent]
+test_tagged_words = [tup[0] for sent in test_run for tup in sent]
+
+print("\n")
+start = time.time()
+tagged_seq = Viterbi(test_tagged_words)
+end = time.time()
+difference = end-start
+print("Time taken in seconds: ", difference)
+check = [i for i, j in zip(tagged_seq, test_run_base) if i == j] 
+accuracy = len(check)/len(tagged_seq)
+print('Viterbi Algorithm Accuracy: ',accuracy*100)
+
+patterns = [
+    (r'.*ing$', 'VERB'),
+    (r'.*ed$', 'VERB'),
+    (r'.*es$', 'VERB'), 
+    (r'.*\'s$', 'NOUN'),
+    (r'.*s$', 'NOUN'),
+    (r'\*T?\*?-[0-9]+$', 'X'),
+    (r'^-?[0-9]+(.[0-9]+)?$', 'NUM'),
+    (r'.*', 'NOUN')
+]
+
+rule_based_tagger = nltk.RegexpTagger(patterns)
+
+def Viterbi_rule_based(words, train_bag = train_tagged_words):
+    state = []
+    T = list(set([pair[1] for pair in train_bag]))
+     
+    for key, word in enumerate(words):
+        p = [] 
+        for tag in T:
+            if key == 0:
+                transition_p = tags_df.loc['.', tag]
+            else:
+                transition_p = tags_df.loc[state[-1], tag]
+            emission_p = word_given_tag(words[key], tag)[0]/word_given_tag(words[key], tag)[1]
+            state_probability = emission_p * transition_p    
+            p.append(state_probability)
+             
+        pmax = max(p)
+        state_max = rule_based_tagger.tag([word])[0][1]       
+        
+         
+        if(pmax==0):
+            state_max = rule_based_tagger.tag([word])[0][1]
+        else:
+            if state_max != 'X':
+                state_max = T[p.index(pmax)]                
+             
+         
+        state.append(state_max)
+    return list(zip(words, state))
+
+print("\n")
+test_sent="Will can see Marry"
+pred_tags_rule=Viterbi_rule_based(test_sent.split())
+pred_tags_withoutRules= Viterbi(test_sent.split())
+print(pred_tags_rule)
+print(pred_tags_withoutRules)
+
+
 ################### Write a program to Implement syntactic parsing of a given text ###################
 ################### P5 ###################
 
 
 # Import required libraries
 import nltk
 nltk.download('punkt')          #pre-trained Punkt tokenizer, which is used to tokenize the words.
```

### Comparing `andtate-0.0.4/andtate.egg-info/PKG-INFO` & `andtate-0.0.5/andtate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andtate
-Version: 0.0.4
+Version: 0.0.5
 Summary: andtate
 Author: AndTate
 Author-email: andtateandtate@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `andtate-0.0.4/andtate.egg-info/SOURCES.txt` & `andtate-0.0.5/andtate.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 andtate/AMDL Train and fine-tune a Decision Tree for the Moons Dataset.py
 andtate/AMDL.py
 andtate/NLP Dependency parsing of a given text.py
 andtate/NLP Implement a tri-gram model.py
 andtate/NLP Lemmatization.py
 andtate/NLP Named Entity Recognition (NER) using NLTK Library.py
 andtate/NLP Named Entity Recognition (NER) using spaCy Library.py
+andtate/NLP POS tagging using HMM.py
 andtate/NLP Stemming.py
 andtate/NLP Syntactic parsing of a given text.py
 andtate/NLP Text summarization using NLTK Library.py
 andtate/NLP Text summarization using gensim Library.py
 andtate/NLP Text summarization using spaCy Library.py
 andtate/NLP Tokenization using Gensim.py
 andtate/NLP Tokenization using NLTK.py
```

### Comparing `andtate-0.0.4/setup.py` & `andtate-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'andtate'
 LONG_DESCRIPTION = 'Finding Glitches And Loop Holes In Matrix And Trying To Break The System'
 
 # Setting up
 setup(
     name="andtate",
     version=VERSION,
```

