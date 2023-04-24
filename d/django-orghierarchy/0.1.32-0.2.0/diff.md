# Comparing `tmp/django-orghierarchy-0.1.32.tar.gz` & `tmp/django-orghierarchy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-orghierarchy-0.1.32.tar", last modified: Thu Mar 23 06:23:36 2023, max compression
+gzip compressed data, was "django-orghierarchy-0.2.0.tar", last modified: Mon Apr 24 07:35:50 2023, max compression
```

## Comparing `django-orghierarchy-0.1.32.tar` & `django-orghierarchy-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.359078 django-orghierarchy-0.1.32/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-03-23 06:23:36.359078 django-orghierarchy-0.1.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.347078 django-orghierarchy-0.1.32/django_orghierarchy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)    20868 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/importers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.347078 django-orghierarchy-0.1.32/django_orghierarchy/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.347078 django-orghierarchy-0.1.32/django_orghierarchy/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/management/commands/import_organizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.351078 django-orghierarchy-0.1.32/django_orghierarchy/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0002_organization_replaced_by.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0003_rm_responsible_org_add_internal_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0004_add_affiliated_org_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0005_add_fields_to_organization_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0006_add_user_editable_to_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0007_set_editable_false_on_mptt_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0008_modify_organization_on_deletes.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0009_add_change_organization_regular_users_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0010_rename_user_editable.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/0011_alter_datasource_user_editable_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/django_orghierarchy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.347078 django-orghierarchy-0.1.32/django_orghierarchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-03-23 06:23:36.000000 django-orghierarchy-0.1.32/django_orghierarchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-23 06:23:36.000000 django-orghierarchy-0.1.32/django_orghierarchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 06:23:36.000000 django-orghierarchy-0.1.32/django_orghierarchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 06:23:36.000000 django-orghierarchy-0.1.32/django_orghierarchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-23 06:23:36.000000 django-orghierarchy-0.1.32/django_orghierarchy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-23 06:23:36.363078 django-orghierarchy-0.1.32/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1411 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.355078 django-orghierarchy-0.1.32/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.359078 django-orghierarchy-0.1.32/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.359078 django-orghierarchy-0.1.32/tests/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/migrations/0002_customdatasource_user_editable_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/settings_custom_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/settings_custom_pk_ds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:36.359078 django-orghierarchy-0.1.32/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/tests/test_custom_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_app/tests/test_custom_pk_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)    25923 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_importers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-23 06:23:26.000000 django-orghierarchy-0.1.32/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:50.884952 django-orghierarchy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-24 07:35:50.888952 django-orghierarchy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:50.880952 django-orghierarchy-0.2.0/django_orghierarchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26587 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/importers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:50.880952 django-orghierarchy-0.2.0/django_orghierarchy/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:50.880952 django-orghierarchy-0.2.0/django_orghierarchy/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/management/commands/import_organizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:50.884952 django-orghierarchy-0.2.0/django_orghierarchy/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0002_organization_replaced_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0003_rm_responsible_org_add_internal_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0004_add_affiliated_org_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0005_add_fields_to_organization_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0006_add_user_editable_to_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0007_set_editable_false_on_mptt_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0008_modify_organization_on_deletes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0009_add_change_organization_regular_users_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0010_rename_user_editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/0011_alter_datasource_user_editable_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/django_orghierarchy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:50.880952 django-orghierarchy-0.2.0/django_orghierarchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-24 07:35:50.000000 django-orghierarchy-0.2.0/django_orghierarchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-24 07:35:50.000000 django-orghierarchy-0.2.0/django_orghierarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:35:50.000000 django-orghierarchy-0.2.0/django_orghierarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 07:35:50.000000 django-orghierarchy-0.2.0/django_orghierarchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 07:35:50.000000 django-orghierarchy-0.2.0/django_orghierarchy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-24 07:35:50.888952 django-orghierarchy-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1742 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:35:50.884952 django-orghierarchy-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27999 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28901 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_importers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_importers_openahjo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 07:35:35.000000 django-orghierarchy-0.2.0/tests/test_utils.py
```

### Comparing `django-orghierarchy-0.1.32/LICENSE` & `django-orghierarchy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/PKG-INFO` & `django-orghierarchy-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,102 @@
-Metadata-Version: 2.1
-Name: django-orghierarchy
-Version: 0.1.32
-Summary: Reusable Django application for hierarchical organizations.
-Home-page: https://github.com/City-of-Helsinki/django-orghierarchy
-Author: City of Helsinki
-Author-email: dev@hel.fi
-License: MIT License
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-License-File: LICENSE
-
 # django-orghierarchy
 
 Reusable Django application for hierarchical organizations
 
 # Installation
 
 1. `pip install django-orghierarchy`
 
 2. Add `django_orghierarchy` to `INSTALLED_APPS`
 
 3. If you wish to use your own Django model as data source model (the same way you hot-swap your own user model in Django), add `DJANGO_ORGHIERARCHY_DATASOURCE_MODEL = 'yourapp.DataSource'` to your project settings. Otherwise, the barebones Django model `DataSource` at django_orghierarchy/models.py is used, it contains the fields a data source model *must* contain to be used with django-orghierarchy. Similarly, django-orghierarchy links to your user model, so `AUTH_USER_MODEL` must be defined in Django project settings as always.
 
 4. Run migrations
 
