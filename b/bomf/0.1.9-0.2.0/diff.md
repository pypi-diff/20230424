# Comparing `tmp/bomf-0.1.9.tar.gz` & `tmp/bomf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.1.9.tar", last modified: Fri Apr 14 10:33:54 2023, max compression
+gzip compressed data, was "bomf-0.2.0.tar", last modified: Mon Apr 24 12:32:52 2023, max compression
```

## Comparing `bomf-0.1.9.tar` & `bomf-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.306327 bomf-0.1.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 10:33:44.000000 bomf-0.1.9/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 10:33:44.000000 bomf-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 10:33:44.000000 bomf-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-14 10:33:44.000000 bomf-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-14 10:33:54.310327 bomf-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-14 10:33:44.000000 bomf-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-14 10:33:44.000000 bomf-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 10:33:44.000000 bomf-0.1.9/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 10:33:44.000000 bomf-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-14 10:33:54.310327 bomf-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 10:33:44.000000 bomf-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.306327 bomf-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/validation/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-14 10:33:44.000000 bomf-0.1.9/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 10:33:54.000000 bomf-0.1.9/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-14 10:33:44.000000 bomf-0.1.9/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:33:54.310327 bomf-0.1.9/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-04-14 10:33:44.000000 bomf-0.1.9/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.909682 bomf-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.901682 bomf-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.901682 bomf-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-24 12:32:44.000000 bomf-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-24 12:32:44.000000 bomf-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 12:32:44.000000 bomf-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-24 12:32:52.909682 bomf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-24 12:32:44.000000 bomf-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-24 12:32:44.000000 bomf-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 12:32:44.000000 bomf-0.2.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-24 12:32:44.000000 bomf-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-24 12:32:52.909682 bomf-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 12:32:44.000000 bomf-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.897682 bomf-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.901682 bomf-0.2.0/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/validation/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-24 12:32:44.000000 bomf-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.909682 bomf-0.2.0/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_validation.py
```

### Comparing `bomf-0.1.9/.github/dependabot.yml` & `bomf-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.github/workflows/black.yml` & `bomf-0.2.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.github/workflows/codeql-analysis.yml` & `bomf-0.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.github/workflows/coverage.yml` & `bomf-0.2.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.github/workflows/packaging_test.yml` & `bomf-0.2.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.github/workflows/python-publish.yml` & `bomf-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.github/workflows/pythonlint.yml` & `bomf-0.2.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.github/workflows/unittests.yml` & `bomf-0.2.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.gitignore` & `bomf-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/.pre-commit-config.yaml` & `bomf-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/LICENSE` & `bomf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/PKG-INFO` & `bomf-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.1.9
+Version: 0.2.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.1.9/README.md` & `bomf-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/pyproject.toml` & `bomf-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/requirements.txt` & `bomf-0.2.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile requirements.in
 #
-attrs==22.2.0
+attrs==23.1.0
     # via -r requirements.in
 bidict==0.22.1
     # via -r requirements.in
 bo4e==0.4.7
     # via -r requirements.in
 frozendict==2.3.7
     # via -r requirements.in
```

### Comparing `bomf-0.1.9/setup.cfg` & `bomf-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf/__init__.py` & `bomf-0.2.0/src/bomf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
         run the entire migration flow from source to target which includes:
         1. create bo4e data source using the source_data_set_to_bo4e_mapper
         2. checking that all the bo4e data sets obey the validation rules
         3. mapping from bo4e to the target data model
         4. loading the target data models into the target system.
         """
         # todo: here we should add some logging and statistics stuff
-        bo4e_datasets = self.source_data_set_to_bo4e_mapper.create_data_sets()
+        bo4e_datasets = await self.source_data_set_to_bo4e_mapper.create_data_sets()
         await self.validation.validate(*bo4e_datasets)
-        target_data_models = self.bo4e_to_target_mapper.create_target_models(bo4e_datasets)
+        target_data_models = await self.bo4e_to_target_mapper.create_target_models(bo4e_datasets)
         loading_summaries = await self.target_loader.load_entities(target_data_models)
         return loading_summaries
```

### Comparing `bomf-0.1.9/src/bomf/filter/__init__.py` & `bomf-0.2.0/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.2.0/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf/loader/entityloader.py` & `bomf-0.2.0/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf/mapper/__init__.py` & `bomf-0.2.0/src/bomf/mapper/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 mappers convert from source data model to BO4E and from BO4E to a target data model
 """
