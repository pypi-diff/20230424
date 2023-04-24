# Comparing `tmp/a_pandas_ex_text_compare-0.10.tar.gz` & `tmp/a_pandas_ex_text_compare-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_text_compare-0.10.tar", last modified: Thu Dec  8 10:42:24 2022, max compression
+gzip compressed data, was "a_pandas_ex_text_compare-0.11.tar", last modified: Mon Apr 24 15:43:20 2023, max compression
```

## Comparing `a_pandas_ex_text_compare-0.10.tar` & `a_pandas_ex_text_compare-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-12-08 10:42:24.181347 a_pandas_ex_text_compare-0.10/
--rw-rw-rw-   0        0        0     1148 2022-12-08 10:42:16.000000 a_pandas_ex_text_compare-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      185 2022-12-08 10:42:15.000000 a_pandas_ex_text_compare-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     9832 2022-12-08 10:42:24.181347 a_pandas_ex_text_compare-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     8783 2022-12-08 10:39:19.000000 a_pandas_ex_text_compare-0.10/README.md
-drwxrwxrwx   0        0        0        0 2022-12-08 10:42:24.178419 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/LICENSE
--rw-rw-rw-   0        0        0     8783 2022-12-08 10:39:19.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/README.MD
--rw-rw-rw-   0        0        0     4320 2022-12-08 10:34:35.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/__init__.py
--rw-rw-rw-   0        0        0       52 2022-12-08 10:42:23.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/requirements.txt
--rw-rw-rw-   0        0        0        2 2022-12-08 10:42:23.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/thirdparty.json
-drwxrwxrwx   0        0        0        0 2022-12-08 10:42:24.180371 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare.egg-info/
--rw-rw-rw-   0        0        0     9832 2022-12-08 10:42:24.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2022-12-08 10:42:24.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-08 10:42:24.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-12-08 10:42:24.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2022-12-08 10:42:24.000000 a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-12-08 10:42:24.182323 a_pandas_ex_text_compare-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1577 2022-12-08 10:42:23.000000 a_pandas_ex_text_compare-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:43:20.758095 a_pandas_ex_text_compare-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-24 15:43:14.000000 a_pandas_ex_text_compare-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      185 2023-04-24 15:43:13.000000 a_pandas_ex_text_compare-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     9482 2023-04-24 15:43:20.758095 a_pandas_ex_text_compare-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     8783 2023-04-15 00:18:33.000000 a_pandas_ex_text_compare-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:43:20.753108 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/
+-rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:33.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/LICENSE
+-rw-rw-rw-   0        0        0     8783 2023-04-15 00:18:33.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/README.MD
+-rw-rw-rw-   0        0        0     4340 2023-04-24 14:51:39.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-04-24 15:43:19.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/requirements.txt
+-rw-rw-rw-   0        0        0    13679 2023-04-24 15:43:19.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-24 15:43:20.757097 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare.egg-info/
+-rw-rw-rw-   0        0        0     9482 2023-04-24 15:43:20.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-04-24 15:43:20.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:43:20.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-24 15:43:20.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-24 15:43:20.000000 a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-24 15:43:20.759092 a_pandas_ex_text_compare-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-04-24 15:43:19.000000 a_pandas_ex_text_compare-0.11/setup.py
```

### Comparing `a_pandas_ex_text_compare-0.10/LICENSE.rst` & `a_pandas_ex_text_compare-0.11/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2022 Johannes Fischer
+ Copyright (c) 2023 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `a_pandas_ex_text_compare-0.10/PKG-INFO` & `a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,100 @@
 Metadata-Version: 2.1
-Name: a_pandas_ex_text_compare
-Version: 0.10
+Name: a-pandas-ex-text-compare
+Version: 0.11
 Summary: Compares 2 texts with each other, and returns a Pandas DataFrame
 Home-page: https://github.com/hansalemaos/a_pandas_ex_text_compare
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: string,text,pandas,DataFrame,read,difflib,fuzz,fuzzy
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Compares 2 texts with each other, and returns a Pandas DataFrame
 
-# Compares 2 texts with each other, and returns a Pandas DataFrame
-
-```python
-pip install a-pandas-ex_text-compare
-```
-
-```python
-from a_pandas_ex_text_compare import pd_add_text_difference
-import pandas as pd
-
-pd_add_text_difference()
-
-
-
-# Examples of possible inputs (bytes, list, string, path (as string))
-
-text1 = """  1. Beautiful isxx better than ugly.
-  2. Explicit isq better than implicit.
-  3. Simple is better than complex.
-  4. Complex is better than complicated.
-"""
-
-text2 = """  
-1. Beautiful is better than ugly.
-  2. Explicit is better than implicit.
-  3. qSimple is better than pcomplex.
-  4. Complicated aais better than complex.
-  5. Flat is better than nested.
-""".splitlines(
-    keepends=True
-)
-text2 = '''The green man wakes and sees her place
-The spectacles upon her face;
-And now she's trying all she can
-To shoot the sleepy, green-coat man.
-He cries and screams and runs away;
-The hare runs after him all day
-The hare runs after him all day
-And hears him call out everywhere:
-"Help! Fire! Help! The Hare! The Hare!"'''.encode()
-
-text1 = b'''The yellow man wakes and sees her place
-The spectacles upon her face;
-The spectacles upon her face;
-And now she is trying all that she can
-To shoot the tired, green-coat man.
-He cries and screams and runs away;
-The hare runs after him the whole day
-And hears him call out everywhere:
-and hears him call out everywhere:
-"Help! Fire! Help! The Hare! The Hare!"'''
-
-text1 = r"C:\Users\Gamer\Documents\Downloads\testread.txt"
-
-
-df = pd.Q_text_difference_to_df(text1, text2, encoding="utf-8")
-print(df.to_string())
-
-"""
-    no                                  aa_text                                  bb_text                            aa_added                   bb_substracted aa_changed bb_changed                                         aa_diff                                      bb_diff                                          aa_parts                                           bb_parts
-0    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         gr                                   (diff_chg, y)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-1    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         gr                                (diff_chg, llow)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-2    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         en                                   (diff_chg, y)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-3    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         en                                (diff_chg, llow)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-4    1            The spectacles upon her face;            The spectacles upon her face;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                  (The spectacles upon her face;,)                   (The spectacles upon her face;,)
-5    2                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
-6    3                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
-7    4         And now she's trying all she can   And now she is trying all that she can                                <NA>                             <NA>          i          '                                  (diff_chg,  i)                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
-8    4         And now she's trying all she can   And now she is trying all that she can                               that                              <NA>       <NA>          '                               (diff_add, that )                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
-9    5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir         sl                                 (diff_chg, tir)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-10   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d         sl                                   (diff_chg, d)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-11   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir        epy                                 (diff_chg, tir)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-12   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d        epy                                   (diff_chg, d)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-13   6      He cries and screams and runs away;      He cries and screams and runs away;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN            (He cries and screams and runs away;,)             (He cries and screams and runs away;,)
-14   7          The hare runs after him all day          The hare runs after him all day                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                (The hare runs after him all day,)                 (The hare runs after him all day,)
-15   8          The hare runs after him all day       And hears him call out everywhere:  And hears him call out everywhere:  The hare runs after him all day       <NA>       <NA>  (diff_add, And hears him call out everywhere:)  (diff_sub, The hare runs after him all day)                (The hare runs after him all day,)              (And hears him call out everywhere:,)
-16   9       And hears him call out everywhere:       And hears him call out everywhere:                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN             (And hears him call out everywhere:,)              (And hears him call out everywhere:,)
-17  10  "Help! Fire! Help! The Hare! The Hare!"  "Help! Fire! Help! The Hare! The Hare!"                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN        ("Help! Fire! Help! The Hare! The Hare!",)         ("Help! Fire! Help! The Hare! The Hare!",)
-
-
-"""
-
-```
+```python
+pip install a-pandas-ex_text-compare
+```
+
+```python
+from a_pandas_ex_text_compare import pd_add_text_difference
+import pandas as pd
+
+pd_add_text_difference()
+
+
+
+# Examples of possible inputs (bytes, list, string, path (as string))
+
+text1 = """  1. Beautiful isxx better than ugly.
+  2. Explicit isq better than implicit.
+  3. Simple is better than complex.
+  4. Complex is better than complicated.
+"""
+
+text2 = """  
+1. Beautiful is better than ugly.
+  2. Explicit is better than implicit.
+  3. qSimple is better than pcomplex.
+  4. Complicated aais better than complex.
+  5. Flat is better than nested.
+""".splitlines(
+    keepends=True
+)
+text2 = '''The green man wakes and sees her place
+The spectacles upon her face;
+And now she's trying all she can
+To shoot the sleepy, green-coat man.
+He cries and screams and runs away;
+The hare runs after him all day
+The hare runs after him all day
+And hears him call out everywhere:
+"Help! Fire! Help! The Hare! The Hare!"'''.encode()
+
+text1 = b'''The yellow man wakes and sees her place
+The spectacles upon her face;
+The spectacles upon her face;
+And now she is trying all that she can
+To shoot the tired, green-coat man.
+He cries and screams and runs away;
+The hare runs after him the whole day
+And hears him call out everywhere:
+and hears him call out everywhere:
+"Help! Fire! Help! The Hare! The Hare!"'''
+
+text1 = r"C:\Users\Gamer\Documents\Downloads\testread.txt"
+
+
+df = pd.Q_text_difference_to_df(text1, text2, encoding="utf-8")
+print(df.to_string())
+
+"""
+    no                                  aa_text                                  bb_text                            aa_added                   bb_substracted aa_changed bb_changed                                         aa_diff                                      bb_diff                                          aa_parts                                           bb_parts
+0    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         gr                                   (diff_chg, y)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+1    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         gr                                (diff_chg, llow)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+2    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         en                                   (diff_chg, y)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+3    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         en                                (diff_chg, llow)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+4    1            The spectacles upon her face;            The spectacles upon her face;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                  (The spectacles upon her face;,)                   (The spectacles upon her face;,)
+5    2                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
+6    3                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
+7    4         And now she's trying all she can   And now she is trying all that she can                                <NA>                             <NA>          i          '                                  (diff_chg,  i)                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
+8    4         And now she's trying all she can   And now she is trying all that she can                               that                              <NA>       <NA>          '                               (diff_add, that )                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
+9    5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir         sl                                 (diff_chg, tir)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+10   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d         sl                                   (diff_chg, d)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+11   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir        epy                                 (diff_chg, tir)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+12   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d        epy                                   (diff_chg, d)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+13   6      He cries and screams and runs away;      He cries and screams and runs away;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN            (He cries and screams and runs away;,)             (He cries and screams and runs away;,)
+14   7          The hare runs after him all day          The hare runs after him all day                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                (The hare runs after him all day,)                 (The hare runs after him all day,)
+15   8          The hare runs after him all day       And hears him call out everywhere:  And hears him call out everywhere:  The hare runs after him all day       <NA>       <NA>  (diff_add, And hears him call out everywhere:)  (diff_sub, The hare runs after him all day)                (The hare runs after him all day,)              (And hears him call out everywhere:,)
+16   9       And hears him call out everywhere:       And hears him call out everywhere:                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN             (And hears him call out everywhere:,)              (And hears him call out everywhere:,)
+17  10  "Help! Fire! Help! The Hare! The Hare!"  "Help! Fire! Help! The Hare! The Hare!"                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN        ("Help! Fire! Help! The Hare! The Hare!",)         ("Help! Fire! Help! The Hare! The Hare!",)
+
+
+"""
+
+```
```

