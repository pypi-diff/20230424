# Comparing `tmp/halig-0.1.8.tar.gz` & `tmp/halig-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halig-0.1.8.tar", last modified: Thu Apr  6 15:38:12 2023, max compression
+gzip compressed data, was "halig-0.2.0.tar", last modified: Mon Apr 24 11:57:28 2023, max compression
```

## Comparing `halig-0.1.8.tar` & `halig-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34670 2023-03-31 07:27:12.162734 halig-0.1.8/LICENSE
--rw-r--r--   0        0        0     1248 2023-04-06 15:13:32.030268 halig-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-04-04 12:01:02.993899 halig-0.1.8/halig/__init__.py
--rw-r--r--   0        0        0       22 2023-04-06 15:36:09.269377 halig-0.1.8/halig/__version__.py
--rw-r--r--   0        0        0        0 2023-03-31 15:57:58.424915 halig-0.1.8/halig/commands/__init__.py
--rw-r--r--   0        0        0      292 2023-04-03 10:08:17.490684 halig-0.1.8/halig/commands/base.py
--rw-r--r--   0        0        0     2767 2023-04-03 09:44:52.171380 halig-0.1.8/halig/commands/edit.py
--rw-r--r--   0        0        0     1076 2023-04-03 10:06:57.010967 halig-0.1.8/halig/commands/notebooks.py
--rw-r--r--   0        0        0     1199 2023-04-03 10:06:57.006967 halig-0.1.8/halig/commands/show.py
--rw-r--r--   0        0        0     1391 2023-04-04 15:42:27.181944 halig-0.1.8/halig/encryption.py
--rw-r--r--   0        0        0     1354 2023-04-06 15:36:28.509315 halig-0.1.8/halig/literals.py
--rw-r--r--   0        0        0     1973 2023-04-06 15:36:09.253377 halig-0.1.8/halig/main.py
--rw-r--r--   0        0        0     1855 2023-04-05 12:05:04.488420 halig-0.1.8/halig/settings.py
--rw-r--r--   0        0        0      733 2023-04-06 15:16:31.893718 halig-0.1.8/halig/utils.py
--rw-r--r--   0        0        0     2623 2023-04-06 15:38:12.012982 halig-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-31 07:27:12.166734 halig-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-01 10:11:11.307829 halig-0.1.8/tests/commands/__init__.py
--rw-r--r--   0        0        0     1645 2023-04-04 12:11:25.943270 halig-0.1.8/tests/commands/conftest.py
--rw-r--r--   0        0        0     1168 2023-04-04 12:11:25.939270 halig-0.1.8/tests/commands/test_edit.py
--rw-r--r--   0        0        0     1563 2023-04-03 08:07:50.529804 halig-0.1.8/tests/commands/test_notebooks.py
--rw-r--r--   0        0        0     1141 2023-04-04 12:11:25.935270 halig-0.1.8/tests/commands/test_show.py
--rw-r--r--   0        0        0     2820 2023-04-04 12:11:25.959270 halig-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     1784 2023-03-31 15:58:50.044795 halig-0.1.8/tests/test_encryption.py
--rw-r--r--   0        0        0     1541 2023-03-31 15:58:50.044795 halig-0.1.8/tests/test_settings.py
--rw-r--r--   0        0        0     1482 2023-04-06 15:29:55.766728 halig-0.1.8/tests/test_utils.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 halig-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34670 2023-04-12 19:46:50.194310 halig-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1248 2023-04-24 10:55:32.886664 halig-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.0/halig/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-24 11:57:00.923504 halig-0.2.0/halig/__version__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.194310 halig-0.2.0/halig/commands/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/base.py
+-rw-r--r--   0        0        0     2767 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/edit.py
+-rw-r--r--   0        0        0     1076 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/notebooks.py
+-rw-r--r--   0        0        0     1199 2023-04-12 19:47:22.382591 halig-0.2.0/halig/commands/show.py
+-rw-r--r--   0        0        0     1391 2023-04-12 19:47:22.382591 halig-0.2.0/halig/encryption.py
+-rw-r--r--   0        0        0     1354 2023-04-12 19:47:22.382591 halig-0.2.0/halig/literals.py
+-rw-r--r--   0        0        0     2868 2023-04-24 11:57:00.923504 halig-0.2.0/halig/main.py
+-rw-r--r--   0        0        0     1855 2023-04-12 19:47:22.382591 halig-0.2.0/halig/settings.py
+-rw-r--r--   0        0        0      733 2023-04-12 19:47:22.382591 halig-0.2.0/halig/utils.py
+-rw-r--r--   0        0        0     2623 2023-04-24 11:57:28.359440 halig-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 19:46:50.202310 halig-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:47:22.382591 halig-0.2.0/tests/commands/__init__.py
+-rw-r--r--   0        0        0     1645 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/conftest.py
+-rw-r--r--   0        0        0     1168 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/test_edit.py
+-rw-r--r--   0        0        0     1563 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/test_notebooks.py
+-rw-r--r--   0        0        0     1141 2023-04-24 10:55:32.886664 halig-0.2.0/tests/commands/test_show.py
+-rw-r--r--   0        0        0     2820 2023-04-12 19:47:22.382591 halig-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1784 2023-04-12 19:47:22.382591 halig-0.2.0/tests/test_encryption.py
+-rw-r--r--   0        0        0     1541 2023-04-12 19:47:22.386591 halig-0.2.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1482 2023-04-24 10:55:32.886664 halig-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 halig-0.2.0/PKG-INFO
```

### Comparing `halig-0.1.8/LICENSE` & `halig-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/README.md` & `halig-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/halig/commands/edit.py` & `halig-0.2.0/halig/commands/edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/halig/commands/notebooks.py` & `halig-0.2.0/halig/commands/notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/halig/commands/show.py` & `halig-0.2.0/halig/commands/show.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/halig/encryption.py` & `halig-0.2.0/halig/encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/halig/literals.py` & `halig-0.2.0/halig/literals.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/halig/settings.py` & `halig-0.2.0/halig/settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/halig/utils.py` & `halig-0.2.0/halig/utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/pyproject.toml` & `halig-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Terminals",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.1.8"
+version = "0.2.0"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "https://git.roboces.dev/catalin/halig"
 Repository = "https://git.roboces.dev/catalin/halig"
```

### Comparing `halig-0.1.8/tests/commands/conftest.py` & `halig-0.2.0/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/tests/commands/test_edit.py` & `halig-0.2.0/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/tests/commands/test_notebooks.py` & `halig-0.2.0/tests/commands/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/tests/commands/test_show.py` & `halig-0.2.0/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/tests/conftest.py` & `halig-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/tests/test_encryption.py` & `halig-0.2.0/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/tests/test_settings.py` & `halig-0.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/tests/test_utils.py` & `halig-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.1.8/PKG-INFO` & `halig-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halig
-Version: 0.1.8
+Version: 0.2.0
 Summary: age-encrypted, file-based, note-taking CLI app
 Keywords: cli notes age rage encryption notebook
 Author-Email: cătălin <185504a9@duck.com>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

