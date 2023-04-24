# Comparing `tmp/html4quiz-0.0.30.tar.gz` & `tmp/html4quiz-0.0.31.tar.gz`

## Comparing `html4quiz-0.0.30.tar` & `html4quiz-0.0.31.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.30/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/_common.py
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.30/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.30/LICENSE.txt
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 html4quiz-0.0.30/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.30/pyproject.toml
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 html4quiz-0.0.30/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 html4quiz-0.0.31/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.31/LICENSE.txt
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 html4quiz-0.0.31/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 html4quiz-0.0.31/PKG-INFO
```

### Comparing `html4quiz-0.0.30/src/html4quiz/_common.py` & `html4quiz-0.0.31/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.30/src/html4quiz/_generateEm.py` & `html4quiz-0.0.31/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.30/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.31/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.30/src/html4quiz/makeChoices.py` & `html4quiz-0.0.31/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.30/LICENSE.txt` & `html4quiz-0.0.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.30/README.md` & `html4quiz-0.0.31/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,45 +2,50 @@
 
 ## What is it?
 
 html4quiz is a package that helps you generate question sheets with as many HTML files as you want and grade answers from text files submitted by students.
 
 ## Features
 <ul>
-<li>Unlike the many quiz generators available online, everything is on your local PC, grows with your creativity, and you own everything.</li>
-<li>Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
-<li>Except for the math equations, each HTML file is complete in itself.</li>
-<li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
-<li>Saving answers to a file can be repeated as many times as desired.</li>
-<li>Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
-<li>A question begins with a short answer in a number or word.</li>
-<li>Questions with numeric answers can be converted to multiple choice questions simply by flipping the option flag.</li>
-<li>Questions can start with multiple choice.</li>
-<li>Mathematical equations in LaTeX format can be included in both question texts and choices.</li>
-<li>Figures can be included in both question text and choices.</li>
-<li>Question text, mathematical equations, and figures are all randomly selected for each question sheet in a controlled manner.</li>
-<li>Randomness is acquired by executing the answer string, which is a short Python script, that is part of question.</li>
-<li>To increase your creativity, user-defined functions can be easily added for the answer string.</li>
-</ul>
+<li><strong>Local</strong>: Everything is on your local PC, grows with your creativity, and you own everything, unlike the many quiz generators available online.</li>
+<li><strong>HTML files</strong>: Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
+<ul><li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
+<li>Saving answers to a file can be repeated as many times as desired.</li></ul>
+<li><strong>Easy grading</strong>: Grade answers in text files submitted by all students can be achieved with a few keystrokes.</li>
+<li><strong>Two kinds of HTML files</strong></li>
+<ol><li>First kind is to preview questions before generating sheets.</li>
+<li>Second kind is the set of sheets.</li></ol>
+<li><strong>Two kinds of questions</strong></li>
+<ol><li>Short answr questions of requiring a number of a word.</li>
+<li>Multiple choice questions whose choices are genterated randomly by one of various methods or by Python coding.</li></ol>
+<li><strong>Figures</strong> as well as <strong>mathematical expressions</strong> in LaTeX format can be included in both question texts and choices.</li>
+<li><strong>Randomness</strong> is controlled completely by users with Python scripts.</li>
+<li><strong>Easy correction</strong>: When some answers are found incorrect after question sheets are distributed, the answers can be corrected by simply re-generate the sheets with the "work" pickle file (refer to Version 0.0.31). </li></ul>
+
 
 ## Where to get it
 
 <pre lang=sh>pip install html4quiz</pre>
 
-<ul>
-<li>The source code is currently hosted on GitHub at: <a href="https://github.com/generateNscore/html4quiz">https://github.com/generateNscore/html4quiz</a></li>
-</ul>
-
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
+<li>Version 0.0.31</li>
+<ul><li>A new flag is added as the last argument to the class "work".</li>
+<ul><li>When some answers are found incorrect after question sheets are distributed, the answers can be corrected and grading can be completed with the corrected answers for the same questions in every sheet.</li>
+<li>The usage that has been used works fine as they are now. They simply use the default value of "False" for the new added flag.</li>
+<li>To work with the new added flag, every information used for the errorneous previous work are assumed to be the same, including the name and heading.</li>
+<li>Simply add the value False as the last argument when the instance is called.</ul>
+</ul>
+<br>
+
 <li>Version 0.0.30</li>
 <ul><li>In addition to using a user-defined function for answers, a new way to use resources saved in <a href="https://github.com/generateNscore/html4quiz/tree/main/res">html4quiz/res</a> is added.</li>
 <li>For details, please look at <a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004.py">Ex004.py</a></li>
 <li><a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004/Ex004/index.html">Previews</a></li>
 </ul>
 <br>
