# Comparing `tmp/dynamics365crm_python-1.0.1.tar.gz` & `tmp/dynamics365crm_python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamics365crm_python-1.0.1.tar", max compression
+gzip compressed data, was "dynamics365crm_python-1.0.2.tar", max compression
```

## Comparing `dynamics365crm_python-1.0.1.tar` & `dynamics365crm_python-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-03-27 20:51:24.008452 dynamics365crm_python-1.0.1/LICENSE
--rw-r--r--   0        0        0     6952 2023-03-27 20:51:24.008684 dynamics365crm_python-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-27 20:51:24.008801 dynamics365crm_python-1.0.1/dynamics365crm/__init__.py
--rw-r--r--   0        0        0    14126 2023-03-27 20:51:24.008999 dynamics365crm_python-1.0.1/dynamics365crm/client.py
--rw-r--r--   0        0        0     1905 2023-03-27 20:51:24.009172 dynamics365crm_python-1.0.1/dynamics365crm/test.py
--rw-r--r--   0        0        0      415 2023-03-27 20:52:13.862250 dynamics365crm_python-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7613 1970-01-01 00:00:00.000000 dynamics365crm_python-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-27 20:51:24.008452 dynamics365crm_python-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6952 2023-03-27 20:51:24.008684 dynamics365crm_python-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 20:51:24.008801 dynamics365crm_python-1.0.2/dynamics365crm/__init__.py
+-rw-r--r--   0        0        0    14126 2023-03-27 20:51:24.008999 dynamics365crm_python-1.0.2/dynamics365crm/client.py
+-rw-r--r--   0        0        0     1905 2023-03-27 20:51:24.009172 dynamics365crm_python-1.0.2/dynamics365crm/test.py
+-rw-r--r--   0        0        0      432 2023-04-24 17:22:11.657637 dynamics365crm_python-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7651 1970-01-01 00:00:00.000000 dynamics365crm_python-1.0.2/PKG-INFO
```

### Comparing `dynamics365crm_python-1.0.1/LICENSE` & `dynamics365crm_python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamics365crm_python-1.0.1/README.md` & `dynamics365crm_python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dynamics365crm_python-1.0.1/dynamics365crm/client.py` & `dynamics365crm_python-1.0.2/dynamics365crm/client.py`

 * *Files identical despite different names*

### Comparing `dynamics365crm_python-1.0.1/dynamics365crm/test.py` & `dynamics365crm_python-1.0.2/dynamics365crm/test.py`

 * *Files identical despite different names*

### Comparing `dynamics365crm_python-1.0.1/PKG-INFO` & `dynamics365crm_python-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dynamics365crm-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: API wrapper for Dynamics365CRM written in Python
 License: MIT
 Author: Miguel Ferrer
 Author-email: ingferrermiguel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: msal (>=1.21.0,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # dynamics365crm-python
 Dynamics365CRM API wrapper for Dynamics 365 written in Python.
 This library works for API version: v9.0
```