+import asyncio
 from abc import ABC, abstractmethod
 from typing import Generic, List, TypeVar
 
 from bomf.model import Bo4eDataSet
 
 TargetDataModel = TypeVar("TargetDataModel")
 """
@@ -24,33 +25,34 @@
     A mapper that maps one or multiple sources into Bo4eDataSets
     """
 
     # the inheriting class is free to combine and bundle the source data as it wants.
     # the only thing it has to provide is a method to create_data_sets (in bo4e).
     # we don't care from where it gets them in the first place
 
-    def create_data_sets(self) -> List[IntermediateDataSet]:
+    async def create_data_sets(self) -> List[IntermediateDataSet]:
         """
         apply the mapping to all the provided source data sets.
 
         """
         raise NotImplementedError("The inheriting class has to implement this method")
 
 
 # pylint:disable=too-few-public-methods
 class Bo4eDataSetToTargetMapper(ABC, Generic[TargetDataModel, IntermediateDataSet]):
     """
     A mapper that transforms data from the intermediate bo4e model to the target data model
     """
 
     @abstractmethod
-    def create_target_model(self, dataset: IntermediateDataSet) -> TargetDataModel:
+    async def create_target_model(self, dataset: IntermediateDataSet) -> TargetDataModel:
         """
         maps the given source data model into an intermediate data set
         """
 
-    def create_target_models(self, datasets: List[IntermediateDataSet]) -> List[TargetDataModel]:
+    async def create_target_models(self, datasets: List[IntermediateDataSet]) -> List[TargetDataModel]:
         """
         apply the mapping to all the provided dataset
         """
         # here we could use some error handling in the future
-        return [self.create_target_model(dataset=dataset) for dataset in datasets]
+        tasks = [self.create_target_model(dataset=dataset) for dataset in datasets]
+        return await asyncio.gather(*tasks)
```

### Comparing `bomf-0.1.9/src/bomf/model/__init__.py` & `bomf-0.2.0/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf/provider/__init__.py` & `bomf-0.2.0/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf/validation/core.py` & `bomf-0.2.0/src/bomf/validation/core.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf/validation/utils.py` & `bomf-0.2.0/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/src/bomf.egg-info/PKG-INFO` & `bomf-0.2.0/src/bomf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.1.9
+Version: 0.2.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.1.9/src/bomf.egg-info/SOURCES.txt` & `bomf-0.2.0/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/tox.ini` & `bomf-0.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/unittests/test_bo4e_data_set.py` & `bomf-0.2.0/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/unittests/test_entity_loader.py` & `bomf-0.2.0/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/unittests/test_filter.py` & `bomf-0.2.0/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/unittests/test_mapper.py` & `bomf-0.2.0/unittests/test_mapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,62 +34,62 @@
 # - the source data model is a dictionary
 # - the intermediate data model are BO4E MaLo and MeLo
 # - the target data model is a list of string
 # This is just to demonstrate the mapping structures.
 
 
 class _DictToMaLoMeLoMapper(SourceToBo4eDataSetMapper):
-    def create_data_sets(self) -> List[_MaLoAndMeLo]:
+    async def create_data_sets(self) -> List[_MaLoAndMeLo]:
         return [
             _MaLoAndMeLo(
                 melo=Messlokation.construct(messlokations_id=source["meloId"]),
                 malo=Marktlokation.construct(marktlokations_id=source["maloId"]),
             )
             for source in [{"maloId": "54321012345", "meloId": "DE000111222333"}]
         ]
 
 
 class _MaLoMeLoToListMapper(Bo4eDataSetToTargetMapper):
