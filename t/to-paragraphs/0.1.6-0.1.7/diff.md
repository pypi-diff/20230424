# Comparing `tmp/to_paragraphs-0.1.6.tar.gz` & `tmp/to_paragraphs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to_paragraphs-0.1.6.tar", max compression
+gzip compressed data, was "to_paragraphs-0.1.7.tar", max compression
```

## Comparing `to_paragraphs-0.1.6.tar` & `to_paragraphs-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2731 2023-04-23 22:55:23.561355 to_paragraphs-0.1.6/README.md
--rw-r--r--   0        0        0      385 2023-04-23 23:17:53.923178 to_paragraphs-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 23:10:12.098911 to_paragraphs-0.1.6/to_paragraphs/__init__.py
--rw-r--r--   0        0        0     2395 2023-04-23 22:46:21.402761 to_paragraphs-0.1.6/to_paragraphs/to_paragraphs.py
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 to_paragraphs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2731 2023-04-23 22:55:23.561355 to_paragraphs-0.1.7/README.md
+-rw-r--r--   0        0        0      385 2023-04-23 23:22:32.971776 to_paragraphs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-04-23 23:21:55.376793 to_paragraphs-0.1.7/to_paragraphs/__init__.py
+-rw-r--r--   0        0        0     2395 2023-04-23 22:46:21.402761 to_paragraphs-0.1.7/to_paragraphs/to_paragraphs.py
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 to_paragraphs-0.1.7/PKG-INFO
```

### Comparing `to_paragraphs-0.1.6/README.md` & `to_paragraphs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `to_paragraphs-0.1.6/to_paragraphs/to_paragraphs.py` & `to_paragraphs-0.1.7/to_paragraphs/to_paragraphs.py`

 * *Files identical despite different names*

### Comparing `to_paragraphs-0.1.6/PKG-INFO` & `to_paragraphs-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-paragraphs
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: GPL-3.0
 Author: Félix Dorn
 Author-email: github@felixdorn.fr
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

