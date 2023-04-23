# Comparing `tmp/jsonclass-0.0.5.tar.gz` & `tmp/jsonclass-0.0.6.tar.gz`

## Comparing `jsonclass-0.0.5.tar` & `jsonclass-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jsonclass-0.0.5/test.sh
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jsonclass-0.0.5/test_upload.sh
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jsonclass-0.0.5/upload.sh
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 jsonclass-0.0.5/src/jsonclass.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jsonclass-0.0.5/tests/test.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jsonclass-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.5/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jsonclass-0.0.5/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jsonclass-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jsonclass-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jsonclass-0.0.6/test_upload.sh
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jsonclass-0.0.6/upload.sh
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jsonclass-0.0.6/src/jsonclass.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 jsonclass-0.0.6/tests/test.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jsonclass-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jsonclass-0.0.6/LICENSE
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jsonclass-0.0.6/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jsonclass-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 jsonclass-0.0.6/PKG-INFO
```

### Comparing `jsonclass-0.0.5/.gitignore` & `jsonclass-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.5/LICENSE` & `jsonclass-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonclass-0.0.5/pyproject.toml` & `jsonclass-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonclass"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="soundagain2", email="soundagain2@proton.me" },
 ]
 description = "Convert json to object and back in Python."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