-    def create_target_model(self, dataset: _MaLoAndMeLo) -> List[str]:
+    async def create_target_model(self, dataset: _MaLoAndMeLo) -> List[str]:
         return [
             dataset.get_business_object(Marktlokation).marktlokations_id,
             dataset.get_business_object(Messlokation).messlokations_id,
         ]
 
 
 class TestMapper:
-    def test_source_to_intermediate_mapper_batch(self):
+    async def test_source_to_intermediate_mapper_batch(self):
         mapper = _DictToMaLoMeLoMapper()
-        actual = mapper.create_data_sets()
+        actual = await mapper.create_data_sets()
         assert actual == [
             _MaLoAndMeLo(
                 melo=Messlokation.construct(messlokations_id="DE000111222333"),
                 malo=Marktlokation.construct(marktlokations_id="54321012345"),
             )
         ]
 
-    def test_intermediate_to_target_mapper(self):
+    async def test_intermediate_to_target_mapper(self):
         """
         tests the single data set mapping
         """
         mapper = _MaLoMeLoToListMapper()
-        actual = mapper.create_target_model(
+        actual = await mapper.create_target_model(
             _MaLoAndMeLo(
                 melo=Messlokation.construct(messlokations_id="DE000111222333"),
                 malo=Marktlokation.construct(marktlokations_id="54321012345"),
             )
         )
         assert actual == ["54321012345", "DE000111222333"]
 
-    def test_intermediate_to_target_mapper_batch(self):
+    async def test_intermediate_to_target_mapper_batch(self):
         """
         test the batch mapping
         """
         mapper = _MaLoMeLoToListMapper()
-        actual = mapper.create_target_models(
+        actual = await mapper.create_target_models(
             [
                 _MaLoAndMeLo(
                     melo=Messlokation.construct(messlokations_id="DE000111222333"),
                     malo=Marktlokation.construct(marktlokations_id="54321012345"),
                 )
             ]
         )
```

### Comparing `bomf-0.1.9/unittests/test_migration.py` & `bomf-0.2.0/unittests/test_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,29 +51,29 @@
 
 
 class _MyToBo4eMapper(SourceToBo4eDataSetMapper[_MyIntermediateDataModel]):
     def __init__(self, what_ever_you_like: List[_MySourceDataModel]):
         # what_ever_you_like is a place holde for all the relation magic that may happen
         self._source_models = what_ever_you_like
 
-    def create_data_sets(self) -> List[_MyIntermediateDataModel]:
+    async def create_data_sets(self) -> List[_MyIntermediateDataModel]:
         return [_MyIntermediateDataModel(data=source) for source in self._source_models]
 
 
 async def _my_rule(data: Dict[str, str]) -> None:
     if "invalid" in data:
         raise ValueError("'invalid' in data")
 
 
 _my_validation = ValidatorSet[_MyIntermediateDataModel]()
 _my_validation.register(_my_rule, {"data": "data"})
 
 
 class _MyToTargetMapper(Bo4eDataSetToTargetMapper[_MyTargetDataModel, _MyIntermediateDataModel]):
-    def create_target_model(self, dataset: _MyIntermediateDataModel) -> _MyTargetDataModel:
+    async def create_target_model(self, dataset: _MyIntermediateDataModel) -> _MyTargetDataModel:
         my_dict = dataset.data
         for my_key, my_value in my_dict.items():
             return [my_key, my_value]
         return ["doesnt", "matter"]
 
 
 class _MyTargetLoader(EntityLoader):
```

### Comparing `bomf-0.1.9/unittests/test_source_data_provider.py` & `bomf-0.2.0/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.1.9/unittests/test_validation.py` & `bomf-0.2.0/unittests/test_validation.py`

 * *Files identical despite different names*

