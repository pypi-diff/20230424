# Comparing `tmp/django_encryption-0.3.0.tar.gz` & `tmp/django_encryption-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_encryption-0.3.0.tar", max compression
+gzip compressed data, was "django_encryption-0.3.1.tar", max compression
```

## Comparing `django_encryption-0.3.0.tar` & `django_encryption-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6084 2023-04-23 13:47:23.036030 django_encryption-0.3.0/README.md
--rw-r--r--   0        0        0       22 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/__init__.py
--rw-r--r--   0        0        0    15879 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/fields.py
--rw-r--r--   0        0        0        0 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/management/commands/__init__.py
--rw-r--r--   0        0        0     3278 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/management/commands/generate_vault_migration.py
--rw-r--r--   0        0        0        0 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/py.typed
--rw-r--r--   0        0        0    11063 2023-04-23 13:47:23.036030 django_encryption-0.3.0/django_encryption/vault_wrapper.py
--rw-r--r--   0        0        0     2159 2023-04-23 13:47:49.040706 django_encryption-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7876 1970-01-01 00:00:00.000000 django_encryption-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6084 2023-04-24 19:54:12.342349 django_encryption-0.3.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-24 19:54:12.342349 django_encryption-0.3.1/django_encryption/__init__.py
+-rw-r--r--   0        0        0    15879 2023-04-24 19:54:12.342349 django_encryption-0.3.1/django_encryption/fields.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:54:12.342349 django_encryption-0.3.1/django_encryption/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:54:12.342349 django_encryption-0.3.1/django_encryption/management/commands/__init__.py
+-rw-r--r--   0        0        0     3278 2023-04-24 19:54:12.342349 django_encryption-0.3.1/django_encryption/management/commands/generate_vault_migration.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:54:12.342349 django_encryption-0.3.1/django_encryption/py.typed
+-rw-r--r--   0        0        0    11063 2023-04-24 19:54:12.342349 django_encryption-0.3.1/django_encryption/vault_wrapper.py
+-rw-r--r--   0        0        0     2160 2023-04-24 19:54:35.958666 django_encryption-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7876 1970-01-01 00:00:00.000000 django_encryption-0.3.1/PKG-INFO
```

### Comparing `django_encryption-0.3.0/README.md` & `django_encryption-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.0/django_encryption/fields.py` & `django_encryption-0.3.1/django_encryption/fields.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.0/django_encryption/management/commands/generate_vault_migration.py` & `django_encryption-0.3.1/django_encryption/management/commands/generate_vault_migration.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.0/django_encryption/vault_wrapper.py` & `django_encryption-0.3.1/django_encryption/vault_wrapper.py`

 * *Files identical despite different names*

### Comparing `django_encryption-0.3.0/pyproject.toml` & `django_encryption-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-encryption"
-version = "0.3.0"
+version = "0.3.1"
 description = "A set of fields that wrap standard Django fields with encryption provided Piiano Vault."
 authors = ["Imri Goldberg <imri.goldberg@piiano.com>"]
 license = "MIT"
 packages = [ { include = "django_encryption" } ]
 readme = "README.md"
 repository = "https://github.com/piiano/vault-python"
 keywords = [ "encryption", "django", "fields" ]
@@ -74,8 +74,8 @@
 
 [testenv]
 whitelist_externals = poetry
 commands = 
     poetry install -v --with dev
     python manage.py test
 
-"""
+"""
```

### Comparing `django_encryption-0.3.0/PKG-INFO` & `django_encryption-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-encryption
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of fields that wrap standard Django fields with encryption provided Piiano Vault.
 Home-page: https://github.com/piiano/vault-python
 License: MIT
 Keywords: encryption,django,fields
 Author: Imri Goldberg
 Author-email: imri.goldberg@piiano.com
 Requires-Python: >=3.8,<4.0
```

