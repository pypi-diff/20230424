# Comparing `tmp/html4quiz-0.0.31.tar.gz` & `tmp/html4quiz-0.0.32.tar.gz`

## Comparing `html4quiz-0.0.31.tar` & `html4quiz-0.0.32.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 html4quiz-0.0.31/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/_common.py
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.31/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.31/LICENSE.txt
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 html4quiz-0.0.31/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.31/pyproject.toml
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 html4quiz-0.0.31/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 html4quiz-0.0.32/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.32/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.32/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 html4quiz-0.0.32/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.32/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.32/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.32/LICENSE.txt
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 html4quiz-0.0.32/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.32/pyproject.toml
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 html4quiz-0.0.32/PKG-INFO
```

### Comparing `html4quiz-0.0.31/updatePackage.txt` & `html4quiz-0.0.32/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.31/src/html4quiz/_common.py` & `html4quiz-0.0.32/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.31/src/html4quiz/_generateEm.py` & `html4quiz-0.0.32/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.31/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.32/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.31/src/html4quiz/makeChoices.py` & `html4quiz-0.0.32/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.31/LICENSE.txt` & `html4quiz-0.0.32/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.31/README.md` & `html4quiz-0.0.32/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -29,21 +29,16 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.31</li>
-<ul><li>A new flag is added as the last argument to the class "work".</li>
-<ul><li>When some answers are found incorrect after question sheets are distributed, the answers can be corrected and grading can be completed with the corrected answers for the same questions in every sheet.</li>
-<li>The usage that has been used works fine as they are now. They simply use the default value of "False" for the new added flag.</li>
-<li>To work with the new added flag, every information used for the errorneous previous work are assumed to be the same, including the name and heading.</li>
-<li>Simply add the value False as the last argument when the instance is called.</ul>
-</ul>
+<li>Version 0.0.32</li>
+<ul><li>A small re-recoding is done.</li></ul>
 <br>
 
 <li>Version 0.0.30</li>
 <ul><li>In addition to using a user-defined function for answers, a new way to use resources saved in <a href="https://github.com/generateNscore/html4quiz/tree/main/res">html4quiz/res</a> is added.</li>
 <li>For details, please look at <a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004.py">Ex004.py</a></li>
 <li><a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004/Ex004/index.html">Previews</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -27,28 +27,16 @@
       generate the sheets with the "work" pickle file (refer to Version
       0.0.31).
 ## Where to get it
 pip install html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.31
-          o A new flag is added as the last argument to the class "work".
-                # When some answers are found incorrect after question sheets
-                  are distributed, the answers can be corrected and grading can
-                  be completed with the corrected answers for the same
-                  questions in every sheet.
-                # The usage that has been used works fine as they are now. They
-                  simply use the default value of "False" for the new added
-                  flag.
-                # To work with the new added flag, every information used for
-                  the errorneous previous work are assumed to be the same,
-                  including the name and heading.
-                # Simply add the value False as the last argument when the
-                  instance is called.
+    * Version 0.0.32
+          o A small re-recoding is done.
     *
     * Version 0.0.30
           o In addition to using a user-defined function for answers, a new way
             to use resources saved in html4quiz/res is added.
           o For details, please look at Ex004.py
           o Previews
     *
```

### Comparing `html4quiz-0.0.31/pyproject.toml` & `html4quiz-0.0.32/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.31"
+version = "0.0.32"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `html4quiz-0.0.31/PKG-INFO` & `html4quiz-0.0.32/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.31
+Version: 0.0.32
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -48,21 +48,16 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
-<li>Version 0.0.31</li>
-<ul><li>A new flag is added as the last argument to the class "work".</li>
-<ul><li>When some answers are found incorrect after question sheets are distributed, the answers can be corrected and grading can be completed with the corrected answers for the same questions in every sheet.</li>
-<li>The usage that has been used works fine as they are now. They simply use the default value of "False" for the new added flag.</li>
-<li>To work with the new added flag, every information used for the errorneous previous work are assumed to be the same, including the name and heading.</li>
-<li>Simply add the value False as the last argument when the instance is called.</ul>
-</ul>
+<li>Version 0.0.32</li>
+<ul><li>A small re-recoding is done.</li></ul>
 <br>
 
 <li>Version 0.0.30</li>
 <ul><li>In addition to using a user-defined function for answers, a new way to use resources saved in <a href="https://github.com/generateNscore/html4quiz/tree/main/res">html4quiz/res</a> is added.</li>
 <li>For details, please look at <a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004.py">Ex004.py</a></li>
 <li><a href="https://generatenscore.github.io/html4quiz/Examples/Ex004/Ex004/Ex004/index.html">Previews</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.31 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.32 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
 github.com/generateNscore/html4quiz/wiki Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
@@ -38,28 +38,16 @@
       generate the sheets with the "work" pickle file (refer to Version
       0.0.31).
 ## Where to get it
 pip install html4quiz
 ## Dependencies
     * None
 ## Changes
-    * Version 0.0.31
-          o A new flag is added as the last argument to the class "work".
-                # When some answers are found incorrect after question sheets
-                  are distributed, the answers can be corrected and grading can
-                  be completed with the corrected answers for the same
-                  questions in every sheet.
-                # The usage that has been used works fine as they are now. They
-                  simply use the default value of "False" for the new added
-                  flag.
-                # To work with the new added flag, every information used for
-                  the errorneous previous work are assumed to be the same,
-                  including the name and heading.
-                # Simply add the value False as the last argument when the
-                  instance is called.
+    * Version 0.0.32
+          o A small re-recoding is done.
     *
     * Version 0.0.30
           o In addition to using a user-defined function for answers, a new way
             to use resources saved in html4quiz/res is added.
           o For details, please look at Ex004.py
           o Previews
     *
```