### Comparing `a_pandas_ex_text_compare-0.10/README.md` & `a_pandas_ex_text_compare-0.11/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/LICENSE` & `a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/LICENSE`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/README.MD` & `a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/README.MD`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare/__init__.py` & `a_pandas_ex_text_compare-0.11/a_pandas_ex_text_compare/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import difflib
 import os
 from typing import Union
 
 import pandas as pd
 import regex
 from flatten_everything import flatten_everything
-from a_pandas_ex_bs4df import pd_add_bs4_to_df
+from a_pandas_ex_bs4df_lite import pd_add_bs4_to_df_lite
+pd_add_bs4_to_df_lite()
 
-pd_add_bs4_to_df()
 
 
 def open_text(text, encoding):
     text1 = text
     if isinstance(text1, str):
         if os.path.exists(text1):
             with open(text1, mode="rb") as f:
@@ -37,15 +37,15 @@
         except Exception:
             return pd.NA
 
     text1 = open_text(text1, encoding)
     text2 = open_text(text2, encoding)
 
     htmla = difflib.HtmlDiff().make_file(text2, text1)
-    df = pd.Q_bs4_to_df(htmla.encode(), parser="lxml")
+    df = pd.Q_bs4_to_df_lite(htmla.encode(), parser="lxml")
     now = (
         pd.DataFrame(
             [
                 [y for y in x if '<td nowrap="nowrap">' in str(y)]
                 for x in df.loc[df.aa_name == "tr"].aa_contents
                 if "diff_" in str(x)
             ]
```

### Comparing `a_pandas_ex_text_compare-0.10/a_pandas_ex_text_compare.egg-info/PKG-INFO` & `a_pandas_ex_text_compare-0.11/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,100 @@
 Metadata-Version: 2.1
-Name: a-pandas-ex-text-compare
-Version: 0.10
+Name: a_pandas_ex_text_compare
+Version: 0.11
 Summary: Compares 2 texts with each other, and returns a Pandas DataFrame
 Home-page: https://github.com/hansalemaos/a_pandas_ex_text_compare
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: string,text,pandas,DataFrame,read,difflib,fuzz,fuzzy
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Compares 2 texts with each other, and returns a Pandas DataFrame
 
-# Compares 2 texts with each other, and returns a Pandas DataFrame
-
-```python
-pip install a-pandas-ex_text-compare
-```
-
-```python
-from a_pandas_ex_text_compare import pd_add_text_difference
-import pandas as pd
-
-pd_add_text_difference()
-
-
-
-# Examples of possible inputs (bytes, list, string, path (as string))
-
-text1 = """  1. Beautiful isxx better than ugly.
-  2. Explicit isq better than implicit.
-  3. Simple is better than complex.
-  4. Complex is better than complicated.
-"""
-
-text2 = """  
-1. Beautiful is better than ugly.
-  2. Explicit is better than implicit.
-  3. qSimple is better than pcomplex.
-  4. Complicated aais better than complex.
-  5. Flat is better than nested.
-""".splitlines(
-    keepends=True
-)
-text2 = '''The green man wakes and sees her place
-The spectacles upon her face;
-And now she's trying all she can
-To shoot the sleepy, green-coat man.
-He cries and screams and runs away;
-The hare runs after him all day
-The hare runs after him all day
-And hears him call out everywhere:
-"Help! Fire! Help! The Hare! The Hare!"'''.encode()
-
-text1 = b'''The yellow man wakes and sees her place
-The spectacles upon her face;
-The spectacles upon her face;
-And now she is trying all that she can
-To shoot the tired, green-coat man.
-He cries and screams and runs away;
-The hare runs after him the whole day
-And hears him call out everywhere:
-and hears him call out everywhere:
-"Help! Fire! Help! The Hare! The Hare!"'''
-
-text1 = r"C:\Users\Gamer\Documents\Downloads\testread.txt"
-
-
-df = pd.Q_text_difference_to_df(text1, text2, encoding="utf-8")
-print(df.to_string())
-
-"""
-    no                                  aa_text                                  bb_text                            aa_added                   bb_substracted aa_changed bb_changed                                         aa_diff                                      bb_diff                                          aa_parts                                           bb_parts
-0    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         gr                                   (diff_chg, y)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-1    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         gr                                (diff_chg, llow)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-2    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         en                                   (diff_chg, y)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-3    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         en                                (diff_chg, llow)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
-4    1            The spectacles upon her face;            The spectacles upon her face;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                  (The spectacles upon her face;,)                   (The spectacles upon her face;,)
-5    2                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
-6    3                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
-7    4         And now she's trying all she can   And now she is trying all that she can                                <NA>                             <NA>          i          '                                  (diff_chg,  i)                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
-8    4         And now she's trying all she can   And now she is trying all that she can                               that                              <NA>       <NA>          '                               (diff_add, that )                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
-9    5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir         sl                                 (diff_chg, tir)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-10   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d         sl                                   (diff_chg, d)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-11   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir        epy                                 (diff_chg, tir)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-12   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d        epy                                   (diff_chg, d)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
-13   6      He cries and screams and runs away;      He cries and screams and runs away;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN            (He cries and screams and runs away;,)             (He cries and screams and runs away;,)
-14   7          The hare runs after him all day          The hare runs after him all day                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                (The hare runs after him all day,)                 (The hare runs after him all day,)
-15   8          The hare runs after him all day       And hears him call out everywhere:  And hears him call out everywhere:  The hare runs after him all day       <NA>       <NA>  (diff_add, And hears him call out everywhere:)  (diff_sub, The hare runs after him all day)                (The hare runs after him all day,)              (And hears him call out everywhere:,)
-16   9       And hears him call out everywhere:       And hears him call out everywhere:                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN             (And hears him call out everywhere:,)              (And hears him call out everywhere:,)
-17  10  "Help! Fire! Help! The Hare! The Hare!"  "Help! Fire! Help! The Hare! The Hare!"                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN        ("Help! Fire! Help! The Hare! The Hare!",)         ("Help! Fire! Help! The Hare! The Hare!",)
-
-
-"""
-
-```
+```python
+pip install a-pandas-ex_text-compare
+```
+
+```python
+from a_pandas_ex_text_compare import pd_add_text_difference
+import pandas as pd
+
+pd_add_text_difference()
+
+
+
+# Examples of possible inputs (bytes, list, string, path (as string))
+
+text1 = """  1. Beautiful isxx better than ugly.
+  2. Explicit isq better than implicit.
+  3. Simple is better than complex.
+  4. Complex is better than complicated.
+"""
+
+text2 = """  
+1. Beautiful is better than ugly.
+  2. Explicit is better than implicit.
+  3. qSimple is better than pcomplex.
+  4. Complicated aais better than complex.
+  5. Flat is better than nested.
+""".splitlines(
+    keepends=True
+)
+text2 = '''The green man wakes and sees her place
+The spectacles upon her face;
+And now she's trying all she can
+To shoot the sleepy, green-coat man.
+He cries and screams and runs away;
+The hare runs after him all day
+The hare runs after him all day
+And hears him call out everywhere:
+"Help! Fire! Help! The Hare! The Hare!"'''.encode()
+
+text1 = b'''The yellow man wakes and sees her place
+The spectacles upon her face;
+The spectacles upon her face;
+And now she is trying all that she can
+To shoot the tired, green-coat man.
+He cries and screams and runs away;
+The hare runs after him the whole day
+And hears him call out everywhere:
+and hears him call out everywhere:
+"Help! Fire! Help! The Hare! The Hare!"'''
+
+text1 = r"C:\Users\Gamer\Documents\Downloads\testread.txt"
+
+
+df = pd.Q_text_difference_to_df(text1, text2, encoding="utf-8")
+print(df.to_string())
+
+"""
+    no                                  aa_text                                  bb_text                            aa_added                   bb_substracted aa_changed bb_changed                                         aa_diff                                      bb_diff                                          aa_parts                                           bb_parts
+0    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         gr                                   (diff_chg, y)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+1    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         gr                                (diff_chg, llow)                               (diff_chg, gr)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+2    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>          y         en                                   (diff_chg, y)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+3    0   The green man wakes and sees her place  The yellow man wakes and sees her place                                <NA>                             <NA>       llow         en                                (diff_chg, llow)                               (diff_chg, en)  (The , gr, e, en,  man wakes and sees her place)  (The , y, e, llow,  man wakes and sees her place)
+4    1            The spectacles upon her face;            The spectacles upon her face;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                  (The spectacles upon her face;,)                   (The spectacles upon her face;,)
+5    2                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
+6    3                                                     The spectacles upon her face;       The spectacles upon her face;                             <NA>       <NA>       <NA>       (diff_add, The spectacles upon her face;)                                          NaN                                                ()                   (The spectacles upon her face;,)
+7    4         And now she's trying all she can   And now she is trying all that she can                                <NA>                             <NA>          i          '                                  (diff_chg,  i)                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
+8    4         And now she's trying all she can   And now she is trying all that she can                               that                              <NA>       <NA>          '                               (diff_add, that )                                (diff_chg, ')            (And now she, ', s trying all she can)   (And now she,  i, s trying all , that , she can)
+9    5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir         sl                                 (diff_chg, tir)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+10   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d         sl                                   (diff_chg, d)                               (diff_chg, sl)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+11   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>        tir        epy                                 (diff_chg, tir)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+12   5     To shoot the sleepy, green-coat man.      To shoot the tired, green-coat man.                                <NA>                             <NA>          d        epy                                   (diff_chg, d)                              (diff_chg, epy)    (To shoot the , sl, e, epy, , green-coat man.)      (To shoot the , tir, e, d, , green-coat man.)
+13   6      He cries and screams and runs away;      He cries and screams and runs away;                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN            (He cries and screams and runs away;,)             (He cries and screams and runs away;,)
+14   7          The hare runs after him all day          The hare runs after him all day                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN                (The hare runs after him all day,)                 (The hare runs after him all day,)
+15   8          The hare runs after him all day       And hears him call out everywhere:  And hears him call out everywhere:  The hare runs after him all day       <NA>       <NA>  (diff_add, And hears him call out everywhere:)  (diff_sub, The hare runs after him all day)                (The hare runs after him all day,)              (And hears him call out everywhere:,)
+16   9       And hears him call out everywhere:       And hears him call out everywhere:                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN             (And hears him call out everywhere:,)              (And hears him call out everywhere:,)
+17  10  "Help! Fire! Help! The Hare! The Hare!"  "Help! Fire! Help! The Hare! The Hare!"                                <NA>                             <NA>       <NA>       <NA>                                             NaN                                          NaN        ("Help! Fire! Help! The Hare! The Hare!",)         ("Help! Fire! Help! The Hare! The Hare!",)
+
+
+"""
+
+```
```

