# Comparing `tmp/ckanext-saml-0.3.0.tar.gz` & `tmp/ckanext-saml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-saml-0.3.0.tar", last modified: Mon Apr  3 20:49:31 2023, max compression
+gzip compressed data, was "ckanext-saml-0.3.1.tar", last modified: Mon Apr 24 12:29:21 2023, max compression
```

## Comparing `ckanext-saml-0.3.0.tar` & `ckanext-saml-0.3.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.819297 ckanext-saml-0.3.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      192 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7026 2023-04-03 20:49:31.819297 ckanext-saml-0.3.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6376 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/saml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       91 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2949 2023-04-03 20:47:42.000000 ckanext-saml-0.3.0/ckanext/saml/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2313 2022-10-24 19:56:23.000000 ckanext-saml-0.3.0/ckanext/saml/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      693 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/saml/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1201 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/logic/action.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.799297 ckanext-saml-0.3.0/ckanext/saml/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/saml/migration/saml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/migration/saml/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/migration/saml/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/migration/saml/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/saml/migration/saml/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      794 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/saml/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       50 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      829 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/model/user.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1823 2023-04-03 20:47:42.000000 ckanext-saml-0.3.0/ckanext/saml/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.799297 ckanext-saml-0.3.0/ckanext/saml/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/saml/templates/admin/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      166 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/templates/admin/base.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.809297 ckanext-saml-0.3.0/ckanext/saml/templates/user/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3617 2023-04-03 20:47:42.000000 ckanext-saml-0.3.0/ckanext/saml/templates/user/edit_user_form.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/templates/user/login.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.819297 ckanext-saml-0.3.0/ckanext/saml/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      242 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.819297 ckanext-saml-0.3.0/ckanext/saml/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1177 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/tests/model/test_user.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1358 2022-11-07 20:14:10.000000 ckanext-saml-0.3.0/ckanext/saml/tests/test_helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       94 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1785 2022-10-24 20:01:19.000000 ckanext-saml-0.3.0/ckanext/saml/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.819297 ckanext-saml-0.3.0/ckanext/saml/views/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/ckanext/saml/views/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9866 2023-04-03 20:47:42.000000 ckanext-saml-0.3.0/ckanext/saml/views/saml.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-03 20:49:31.819297 ckanext-saml-0.3.0/ckanext_saml.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7026 2023-04-03 20:49:31.000000 ckanext-saml-0.3.0/ckanext_saml.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1405 2023-04-03 20:49:31.000000 ckanext-saml-0.3.0/ckanext_saml.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-03 20:49:31.000000 ckanext-saml-0.3.0/ckanext_saml.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      110 2023-04-03 20:49:31.000000 ckanext-saml-0.3.0/ckanext_saml.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-03 20:49:31.000000 ckanext-saml-0.3.0/ckanext_saml.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       68 2023-04-03 20:49:31.000000 ckanext-saml-0.3.0/ckanext_saml.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-03 20:49:31.000000 ckanext-saml-0.3.0/ckanext_saml.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1664 2023-04-03 20:49:31.819297 ckanext-saml-0.3.0/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-24 19:17:59.000000 ckanext-saml-0.3.0/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      199 2023-04-11 20:10:06.000000 ckanext-saml-0.3.1/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7026 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6376 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.234967 ckanext-saml-0.3.1/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       91 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2949 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2313 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      693 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1201 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/logic/action.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.234967 ckanext-saml-0.3.1/ckanext/saml/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/migration/saml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      794 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       50 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      829 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/model/user.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1823 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.234967 ckanext-saml-0.3.1/ckanext/saml/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/templates/admin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      166 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/templates/admin/base.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/templates/user/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3663 2023-04-24 12:27:53.000000 ckanext-saml-0.3.1/ckanext/saml/templates/user/edit_user_form.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/templates/user/login.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      242 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1177 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/tests/model/test_user.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1358 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/tests/test_helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       94 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1785 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/utils.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.244967 ckanext-saml-0.3.1/ckanext/saml/views/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/ckanext/saml/views/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9866 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/ckanext/saml/views/saml.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/ckanext_saml.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7026 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1405 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      110 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       68 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:29:21.000000 ckanext-saml-0.3.1/ckanext_saml.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2023-04-11 20:04:41.000000 ckanext-saml-0.3.1/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1664 2023-04-24 12:29:21.254967 ckanext-saml-0.3.1/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-24 19:17:59.000000 ckanext-saml-0.3.1/setup.py
```

### Comparing `ckanext-saml-0.3.0/LICENSE` & `ckanext-saml-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/PKG-INFO` & `ckanext-saml-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-saml
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/DataShades/ckanext-saml
 Author: Yan Rudendo
 Author-email: yan.rudenko@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-saml-0.3.0/README.md` & `ckanext-saml-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/config.py` & `ckanext-saml-0.3.1/ckanext/saml/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/helpers.py` & `ckanext-saml-0.3.1/ckanext/saml/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/interfaces.py` & `ckanext-saml-0.3.1/ckanext/saml/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/logic/action.py` & `ckanext-saml-0.3.1/ckanext/saml/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/migration/saml/alembic.ini` & `ckanext-saml-0.3.1/ckanext/saml/migration/saml/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/migration/saml/env.py` & `ckanext-saml-0.3.1/ckanext/saml/migration/saml/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py` & `ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/25dc326c059e_add_foreign_key_constraint_on_user_id.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py` & `ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/92745f8a6168_create_user_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py` & `ckanext-saml-0.3.1/ckanext/saml/migration/saml/versions/e8e7ebedf90d_add_attributes_column_to_saml2_user_.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/model/user.py` & `ckanext-saml-0.3.1/ckanext/saml/model/user.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/plugin.py` & `ckanext-saml-0.3.1/ckanext/saml/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/templates/user/edit_user_form.html` & `ckanext-saml-0.3.1/ckanext/saml/templates/user/edit_user_form.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% import 'macros/form.html' as form %}
 {% set is_saml_user = h.saml_is_saml_user(g.user) %}
 
 <form id="user-edit-form" class="dataset-form" method="post" action="{{ action }}" enctype="multipart/form-data">
