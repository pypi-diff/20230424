# Comparing `tmp/html4quiz-0.0.36.tar.gz` & `tmp/html4quiz-0.0.37.tar.gz`

## Comparing `html4quiz-0.0.36.tar` & `html4quiz-0.0.37.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 html4quiz-0.0.36/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.36/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.36/src/html4quiz/_common.py
--rw-r--r--   0        0        0    29328 2020-02-02 00:00:00.000000 html4quiz-0.0.36/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.36/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.36/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.36/LICENSE.txt
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 html4quiz-0.0.36/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 html4quiz-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 html4quiz-0.0.37/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.37/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.37/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    29328 2020-02-02 00:00:00.000000 html4quiz-0.0.37/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.37/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.37/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.37/LICENSE.txt
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 html4quiz-0.0.37/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 html4quiz-0.0.37/PKG-INFO
```

### Comparing `html4quiz-0.0.36/updatePackage.txt` & `html4quiz-0.0.37/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.36/src/html4quiz/_common.py` & `html4quiz-0.0.37/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.36/src/html4quiz/_generateEm.py` & `html4quiz-0.0.37/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.36/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.37/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.36/src/html4quiz/makeChoices.py` & `html4quiz-0.0.37/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.36/LICENSE.txt` & `html4quiz-0.0.37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.36/README.md` & `html4quiz-0.0.37/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 <ul>
 <li><strong>Local</strong>: Everything is on your local PC, grows with your creativity, and you own everything, unlike the many quiz generators available online.</li>
 <li><strong>HTML files</strong>: Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
 <ul><li>Each HTML file is complete in itself with everything included.</li>
 <li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
 <li>Answers can be changed, and saving answers to a text file can be repeated as many times as desired until the file is submitted.</li></ul>
 <li><strong>Easy grading</strong>: Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
-<li><strong>Three kinds of HTML files</strong></li>
+<li><strong>Two kinds of HTML files</strong></li>
 <ol><li>First kind is to preview questions before generating sheets.</li>
 <li>Second kind is the set of sheets.</li></ol>
-<li><strong>Two kinds of questions</strong></li>
+<li><strong>Three kinds of questions</strong></li>
 <ol><li>Short answr questions of requiring a number of a word.</li>
 <li>Multiple choice questions whose choices are genterated randomly by one of various methods or by Python coding.</li>
-<li>Unlike the previous two kinds, students have to "play" the simulation provided with question to answer (refer to Ex005).</li></ol>
+<li>Unlike the previous two kinds, students have to "play" the simulation provided with question to answer (refer to <a href="https://generatenscore.github.io/html4quiz/Examples/Ex005/Ex005/Ex005/index.html">Ex005 Preview</a>).</li></ol>
 <li><strong>Figures</strong> as well as <strong>mathematical expressions</strong> in LaTeX format can be included in both question texts and choices.</li>
 <li><strong>Randomness</strong> is controlled completely by users with Python scripts.</li>
 <li><strong>Easy correction</strong>: When some answers are found incorrect after question sheets are distributed, the answers can be corrected by simply re-generate the sheets with the "work" pickle file (refer to Version 0.0.29). </li></ul>
 
 
 ## Where to get it
 
@@ -31,15 +31,15 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.36</li>
+<li>Version 0.0.37</li>
 <ul><li>Third kind question is added (refer to <a href="https://generatenscore.github.io/html4quiz/Examples/Ex005/Ex005/Ex005/index.html">Ex005 Preview</a>).</li></ul>
 <br>
 
 <li>Version 0.0.33</li>
 <ul><li>A small re-coding is done.</li></ul>
 <br>
```

#### html2text {}

```diff
@@ -10,36 +10,37 @@
           o Students use their mobile devices to read, answer questions, save
             answers to a text file for submission within the same HTML page,
             and submit the text file as directed over the network.
           o Answers can be changed, and saving answers to a text file can be
             repeated as many times as desired until the file is submitted.
     * Easy grading: Grade answers in text files submitted by all students can
       be achieved with a few keystrokes.
-    * Three kinds of HTML files
+    * Two kinds of HTML files
          1. First kind is to preview questions before generating sheets.
          2. Second kind is the set of sheets.
-    * Two kinds of questions
+    * Three kinds of questions
          1. Short answr questions of requiring a number of a word.
          2. Multiple choice questions whose choices are genterated randomly by
             one of various methods or by Python coding.
          3. Unlike the previous two kinds, students have to "play" the
