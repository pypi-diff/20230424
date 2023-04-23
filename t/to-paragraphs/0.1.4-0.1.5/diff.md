# Comparing `tmp/to_paragraphs-0.1.4.tar.gz` & `tmp/to_paragraphs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to_paragraphs-0.1.4.tar", max compression
+gzip compressed data, was "to_paragraphs-0.1.5.tar", max compression
```

## Comparing `to_paragraphs-0.1.4.tar` & `to_paragraphs-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     2731 2023-04-23 22:55:23.561355 to_paragraphs-0.1.4/README.md
--rw-r--r--   0        0        0      385 2023-04-23 23:05:25.474179 to_paragraphs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2395 2023-04-23 22:46:21.402761 to_paragraphs-0.1.4/to_paragraphs/main.py
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 to_paragraphs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2731 2023-04-23 22:55:23.561355 to_paragraphs-0.1.5/README.md
+-rw-r--r--   0        0        0      385 2023-04-23 23:10:19.242730 to_paragraphs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 23:10:12.098911 to_paragraphs-0.1.5/to_paragraphs/__init__.py
+-rw-r--r--   0        0        0     2395 2023-04-23 22:46:21.402761 to_paragraphs-0.1.5/to_paragraphs/main.py
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 to_paragraphs-0.1.5/PKG-INFO
```

### Comparing `to_paragraphs-0.1.4/README.md` & `to_paragraphs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `to_paragraphs-0.1.4/to_paragraphs/main.py` & `to_paragraphs-0.1.5/to_paragraphs/main.py`

 * *Files identical despite different names*

### Comparing `to_paragraphs-0.1.4/PKG-INFO` & `to_paragraphs-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-paragraphs
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: GPL-3.0
 Author: Félix Dorn
 Author-email: github@felixdorn.fr
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