+    {{ h.csrf_input() if "csrf_input" in h }}
     {{ form.errors(error_summary) }}
 
     <fieldset>
         <legend>{{ _('Change details') }}</legend>
         {{ form.input('name', label=_('Username'), id='field-username', value=data.name, error=errors.name, classes=['control-medium'], attrs={'readonly': '', 'class': 'form-control'}) }}
 
         {{ form.input('fullname', label=_('Full name'), id='field-fullname', value=data.fullname, error=errors.fullname, placeholder=_('eg. Joe Bloggs'), classes=['control-medium']) }}
```

### Comparing `ckanext-saml-0.3.0/ckanext/saml/tests/model/test_user.py` & `ckanext-saml-0.3.1/ckanext/saml/tests/model/test_user.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/tests/test_helpers.py` & `ckanext-saml-0.3.1/ckanext/saml/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/utils.py` & `ckanext-saml-0.3.1/ckanext/saml/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext/saml/views/saml.py` & `ckanext-saml-0.3.1/ckanext/saml/views/saml.py`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/ckanext_saml.egg-info/PKG-INFO` & `ckanext-saml-0.3.1/ckanext_saml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-saml
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/DataShades/ckanext-saml
 Author: Yan Rudendo
 Author-email: yan.rudenko@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-saml-0.3.0/ckanext_saml.egg-info/SOURCES.txt` & `ckanext-saml-0.3.1/ckanext_saml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-saml-0.3.0/setup.cfg` & `ckanext-saml-0.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-saml
-version = 0.3.0
+version = 0.3.1
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-saml
 author = Yan Rudendo
 author_email = yan.rudenko@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-saml-0.3.0/setup.py` & `ckanext-saml-0.3.1/setup.py`

 * *Files identical despite different names*

