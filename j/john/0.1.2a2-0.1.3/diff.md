# Comparing `tmp/john-0.1.2a2.tar.gz` & `tmp/john-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "john-0.1.2a2.tar", max compression
+gzip compressed data, was "john-0.1.3.tar", max compression
```

## Comparing `john-0.1.2a2.tar` & `john-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1088 2023-03-19 23:50:37.808076 john-0.1.2a2/LICENSE
--rw-r--r--   0        0        0      255 2023-03-19 23:50:37.808076 john-0.1.2a2/README.md
--rw-r--r--   0        0        0       61 2023-03-19 23:50:37.808076 john-0.1.2a2/john/__init__.py
--rw-r--r--   0        0        0      100 2023-03-19 23:50:37.808076 john-0.1.2a2/john/factory.py
--rw-r--r--   0        0        0     3176 2023-03-20 15:48:38.003429 john-0.1.2a2/john/test_case.py
--rw-r--r--   0        0        0      597 2023-03-20 15:48:48.131399 john-0.1.2a2/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 john-0.1.2a2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-03-21 10:05:12.550676 john-0.1.3/LICENSE
+-rw-r--r--   0        0        0      255 2023-03-21 10:05:12.550676 john-0.1.3/README.md
+-rw-r--r--   0        0        0      106 2023-03-21 20:11:46.268306 john-0.1.3/john/__init__.py
+-rw-r--r--   0        0        0      242 2023-03-21 20:11:10.483784 john-0.1.3/john/category.py
+-rw-r--r--   0        0        0      100 2023-03-21 10:05:12.550676 john-0.1.3/john/factory.py
+-rw-r--r--   0        0        0     7449 2023-03-22 11:37:54.140749 john-0.1.3/john/test_case.py
+-rw-r--r--   0        0        0      649 2023-03-22 12:17:45.711934 john-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 john-0.1.3/PKG-INFO
```

### Comparing `john-0.1.2a2/LICENSE` & `john-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `john-0.1.2a2/pyproject.toml` & `john-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "john"
-version = "0.1.2a2"
+version = "0.1.3"
 description = "Jeneral Outlying Helper Nuggetoids"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+repository = "https://github.com/wideopensource/john"
 
 [project.urls]
 "Homepage" = "https://github.com/wideopensource/john"
 "Bug Tracker" = "https://github.com/wideopensource/john/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `john-0.1.2a2/PKG-INFO` & `john-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: john
-Version: 0.1.2a2
+Version: 0.1.3
 Summary: Jeneral Outlying Helper Nuggetoids
+Home-page: https://github.com/wideopensource/john
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Project-URL: Repository, https://github.com/wideopensource/john
 Description-Content-Type: text/markdown
 
 # john
 
 ### tl:dr
 
 A collection of random utility classes used internally by the WideOpenTech packages.
```

