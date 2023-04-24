# Comparing `tmp/john-0.1.4a0.tar.gz` & `tmp/john-0.1.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "john-0.1.4a0.tar", max compression
+gzip compressed data, was "john-0.1.4a1.tar", max compression
```

## Comparing `john-0.1.4a0.tar` & `john-0.1.4a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1108 2023-04-24 10:27:11.710010 john-0.1.4a0/LICENSE
--rw-r--r--   0        0        0      268 2023-04-24 10:27:11.710010 john-0.1.4a0/README.md
--rw-r--r--   0        0        0       85 2023-04-24 13:37:39.992745 john-0.1.4a0/john/__init__.py
--rw-r--r--   0        0        0      106 2023-04-24 10:27:11.710010 john-0.1.4a0/john/factory.py
--rw-r--r--   0        0        0     1454 2023-04-24 13:53:36.223605 john-0.1.4a0/john/tdd.py
--rw-r--r--   0        0        0     7727 2023-04-24 13:38:05.344784 john-0.1.4a0/john/test_case.py
--rw-r--r--   0        0        0      681 2023-04-24 15:35:26.356124 john-0.1.4a0/pyproject.toml
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 john-0.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-04-24 10:27:11.710010 john-0.1.4a1/LICENSE
+-rw-r--r--   0        0        0      268 2023-04-24 10:27:11.710010 john-0.1.4a1/README.md
+-rw-r--r--   0        0        0       85 2023-04-24 13:37:39.992745 john-0.1.4a1/john/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-24 10:27:11.710010 john-0.1.4a1/john/factory.py
+-rw-r--r--   0        0        0     1375 2023-04-24 15:49:15.036240 john-0.1.4a1/john/tdd.py
+-rw-r--r--   0        0        0     7727 2023-04-24 13:38:05.344784 john-0.1.4a1/john/test_case.py
+-rw-r--r--   0        0        0      681 2023-04-24 15:53:18.921369 john-0.1.4a1/pyproject.toml
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 john-0.1.4a1/PKG-INFO
```

### Comparing `john-0.1.4a0/LICENSE` & `john-0.1.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `john-0.1.4a0/john/tdd.py` & `john-0.1.4a1/john/tdd.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,14 @@
         return super().tearDownClass()
 
     @property
     def sut(self):
         self._ensure_sut()
         return self.__class__._sut
     
-    def __init__(self, methodName: str):
-        super().__init__(methodName)
-
     def _ensure_tube(self) -> None:
         if not self.__class__._tube:
             self.__class__._sut = None
 
             test_case_module = importlib.import_module(self.__module__)
             test_case_filename = test_case_module.__file__
             test_case_name = os.path.splitext(
```

### Comparing `john-0.1.4a0/john/test_case.py` & `john-0.1.4a1/john/test_case.py`

 * *Files identical despite different names*

### Comparing `john-0.1.4a0/pyproject.toml` & `john-0.1.4a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "john"
-version = "0.1.4a0"
+version = "0.1.4a1"
 description = "Jeneral Outlying Helper Nuggetoids"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `john-0.1.4a0/PKG-INFO` & `john-0.1.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: john
-Version: 0.1.4a0
+Version: 0.1.4a1
 Summary: Jeneral Outlying Helper Nuggetoids
 Home-page: https://github.com/wideopensource/john
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