-    ```python
-    python manage.py migrate django_orghierarchy
-    ```
+ ```bash
+ python manage.py migrate django_orghierarchy
+ ```
+
 
 # Usage
 
 The `Organization` class is the main feature of django-orghierarchy. We use [`django-mptt`](https://github.com/django-mptt/django-mptt/) to implement an organization hierarchy that can be as deep as you wish. Each organization has a name, a data source (referring to the system the organization data is from), origin_id (referring to organization id in the original data source), founding date and dissolution date, status (*normal* or *affiliated*), a place in a forest of organization trees, and possibly a *replacement organization*, which means a link to any other organization across the trees (making the forest strictly a directed graph, not a bunch of trees). Replacement organization allows linking dissolved organization structures to new ones so that old user rights are automatically transferred across the hierarchy to the replacing organization.
 
 Each organization may have `admin_users` and `regular_users`, which are linked to your Django user model. Also, an organization may have `sub_organizations` and `affiliated_organizations`. You may have any number of top level organizations. Also, some extra user permissions are defined, i.e. `add_affiliated_organization`, `change_affiliated_organization`, `delete_affiliated_organization`, `replace_organization` and `change_organization_regular_users`. These permissions are for adding *regular users* and *affiliated organizations* in Django-admin, and creating *replacement* links, without being allowed to touch the *admin users* or the existing organization hierarchy. *Affiliated* organizations usually have more limited rights than *normal* organizations within the hierarchy; they are meant for external organizations you collaborate with and wish to grant limited rights to.
 
 Your desired user rights and permissions for each user group in each level of the organization depend on your application details, so you should implement your own user rights checks depending on your needs. You may e.g. create a user model permissions mixin that uses information on the user organization, as done in [Linkedevents permissions](https://github.com/City-of-Helsinki/linkedevents/blob/master/events/permissions.py) and [Linkedevents user model](https://github.com/City-of-Helsinki/linkedevents/blob/master/helevents/models.py). The user rights model is originally specified [here](https://github.com/City-of-Helsinki/linkedevents/issues/235).
 
 You may import an existing organization hierarchy from a REST API corresponding to the [6Aika Paatos decisionmaking API specification](https://github.com/6aika/api-paatos), based on the [Popolo project](http://www.popoloproject.com/), with the included importer, for example:
-
-    python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/"
+```bash
+python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/"
+```
     
 You may give the organization data source a specific id to correspond to your own data source model ids in your project:
-
-    python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/" -s original_id:imported_id
+```bash
+python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/" -s original_id:imported_id
+```
 
 Otherwise, the data source id in the original API is used for the imported organizations (`helsinki` in the Helsinki API).
 
+
 # Development
 
+Install requirements.
+
+```bash
+# Package requirements
+pip install -e .
+# Development requirements
+pip install -r requirements.txt
+```
+
+
 ## Tests
 
+
 ### Unit tests
 
-Run tests
+Run the tests.
 
-    py.test
+```bash
+pytest
+```
 
-Run tests with coverage report
+Run the tests with coverage report.
 
-    py.test --cov-report html --cov .
+```bash
+pytest --cov-report html --cov .
+```
     
 Open htmlcov/index.html for the coverage report.
 
+
+### Running tests against multiple environments
+
+You can run the tests against multiple environments by using [tox](https://tox.readthedocs.io/en/latest/).
+Install `tox` globally and run:
+
+```bash
+tox
+```
+
+Use the `-f` option to specify target environments.
+
+```bash
+# Target only Python 3.9 environments
+tox -f py39
+# Target Python 3.9 and Django 3.2
+tox -f py39 django32
+```
+
+
 ### Integration tests
 
 We need to provide different settings files for the test as the
 setting variables for swappable model are only evaluated the first
-time the module is imported.
-
-Run tests
-
-    python manage.py test --tag=custom_ds --settings=tests.test_app.settings_custom_ds
-    python manage.py test --tag=custom_pk_ds --settings=tests.test_app.settings_custom_pk_ds
+time the module is imported. Integration tests are skipped by default.
 
+Run the integration tests.
+```bash
+pytest -m custom_ds --ds=tests.test_app.settings_custom_ds
+pytest -m custom_pk_ds --ds=tests.test_app.settings_custom_pk_ds
+```
```

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/admin.py` & `django-orghierarchy-0.2.0/django_orghierarchy/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from functools import reduce
+
 import swapper
 from django.contrib import admin
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 from mptt.admin import DraggableMPTTAdmin
-from functools import reduce
 
 from .forms import AffiliatedOrganizationForm, OrganizationForm, SubOrganizationForm
-from .models import OrganizationClass, Organization
+from .models import Organization, OrganizationClass
 from .utils import get_data_source_model
 
 data_source_model = swapper.get_model_name('django_orghierarchy', 'DataSource')
 # Only register admin when using default data source model
 # When the data source model is swapped, client code should
 # be responsible for creating admin page for the model
 if data_source_model == 'django_orghierarchy.DataSource':
@@ -161,26 +162,31 @@
 
 @admin.register(Organization)
 class OrganizationAdmin(DraggableMPTTAdmin):
     filter_horizontal = ('admin_users', 'regular_users')
     form = OrganizationForm
     inlines = [ProtectedSubOrganizationInline, SubOrganizationInline, AddSubOrganizationInline,
                ProtectedAffiliatedOrganizationInline, AffiliatedOrganizationInline, AddAffiliatedOrganizationInline]
-    search_fields = ('name', )
+    search_fields = ('name', 'id', 'origin_id', 'classification__id')
+    list_display = (*DraggableMPTTAdmin.list_display, 'identifier', 'classification_id')
 
     # these fields may not be changed at all in existing organizations
     existing_readonly_fields = ('id', 'data_source', 'origin_id', 'internal_type')
     # these fields may not be changed at all in protected organizations
     protected_readonly_fields = existing_readonly_fields + ('origin_id', 'classification', 'name', 'founding_date',
                                                             'dissolution_date', 'parent',)
 
+    def identifier(self, obj):
+        # Disable sorting on this column
+        return obj.id
+
     def get_queryset(self, request):
         if not request.user.is_superuser:
             if not request.user.admin_organizations.all():
-                return []
+                return Organization.objects.none()
             # regular admins have rights to all organizations below their level
             admin_orgs = []
             for admin_org in request.user.admin_organizations.all():
                 admin_orgs.append(admin_org.get_descendants(include_self=True))
             # for multiple admin_orgs, we have to combine the querysets and filter distinct
             return reduce(lambda a, b: a | b, admin_orgs).distinct()
         return super().get_queryset(request)
@@ -202,15 +208,15 @@
             # affiliated organizations, this i  s to make sure user cannot edit
             # current organization if he does not have change permission on
             # organization
             readonly_fields = self.form.base_fields.copy()
             if request.user.has_perm('django_orghierarchy.change_organization_regular_users'):
                 del readonly_fields['regular_users']
             return readonly_fields
-        if obj and not obj.data_source.user_editable_organizations:
+        if obj and obj.data_source and not obj.data_source.user_editable_organizations:
             # Organization data from protected data sources may not be edited
             if not request.user.has_perm('django_orghierarchy.replace_organization'):
                 # Replacing an organization in the hierarchy requires extra privileges
                 return self.protected_readonly_fields + ('replaced_by',)
             # Protected organizations allow only user fields to be changed
             return self.protected_readonly_fields
         # Editable organizations have no such restrictions, but replacement still requires extra privileges
```

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/api.py` & `django-orghierarchy-0.2.0/django_orghierarchy/api.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/forms.py` & `django-orghierarchy-0.2.0/django_orghierarchy/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,17 @@
             if self.instance.id:
                 # prevent self reference
                 qs = qs.exclude(id=self.instance.id)
             self.fields['replaced_by'].queryset = qs
 
         if 'data_source' in self.fields:
             # Only allow selecting data source within editable sources
-            self.fields['data_source'].queryset = get_data_source_model().objects.filter(user_editable_organizations=True)
-
+            self.fields['data_source'].queryset = (
+                get_data_source_model().objects.filter(user_editable_organizations=True)
+            )
         if 'parent' in self.fields and self.instance.id:
             # prevent recursive reference
             desc_ids = self.instance.get_descendants(include_self=True).values_list('id', flat=True)
             self.fields['parent'].queryset = Organization.objects.exclude(id__in=desc_ids)
 
     def clean(self):
         cleaned_data = super().clean()
@@ -66,15 +67,17 @@
             kwargs['initial'] = {}
         kwargs['initial']['internal_type'] = self.default_internal_type
         super().__init__(*args, **kwargs)
 
         # the fields can be dynamically exclude, for example set them to readonly in admin
         if 'data_source' in self.fields:
             # Only allow selecting data source within editable sources
-            self.fields['data_source'].queryset = get_data_source_model().objects.filter(user_editable_organizations=True)
+            self.fields['data_source'].queryset = (
+                get_data_source_model().objects.filter(user_editable_organizations=True)
+            )
 
     def clean_internal_type(self):
         return self.initial['internal_type']  # do not allow changing internal_type
 
 
 class AffiliatedOrganizationForm(SubOrganizationForm):
     default_internal_type = Organization.AFFILIATED
```

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/importers.py` & `django-orghierarchy-0.2.0/django_orghierarchy/importers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import copy
 import logging
 import re
+import urllib.parse
+import warnings
 from enum import Enum
 
 import requests
 from django.core.exceptions import ValidationError
 from django.core.validators import URLValidator
 from django.db import transaction
 
-from .models import OrganizationClass, Organization
+from .models import Organization, OrganizationClass
 from .utils import get_data_source_model
 
 logger = logging.getLogger(__name__)
 
 
 class DataImportError(Exception):
     pass
@@ -20,61 +22,76 @@
 
 class DataType(Enum):
     VALUE = 'value'
     STR_LOWER = 'str_lower'
     LINK = 'link'
     REGEX = 'regex'
     ORG_ID = 'org_id'
+    ORG_ID_REGEX = 'org_id_regex'
 
 
 class RestAPIImporter:
-    """This class allows importing organization data from a REST API endpoint. The default
-    configuration supports the 6aika Open Decision API specification:
+    """This class allows importing organization data from a REST API endpoint. The
+    default configuration supports the 6aika Open Decision API specification:
     https://github.com/6aika/api-paatos
 
-    The importer will also create data sources and organization classes if does not exist.
-    If a single value is provided to `data_source` and `classification` fields, then the
-    importer assumes the value is the name of the data source or organization class. If
-    an object (dict) is provided to `data_source` and `classification` fields, then the
-    importer will create objects with object data. Either full object data or a link to
-    full object data should be provided to parent field so that the importer can create
-    parent organization before creating child organization.
-
-    For use in multi-source setups, the importer may optionally create a parent organization
-    for the data source that is the common parent of all imported top-level organizations.
-    This way, separate organization hierarchies from different data sources may be stored
-    in the same application.
+    The importer will also create data sources and organization classes if does not
+    exist. If a single value is provided to `data_source` and `classification` fields,
+    then the importer assumes the value is the name of the data source or organization
+    class. If an object (dict) is provided to `data_source` and `classification` fields,
+    then the importer will create objects with object data. Either full object data or a
+    link to full object data should be provided to parent field so that the importer can
+    create parent organization before creating child organization.
+
+    For use in multi-source setups, the importer may optionally create a parent
+    organization for the data source that is the common parent of all imported top-level
+    organizations. This way, separate organization hierarchies from different data
+    sources may be stored in the same application.
 
     The client code can override the default config or pass in a config object to allow
     the importer parsing different REST API structures.
 
     Config options:
-        - next_key: The url to the next page if the source data is paginated, or None if not.
-        - results_key: The object key to the list of organization objects, or None if the list is at
-            root level.
-        - fields: The fields of which the values will be imported. The same fields will be imported
-            in organization classes, if present.
-        - update_fields: The fields to update if the organization with same origin_id and data
-            source exists.
+        - next_key: The url to the next page if the source data is paginated, or None if
+            not.
+        - results_key: The object key to the list of organization objects, or None if
+            the list is at root level.
+        - fields: The fields of which the values will be imported. The same fields will
+            be imported in organization classes, if present.
+        - update_fields: The fields to update if the organization with same origin_id
+            and data source exists.
+        - skip_classifications: List of organization classifications which will cause
+            organizations of this type to be skipped upon import.
+        - has_meta: Does the JSON contain a separate object for pagination. Default
+            False.
+        - deprecated: Is the configuration considered deprecated. Default False.
         - field_config: Configs for each field. Config options:
             - source_field: The source data object key where the field value comes from.
                 Defaults to original field name.
-            - data_type: The data type for the field, can be 'value', 'str_lower', 'link', 'regex' or 'org_id'.
-                Defaults to 'value'. If the data type is 'value', it will return the value
-                from source data; if the data type is 'str_lower', it will return the value stringified
-                and lowercased; if the data type is 'link', it will return the data fetched
-                from the link; if the data type is 'regex', it will return the value extracted
-                from the given pattern. If the data type is 'org_id', it will return the organization
-                in the JSON with the given 'id'.
+            - data_type: The data type for the field, can be 'value', 'str_lower',
+                'link', 'regex', 'org_id' or 'org_id_regex'.
+                Defaults to 'value'. If the data type is 'value', it will return the
+                value from source data; if the data type is 'str_lower', it will return
+                the value stringified and lowercased; if the data type is 'link', it
+                will return the data fetched from the link; if the data type is 'regex',
+                it will return the value extracted from the given pattern. If the data
+                type is 'org_id' or 'org_id_regex', it will return the organization in
+                the JSON with the given 'id'.
+            - pattern: The pattern to extract the value from the source data. Only used
+                when data_type is 'regex' or 'org_id_regex'.
+            - unquote: Should the value be run through urllib.parse.unquote. Defaults to
+                 False.
+            - unwrap_list: Value is wrapped inside of a list. Return the first value on
+                the list. Defaults to False.
             - optional: Whether the importer will continue if the field is missing.
                 Defaults to False.
         - rename_data_source: Data sources that are renamed during import.
         - default_data_source: Data source id to use for objects without data source.
-        - default_parent_organization: If set, name of the parent organization to be created for all
-            imported top level organizations.
+        - default_parent_organization: If set, name of the parent organization to be
+            created for all imported top level organizations.
 
     Example config:
         {
             'next_key': 'next',
             'results_key: 'results',
             'fields': ['origin_id', 'data_source', 'classification'],
             'update_fields': ['classification'],
@@ -93,15 +110,18 @@
                 'original_name_2': 'new_name_2',
             },
             'default_data_source': 'new_name_1',
             'default_parent_organization': None
         }
     """
 
+    # https://api.hel.fi/paatos/v1/organization/
     paatos_config = {
+        'deprecated': True,
+        'has_meta': False,
         'next_key': 'next',
         'results_key': 'results',
         'fields': [
             'data_source', 'origin_id', 'classification',
             'name', 'founding_date', 'dissolution_date',
             'parent',
         ],
@@ -111,20 +131,60 @@
         ],
         'field_config': {
             'parent': {
                 'data_type': 'link',
             },
             'origin_id': {
                 'data_type': 'str_lower',
-            }
+            },
+        },
+        'default_data_source': 'OpenDecisionAPI',
+    }
+
+    # https://dev.hel.fi/apis/openahjo
+    # https://dev.hel.fi/paatokset/v1/organization/
+    # https://github.com/City-of-Helsinki/openahjo
+    openahjo_config = {
+        'has_meta': True,
+        'next_key': 'next',
+        'results_key': 'objects',
+        'fields': [
+            'origin_id', 'classification',
+            'name', 'founding_date', 'dissolution_date',
+            'parent',
+        ],
+        'skip_classifications': ['office_holder', 'team', 'subteam', 'trustee'],
+        'update_fields': [
+            'classification', 'name', 'founding_date',
+            'dissolution_date', 'parent',
+        ],
+        'field_config': {
+            'name': {
+                'source_field': 'name_fi',
+            },
+            'classification': {
+                'source_field': 'type',
+            },
+            'parent': {
+                'source_field': 'parents',
+                'data_type': 'org_id_regex',
+                'unwrap_list': True,
+                'unquote': True,
+                'pattern': r"\/(\w+:\w+)\/$",
+                'optional': True,
+            },
+            'origin_id': {
+                'data_type': 'str_lower',
+            },
         },
-        'default_data_source': 'OpenDecisionAPI'
+        'default_data_source': 'OpenAhjoAPI',
     }
 
     tprek_config = {
+        'has_meta': False,
         'next_key': None,
         'results_key': None,
         'fields': [
             'origin_id', 'classification',
             'name', 'parent',
         ],
         'update_fields': [
@@ -143,21 +203,22 @@
             'classification': {
                 'source_field': 'organization_type',
                 'optional': True,
             },
             'name': {
                 'source_field': 'name_fi',
                 'optional': True,
-            }
+            },
         },
         'default_data_source': 'tprek',
-        'default_parent_organization': 'Pääkaupunkiseudun toimipisterekisteri'
+        'default_parent_organization': 'Pääkaupunkiseudun toimipisterekisteri',
     }
 
     default_config = paatos_config
+    timeout = 10
 
     def __init__(self, url, config=None):
         self.url = url
 
         self.config = copy.deepcopy(self.default_config)
         config = copy.deepcopy(config)
         if config:
@@ -168,24 +229,31 @@
             for field in config.get('fields', None):
                 if field in given_field_config:
                     merged_field_config[field] = given_field_config[field]
                 elif field in default_field_config:
                     merged_field_config[field] = default_field_config[field]
             self.config['field_config'] = merged_field_config
             self.config.update(config)
-        logger.info('Importing organization data from %s with the following config:' % self.url)
+        logger.info(f'Importing organization data from {self.url} with the following config:')
         logger.info(self.config)
         self.related_import_methods = {
             'data_source': self._import_data_source,
             'classification': self._import_organization_class,
             'parent': self._import_organization,
         }
 
+        if self.config.get('deprecated', False):
+            warnings.warn(
+                'RestAPIImporter is initialized with a deprecated configuration.',
+                DeprecationWarning, stacklevel=2
+            )
+
         self._organization_classes = {}
         self._data_sources = {}
+        self._organizations = {}
         self._default_parent = None
         if self.config.get('default_parent_organization', None):
             origin_id_config = self.config['field_config'].get('origin_id', None)
             origin_id_field = origin_id_config['source_field'] if origin_id_config else 'origin_id'
             data_source_config = self.config['field_config'].get('data_source', None)
             data_source_field = data_source_config['source_field'] if data_source_config else 'data_source'
             name_config = self.config['field_config'].get('name', None)
@@ -212,14 +280,19 @@
         return self.config['update_fields']
 
     @property
     def field_config(self):
         return self.config['field_config']
 
     @property
+    def has_meta(self):
+        """Whether the response contains a separate object for pagination."""
+        return self.config.get('has_meta', False)
+
+    @property
     def next_key(self):
         """Object key that stores the link to the next page"""
         return self.config['next_key']
 
     @property
     def results_key(self):
         """Object key that stores the list of organizations"""
@@ -227,18 +300,36 @@
 
     @property
     def rename_data_source(self):
         """Data source renaming configs"""
         return self.config.get('rename_data_source') or {}
 
     @property
+    def skip_classifications(self):
+        """List of organization classifications to skip"""
+        return self.config.get('skip_classifications') or []
+
+    @property
     def default_data_source(self):
         """Default data source string"""
         return self.config['default_data_source']
 
+    def _build_resource_url(self, resource_id) -> str:
+        """Build an url for the given resource id.
+
+        Resource identifiers in the data might be missing the scheme+host part.
+        With
+        - self.url = "https://dev.hel.fi/paatokset/v1/organization/" and
+        - resource_id = "/paatokset/v1/organization/?limit=20&offset=20"
+
+        the expected output is:
+        "https://dev.hel.fi/paatokset/v1/organization/?limit=20&offset=20"
+        """
+        return urllib.parse.urljoin(self.url, resource_id)
+
     def _get_organization_class(self, data):
         """Get organization class for the given object data
 
         The method will first try to get the organization class from cache, and
         then get from database if not cached.
         """
         # organization class supports id, data_source, origin_id and name.
@@ -252,22 +343,24 @@
                 data['origin_id'] = identifier.split(':')[1]
         # provided id used if origin id missing
         if 'origin_id' not in data or not data['origin_id']:
             data['origin_id'] = identifier
         # default data source used if missing
         if 'data_source' not in data or not data['data_source']:
             data['data_source'] = self.default_data_source
+        data_source_instance = self.related_import_methods['data_source'](data['data_source'])
         # reformat id to fit our model
         if not isinstance(identifier, str) or ':' not in identifier:
-            data['id'] = data['data_source'] + ':' + str(identifier)
-        data['data_source'] = self.related_import_methods['data_source'](data['data_source'])
+            data['id'] = data_source_instance.pk + ':' + str(identifier)
+        data['data_source'] = data_source_instance
         # extra fields should not crash the import. Only use specified fields.
         data = {field: value for (field, value) in data.items() if field in supported_fields}
         if identifier not in self._organization_classes:
-            organization_class, _ = OrganizationClass.objects.get_or_create(**data)
+            defaults = {'name': data.pop('name', data['id'])}
+            organization_class, _ = OrganizationClass.objects.get_or_create(**data, defaults=defaults)
             self._organization_classes[identifier] = organization_class
         return self._organization_classes[identifier]
 
     def _get_data_source(self, data):
         """Get data source for the given object data
 
         The method will first try to get the data source from cache, and
@@ -302,84 +395,117 @@
         config = self.field_config.get('origin_id') or {}
         if isinstance(data, dict):
             incoming_data = data
         else:
             raise DataImportError('Organization data must be dict.')
         origin_id = self._get_field_value(incoming_data, 'origin_id', config)
 
+        if origin_id in self._organizations:
+            # No need to re-import/update an organization which is already
+            # imported once in this run.
+            logger.debug(f'Using cached Organization: {origin_id}')
+            return self._organizations[origin_id]
+
         # data source may be missing altogether, or it may be optional
         data_source = None
         config = self.field_config.get('data_source') or {}
         try:
             data_source = self._get_field_value(incoming_data, 'data_source', config)
-        except DataImportError as exception:
+        except DataImportError:
             if not config or config.get('optional'):
                 pass
             else:
-                raise exception
+                raise
         if not data_source:
             data_source = self._get_field_value(
                 {'data_source': self.default_data_source}, 'data_source', {'data_type': 'value'})
 
+        logger.debug(f'Importing Organization: {origin_id}')
+
         # id is never imported in default config
 
         try:
-            values_to_update = {}
-            for field in self.update_fields:
-                config = self.field_config.get(field) or {}
-                try:
-                    value = self._get_field_value(incoming_data, field, config)
-                except DataImportError as exception:
-                    if config.get('optional'):
-                        continue
-                    else:
-                        raise exception
-                values_to_update[field] = value
-
-            # Organization parent (and its parent) have been imported and updated recursively. If one of
-            # them used to be the descendant of this organization, this might result in mptt InvalidMove
-            # exception if this organization instance is not up to date with the database.
-            # See https://github.com/django-mptt/django-mptt/issues/650
-
-            # Therefore, we may only fetch the organization from the db *after* all its parents have been
-            # processed, to get up to date status of the mptt tree before saving each organization.
-            # enforce lower case id standard, but recognize upper case ids as equal:
-            organization = Organization.objects.get(origin_id__iexact=origin_id, data_source=data_source)
-            logger.info('Organization already exists: {0}'.format(organization.id))
-            for field, value in values_to_update.items():
-                setattr(organization, field, value)
-            if (
-                self.config.get('default_parent_organization', None)
-                and not organization.parent
-                and organization != self._default_parent
-            ):
-                organization.parent = self._default_parent
+            return self._import_organization_update(incoming_data, origin_id, data_source)
+        except Organization.DoesNotExist:
+            return self._import_organization_create(incoming_data, origin_id, data_source)
+
+    def _import_organization_update(self, incoming_data, origin_id, data_source):
+        """Update an existing organization upon import."""
+        values_to_update = {}
+        for field in self.update_fields:
+            config = self.field_config.get(field) or {}
+            try:
+                value = self._get_field_value(incoming_data, field, config)
+            except DataImportError:
+                if config.get('optional'):
+                    continue
+                else:
+                    raise
+            values_to_update[field] = value
+
+        # Organization parent (and its parent) have been imported and updated recursively. If one of
+        # them used to be the descendant of this organization, this might result in mptt InvalidMove
+        # exception if this organization instance is not up-to-date with the database.
+        # See https://github.com/django-mptt/django-mptt/issues/650
+
+        # Therefore, we may only fetch the organization from the db *after* all its parents have been
+        # processed, to get up-to-date status of the mptt tree before saving each organization.
+        # enforce lower case id standard, but recognize upper case ids as equal:
+        organization = Organization.objects.get(origin_id__iexact=origin_id,
+                                                data_source=data_source)
+        logger.info(f'Updating organization: {origin_id}')
+        for field, value in values_to_update.items():
+            setattr(organization, field, value)
+        if (
+            self.config.get('default_parent_organization', None)
+            and not organization.parent
+            and organization != self._default_parent
+        ):
+            organization.parent = self._default_parent
+        organization.save()
+        logger.debug(f'Caching Organization: {origin_id}')
+        self._organizations[organization.origin_id] = organization
+
+        return organization
+
+    def _import_organization_create(self, incoming_data, origin_id, data_source):
+        """Create a new Organization instance upon import."""
+        object_data = {'origin_id': origin_id, 'data_source': data_source}
+        for field in self.fields:
+            config = self.field_config.get(field) or {}
+            try:
+                object_data[field] = self._get_field_value(incoming_data, field, config)
+            except DataImportError:
+                if config.get('optional'):
+                    continue
+                else:
+                    raise
+
+        # Check if we're supposed to skip importing organizations of this class
+        classification = object_data.get('classification')
+        if classification and classification.origin_id in self.skip_classifications:
+            self._organizations[origin_id] = None
+            logger.info(
+                f'Skipping organization: {origin_id} with type: {classification}'
+            )
+            return None
+
+        logger.info(f'Creating Organization: {origin_id}')
+        organization = Organization.objects.create(**object_data)
+        if (
+            self.config.get('default_parent_organization', None)
+            and not organization.parent
+            and organization != self._default_parent
+        ):
+            organization.parent = self._default_parent
             organization.save()
+        logger.debug(f'Caching Organization: {origin_id}')
+        self._organizations[origin_id] = organization
 
-            return organization
-        except Organization.DoesNotExist:
-            object_data = {'origin_id': origin_id, 'data_source': data_source}
-            for field in self.fields:
-                config = self.field_config.get(field) or {}
-                try:
-                    object_data[field] = self._get_field_value(incoming_data, field, config)
-                except DataImportError as exception:
-                    if config.get('optional'):
-                        continue
-                    else:
-                        raise exception
-            organization = Organization.objects.create(**object_data)
-            if (
-                self.config.get('default_parent_organization', None)
-                and not organization.parent
-                and organization != self._default_parent
-            ):
-                organization.parent = self._default_parent
-                organization.save()
-            return organization
+        return organization
 
     def _import_data_source(self, data):
         """Import data source
 
         If a single value is provided to data_source field, it assume it's
         the id of the data source.
         """
@@ -407,32 +533,36 @@
         return self._get_organization_class(object_data)
 
     def _data_iter(self, url):
         """Iterate over data items in the REST API endpoint.
 
         The iterator will follow over next page links if available.
         """
-        logger.info('Start reading data from {0} ...'.format(url))
+        logger.info(f'Start reading data from {url} ...')
 
-        r = requests.get(url)
+        r = requests.get(url, timeout=self.timeout)
         try:
             r.raise_for_status()
         except requests.HTTPError as e:
-            raise DataImportError(e)
+            raise DataImportError(e) from e
 
         data = r.json()
         for data_item in data[self.results_key] if self.results_key else data:
             yield data_item
 
-        logger.info('Reading data from {0} completed'.format(url))
+        logger.info(f'Reading data from {url} completed')
 
-        if self.next_key and data[self.next_key]:
-            next_url = data[self.next_key]
-            yield from self._data_iter(next_url)
+        if self.next_key:
+            if self.has_meta:
+                next_page_url = data["meta"][self.next_key]
+            else:
+                next_page_url = data[self.next_key]
 
+            if next_page_url:
+                yield from self._data_iter(self._build_resource_url(next_page_url))
 
     def _get_field_value(self, data_item, field, config):
         """Get source value for the field from the data item
 
         If source_field is specified in field config, the source_field
         will be used to get the source value, otherwise the model field
         will be used.
@@ -442,43 +572,59 @@
         If the data type is DataType.ORG_ID, corresponding organization will be returned;
         If the data type is DataType.LINK, the data in the link will be returned;
         If the data type is DataType.REGEX, the extracted value for the pattern will be returned.
         """
         source_field = config.get('source_field') or field
         try:
             value = data_item[source_field]
-        except KeyError:
-            raise DataImportError('Field not found in source data: {0}'.format(source_field))
+        except KeyError as e:
+            raise DataImportError(f'Field not found in source data: {source_field}') from e
+
+        if config.get('unwrap_list') and not value and isinstance(value, list):
+            # Unwrap an empty list to avoid possible errors.
+            value = None
 
         if not value:
             return value
 
         if config.get('data_type'):
             try:
                 data_type = DataType(config['data_type'])
             except ValueError:
-                raise DataImportError('Invalid data type: {0}. Supported data types are: {1}'.format(
-                    config['data_type'],
-                    ', '.join([e.value for e in DataType]),
-                ))
+                raise DataImportError(
+                    f'Invalid data type: {config["data_type"]}. '
+                    f'Supported data types are: {", ".join([e.value for e in DataType])}'
+                )
         else:
             data_type = DataType.VALUE
 
+        if data_type in (DataType.REGEX, DataType.ORG_ID_REGEX) and not config.get('pattern'):
+            raise DataImportError(f'No regex pattern provided for the field: {field}')
+
+        if config.get('unwrap_list'):
+            if len(value) > 1:
+                warnings.warn(
+                    'More than one value in the list, unwrap_list only unwraps the '
+                    'first value in the list.', UserWarning, stacklevel=2
+                )
+            value = value[0]
+        if config.get('unquote'):
+            value = urllib.parse.unquote(value)
+
         if data_type == DataType.STR_LOWER:
             value = str(value).lower()
         elif data_type == DataType.ORG_ID:
             value = self._data_dict.get(value, None)
+        elif data_type == DataType.ORG_ID_REGEX:
+            value = self._get_regex_data(value, config['pattern'])
+            value = self._data_dict.get(value, None)
         elif data_type == DataType.LINK:
             value = self._get_link_data(value)
         elif data_type == DataType.REGEX:
-            try:
-                pattern = config['pattern']
-            except KeyError:
-                raise DataImportError('No regex pattern provided for the field: {0}'.format(field))
-            value = self._get_regex_data(value, pattern)
+            value = self._get_regex_data(value, config['pattern'])
 
         # import related objects
         if field in self.related_import_methods:
             import_method = self.related_import_methods[field]
             value = import_method(value)
 
         return value
@@ -487,28 +633,27 @@
     def _get_regex_data(value, pattern):
         """Extract value from original string value with the given regex pattern"""
         match = re.search(pattern, value)
         if match:
             data = match.group(1)
         else:
             raise DataImportError(
-                'Cannot extract value from string {0} with pattern {1}'.format(value, pattern)
+                f'Cannot extract value from string {value} with pattern {pattern}'
             )
         return data
 
-    @staticmethod
-    def _get_link_data(value):
+    def _get_link_data(self, value):
         """Get data fetched from the link"""
         validator = URLValidator()
         try:
             validator(value)
-        except ValidationError:
-            raise DataImportError('Invalid URL: {0}'.format(value))
+        except ValidationError as e:
+            raise DataImportError(f'Invalid URL: {value}') from e
 
-        r = requests.get(value)
+        r = requests.get(value, timeout=self.timeout)
 
         try:
             r.raise_for_status()
         except requests.HTTPError as e:
-            raise DataImportError(e)
+            raise DataImportError(e) from e
 
         return r.json()
```

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/management/commands/import_organizations.py` & `django-orghierarchy-0.2.0/django_orghierarchy/management/commands/import_organizations.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         )
 
         parser.add_argument(
             '-c',
             '--config',
             dest='config',
             default='paatos',
-            choices=['paatos', 'tprek'],
+            choices=['paatos', 'tprek', 'openahjo'],
             help='REST API configuration to use when importing.'
         )
 
     def _parse_rename_data_source(self, value):
         try:
             old_name, new_name = value.split(':')
         except ValueError:
```

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0001_initial.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0002_organization_replaced_by.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0002_organization_replaced_by.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0003_rm_responsible_org_add_internal_type.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0003_rm_responsible_org_add_internal_type.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0004_add_affiliated_org_permissions.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0004_add_affiliated_org_permissions.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0005_add_fields_to_organization_class.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0005_add_fields_to_organization_class.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0006_add_user_editable_to_data_source.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0006_add_user_editable_to_data_source.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0007_set_editable_false_on_mptt_fields.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0007_set_editable_false_on_mptt_fields.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0008_modify_organization_on_deletes.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0008_modify_organization_on_deletes.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/migrations/0009_add_change_organization_regular_users_permission.py` & `django-orghierarchy-0.2.0/django_orghierarchy/migrations/0009_add_change_organization_regular_users_permission.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy/models.py` & `django-orghierarchy-0.2.0/django_orghierarchy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     """Abstract data source model.
 
     Abstract data source model that provides required fields
     for custom data source model.
     """
     id = models.CharField(max_length=100, primary_key=True)
     name = models.CharField(max_length=255)
-    user_editable_organizations = models.BooleanField(default=False, verbose_name=_('Organizations may be edited by users'))
+    user_editable_organizations = models.BooleanField(
+        default=False, verbose_name=_('Organizations may be edited by users')
+    )
 
     class Meta:
         abstract = True
 
     def __str__(self):
         return self.name
```

### Comparing `django-orghierarchy-0.1.32/django_orghierarchy.egg-info/PKG-INFO` & `django-orghierarchy-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: django-orghierarchy
-Version: 0.1.32
+Version: 0.2.0
 Summary: Reusable Django application for hierarchical organizations.
 Home-page: https://github.com/City-of-Helsinki/django-orghierarchy
 Author: City of Helsinki
 Author-email: dev@hel.fi
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.6
 License-File: LICENSE
 
 # django-orghierarchy
 
 Reusable Django application for hierarchical organizations
 
 # Installation
@@ -31,56 +37,95 @@
 
 2. Add `django_orghierarchy` to `INSTALLED_APPS`
 
 3. If you wish to use your own Django model as data source model (the same way you hot-swap your own user model in Django), add `DJANGO_ORGHIERARCHY_DATASOURCE_MODEL = 'yourapp.DataSource'` to your project settings. Otherwise, the barebones Django model `DataSource` at django_orghierarchy/models.py is used, it contains the fields a data source model *must* contain to be used with django-orghierarchy. Similarly, django-orghierarchy links to your user model, so `AUTH_USER_MODEL` must be defined in Django project settings as always.
 
 4. Run migrations
 
-    ```python
-    python manage.py migrate django_orghierarchy
-    ```
+ ```bash
+ python manage.py migrate django_orghierarchy
+ ```
+
 
 # Usage
 
 The `Organization` class is the main feature of django-orghierarchy. We use [`django-mptt`](https://github.com/django-mptt/django-mptt/) to implement an organization hierarchy that can be as deep as you wish. Each organization has a name, a data source (referring to the system the organization data is from), origin_id (referring to organization id in the original data source), founding date and dissolution date, status (*normal* or *affiliated*), a place in a forest of organization trees, and possibly a *replacement organization*, which means a link to any other organization across the trees (making the forest strictly a directed graph, not a bunch of trees). Replacement organization allows linking dissolved organization structures to new ones so that old user rights are automatically transferred across the hierarchy to the replacing organization.
 
 Each organization may have `admin_users` and `regular_users`, which are linked to your Django user model. Also, an organization may have `sub_organizations` and `affiliated_organizations`. You may have any number of top level organizations. Also, some extra user permissions are defined, i.e. `add_affiliated_organization`, `change_affiliated_organization`, `delete_affiliated_organization`, `replace_organization` and `change_organization_regular_users`. These permissions are for adding *regular users* and *affiliated organizations* in Django-admin, and creating *replacement* links, without being allowed to touch the *admin users* or the existing organization hierarchy. *Affiliated* organizations usually have more limited rights than *normal* organizations within the hierarchy; they are meant for external organizations you collaborate with and wish to grant limited rights to.
 
 Your desired user rights and permissions for each user group in each level of the organization depend on your application details, so you should implement your own user rights checks depending on your needs. You may e.g. create a user model permissions mixin that uses information on the user organization, as done in [Linkedevents permissions](https://github.com/City-of-Helsinki/linkedevents/blob/master/events/permissions.py) and [Linkedevents user model](https://github.com/City-of-Helsinki/linkedevents/blob/master/helevents/models.py). The user rights model is originally specified [here](https://github.com/City-of-Helsinki/linkedevents/issues/235).
 
 You may import an existing organization hierarchy from a REST API corresponding to the [6Aika Paatos decisionmaking API specification](https://github.com/6aika/api-paatos), based on the [Popolo project](http://www.popoloproject.com/), with the included importer, for example:
-
-    python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/"
+```bash
+python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/"
+```
     
 You may give the organization data source a specific id to correspond to your own data source model ids in your project:
-
-    python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/" -s original_id:imported_id
+```bash
+python manage.py import_organizations "https://api.hel.fi/paatos/v1/organization/" -s original_id:imported_id
+```
 
 Otherwise, the data source id in the original API is used for the imported organizations (`helsinki` in the Helsinki API).
 
+
 # Development
 
+Install requirements.
+
+```bash
+# Package requirements
+pip install -e .
+# Development requirements
+pip install -r requirements.txt
+```
+
+
 ## Tests
 
+
 ### Unit tests
 
-Run tests
+Run the tests.
 
-    py.test
+```bash
+pytest
+```
 
-Run tests with coverage report
+Run the tests with coverage report.
 
-    py.test --cov-report html --cov .
+```bash
+pytest --cov-report html --cov .
+```
     
 Open htmlcov/index.html for the coverage report.
 
+
+### Running tests against multiple environments
+
+You can run the tests against multiple environments by using [tox](https://tox.readthedocs.io/en/latest/).
+Install `tox` globally and run:
+
+```bash
+tox
+```
+
+Use the `-f` option to specify target environments.
+
+```bash
+# Target only Python 3.9 environments
+tox -f py39
+# Target Python 3.9 and Django 3.2
+tox -f py39 django32
+```
+
+
 ### Integration tests
 
 We need to provide different settings files for the test as the
 setting variables for swappable model are only evaluated the first
-time the module is imported.
-
-Run tests
-
-    python manage.py test --tag=custom_ds --settings=tests.test_app.settings_custom_ds
-    python manage.py test --tag=custom_pk_ds --settings=tests.test_app.settings_custom_pk_ds
+time the module is imported. Integration tests are skipped by default.
 
+Run the integration tests.
+```bash
+pytest -m custom_ds --ds=tests.test_app.settings_custom_ds
+pytest -m custom_pk_ds --ds=tests.test_app.settings_custom_pk_ds
+```
```

### Comparing `django-orghierarchy-0.1.32/tests/test_admin.py` & `django-orghierarchy-0.2.0/tests/test_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from django.contrib import admin
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.models import Permission
-from django.test import TestCase, RequestFactory
+from django.test import RequestFactory, TestCase
 
-from django_orghierarchy.admin import OrganizationAdmin, SubOrganizationInline, AddSubOrganizationInline,\
-    ProtectedSubOrganizationInline, AffiliatedOrganizationInline, AddAffiliatedOrganizationInline,\
-    ProtectedAffiliatedOrganizationInline
+from django_orghierarchy.admin import (
+    AddAffiliatedOrganizationInline,
+    AddSubOrganizationInline,
+    AffiliatedOrganizationInline,
+    OrganizationAdmin,
+    ProtectedAffiliatedOrganizationInline,
+    ProtectedSubOrganizationInline,
+    SubOrganizationInline,
+)
 from django_orghierarchy.models import DataSource, Organization
-from .factories import OrganizationClassFactory, OrganizationFactory, DataSourceFactory
+
+from .factories import DataSourceFactory, OrganizationClassFactory, OrganizationFactory
 from .utils import clear_user_perm_cache, make_admin
 
 
 class TestDataSourceAdmin(TestCase):
 
     def test_data_source_admin_is_registered(self):
         is_registered = admin.site.is_registered(DataSource)
@@ -429,15 +436,17 @@
         self.admin = make_admin()
         self.site = AdminSite()
         self.factory = RequestFactory()
 
         self.organization = OrganizationFactory()
         self.affiliated_organization = OrganizationFactory(
             internal_type=Organization.AFFILIATED, parent=self.organization)
-        self.editable_organization = OrganizationFactory(data_source=(DataSourceFactory(user_editable_organizations=True)))
+        self.editable_organization = OrganizationFactory(
+            data_source=(DataSourceFactory(user_editable_organizations=True))
+        )
 
     def test_get_queryset(self):
         org = OrganizationFactory()
         sub_org = OrganizationFactory()
         another_sub_org = OrganizationFactory()
         sub_org.parent = self.organization
         another_sub_org.parent = org
@@ -448,31 +457,35 @@
 
         oa = OrganizationAdmin(Organization, self.site)
         request = self.factory.get('/fake-url/')
 
         # test against superuser admin
         request.user = self.admin
         qs = oa.get_queryset(request)
+        self.assertIsInstance(qs, Organization.objects._queryset_class)
         self.assertQuerysetEqual(
             qs,
             [repr(self.organization), repr(self.affiliated_organization), repr(self.editable_organization),
              repr(org), repr(sub_org), repr(another_sub_org)],
             ordered=False)
 
         # test against non-superuser admin
         request.user = normal_admin
         qs = oa.get_queryset(request)
+        self.assertIsInstance(qs, Organization.objects._queryset_class)
         self.assertQuerysetEqual(qs, [])
 
         self.organization.admin_users.add(normal_admin)
         qs = oa.get_queryset(request)
+        self.assertIsInstance(qs, Organization.objects._queryset_class)
         self.assertQuerysetEqual(qs, [repr(self.organization), repr(self.affiliated_organization), repr(sub_org)])
 
         org.admin_users.add(normal_admin)
         qs = oa.get_queryset(request)
+        self.assertIsInstance(qs, Organization.objects._queryset_class)
         self.assertQuerysetEqual(
             qs,
             [repr(self.organization), repr(self.affiliated_organization), repr(org), repr(sub_org),
              repr(another_sub_org)],
             ordered=False)
 
     def test_save_model(self):
```

### Comparing `django-orghierarchy-0.1.32/tests/test_api.py` & `django-orghierarchy-0.2.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-orghierarchy-0.1.32/tests/test_app/tests/test_custom_pk_data_source.py` & `django-orghierarchy-0.2.0/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-from django.contrib import admin
-from django.test import TestCase, tag
+from unittest.mock import MagicMock, patch
 
-from django_orghierarchy.utils import get_data_source_model
-from django_orghierarchy.models import DataSource, Organization
-from ..models import CustomPrimaryKeyDataSource
+from django.test import TestCase
 
+from django_orghierarchy.models import DataSource
+from django_orghierarchy.utils import get_data_source_model, swapper
 
-@tag('custom_pk_ds')
-class TestCustomPrimaryKeyDataSource(TestCase):
 
-    def test_get_data_source_model(self):
+class TestGetDataSourceModel(TestCase):
+
+    def test_get_data_source_model_return_default_model(self):
         model = get_data_source_model()
-        self.assertIs(model, CustomPrimaryKeyDataSource)
+        self.assertIs(model, DataSource)
 
-    def test_related_data_source_model(self):
-        field = Organization._meta.get_field('data_source')
-        self.assertIs(field.related_model, CustomPrimaryKeyDataSource)
-
-    def test_default_data_source_admin_not_registered(self):
-        is_registered = admin.site.is_registered(DataSource)
-        self.assertFalse(is_registered)
+    @patch('swapper.load_model', MagicMock())
+    def test_get_data_source_model_swapper_load_model_called(self):
+        get_data_source_model()
+        self.assertTrue(swapper.load_model.called)
```

### Comparing `django-orghierarchy-0.1.32/tests/test_commands.py` & `django-orghierarchy-0.2.0/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.core.management import call_command, CommandError
 from django.test import TestCase
 
 from django_orghierarchy.importers import DataImportError
 from django_orghierarchy.models import Organization, OrganizationClass
 from django_orghierarchy.utils import get_data_source_model
+
 from .test_importers import mock_request_get
 
 
 class TestRestImportCommand(TestCase):
 
     @patch('requests.get', MagicMock(side_effect=mock_request_get))
     def test_rest_import_success(self):
```

### Comparing `django-orghierarchy-0.1.32/tests/test_forms.py` & `django-orghierarchy-0.2.0/tests/test_forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from django.test import TestCase
 
-from django_orghierarchy.forms import OrganizationForm, SubOrganizationForm, AffiliatedOrganizationForm
+from django_orghierarchy.forms import (
+    AffiliatedOrganizationForm,
+    OrganizationForm,
+    SubOrganizationForm,
+)
 from django_orghierarchy.models import Organization
-from .factories import OrganizationClassFactory, DataSourceFactory, OrganizationFactory
+
+from .factories import DataSourceFactory, OrganizationClassFactory, OrganizationFactory
 
 
 class TestOrganizationForm(TestCase):
 
     def setUp(self):
         self.organization = OrganizationFactory()
         self.data_source = DataSourceFactory(user_editable_organizations=True)
```

### Comparing `django-orghierarchy-0.1.32/tests/test_importers.py` & `django-orghierarchy-0.2.0/tests/test_importers.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 tprek_organizations = {
     '111': tprek_organization_1,
     '222': tprek_organization_2,
     '333': tprek_organization_3,
 }
 
 
-def mock_request_get(url):
+def mock_request_get(url, *args, **kwargs):
     m = re.search(r'http://fake.url/organizations/(\d+)/', url)
     if m:
         org_id = m.group(1)
         return MockResponse(organizations[org_id])
 
     m = re.search(r'http://fake.url/organizations/\?page=(\d+)$', url)
     if m:
@@ -120,27 +120,30 @@
     m = re.search(r'http://fake.url/', url)
     if m:
         return MockResponse({'next_page': None, 'items': []}, status_code=200)
 
     return MockResponse({}, status_code=404)
 
 
-def mock_tprek_request_get(url):
+def mock_tprek_request_get(url, *args, **kwargs):
     m = re.search(r'http://fake.tprek.url/department/', url)
     if m:
         return MockResponse(tprek_organizations.values())
 
     return MockResponse({}, status_code=404)
 
 
 class TestRestApiImporter(TestCase):
 
-    @patch('requests.get', MagicMock(side_effect=mock_request_get))
     def setUp(self):
-        self.importer = RestAPIImporter('http://fake.url/organizations/?page=1')
+        self.importer = self.get_importer()
+
+    @patch('requests.get', MagicMock(side_effect=mock_request_get))
+    def get_importer(self):
+        return RestAPIImporter('http://fake.url/organizations/?page=1')
 
     @patch('requests.get', MagicMock(side_effect=mock_request_get))
     def test_custom_config(self):
         config = {
             'next_key': 'next_page',
             'results_key': 'items',
             'fields': ['classification', 'origin_id', 'name', 'parent'],
@@ -233,15 +236,18 @@
         self.assertEqual(organization.parent.name, 'Organization-2')
         self.assertNotEqual(organization.parent_id, 222)
         changed_organization = organization_2.copy()
         new_parent = organization_1.copy()
         changed_organization["parent"] = "http://fake.url/organizations/111/"
         new_parent["parent"] = None
         organizations["111"] = new_parent
-        organization = self.importer._import_organization(changed_organization)
+
+        # Re-initialize the importer to clear the caches and data
+        importer = self.get_importer()
+        organization = importer._import_organization(changed_organization)
         # Now the parents should have switched.
         self.assertQuerysetEqual(qs, [repr(organization.parent), repr(organization)], ordered=False)
         self.assertEqual(organization.name, 'Organization-2')
         self.assertNotEqual(organization.id, 222)
         self.assertEqual(organization.parent.name, 'Organization-1')
         self.assertNotEqual(organization.id, 111)
         # tear down this test, as it had a side effect
@@ -256,14 +262,26 @@
         )
         self.importer._import_organization(organization_2)
         organization.refresh_from_db()
 
         self.assertQuerysetEqual(Organization.objects.all(), [repr(organization)])
         self.assertEqual(organization.name, 'Organization-2')
 
+    @patch('requests.get', MagicMock(side_effect=mock_request_get))
+    def test_import_organization_data_with_skip_classifications(self):
+        """Organization is not imported if it's in the classification skip list."""
+        self.importer.config["skip_classifications"] = ["test-class-1"]
+        organization = self.importer._import_organization(organization_1)
+        self.assertIsNone(organization)
+
+        # Re-initialize the importer to clear the caches and data
+        importer = self.get_importer()
+        organization = importer._import_organization(organization_1)
+        self.assertEqual(organization.id, "test-source-1:abc-123")
+
     def test_import_data_source_with_string(self):
         data_source = self.importer._import_data_source('test-data-source')
         data_source_model = get_data_source_model()
         qs = data_source_model.objects.all()
         self.assertQuerysetEqual(qs, [repr(data_source)])
         self.assertEqual(data_source.id, 'test-data-source')
 
@@ -278,20 +296,32 @@
         self.assertEqual(data_source.id, 'test-data-source')
 
     def test_import_organization_class_with_string(self):
         organization_class = self.importer._import_organization_class('test-source-1:test-org-class')
         qs = OrganizationClass.objects.all()
         self.assertQuerysetEqual(qs, [repr(organization_class)])
         self.assertEqual(organization_class.id, 'test-source-1:test-org-class')
+        self.assertEqual(organization_class.name, 'test-source-1:test-org-class')
 
     def test_import_organization_class_with_simple_string(self):
         organization_class = self.importer._import_organization_class('class-with-no-source')
         qs = OrganizationClass.objects.all()
         self.assertQuerysetEqual(qs, [repr(organization_class)])
         self.assertEqual(organization_class.id, 'OpenDecisionAPI:class-with-no-source')
+        self.assertEqual(organization_class.name, 'OpenDecisionAPI:class-with-no-source')
+
+    def test_import_organization_class_with_simple_string_and_remapped_data_source(self):
+        self.importer.config['rename_data_source'] = {'OpenDecisionAPI': 'remapped'}
+
+        organization_class = self.importer._import_organization_class('class-with-no-source')
+
+        qs = OrganizationClass.objects.all()
+        self.assertQuerysetEqual(qs, [repr(organization_class)])
+        self.assertEqual(organization_class.id, 'remapped:class-with-no-source')
+        self.assertEqual(organization_class.name, 'remapped:class-with-no-source')
 
     def test_import_organization_class_with_dict_data(self):
         data = {
             'id': 999,
             'origin_id': 'test-org-class',
             'name': 'test-org-class',
             'data_source': 'test-source-1',
@@ -433,17 +463,20 @@
         data = self.importer._get_link_data(url)
         self.assertEqual(data, organization_1)
 
 
 class TestTprekRestApiImporter(TestRestApiImporter):
     # here we test all the features of the TPREK import that are different from default REST import
 
-    @patch('requests.get', MagicMock(side_effect=mock_tprek_request_get))
     def setUp(self):
-        self.config = {
+        self.importer = self.get_importer()
+
+    @patch('requests.get', MagicMock(side_effect=mock_tprek_request_get))
+    def get_importer(self):
+        config = {
             'next_key': None,
             'results_key': None,
             'fields': [
                 'origin_id', 'classification',
                 'name', 'parent',
             ],
             'update_fields': [
@@ -467,15 +500,15 @@
                     'source_field': 'name_fi',
                     'optional': True,
                 }
             },
             'default_data_source': 'tprek',
             'default_parent_organization': 'Pääkaupunkiseudun toimipisterekisteri'
         }
-        self.importer = RestAPIImporter('http://fake.tprek.url/department/', self.config)
+        return RestAPIImporter('http://fake.tprek.url/department/', config)
 
     @patch('requests.get', MagicMock(side_effect=mock_tprek_request_get))
     def test_get_data_source(self):
         data = {'id': 'tprek'}
         data_source = self.importer._get_data_source(data)
         self.assertEqual(data_source.id, 'tprek')
         data_source_model = get_data_source_model()
@@ -493,19 +526,19 @@
 
     @patch('requests.get', MagicMock(side_effect=mock_tprek_request_get))
     def test_get_field_value_related_fields(self):
         value = self.importer._get_field_value({'data_source': 'tprek'}, 'data_source', {})
         self.assertEqual(value.id, 'tprek')
 
         value = self.importer._get_field_value(tprek_organization_1, 'classification',
-                                               self.config['field_config']['classification'])
+                                               self.importer.config['field_config']['classification'])
         self.assertEqual(value.id, 'tprek:TEST_TYPE_1')
 
         value = self.importer._get_field_value(tprek_organization_1, 'parent',
-                                               self.config['field_config']['parent'])
+                                               self.importer.config['field_config']['parent'])
         self.assertEqual(value.id, 'tprek:222')
 
     @patch('requests.get', MagicMock(side_effect=mock_tprek_request_get))
     def test_data_iter(self):
         url = 'http://fake.tprek.url/department/'
         iterator = self.importer._data_iter(url)
         iter_len = len(list(iterator))
@@ -523,27 +556,50 @@
         self.assertEqual(OrganizationClass.objects.count(), 2)
 
     def test_import_organization_class_with_simple_string(self):
         organization_class = self.importer._import_organization_class('class-with-no-source')
         qs = OrganizationClass.objects.all()
         self.assertQuerysetEqual(qs, [repr(organization_class)])
         self.assertEqual(organization_class.id, 'tprek:class-with-no-source')
+        self.assertEqual(organization_class.name, 'tprek:class-with-no-source')
+
+    def test_import_organization_class_with_simple_string_and_remapped_data_source(self):
+        self.importer.config['rename_data_source'] = {'tprek': 'remapped'}
+
+        organization_class = self.importer._import_organization_class('class-with-no-source')
+
+        qs = OrganizationClass.objects.all()
+        self.assertQuerysetEqual(qs, [repr(organization_class)])
+        self.assertEqual(organization_class.id, 'remapped:class-with-no-source')
+        self.assertEqual(organization_class.name, 'remapped:class-with-no-source')
 
     def test_import_organization_class_with_dict_data(self):
         pass
 
     def test_import_organization_class_with_simple_dict_data(self):
         pass
 
     def test_import_data_source_with_string(self):
         pass
 
     def test_import_data_source_with_dict_data(self):
         pass
 
+    @patch('requests.get', MagicMock(side_effect=mock_tprek_request_get))
+    def test_import_organization_data_with_skip_classifications(self):
+        """Organization is not imported if it's in the classification skip list."""
+        self.importer.config["skip_classifications"] = ["TEST_TYPE_1"]
+        organization = self.importer._import_organization(tprek_organization_1)
+        self.assertIsNone(organization)
+
+        # Re-initialize the importer to clear the caches and data
+        importer = self.get_importer()
+        organization = importer._import_organization(tprek_organization_1)
+        self.assertEqual(organization.id, 'tprek:111')
+
     def test_import_organization_update_existing(self):
         organization = OrganizationFactory(
             name='existing-organization',
             origin_id=tprek_organization_2['id'],
             data_source=self.importer._import_data_source('tprek'),
         )
         self.importer._import_organization(tprek_organization_2)
@@ -557,26 +613,29 @@
     def test_import_organization_with_parent(self):
         organization = self.importer._import_organization(tprek_organization_1)
         qs = Organization.objects.all()
         default_parent = Organization.objects.get(id='tprek:tprek')
 
         # also created parent organization.
         # parent will have the default parent organization
-        self.assertQuerysetEqual(qs, [repr(default_parent), repr(organization.parent), repr(organization)], ordered=False)
+        self.assertQuerysetEqual(
+            qs,
+            [repr(default_parent), repr(organization.parent), repr(organization)],
+            ordered=False
+        )
         self.assertEqual(organization.name, 'Organization-1')
         self.assertEqual(organization.id, 'tprek:111')
         self.assertEqual(organization.parent.name, 'Organization-2')
         self.assertEqual(organization.parent_id, 'tprek:222')
         self.assertEqual(organization.parent.parent.name, 'Pääkaupunkiseudun toimipisterekisteri')
         self.assertEqual(organization.parent.parent_id, 'tprek:tprek')
 
     @patch('requests.get', MagicMock(side_effect=mock_request_get))
     def test_import_organization_with_missing_parent(self):
         organization = self.importer._import_organization(tprek_organization_3)
-        print(organization)
         qs = Organization.objects.all()
 
         # also created parent organization.
         # parent was not found, so organization will have the default
         default_parent = Organization.objects.get(id='tprek:tprek')
         self.assertQuerysetEqual(qs, [repr(default_parent), repr(organization)])
         self.assertEqual(organization.name, 'Organization-3')
@@ -600,15 +659,19 @@
     def test_import_organization_flip_parents(self):
         organization = self.importer._import_organization(tprek_organization_1)
         qs = Organization.objects.all()
         default_parent = Organization.objects.get(id='tprek:tprek')
 
         # also created parent organization.
         # parent will have the default parent organization
-        self.assertQuerysetEqual(qs, [repr(default_parent), repr(organization.parent), repr(organization)], ordered=False)
+        self.assertQuerysetEqual(
+            qs,
+            [repr(default_parent), repr(organization.parent), repr(organization)],
+            ordered=False
+        )
         self.assertEqual(organization.name, 'Organization-1')
         self.assertEqual(organization.id, 'tprek:111')
         self.assertEqual(organization.parent.name, 'Organization-2')
         self.assertEqual(organization.parent_id, 'tprek:222')
         self.assertEqual(organization.parent.parent.name, 'Pääkaupunkiseudun toimipisterekisteri')
         self.assertEqual(organization.parent.parent_id, 'tprek:tprek')
 
@@ -616,18 +679,22 @@
         new_parent = tprek_organization_1.copy()
         changed_organization["parent_id"] = "111"
         new_parent["parent_id"] = None
         tprek_organizations["111"] = new_parent
 
         # We must init a new importer, since importing by organization id will use a cached dict of all the
         # organizations in the importer.
-        new_importer = RestAPIImporter('http://fake.tprek.url/department/', self.config)
+        new_importer = self.get_importer()
         organization = new_importer._import_organization(changed_organization)
         # Now the parents should have switched.
-        self.assertQuerysetEqual(qs, [repr(default_parent), repr(organization.parent), repr(organization)], ordered=False)
+        self.assertQuerysetEqual(
+            qs,
+            [repr(default_parent), repr(organization.parent), repr(organization)],
+            ordered=False
+        )
         self.assertEqual(organization.name, 'Organization-2')
         self.assertEqual(organization.id, 'tprek:222')
         self.assertEqual(organization.parent.name, 'Organization-1')
         self.assertEqual(organization.parent_id, 'tprek:111')
         self.assertEqual(organization.parent.parent.name, 'Pääkaupunkiseudun toimipisterekisteri')
         self.assertEqual(organization.parent.parent_id, 'tprek:tprek')
         # tear down this test, as it had a side effect
```

### Comparing `django-orghierarchy-0.1.32/tests/test_models.py` & `django-orghierarchy-0.2.0/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.test import TestCase
 
 from django_orghierarchy.models import Organization
+
 from .factories import DataSourceFactory, OrganizationClassFactory, OrganizationFactory
 
 
 class TestDataSource(TestCase):
 
     def setUp(self):
         self.data_source = DataSourceFactory(name='test name')
```