-            simulation provided with question to answer (refer to Ex005).
+            simulation provided with question to answer (refer to Ex005
+            Preview).
     * Figures as well as mathematical expressions in LaTeX format can be
       included in both question texts and choices.
     * Randomness is controlled completely by users with Python scripts.
     * Easy correction: When some answers are found incorrect after question
       sheets are distributed, the answers can be corrected by simply re-
       generate the sheets with the "work" pickle file (refer to Version
       0.0.29).
 ## Where to get it
 pip install html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.36
+    * Version 0.0.37
           o Third kind question is added (refer to Ex005_Preview).
     *
     * Version 0.0.33
           o A small re-coding is done.
     *
     * Version 0.0.30
           o In addition to using a user-defined function for answers, a new way
```

### Comparing `html4quiz-0.0.36/pyproject.toml` & `html4quiz-0.0.37/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.36"
+version = "0.0.37"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.36/PKG-INFO` & `html4quiz-0.0.37/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.36
+Version: 0.0.37
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -27,21 +27,21 @@
 <ul>
 <li><strong>Local</strong>: Everything is on your local PC, grows with your creativity, and you own everything, unlike the many quiz generators available online.</li>
 <li><strong>HTML files</strong>: Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
 <ul><li>Each HTML file is complete in itself with everything included.</li>
 <li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
 <li>Answers can be changed, and saving answers to a text file can be repeated as many times as desired until the file is submitted.</li></ul>
 <li><strong>Easy grading</strong>: Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
-<li><strong>Three kinds of HTML files</strong></li>
+<li><strong>Two kinds of HTML files</strong></li>
 <ol><li>First kind is to preview questions before generating sheets.</li>
 <li>Second kind is the set of sheets.</li></ol>
-<li><strong>Two kinds of questions</strong></li>
+<li><strong>Three kinds of questions</strong></li>
 <ol><li>Short answr questions of requiring a number of a word.</li>
 <li>Multiple choice questions whose choices are genterated randomly by one of various methods or by Python coding.</li>
-<li>Unlike the previous two kinds, students have to "play" the simulation provided with question to answer (refer to Ex005).</li></ol>
+<li>Unlike the previous two kinds, students have to "play" the simulation provided with question to answer (refer to <a href="https://generatenscore.github.io/html4quiz/Examples/Ex005/Ex005/Ex005/index.html">Ex005 Preview</a>).</li></ol>
 <li><strong>Figures</strong> as well as <strong>mathematical expressions</strong> in LaTeX format can be included in both question texts and choices.</li>
 <li><strong>Randomness</strong> is controlled completely by users with Python scripts.</li>
 <li><strong>Easy correction</strong>: When some answers are found incorrect after question sheets are distributed, the answers can be corrected by simply re-generate the sheets with the "work" pickle file (refer to Version 0.0.29). </li></ul>
 
 
 ## Where to get it
 
@@ -50,15 +50,15 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.36</li>
+<li>Version 0.0.37</li>
 <ul><li>Third kind question is added (refer to <a href="https://generatenscore.github.io/html4quiz/Examples/Ex005/Ex005/Ex005/index.html">Ex005 Preview</a>).</li></ul>
 <br>
 
 <li>Version 0.0.33</li>
 <ul><li>A small re-coding is done.</li></ul>
 <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.36 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.37 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
 github.com/generateNscore/html4quiz/wiki Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
@@ -21,36 +21,37 @@
           o Students use their mobile devices to read, answer questions, save
             answers to a text file for submission within the same HTML page,
             and submit the text file as directed over the network.
           o Answers can be changed, and saving answers to a text file can be
             repeated as many times as desired until the file is submitted.
     * Easy grading: Grade answers in text files submitted by all students can
       be achieved with a few keystrokes.
-    * Three kinds of HTML files
+    * Two kinds of HTML files
          1. First kind is to preview questions before generating sheets.
          2. Second kind is the set of sheets.
-    * Two kinds of questions
+    * Three kinds of questions
          1. Short answr questions of requiring a number of a word.
          2. Multiple choice questions whose choices are genterated randomly by
             one of various methods or by Python coding.
          3. Unlike the previous two kinds, students have to "play" the
-            simulation provided with question to answer (refer to Ex005).
+            simulation provided with question to answer (refer to Ex005
+            Preview).
     * Figures as well as mathematical expressions in LaTeX format can be
       included in both question texts and choices.
     * Randomness is controlled completely by users with Python scripts.
     * Easy correction: When some answers are found incorrect after question
       sheets are distributed, the answers can be corrected by simply re-
       generate the sheets with the "work" pickle file (refer to Version
       0.0.29).
 ## Where to get it
 pip install html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.36
+    * Version 0.0.37
           o Third kind question is added (refer to Ex005_Preview).
     *
     * Version 0.0.33
           o A small re-coding is done.
     *
     * Version 0.0.30
           o In addition to using a user-defined function for answers, a new way
```