```

#### html2text {}

```diff
@@ -1,41 +1,55 @@
 # html4quiz ## What is it? html4quiz is a package that helps you generate
 question sheets with as many HTML files as you want and grade answers from text
 files submitted by students. ## Features
-    * Unlike the many quiz generators available online, everything is on your
-      local PC, grows with your creativity, and you own everything.
-    * Question sheets in HTML files, each named with a corresponding
-      identification number, are distributed to students over the network.
-    * Except for the math equations, each HTML file is complete in itself.
-    * Students use their mobile devices to read, answer questions, save answers
-      to a text file for submission within the same HTML page, and submit the
-      text file as directed over the network.
-    * Saving answers to a file can be repeated as many times as desired.
-    * Grade answers in text files submitted by all students can be achieved
-      with a few keystrokes.
-    * A question begins with a short answer in a number or word.
-    * Questions with numeric answers can be converted to multiple choice
-      questions simply by flipping the option flag.
-    * Questions can start with multiple choice.
-    * Mathematical equations in LaTeX format can be included in both question
-      texts and choices.
-    * Figures can be included in both question text and choices.
-    * Question text, mathematical equations, and figures are all randomly
-      selected for each question sheet in a controlled manner.
-    * Randomness is acquired by executing the answer string, which is a short
-      Python script, that is part of question.
-    * To increase your creativity, user-defined functions can be easily added
-      for the answer string.
+    * Local: Everything is on your local PC, grows with your creativity, and
+      you own everything, unlike the many quiz generators available online.
+    * HTML files: Question sheets in HTML files, each named with a
+      corresponding identification number, are distributed to students over the
+      network.
+          o Students use their mobile devices to read, answer questions, save
+            answers to a text file for submission within the same HTML page,
+            and submit the text file as directed over the network.
+          o Saving answers to a file can be repeated as many times as desired.
+    * Easy grading: Grade answers in text files submitted by all students can
+      be achieved with a few keystrokes.
+    * Two kinds of HTML files
+         1. First kind is to preview questions before generating sheets.
+         2. Second kind is the set of sheets.
+    * Two kinds of questions
+         1. Short answr questions of requiring a number of a word.
+         2. Multiple choice questions whose choices are genterated randomly by
+            one of various methods or by Python coding.
+    * Figures as well as mathematical expressions in LaTeX format can be
+      included in both question texts and choices.
+    * Randomness is controlled completely by users with Python scripts.
+    * Easy correction: When some answers are found incorrect after question
+      sheets are distributed, the answers can be corrected by simply re-
+      generate the sheets with the "work" pickle file (refer to Version
+      0.0.31).
 ## Where to get it
 pip install html4quiz
-    * The source code is currently hosted on GitHub at: https://github.com/
-      generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
+    * Version 0.0.31
+          o A new flag is added as the last argument to the class "work".
+                # When some answers are found incorrect after question sheets
+                  are distributed, the answers can be corrected and grading can
+                  be completed with the corrected answers for the same
+                  questions in every sheet.
+                # The usage that has been used works fine as they are now. They
+                  simply use the default value of "False" for the new added
+                  flag.
+                # To work with the new added flag, every information used for
+                  the errorneous previous work are assumed to be the same,
+                  including the name and heading.
+                # Simply add the value False as the last argument when the
+                  instance is called.
+    *
     * Version 0.0.30
           o In addition to using a user-defined function for answers, a new way
             to use resources saved in html4quiz/res is added.
           o For details, please look at Ex004.py
           o Previews
     *
     * Version 0.0.29
```

### Comparing `html4quiz-0.0.30/pyproject.toml` & `html4quiz-0.0.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.30"
+version = "0.0.31"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

