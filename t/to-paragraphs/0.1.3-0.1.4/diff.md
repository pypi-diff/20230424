# Comparing `tmp/to_paragraphs-0.1.3.tar.gz` & `tmp/to_paragraphs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to_paragraphs-0.1.3.tar", max compression
+gzip compressed data, was "to_paragraphs-0.1.4.tar", max compression
```

## Comparing `to_paragraphs-0.1.3.tar` & `to_paragraphs-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2731 2023-04-23 22:55:23.561355 to_paragraphs-0.1.3/README.md
--rw-r--r--   0        0        0      384 2023-04-23 23:04:04.748222 to_paragraphs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2395 2023-04-23 22:46:21.402761 to_paragraphs-0.1.3/to_paragraphs/main.py
--rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 to_paragraphs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2731 2023-04-23 22:55:23.561355 to_paragraphs-0.1.4/README.md
+-rw-r--r--   0        0        0      385 2023-04-23 23:05:25.474179 to_paragraphs-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2395 2023-04-23 22:46:21.402761 to_paragraphs-0.1.4/to_paragraphs/main.py
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 to_paragraphs-0.1.4/PKG-INFO
```

### Comparing `to_paragraphs-0.1.3/README.md` & `to_paragraphs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `to_paragraphs-0.1.3/to_paragraphs/main.py` & `to_paragraphs-0.1.4/to_paragraphs/main.py`

 * *Files identical despite different names*

### Comparing `to_paragraphs-0.1.3/PKG-INFO` & `to_paragraphs-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: to-paragraphs
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: GPL-3.0
 Author: Félix Dorn
 Author-email: github@felixdorn.fr
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # to_paragraphs
```

