# Comparing `tmp/cz_nhm-0.3.0.tar.gz` & `tmp/cz_nhm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_nhm-0.3.0.tar", last modified: Wed Feb  1 11:05:32 2023, max compression
+gzip compressed data, was "cz_nhm-0.4.0.tar", last modified: Mon Apr 24 12:01:13 2023, max compression
```

## Comparing `cz_nhm-0.3.0.tar` & `cz_nhm-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:05:32.434236 cz_nhm-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-01 11:05:21.000000 cz_nhm-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-01 11:05:32.434236 cz_nhm-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-01 11:05:21.000000 cz_nhm-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 11:05:32.434236 cz_nhm-0.3.0/cz_nhm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-01 11:05:32.000000 cz_nhm-0.3.0/cz_nhm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-01 11:05:32.000000 cz_nhm-0.3.0/cz_nhm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 11:05:32.000000 cz_nhm-0.3.0/cz_nhm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-01 11:05:32.000000 cz_nhm-0.3.0/cz_nhm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-01 11:05:32.000000 cz_nhm-0.3.0/cz_nhm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-02-01 11:05:21.000000 cz_nhm-0.3.0/cz_nhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-01 11:05:21.000000 cz_nhm-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 11:05:32.434236 cz_nhm-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:13.987220 cz_nhm-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 12:01:02.000000 cz_nhm-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-24 12:01:13.987220 cz_nhm-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-24 12:01:02.000000 cz_nhm-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:13.987220 cz_nhm-0.4.0/cz_nhm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-24 12:01:13.000000 cz_nhm-0.4.0/cz_nhm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-24 12:01:13.000000 cz_nhm-0.4.0/cz_nhm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:01:13.000000 cz_nhm-0.4.0/cz_nhm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 12:01:13.000000 cz_nhm-0.4.0/cz_nhm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 12:01:13.000000 cz_nhm-0.4.0/cz_nhm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 12:01:13.000000 cz_nhm-0.4.0/cz_nhm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-24 12:01:02.000000 cz_nhm-0.4.0/cz_nhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-24 12:01:02.000000 cz_nhm-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:01:13.987220 cz_nhm-0.4.0/setup.cfg
```

### Comparing `cz_nhm-0.3.0/LICENSE` & `cz_nhm-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cz_nhm-0.3.0/PKG-INFO` & `cz_nhm-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz_nhm
-Version: 0.3.0
+Version: 0.4.0
 Summary: Commitizen config for the NHM, London
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: MIT
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/cz-nhm
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/cz-nhm/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cz_nhm-0.3.0/cz_nhm.egg-info/PKG-INFO` & `cz_nhm-0.4.0/cz_nhm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-nhm
-Version: 0.3.0
+Version: 0.4.0
 Summary: Commitizen config for the NHM, London
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: MIT
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/cz-nhm
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/cz-nhm/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cz_nhm-0.3.0/cz_nhm.py` & `cz_nhm-0.4.0/cz_nhm.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,10 +203,7 @@
         return (
             r'(?s)'  # To explictly make . match new line
             rf'({"|".join([c for c in change_types if c.short_name != "BREAKING CHANGE"])})'  # type
             r'(\(\S+\))?!?:'  # scope
             r'( [^\n\r]+)'  # subject
             r'((\n\n.*)|(\s*))?$'
         )
-
-
-discover_this = NHMCz
```

### Comparing `cz_nhm-0.3.0/pyproject.toml` & `cz_nhm-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cz_nhm"
-version = "0.3.0"
+version = "0.4.0"
 description = "Commitizen config for the NHM, London"
 readme = "README.md"
 license = { text = "MIT" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
 classifiers = [
@@ -15,14 +15,17 @@
     "commitizen"
 ]
 
 [project.urls]
 repository = "https://github.com/NaturalHistoryMuseum/cz-nhm"
 changelog = "https://github.com/NaturalHistoryMuseum/cz-nhm/blob/main/CHANGELOG.md"
 
+[project.entry-points."commitizen.plugin"]
+plugin = "cz_nhm:NHMCz"
+
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [tool]
@@ -41,14 +44,14 @@
 wrap-summaries = 88
 wrap-descriptions = 88
 pre-summary-newline = true
 make-summary-multi-line = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.0"
+version = "0.4.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = false
 version_files = [
     "pyproject.toml:version"
 ]
```

